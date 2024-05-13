# Comparing `tmp/deeporigin-0.0.6.tar.gz` & `tmp/deeporigin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.0.6.tar", last modified: Wed May  1 19:47:53 2024, max compression
+gzip compressed data, was "deeporigin-0.0.7.tar", last modified: Thu May  2 15:05:32 2024, max compression
```

## Comparing `deeporigin-0.0.6.tar` & `deeporigin-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 19:47:49.000000 deeporigin-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 19:47:49.000000 deeporigin-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 19:47:53.335903 deeporigin-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 19:47:49.000000 deeporigin-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 19:47:49.000000 deeporigin-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:47:53.335903 deeporigin-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 19:47:51.000000 deeporigin-0.0.6/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/do_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.331903 deeporigin-0.0.6/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15706 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.331903 deeporigin-0.0.6/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_cli_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.483947 deeporigin-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 15:05:28.000000 deeporigin-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 15:05:28.000000 deeporigin-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-02 15:05:32.483947 deeporigin-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 15:05:28.000000 deeporigin-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.483947 deeporigin-0.0.7/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 15:05:32.000000 deeporigin-0.0.7/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-02 15:05:28.000000 deeporigin-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:05:32.483947 deeporigin-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.475947 deeporigin-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 15:05:30.000000 deeporigin-0.0.7/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.475947 deeporigin-0.0.7/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.475947 deeporigin-0.0.7/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/do_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.479947 deeporigin-0.0.7/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16050 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.479947 deeporigin-0.0.7/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.483947 deeporigin-0.0.7/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 15:05:28.000000 deeporigin-0.0.7/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:05:32.483947 deeporigin-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-05-02 15:05:28.000000 deeporigin-0.0.7/tests/test_variables.py
```

### Comparing `deeporigin-0.0.6/LICENSE.txt` & `deeporigin-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/PKG-INFO` & `deeporigin-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.6/README.md` & `deeporigin-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 > [!WARNING]  
 > The `deeporigin` client is under active development. Features
 > may change, or be removed. 
 
 ## Installation 
 
 > [!CAUTION]
-> You are strongly advised to install this in a virtual environment. 
+> As a best practice, we recommend  installing this in a virtual environment. 
 
 ### For end users
 
 ```bash
 pip install deeporigin
 ```
```

### Comparing `deeporigin-0.0.6/deeporigin.egg-info/PKG-INFO` & `deeporigin-0.0.7/deeporigin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.6/deeporigin.egg-info/SOURCES.txt` & `deeporigin-0.0.7/deeporigin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 src/context.py
 src/do_api.py
 src/exceptions.py
 src/feature_flags.py
 src/utils.py
 src/warnings.py
 src/cli/__init__.py
-src/cli/auth.py
 src/cli/context.py
 src/cli/data.py
 src/cli/variables.py
 src/config/__init__.py
 src/config/default.yml
 src/managed_data/__init__.py
 src/managed_data/_api.py
```

### Comparing `deeporigin-0.0.6/pyproject.toml` & `deeporigin-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/__init__.py` & `deeporigin-0.0.7/src/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/cli/__init__.py` & `deeporigin-0.0.7/src/cli/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import functools
 import sys
 import warnings
 
 import cement
 import termcolor
+from deeporigin import cache_do_api_tokens, get_do_api_tokens
+from deeporigin.config import get_value
+from deeporigin.utils import _print_dict
 
 from .. import __version__
 from ..exceptions import DeepOriginException
 from ..warnings import DeepOriginWarning
-from .auth import CONTROLLERS as AUTH_CONTROLLERS
 from .context import CONTROLLERS as CONTEXT_CONTROLLERS
 from .data import CONTROLLERS as DATA_CONTROLLERS
 from .variables import CONTROLLERS as VARIABLE_CONTROLLERS
 
 __all__ = ["main", "App"]
 
 
@@ -38,25 +40,54 @@
     def _default(self):
         args = self.app.pargs
         if args.version:
             print(__version__)
         else:
             raise SystemExit(self._parser.print_help())
 
+    @cement.ex(
+        help="Authenticate to the Deep Origin platform",
+    )
+    def authenticate(self):
+        """list the columns of the row and their values, where applicable"""
+        access_token, refresh_token = get_do_api_tokens(verbose=True)
+
+        cache_do_api_tokens(access_token, refresh_token)
+
+    @cement.ex(
+        help="Show configuration",
+        arguments=[
+            (
+                ["--json"],
+                {
+                    "action": "store_true",
+                    "help": "Whether to return JSON formatted data [default: False]",
+                },
+            ),
+        ],
+    )
+    def config(self):
+        """list the columns of the row and their values, where applicable"""
+
+        data = get_value()
+
+        data.pop("list_bench_variables_query_template", None)
+
+        _print_dict(data, json=self.app.pargs.json)
+
 
 class App(cement.App):
     class Meta:
         label = "deep-origin"
         base_controller = "base"
         handlers = (
             [BaseController]
             + VARIABLE_CONTROLLERS
             + CONTEXT_CONTROLLERS
             + DATA_CONTROLLERS
-            + AUTH_CONTROLLERS
         )
 
 
 def except_hook(built_in_except_hook, type, value, tb):
     if issubclass(type, DeepOriginException):
         sys.stderr.write(termcolor.colored(value, "red") + "\n")
     else:
```

### Comparing `deeporigin-0.0.6/src/cli/context.py` & `deeporigin-0.0.7/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/cli/data.py` & `deeporigin-0.0.7/src/cli/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,17 @@
 """this implements controllers and hooks to connect to
 managed_data.py"""
 
-import json
 import os
-from typing import Union
 
 import cement
-from beartype import beartype
 from deeporigin.exceptions import DeepOriginException
 from deeporigin.managed_data import _api, api
 from deeporigin.managed_data.client import DeepOriginClient
-from deeporigin.utils import PREFIX
-from tabulate import tabulate
-
-
-@beartype
-def _print_tree(tree: dict, offset: int = 0) -> None:
-    """helper function to pretty print a tree"""
-    print(" " * offset + tree["hid"])
-
-    if "children" not in tree.keys():
-        return
-    for child in tree["children"]:
-        _print_tree(child, offset + 2)
-
-
-def _print_dict(
-    data: dict,
-    *,
-    json: bool = True,
-    transpose: bool = True,
-) -> None:
-    """helper function to pretty print a dict as a table"""
-
-    if json:
-        _show_json(data)
-    else:
-        if transpose:
-            data = data.items()
-            headers = ["Name", "Value"]
-        else:
-            headers = "keys"
-        print(
-            tabulate(
-                data,
-                headers=headers,
-                tablefmt="rounded_outline",
-            )
-        )
+from deeporigin.utils import PREFIX, _print_dict, _print_tree, _show_json, _truncate
 
 
 class DataController(cement.Controller):
     class Meta:
         label = "data"
         stacked_on = "base"
         stacked_type = "nested"
@@ -69,15 +29,15 @@
         except Exception:
             client = DeepOriginClient()  # pragma: no cover
             client.authenticate(refresh_tokens=False)  # pragma: no cover
 
             return client  # pragma: no cover
 
     @cement.ex(
-        help="Merge to databases into a single one, integrating cross-references",
+        help="Merge two databases into a single one, integrating cross-references",
         arguments=[
             (
                 ["--databases"],
                 {
                     "help": "List of databases to merge",
                     "action": "store",
                     "nargs": "*",
@@ -125,14 +85,31 @@
 
         for df in dfs:
             files = df.attrs["file_ids"]
             for file in files:
                 _api.download_file(file, destination=destination)
 
     @cement.ex(
+        help="Download a file from Deep Origin",
+        arguments=[
+            (
+                ["file_id"],
+                {"help": "File ID", "action": "store"},
+            ),
+        ],
+    )
+    def download_file(self):
+        """download file"""
+
+        _api.download_file(
+            self.app.pargs.file_id,
+            client=self._get_client(),
+        )
+
+    @cement.ex(
         help="Describe and get metadata of file uploaded to database in your Deep Origin data management system",
         arguments=[
             (
                 ["file_id"],
                 {"help": "File ID", "action": "store"},
             ),
             (
@@ -173,14 +150,28 @@
     def describe_row(self):
         """describe row"""
 
         data = _api.describe_row(
             self.app.pargs.row_id,
             client=self._get_client(),
         )
+        data.pop("rowJsonSchema", None)
+
+        if "cols" in data.keys():
+            col_names = [col["name"] for col in data["cols"]]
+            col_keys = [col["key"] for col in data["cols"]]
+
+            col_names = ", ".join(col_names)
+            col_keys = ", ".join(col_keys)
+
+            if data["type"] == "database" and not self.app.pargs.json:
+                data["Column Names"] = _truncate(col_names)
+                data["Column Keys"] = _truncate(col_keys)
+
+                data.pop("cols", None)
 
         _print_dict(data, json=self.app.pargs.json)
 
     @cement.ex(
         help="List files in a database or row",
         arguments=[
             (
@@ -407,17 +398,11 @@
             # upload(args.source, args.destination)
         else:
             raise DeepOriginException(
                 f"Exactly one of <source> and <destination> should be prefixed with `{PREFIX}`"
             )
 
 
-@beartype
-def _show_json(data: Union[list, dict]) -> None:
-    """utility for pretty printing JSON"""
-    print(json.dumps(data, indent=2))
-
-
 CONTROLLERS = [
     DataController,
     CopyController,
 ]
```

### Comparing `deeporigin-0.0.6/src/cli/variables.py` & `deeporigin-0.0.7/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/config/__init__.py` & `deeporigin-0.0.7/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/config/default.yml` & `deeporigin-0.0.7/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/context.py` & `deeporigin-0.0.7/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/do_api.py` & `deeporigin-0.0.7/src/do_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/feature_flags.py` & `deeporigin-0.0.7/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/managed_data/_api.py` & `deeporigin-0.0.7/src/managed_data/_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/managed_data/api.py` & `deeporigin-0.0.7/src/managed_data/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The `deeporigin.managed_data.api` module contains high-level functions for
 interacting with Deep Origin managed data."""
 
 import os
+from pathlib import Path
 from typing import Any, Optional, Union
 
 from beartype import beartype
 from deeporigin.exceptions import DeepOriginException
 from deeporigin.managed_data._api import (
     convert_id_format,
     describe_file,
@@ -136,14 +137,16 @@
     Args:
         source: ID (or human ID) of a resource on Deep Origin.
         destination: Path to local directory to save resources.
         include_files: if `True`, download files in database.
 
     """
 
+    Path(destination).mkdir(parents=True, exist_ok=True)
+
     if not os.path.isdir(destination):
         raise DeepOriginException(f"{destination} should be a path to a folder.")
 
     source = source.replace(PREFIX, "")
 
     # first, need to determine what this is.
     obj = describe_row(source, client=client)
@@ -314,26 +317,37 @@
 ):
     """Internal function parse column values
 
     Warning: Internal function
         Do not use this function.
     """
 
-    value = [field["value"] for field in fields if field["columnId"] == column["id"]]
+    field = [field for field in fields if field["columnId"] == column["id"]]
+
+    if len(field) == 0:
+        return [None]
+
+    if "value" not in field[0].keys():
+        return [None]
+    value = [field[0]["value"]]
 
     # special treatment for some column types
     if column["type"] == "select" and len(value) == 1:
         value = value[0]["selectedOptions"]
     elif column["type"] == "file" and len(value) == 1:
         value = value[0]["fileIds"]
 
         file_ids.extend(value)
 
         if use_file_names:
-            value = [describe_file(file_id)["name"] for file_id in value]
+            try:
+                value = [describe_file(file_id)["name"] for file_id in value]
+            except DeepOriginException:
+                # something went wrong, ignore
+                pass
     elif column["type"] == "reference" and len(value) == 1:
         value = value[0]["rowIds"]
         reference_ids.extend(value)
 
         if reference_format == "human-id":
             value = convert_id_format(ids=value)
             value = [thing["hid"] for thing in value]
```

### Comparing `deeporigin-0.0.6/src/managed_data/client.py` & `deeporigin-0.0.7/src/managed_data/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
 def _check_response(response: requests.models.Response) -> Union[dict, list]:
     """utility function to check responses"""
 
     if response.status_code == 404:
         raise DeepOriginException(
             f"[Error 404] The requested resource was not found. The response was: {response.json()}"
         )
+    elif response.status_code == 400:
+        raise DeepOriginException(f"[Error 400] The response was: {response.json()}")
 
     response.raise_for_status()
     response = response.json()
 
     if "error" in response:
         raise DeepOriginException(response["error"])
```

### Comparing `deeporigin-0.0.6/src/managed_data/schema.py` & `deeporigin-0.0.7/src/managed_data/schema.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/base_type.py` & `deeporigin-0.0.7/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/core.py` & `deeporigin-0.0.7/src/variables/core.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/__init__.py` & `deeporigin-0.0.7/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/aws_profile.py` & `deeporigin-0.0.7/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/env_var.py` & `deeporigin-0.0.7/src/variables/types/env_var.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/file.py` & `deeporigin-0.0.7/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/git_http_credentials.py` & `deeporigin-0.0.7/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/private_gpg_key.py` & `deeporigin-0.0.7/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/private_ssh_key.py` & `deeporigin-0.0.7/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/secret_env_var_value.py` & `deeporigin-0.0.7/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/secret_file_value.py` & `deeporigin-0.0.7/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/src/variables/types/xpress_license_file.py` & `deeporigin-0.0.7/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_cli.py` & `deeporigin-0.0.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_cli_data.py` & `deeporigin-0.0.7/tests/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_config.py` & `deeporigin-0.0.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_context.py` & `deeporigin-0.0.7/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_feature_flags.py` & `deeporigin-0.0.7/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.6/tests/test_managed_data.py` & `deeporigin-0.0.7/tests/test_managed_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,16 @@
                 file_id,
                 client=config["client"],
                 destination="non-existent-path",
             )
 
     else:
         _api.download_file(file_id, client=config["client"])
+        data = _api.describe_file(file_id)
+        os.remove(data["name"])
 
 
 def test_describe_file(config):
     file_id = config["file"]["id"]
 
     data = _api.describe_file(file_id, client=config["client"])
```

### Comparing `deeporigin-0.0.6/tests/test_variables.py` & `deeporigin-0.0.7/tests/test_variables.py`

 * *Files identical despite different names*

