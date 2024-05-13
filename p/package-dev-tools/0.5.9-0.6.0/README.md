# Comparing `tmp/package-dev-tools-0.5.9.tar.gz` & `tmp/package_dev_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package-dev-tools-0.5.9.tar", last modified: Sat Feb 24 23:19:41 2024, max compression
+gzip compressed data, was "package_dev_tools-0.6.0.tar", last modified: Mon May 13 06:07:23 2024, max compression
```

## Comparing `package-dev-tools-0.5.9.tar` & `package_dev_tools-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.711881 package-dev-tools-0.5.9/bin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/bin/pre-commit/
--rwxr-xr-x   0 runner    (1001) docker     (127)      269 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/bin/pre-commit/bump-version
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/bin/pre-commit/check-version
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.711881 package-dev-tools-0.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/src/package_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/src/package_dev_tools/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/cleanup_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/cleanup_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/instantiate_new_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/substitute_template_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.715881 package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/sync_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/trigger_template_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/src/package_dev_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/check_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/check_shields.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/cleanup_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/extract_package_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/extract_required_python_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/extract_supported_python_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/instantiate_new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/substitute_template_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/sync_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/cli/trigger_template_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/src/package_dev_tools/models/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/models/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/check_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/check_shields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/src/package_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/utils/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-02-24 23:19:32.000000 package-dev-tools-0.5.9/src/package_dev_tools/utils/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 23:19:41.719882 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-24 23:19:41.000000 package-dev-tools-0.5.9/src/package_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.145450 package_dev_tools-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-13 06:07:23.145450 package_dev_tools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.133450 package_dev_tools-0.6.0/bin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.137450 package_dev_tools-0.6.0/bin/pre-commit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      269 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/bin/pre-commit/bump-version
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/bin/pre-commit/check-version
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:07:23.145450 package_dev_tools-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.133450 package_dev_tools-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.137450 package_dev_tools-0.6.0/src/package_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.137450 package_dev_tools-0.6.0/src/package_dev_tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.137450 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/cleanup_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/cleanup_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/instantiate_new_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/substitute_template_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/sync_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/trigger_template_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/check_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/check_shields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/cleanup_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/extract_package_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/extract_required_python_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/extract_supported_python_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/instantiate_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/substitute_template_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/sync_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/cli/trigger_template_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/models/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/check_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/check_shields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/utils/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-13 06:07:09.000000 package_dev_tools-0.6.0/src/package_dev_tools/utils/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:07:23.141450 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 06:07:23.000000 package_dev_tools-0.6.0/src/package_dev_tools.egg-info/top_level.txt
```

### Comparing `package-dev-tools-0.5.9/LICENSE` & `package_dev_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/PKG-INFO` & `package_dev_tools-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: package-dev-tools
-Version: 0.5.9
+Version: 0.6.0
 Summary: CI/CD tools for Python packages
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/package-dev-tools
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: autotyping<24,>=23.3.0
+Requires-Dist: autotyping<25,>=23.3.0
 Requires-Dist: bump2version<2,>=1.0.1
 Requires-Dist: coverage<8,>=7.4.0
-Requires-Dist: mypy<2,>=1.8.0
-Requires-Dist: package-utils<1,>=0.4.3
+Requires-Dist: mypy<2,>=1.10.0
+Requires-Dist: package-utils<1,>=0.6.1
 Requires-Dist: pre-commit<4,>=3.5.0
+Requires-Dist: powercli<1,>=0.1.2
 Requires-Dist: pygithub<3,>=2.1.1
 Requires-Dist: pytest<9,>=7.4.3
 Requires-Dist: python-slugify<9,>=8.0.1
 Requires-Dist: simple-classproperty<5,>=4.0.2
-Requires-Dist: superpathlib<3,>=1.3.9
+Requires-Dist: superpathlib<3,>=2.0.0
 Requires-Dist: toml<1,>=0.10.2
-Requires-Dist: quinten-cli<2,>=1.1.12
 Provides-Extra: dev
 Requires-Dist: hypothesis<7,>=6.91.0; extra == "dev"
 Requires-Dist: package-dev-utils<1,>=0.1.6; extra == "dev"
 Requires-Dist: types-requests<3,>=2.31.0.10; extra == "dev"
 Requires-Dist: types-toml<1,>=0.10.8.7; extra == "dev"
 
 # Package Dev Tools
 [![PyPI version](https://badge.fury.io/py/package-dev-tools.svg)](https://badge.fury.io/py/package-dev-tools)
 ![Python version](https://img.shields.io/badge/python-3.10+-brightgreen)
 ![Operating system](https://img.shields.io/badge/os-linux%20%7c%20macOS%20%7c%20windows-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Usage
-* Use [actions](https://github.com/quintenroets/package-dev-tools/tree/main/actions) in .github/workflows
-* Use [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in .pre-commit-config.yaml
-
-see [python-package-template](https://github.com/quintenroets/python-package-template) for examples
+Use the [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in your .pre-commit-config.yaml
+* see [.pre-commit-config.yaml](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-config.yaml) for examples
 
 ## Installation
 ```shell
 pip install package-dev-tools
 ```
```

### Comparing `package-dev-tools-0.5.9/README.md` & `package_dev_tools-0.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Package Dev Tools
 [![PyPI version](https://badge.fury.io/py/package-dev-tools.svg)](https://badge.fury.io/py/package-dev-tools)
 ![Python version](https://img.shields.io/badge/python-3.10+-brightgreen)
 ![Operating system](https://img.shields.io/badge/os-linux%20%7c%20macOS%20%7c%20windows-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Usage
-* Use [actions](https://github.com/quintenroets/package-dev-tools/tree/main/actions) in .github/workflows
-* Use [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in .pre-commit-config.yaml
-
-see [python-package-template](https://github.com/quintenroets/python-package-template) for examples
+Use the [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in your .pre-commit-config.yaml
+* see [.pre-commit-config.yaml](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-config.yaml) for examples
 
 ## Installation
 ```shell
 pip install package-dev-tools
 ```
```

### Comparing `package-dev-tools-0.5.9/pyproject.toml` & `package_dev_tools-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "package-dev-tools"
-version = "0.5.9"
+version = "0.6.0"
 description = "CI/CD tools for Python packages"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-    "autotyping >=23.3.0, <24",
+    "autotyping >=23.3.0, <25",
     "bump2version >=1.0.1, <2",
     "coverage >=7.4.0, <8",
-    "mypy >=1.8.0, <2",
-    "package-utils >=0.4.3, <1",
+    "mypy >=1.10.0, <2",
+    "package-utils >=0.6.1, <1",
     "pre-commit >=3.5.0, <4",
+    "powercli >=0.1.2, <1",
     "pygithub >=2.1.1, <3",
     "pytest >=7.4.3, <9",
     "python-slugify >=8.0.1, <9",
     "simple-classproperty >=4.0.2, <5",
-    "superpathlib >=1.3.9, <3",
+    "superpathlib >=2.0.0, <3",
     "toml >=0.10.2, <1",
-    "quinten-cli >=1.1.12, <2",
 ]
 
 [project.optional-dependencies]
 dev = [
     "hypothesis >=6.91.0, <7",
     "package-dev-utils >=0.1.6, <1",
 
@@ -64,27 +64,29 @@
 
 [tool.pytest.ini_options]
 pythonpath = [
     "src", ".",
 ]
 
 [tool.ruff]
+fix = true
+
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "UP",  # pyupgrade
 ]
-fix = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["src"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.setuptools]
 script-files = [
     "bin/pre-commit/bump-version",
     "bin/pre-commit/check-version",
 ]
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/cleanup_readme.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/cleanup_readme.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/cleanup_workflows.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/cleanup_workflows.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/instantiate_new_project.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/instantiate_new_project.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/project.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/project.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/substitute_template_name.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/instantiate_new_project/substitute_template_name/substitute_template_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,10 +85,10 @@
                 self.new_project.package_name,
             )
             renamed_path = Path(renamed_path_str)
             path.rename(renamed_path)
 
     def generate_project_files(self) -> Iterator[Path]:
         command = ("git", "ls-tree", "-r", "HEAD", "--name-only")
-        relative_paths = cli.lines(command, cwd=self.path)
+        relative_paths = cli.capture_output_lines(command, cwd=self.path)
         for path in relative_paths:
             yield self.path / path
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/sync_template.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/sync_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import typing
+from collections.abc import Iterator
 from dataclasses import dataclass, field
 from functools import cached_property
 
 import cli
 import github.Auth
 from github.Commit import Commit
 from github.Repository import Repository
-from plib import Path
+from slugify import slugify
+from superpathlib import Path
 
 from ..instantiate_new_project import ProjectInstantiator
 from ..instantiate_new_project.git import GitInterface
 from ..instantiate_new_project.substitute_template_name import substitute_template_name
 from . import git
 
 
@@ -21,14 +22,26 @@
     template_repository: str = "quintenroets/python-package-template"
     only_latest_commit: bool = True
     default_branch: str = "main"
     update_branch: str = "sync-template"
     downloaded_repository_folder: Path = field(init=False)
     downloaded_template_repository_folder: Path = field(init=False)
 
+    @property
+    def project_name(self) -> str:
+        return self.extract_name(self.repository)
+
+    @property
+    def template_name(self) -> str:
+        return self.extract_name(self.template_repository)
+
+    @classmethod
+    def extract_name(cls, repository: str) -> str:
+        return repository.split("/")[-1]
+
     def run(self) -> None:
         self.downloaded_repository_folder = Path.tempfile(create=False)
         self.downloaded_template_repository_folder = Path.tempfile(create=False)
         paths = (
             self.downloaded_repository_folder,
             self.downloaded_template_repository_folder,
         )
@@ -69,38 +82,30 @@
             is_updated = self.commit_updated_files()
         return is_updated
 
     def extract_template_updates(self) -> str:
         if not self.downloaded_template_repository_folder.exists():
             self.clone_template_repository()
         cwd = self.downloaded_template_repository_folder
-        result = cli.get("git", "diff", "-U0", "HEAD^", "HEAD", cwd=cwd)
-        return typing.cast(str, result)
+        return cli.capture_output("git", "diff", "-U0", "HEAD^", "HEAD", cwd=cwd)
 
     def clone_template_repository(self) -> None:
         url = self.template_repository_client.clone_url
         path = self.downloaded_template_repository_folder
         cli.run("git", "clone", url, path)
 
     def run_git(
         self, *args: str | Path, input_: str | None = None, check: bool = True
     ) -> None:
-        cli.run(
-            "git",
-            *args,
-            input=input_,
-            cwd=self.downloaded_repository_folder,
-            check=check,
-        )
+        cwd = self.downloaded_repository_folder
+        cli.run("git", *args, input=input_, cwd=cwd, check=check)
 
     def instantiate_template(self) -> None:
-        project_name = self.repository.split("/")[-1]
-
         path = substitute_template_name.Path(self.downloaded_template_repository_folder)
-        instantiator = ProjectInstantiator(project_name=project_name, path=path)
+        instantiator = ProjectInstantiator(project_name=self.project_name, path=path)
         instantiator.run()
 
     def pull_template(self) -> None:
         self.run_git("config", "pull.rebase", "false")
         self.configure_git()
         command = (
             "pull",
@@ -115,46 +120,54 @@
         self.run_git(*command)
 
     def commit_updated_files(self) -> bool:
         if self.only_latest_commit:
             self.reset_files_not_in_template_commit()
         self.apply_ignore_patterns()
         self.configure_git()
+        command = "commit", "-m", self.latest_commit.commit.message, "--no-verify"
         try:
-            self.run_git(
-                "commit", "-m", self.latest_commit.commit.message, "--no-verify"
-            )
+            self.run_git(*command)
             is_updated = True
         except cli.CalledProcessError:
             is_updated = False
         return is_updated
 
     def reset_files_not_in_template_commit(self) -> None:
         self.run_git("reset")
+        files = self.generate_instantiated_files_in_template_commit()
+        for file_ in files:
+            self.run_git("add", file_, check=False)
+
+    def generate_instantiated_files_in_template_commit(self) -> Iterator[str]:
+        package_name = slugify(self.project_name, separator="_")
+        template_package_name = slugify(self.template_name, separator="_")
+        for file_ in self.generate_files_in_template_commit():
+            yield file_.replace(template_package_name, package_name)
+
+    def generate_files_in_template_commit(self) -> Iterator[str]:
         for changed_file in self.latest_commit.files:
-            if changed_file.previous_filename:
-                self.run_git("add", changed_file.previous_filename, check=False)
-            self.run_git("add", changed_file.filename, check=False)
+            if changed_file.previous_filename is not None:
+                yield changed_file.previous_filename
+            yield changed_file.filename
 
     def apply_ignore_patterns(self) -> None:
         path = self.downloaded_repository_folder / self.ignore_patterns_path
         if path.exists():
             for pattern in path.lines:
                 if pattern.endswith("/"):
                     pattern = f"{pattern}*"
                 self.run_git("reset", pattern)
 
     def push_updates(self) -> None:
         self.run_git("push", "--set-upstream", "origin", self.update_branch)
+        title = "Sync template changes"
         try:
             self.repository_client.create_pull(
-                self.default_branch,
-                self.update_branch,
-                title="Sync template changes",
-                body="",
+                self.default_branch, self.update_branch, title=title, body=""
             )
         except github.GithubException:
             pass  # Pull request already created
 
     @cached_property
     def repository_client(self) -> Repository:
         return self.client.get_repo(self.repository)
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/actions/template_sync/trigger_template_sync.py` & `package_dev_tools-0.6.0/src/package_dev_tools/actions/template_sync/trigger_template_sync.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/models/path.py` & `package_dev_tools-0.6.0/src/package_dev_tools/models/path.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-
 from typing import TypeVar
 
-import plib
+import superpathlib
 from simple_classproperty import classproperty
 
 T = TypeVar("T", bound="Path")
 
 
-class Path(plib.Path):
-    @classproperty
-    def readme(cls: type[T]) -> T:  # type: ignore
-        return cls("README.md")
-
-    @classproperty
-    def workflows(cls: type[T]) -> T:  # type: ignore
-        return cls(".github") / "workflows"
-
+class Path(superpathlib.Path):
     @property
     def has_text_content(self) -> bool:
         try:
             self.text
             has_text = True
         except UnicodeDecodeError:
             has_text = False
         return has_text
+
+    @classmethod
+    @classproperty
+    def readme(cls: type[T]) -> T:
+        return cls("README.md")
+
+    @classmethod
+    @classproperty
+    def workflows(cls: type[T]) -> T:
+        return cls(".github") / "workflows"
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/check_coverage.py` & `package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/check_coverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import sys
-import typing
 from collections.abc import Iterator
 
 import cli
 
 from ..models import Path
 from ..utils.badge import Badge, BadgeUpdater
 
 
 def check_coverage(verify_all_files_tested: bool = True) -> None:
     verify_coverage_results()
     if verify_all_files_tested:
         verify_all_python_files_tested()
 
     try:
-        coverage_percentage = cli.get("coverage report --format total")
-    except cli.exceptions.CalledProcessError as exception:
-        cli.get("coverage html", check=False)
+        coverage_percentage = cli.capture_output("coverage report -i --format total")
+    except cli.CalledProcessError as exception:
+        cli.capture_output("coverage html -i", check=False)
+        cli.run("coverage report -mi", check=False)
         raise exception
-    coverage_percentage = typing.cast(str, coverage_percentage)
     coverage_percentage_has_changed = update_coverage_shield(coverage_percentage)
     if coverage_percentage_has_changed:
         print(f"Updated test coverage: {coverage_percentage}%")
-        cli.get("coverage html")
+        cli.capture_output("coverage html")
     exit_code = 1 if coverage_percentage_has_changed else 0
     sys.exit(exit_code)
 
 
 def update_coverage_shield(coverage_percentage: float | str) -> bool:
     if isinstance(coverage_percentage, str):
         coverage_percentage = float(coverage_percentage)
     coverage_percentage_int = round(coverage_percentage)
     badge = Badge("Coverage", f"coverage-{coverage_percentage_int}%25")
     return BadgeUpdater(badge).run()
 
 
 def verify_all_python_files_tested() -> None:
     python_files = set(generate_python_files())
-    coverage_lines = cli.lines("coverage report", check=False)
+    coverage_lines = cli.capture_output_lines("coverage report -i", check=False)
     covered_files = set(line.split()[0] for line in coverage_lines[2:-2])
     not_covered_files = python_files - covered_files
     if not_covered_files:
+        cli.run("coverage html -i", check=False)
         message_parts = (
             "The following files are not covered by tests:",
             *not_covered_files,
         )
         message = "\n\t".join(message_parts)
         raise Exception(message)
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/pre_commit/check_shields.py` & `package_dev_tools-0.6.0/src/package_dev_tools/pre_commit/check_shields.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/utils/badge.py` & `package_dev_tools-0.6.0/src/package_dev_tools/utils/badge.py`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools/utils/package.py` & `package_dev_tools-0.6.0/src/package_dev_tools/utils/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from collections.abc import Iterator
 from dataclasses import dataclass, field
 from typing import Any, ClassVar
 
 import requests
 import toml
-from plib import Path
+from superpathlib import Path
 
 
 @dataclass
 class PackageInfo:
     path: Path = field(default_factory=Path.cwd)
     os_mapper: ClassVar[dict[str, str]] = {"ubuntu": "linux", "macos": "macOS"}
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools.egg-info/PKG-INFO` & `package_dev_tools-0.6.0/src/package_dev_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: package-dev-tools
-Version: 0.5.9
+Version: 0.6.0
 Summary: CI/CD tools for Python packages
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/package-dev-tools
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: autotyping<24,>=23.3.0
+Requires-Dist: autotyping<25,>=23.3.0
 Requires-Dist: bump2version<2,>=1.0.1
 Requires-Dist: coverage<8,>=7.4.0
-Requires-Dist: mypy<2,>=1.8.0
-Requires-Dist: package-utils<1,>=0.4.3
+Requires-Dist: mypy<2,>=1.10.0
+Requires-Dist: package-utils<1,>=0.6.1
 Requires-Dist: pre-commit<4,>=3.5.0
+Requires-Dist: powercli<1,>=0.1.2
 Requires-Dist: pygithub<3,>=2.1.1
 Requires-Dist: pytest<9,>=7.4.3
 Requires-Dist: python-slugify<9,>=8.0.1
 Requires-Dist: simple-classproperty<5,>=4.0.2
-Requires-Dist: superpathlib<3,>=1.3.9
+Requires-Dist: superpathlib<3,>=2.0.0
 Requires-Dist: toml<1,>=0.10.2
-Requires-Dist: quinten-cli<2,>=1.1.12
 Provides-Extra: dev
 Requires-Dist: hypothesis<7,>=6.91.0; extra == "dev"
 Requires-Dist: package-dev-utils<1,>=0.1.6; extra == "dev"
 Requires-Dist: types-requests<3,>=2.31.0.10; extra == "dev"
 Requires-Dist: types-toml<1,>=0.10.8.7; extra == "dev"
 
 # Package Dev Tools
 [![PyPI version](https://badge.fury.io/py/package-dev-tools.svg)](https://badge.fury.io/py/package-dev-tools)
 ![Python version](https://img.shields.io/badge/python-3.10+-brightgreen)
 ![Operating system](https://img.shields.io/badge/os-linux%20%7c%20macOS%20%7c%20windows-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
 
 ## Usage
-* Use [actions](https://github.com/quintenroets/package-dev-tools/tree/main/actions) in .github/workflows
-* Use [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in .pre-commit-config.yaml
-
-see [python-package-template](https://github.com/quintenroets/python-package-template) for examples
+Use the [pre-commit hooks](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-hooks.yaml) in your .pre-commit-config.yaml
+* see [.pre-commit-config.yaml](https://github.com/quintenroets/package-dev-tools/tree/main/.pre-commit-config.yaml) for examples
 
 ## Installation
 ```shell
 pip install package-dev-tools
 ```
```

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools.egg-info/SOURCES.txt` & `package_dev_tools-0.6.0/src/package_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `package-dev-tools-0.5.9/src/package_dev_tools.egg-info/entry_points.txt` & `package_dev_tools-0.6.0/src/package_dev_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

