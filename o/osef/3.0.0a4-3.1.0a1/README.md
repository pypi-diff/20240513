# Comparing `tmp/osef-3.0.0a4.tar.gz` & `tmp/osef-3.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osef-3.0.0a4.tar", last modified: Wed Dec 20 13:57:04 2023, max compression
+gzip compressed data, was "osef-3.1.0a1.tar", last modified: Mon May 13 09:33:48 2024, max compression
```

## Comparing `osef-3.0.0a4.tar` & `osef-3.1.0a1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.612485 osef-3.0.0a4/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-12-14 10:31:13.000000 osef-3.0.0a4/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-12-15 16:29:51.000000 osef-3.0.0a4/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.528478 osef-3.0.0a4/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.568482 osef-3.0.0a4/.gitlab/merge_request_templates/
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-12-14 10:31:13.000000 osef-3.0.0a4/.gitlab/merge_request_templates/Default.md
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-12-15 16:29:51.000000 osef-3.0.0a4/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.588483 osef-3.0.0a4/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-12-14 10:31:13.000000 osef-3.0.0a4/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     9974 2023-12-18 13:59:12.000000 osef-3.0.0a4/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-12-14 10:31:13.000000 osef-3.0.0a4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-12-15 16:29:51.000000 osef-3.0.0a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1998 2023-12-20 13:57:04.612485 osef-3.0.0a4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-12-15 16:29:51.000000 osef-3.0.0a4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-12-14 10:31:13.000000 osef-3.0.0a4/RELEASE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.604485 osef-3.0.0a4/devops/
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-12-15 16:29:51.000000 osef-3.0.0a4/devops/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.604485 osef-3.0.0a4/devops/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2821 2023-12-15 16:29:51.000000 osef-3.0.0a4/devops/CI/deploy.yml
--rwxrwxrwx   0 root         (0) root         (0)      329 2023-12-15 16:29:51.000000 osef-3.0.0a4/devops/local_lint.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.604485 osef-3.0.0a4/osef/
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-12-14 10:31:13.000000 osef-3.0.0a4/osef/_logger.py
--rw-r--r--   0 root         (0) root         (0)      413 2023-12-20 13:57:03.000000 osef-3.0.0a4/osef/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.608485 osef-3.0.0a4/osef/frame_helper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-20 13:56:27.000000 osef-3.0.0a4/osef/frame_helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/frame_helper/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3822 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/frame_helper/field_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     9303 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/frame_helper/frame_edition.py
--rw-rw-rw-   0 root         (0) root         (0)    20679 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/frame_helper/osef_frame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.608485 osef-3.0.0a4/osef/packing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-20 13:56:27.000000 osef-3.0.0a4/osef/packing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3499 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/packing/packer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.608485 osef-3.0.0a4/osef/parsing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-20 13:56:27.000000 osef-3.0.0a4/osef/parsing/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6741 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/_lazy_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     5886 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/_parser_common.py
--rwxrwxrwx   0 root         (0) root         (0)     7818 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/osef_stream.py
--rwxrwxrwx   0 root         (0) root         (0)     6552 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2628 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/parsing/scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.612485 osef-3.0.0a4/osef/spec/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-20 13:56:27.000000 osef-3.0.0a4/osef/spec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/spec/_formats.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/spec/_packers.py
--rw-rw-rw-   0 root         (0) root         (0)    12598 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/spec/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     3315 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/spec/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    47959 2023-12-15 16:29:51.000000 osef-3.0.0a4/osef/spec/osef_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 13:57:04.612485 osef-3.0.0a4/osef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1998 2023-12-20 13:57:03.000000 osef-3.0.0a4/osef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      982 2023-12-20 13:57:04.000000 osef-3.0.0a4/osef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-20 13:57:03.000000 osef-3.0.0a4/osef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-12-20 13:57:03.000000 osef-3.0.0a4/osef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-12-20 13:57:03.000000 osef-3.0.0a4/osef.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1021 2023-12-18 13:59:12.000000 osef-3.0.0a4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-20 13:57:04.612485 osef-3.0.0a4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-12-15 16:29:51.000000 osef-3.0.0a4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-12-15 16:29:51.000000 osef-3.0.0a4/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.980080 osef-3.1.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-13 09:29:38.000000 osef-3.1.0a1/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-05-13 09:29:38.000000 osef-3.1.0a1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.972080 osef-3.1.0a1/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.972080 osef-3.1.0a1/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-05-13 09:29:38.000000 osef-3.1.0a1/.gitlab/merge_request_templates/Default.md
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2024-05-13 09:29:38.000000 osef-3.1.0a1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.972080 osef-3.1.0a1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-13 09:29:38.000000 osef-3.1.0a1/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2024-05-13 09:29:38.000000 osef-3.1.0a1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2024-05-13 09:29:38.000000 osef-3.1.0a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-13 09:29:38.000000 osef-3.1.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-05-13 09:33:48.980080 osef-3.1.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2024-05-13 09:29:38.000000 osef-3.1.0a1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-05-13 09:29:38.000000 osef-3.1.0a1/RELEASE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.972080 osef-3.1.0a1/devops/
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2024-05-13 09:29:38.000000 osef-3.1.0a1/devops/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.972080 osef-3.1.0a1/devops/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2024-05-13 09:29:38.000000 osef-3.1.0a1/devops/CI/deploy.yml
+-rwxrwxrwx   0 root         (0) root         (0)      329 2024-05-13 09:29:38.000000 osef-3.1.0a1/devops/local_lint.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.976080 osef-3.1.0a1/osef/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/_logger.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.976080 osef-3.1.0a1/osef/frame_helper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 09:33:42.000000 osef-3.1.0a1/osef/frame_helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/frame_helper/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/frame_helper/field_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/frame_helper/frame_edition.py
+-rw-rw-rw-   0 root         (0) root         (0)    22222 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/frame_helper/osef_frame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.976080 osef-3.1.0a1/osef/packing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 09:33:42.000000 osef-3.1.0a1/osef/packing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/packing/packer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.976080 osef-3.1.0a1/osef/parsing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 09:33:42.000000 osef-3.1.0a1/osef/parsing/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6741 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/_lazy_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     5886 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/_parser_common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8070 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/osef_stream.py
+-rwxrwxrwx   0 root         (0) root         (0)     6552 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/parsing/scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.980080 osef-3.1.0a1/osef/spec/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 09:33:42.000000 osef-3.1.0a1/osef/spec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/spec/_formats.py
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/spec/_packers.py
+-rw-rw-rw-   0 root         (0) root         (0)    13919 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/spec/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/spec/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    53406 2024-05-13 09:29:38.000000 osef-3.1.0a1/osef/spec/osef_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:33:48.980080 osef-3.1.0a1/osef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      982 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-13 09:33:48.000000 osef-3.1.0a1/osef.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-13 09:29:38.000000 osef-3.1.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:33:48.980080 osef-3.1.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-13 09:29:38.000000 osef-3.1.0a1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-13 09:29:38.000000 osef-3.1.0a1/test_requirements.txt
```

### Comparing `osef-3.0.0a4/.gitlab-ci.yml` & `osef-3.1.0a1/.gitlab-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 # CI file for OSEF Library
 
 variables:
   DOCKER_CACHE_REGISTRY: registry-cache-docker.berite.outsig.ht/
   GITLAB_CACHE_REGISTRY: registry-cache-gitlab.berite.outsig.ht/
 
+default:
+  image: ${DOCKER_CACHE_REGISTRY}library/python:3.8
+  tags: ['amd64-build']
+
+workflow:
+  auto_cancel:
+    on_new_commit: interruptible
+  rules:
+    - if: $CI_MERGE_REQUEST_ID
+      when: never
+    - if: $CI_COMMIT_REF_PROTECTED == 'true'
+      auto_cancel:
+        on_new_commit: none
+    - when: always
 
 # Define CI stages.
 stages:
   - format
   - test
   - coverage
   - deploy
@@ -19,16 +33,14 @@
 
 #######################################################
 # BASE: Python base job
 #######################################################
 .python_base:
   # Change pip's cache directory to be inside the project directory since we can
   # only cache local items.
-  image: ${DOCKER_CACHE_REGISTRY}library/python:3.8
-  tags: [amd64-build]
   before_script:
     - python -V  # Print out python version for debugging
     - pip install -r test_requirements.txt
     - pip install .
 
 
 # Format all python code
```

### Comparing `osef-3.0.0a4/CHANGELOG.md` & `osef-3.1.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## Unreleased
+
+## [3.1.0a1] - 2023-05-7
+
+### Added
+
+- Added vectorialized `remove_objects` function
+- Added Socket host and port information to OsefStream exceptions
+
+### Changed
+
+- OSEF spec `1.17.0`
+
+## [3.0.0] - 2023-02-15
+
+### Fixed
+- `remove_object` now tolerates OSEF with an AugmentedCloud which has no object_id_32_bits field.
+- Documentation CI job now has a valid image/tag
+
+### Added
+- Support for `TIME_INTERVAL`, `TIME_DOMAIN`, `START_TIMESTAMP` and `END_TIMESTAMP`
+- Support for `CLASSIFICATION_CONFIDENCE`, `CLASS_PROBABILITIES`, `CLASSIFIER_DEF` and `ENABLED_CLASS_IDS`
+- Properties for speed norms and rotation matrices in the TrackedObjects class
+- Support for `CLASSIFICATION_CONFIDENCE` in osef_frame and field_classes submodules
+
 ## [3.0.0a4] - 2023-12-18
 
 ### Fixed
 - Fixed pyproject.toml packaging.
 
 ## [3.0.0a3] - 2023-12-18
```

### Comparing `osef-3.0.0a4/LICENSE` & `osef-3.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/PKG-INFO` & `osef-3.1.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osef
-Version: 3.0.0a4
+Version: 3.1.0a1
 Summary: Osef python library.
 Author-email: Outsight Developpers <support@outsight.tech>
 Project-URL: Documentation, https://outsight-tech.gitlab.io/common/osef-python-library/
 Project-URL: Support, https://support.outsight.ai
 Project-URL: Changes, https://outsight-tech.gitlab.io/common/osef-python-library/CHANGELOG.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `osef-3.0.0a4/README.md` & `osef-3.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/devops/.pylintrc` & `osef-3.1.0a1/devops/.pylintrc`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/devops/CI/deploy.yml` & `osef-3.1.0a1/devops/CI/deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,14 @@
       else
         echo "Changelog invalid for $version"
         false
       fi
 
 # Deploy python OSEF library publicly after tagging.
 deploy_osef_library:
-  image: ${DOCKER_CACHE_REGISTRY}library/python:3.8
-  tags: [amd64-build]
   stage: deploy
   rules:
     - if: '$CI_COMMIT_TAG =~ /^\d+\.\d+\.\d+((a|b|rc)\d+)?$/'
   needs: ["check_changelog"]
   before_script:
     # Install Git LFS.
     - apt-get update && apt-get install -y git-lfs
```

### Comparing `osef-3.0.0a4/osef/frame_helper/exceptions.py` & `osef-3.1.0a1/osef/frame_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/frame_helper/field_classes.py` & `osef-3.1.0a1/osef/frame_helper/field_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     speed_vector: npt.NDArray[np.float32]
     bbox_size: npt.NDArray[np.float32]
     translation: npt.NDArray[np.float32]
     rotation: npt.NDArray[np.float32]
     properties: Optional[ObjectProperties] = None
     geographic_pose: Optional[GeographicPose] = None
     geographic_speed: Optional[GeographicSpeed] = None
+    classification_confidence: Optional[np.float32] = None
 
     @property
     def class_name(self) -> str:
         """Name of the object class."""
         return osef_types.ClassId(self.class_id).name
 
     @property
```

### Comparing `osef-3.0.0a4/osef/frame_helper/frame_edition.py` & `osef-3.1.0a1/osef/frame_helper/frame_edition.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,37 +181,86 @@
 
     # Remove zone bindings before removing the ID.
     if OsefKeys.ZONES_OBJECTS_BINDING_32_BITS in _get_scan_frame_dict(frame_dict):
         remove_object_binding(frame_dict, object_id)
 
     # Remove all data related to the object.
     for tracked_objects_key, tracked_object_field in tracked_object_dict.items():
-        # Warning: All fields of the augmented cloud will be filtered
+        # Warning: All fields of the tracked objects will be filtered
         if isinstance(tracked_object_field, np.ndarray):
             new_field_value = np.delete(
                 tracked_object_dict[tracked_objects_key], object_indices, axis=0
             )
             set_tracked_objects_field(frame_dict, tracked_objects_key, new_field_value)
 
     # Set the object ID to 0 in the augmented cloud
-    if (aug_cloud_dict := _get_aug_cloud_dict(frame_dict)) is not None:
-        object_mask = aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS.value] == object_id
+    if (
+        aug_cloud_dict := _get_aug_cloud_dict(frame_dict)
+    ) is not None and OsefKeys.OBJECT_ID_32_BITS in aug_cloud_dict:
+        object_mask = aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS] == object_id
 
         # Check if the augmented_cloud field is writeable, else make a copy
         new_object_ids = (
             aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS]
             if aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS].flags.writeable
             else np.copy(aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS])
         )
         new_object_ids[object_mask] = 0
         set_augmented_cloud_field(
             frame_dict, OsefKeys.OBJECT_ID_32_BITS, new_object_ids
         )
 
 
+def remove_objects(frame_dict: dict, mask: npt.NDArray[np.bool_]) -> None:
+    """Remove tracked objects from an OSEF frame.
+
+    :param frame_dict: OSEF frame dictionary to edit.
+    :param mask: mask of object to keep (False: remove object, True: keep object)
+    """
+    tracked_object_dict = _get_tracked_objects_dict(frame_dict)
+
+    if mask.size != tracked_object_dict[OsefKeys.NUMBER_OF_OBJECTS]:
+        raise ValueError("Given mask must be of size number_of_objects")
+
+    # Update the number of objects.
+    tracked_object_dict[OsefKeys.NUMBER_OF_OBJECTS] = np.count_nonzero(mask)
+
+    # Remove zone bindings before removing the ID.
+    if OsefKeys.ZONES_OBJECTS_BINDING_32_BITS in _get_scan_frame_dict(frame_dict):
+        for object_id in tracked_object_dict[OsefKeys.OBJECT_ID_32_BITS][mask]:
+            remove_object_binding(frame_dict, object_id)
+
+    # Set the object ID to 0 in the augmented cloud
+    if (
+        aug_cloud_dict := _get_aug_cloud_dict(frame_dict)
+    ) is not None and OsefKeys.OBJECT_ID_32_BITS in aug_cloud_dict:
+        object_mask = np.isin(
+            aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS],
+            np.invert(tracked_object_dict[OsefKeys.OBJECT_ID_32_BITS][mask]),
+        )
+
+        # Check if the augmented_cloud field is writeable, else make a copy
+        new_object_ids = (
+            aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS]
+            if aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS].flags.writeable
+            else np.copy(aug_cloud_dict[OsefKeys.OBJECT_ID_32_BITS])
+        )
+        new_object_ids[object_mask] = 0
+        set_augmented_cloud_field(
+            frame_dict, OsefKeys.OBJECT_ID_32_BITS, new_object_ids
+        )
+
+    # Remove all data related to the object.
+    for tracked_objects_key, tracked_object_field in tracked_object_dict.items():
+        # Warning: All fields of the tracked objects will be filtered
+        if isinstance(tracked_object_field, np.ndarray):
+            new_field_value = tracked_object_dict[tracked_objects_key][mask]
+            set_tracked_objects_field(frame_dict, tracked_objects_key, new_field_value)
+
+
 def remove_object_binding(frame_dict: Dict, object_id: int) -> None:
     """Remove zone-object bindings of a given object ID.
 
     :param frame_dict: OSEF frame dictionary to edit.
     :param object_id: ID of the object to remove from the zone binding field.
     """
     tracked_object_dict = _get_tracked_objects_dict(frame_dict)
```

### Comparing `osef-3.0.0a4/osef/frame_helper/osef_frame.py` & `osef-3.1.0a1/osef/frame_helper/osef_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,23 @@
         return [ClassId(class_id).name for class_id in self.class_ids]
 
     @property
     def speed_vectors(self) -> npt.NDArray[np.float32]:
         """Get numpy array of object speeds."""
         return self._tracked_objects.get(OsefKeys.SPEED_VECTORS)
 
+    # TODO. Make this kind of properties lazy.
+    @property
+    def speed_norms(self) -> npt.NDArray[np.float32]:
+        """Get the array of speed norms of each tracked object.
+
+        The 3 components of the speed vector are used to compute the speed norm.
+        """
+        return np.linalg.norm(self.speed_vectors, axis=1)
+
     @property
     def poses(self) -> List[Pose]:
         """Get object poses."""
         pose_array_values = self._tracked_objects.get(OsefKeys.POSE_ARRAY)
         translations, rotations = _build_pose_array(pose_array_values)
         return [
             Pose(translation, rotation)
@@ -274,14 +283,23 @@
     @property
     def position_vectors(self) -> npt.NDArray[np.float32]:
         """Get numpy array of object positions."""
         pose_array_values = self._tracked_objects.get(OsefKeys.POSE_ARRAY)
         return pose_array_values[:, :3]
 
     @property
+    def rotation_matrices(self) -> npt.NDArray[np.float32]:
+        """
+        Get array of rotation matrices for each tracked object
+        The output array has a shape (N, 3, 3) for N tracked objects.
+        """
+        pose_array_values = self._tracked_objects.get(OsefKeys.POSE_ARRAY)
+        return _build_rotations(pose_array_values)
+
+    @property
     def slam_poses(self) -> Optional[List[Pose]]:
         """Get object poses from SLAM."""
         if (
             slam_pose_values := self._tracked_objects.get(
                 OsefKeys.SLAM_POSE_ARRAY.value
             )
         ) is None:
@@ -344,14 +362,19 @@
                     :, constants.ObjectPropertiesIndexes.HAS_VALID_SLAM_POSE
                 ],
                 property_values[:, constants.ObjectPropertiesIndexes.IS_STATIC],
             )
         ]
 
     @property
+    def classification_confidence(self) -> Optional[npt.NDArray[np.float32]]:
+        """Get the classification confidence."""
+        return self._tracked_objects.get(OsefKeys.CLASSIFICATION_CONFIDENCE)
+
+    @property
     def bbox_footprint_vertices(self) -> npt.NDArray[np.float32]:
         """Get the coordinates of the projected bounding boxes.
 
         The output array has a shape of (N, 4, 2) with 4 2D-vertices for each object.
         Note that all bounding boxes will be considered as a cuboid.
         """
         num_of_vertices = 4
@@ -439,37 +462,44 @@
             [self.geographic_poses, self.geographic_speeds]
             if (
                 OsefKeys.GEOGRAPHIC_POSE_ARRAY in self._tracked_objects
                 and OsefKeys.GEOGRAPHIC_SPEED_ARRAY in self._tracked_objects
             )
             else [np.full(self.number_of_objects, None)] * 2
         )
+        object_fields += (
+            [self.classification_confidence]
+            if OsefKeys.CLASSIFICATION_CONFIDENCE in self._tracked_objects
+            else [np.full(self.number_of_objects, None)]
+        )
 
         return [
             TrackedObjectData(
                 object_id,
                 class_id,
                 speed_vector,
                 bbox,
                 translation,
                 rotation,
                 properties,
                 geographic_pose,
                 geographic_speed,
+                classification_confidence,
             )
             for (
                 object_id,
                 class_id,
                 speed_vector,
                 bbox,
                 translation,
                 rotation,
                 properties,
                 geographic_pose,
                 geographic_speed,
+                classification_confidence,
             ) in zip(
                 *object_fields
                 if condition is None
                 else (_filter_field(field, condition) for field in object_fields)
             )
         ]
 
@@ -566,21 +596,32 @@
     :param pose_values: raw pose values defined as Tx Ty Tz Vxx Vyx Vzx Vxy Vyy Vzy Vxz Vyz Vzz
     :return: position vector
     :return: rotation matrix
     """
     return pose_values[:3], np.transpose(np.reshape(pose_values[3:], (3, 3)))
 
 
+def _build_rotations(
+    pose_array: npt.NDArray[np.float32],
+) -> npt.NDArray[np.float32]:
+    """Build rotations of an array of poses from the raw values.
+
+    :param pose_values: array of raw pose values of shape (N, 12)
+    :return: array of rotation matrices of shape (N, 3, 3)
+    """
+    return np.transpose(
+        np.reshape(pose_array[:, 3:], (len(pose_array), 3, 3)), axes=(0, 2, 1)
+    )
+
+
 def _build_pose_array(
     pose_array: npt.NDArray[np.float32],
 ) -> Tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
     """Build tranlsation and rotation of an array of poses from the raw values.
 
     :param pose_values: array of raw pose values of shape (N, 12)
     :return: array of position vectors of shape (N, 3)
     :return: array of rotation matrices of shape (N, 3, 3)
     """
     translations = pose_array[:, :3]
-    rotations = np.transpose(
-        np.reshape(pose_array[:, 3:], (len(pose_array), 3, 3)), axes=(0, 2, 1)
-    )
+    rotations = _build_rotations(pose_array)
     return translations, rotations
```

### Comparing `osef-3.0.0a4/osef/packing/packer.py` & `osef-3.1.0a1/osef/packing/packer.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/parsing/_lazy_parser.py` & `osef-3.1.0a1/osef/parsing/_lazy_parser.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/parsing/_parser.py` & `osef-3.1.0a1/osef/parsing/_parser.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/parsing/_parser_common.py` & `osef-3.1.0a1/osef/parsing/_parser_common.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/parsing/osef_stream.py` & `osef-3.1.0a1/osef/parsing/osef_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,23 +104,29 @@
         :param size: of binary value to be read
         :raises EOFError: if no value can be read or if it is empty.
         :raises OsefConnectionException: If no TCP socket.
         :return: Read binary value
         """
         msg = b""
         if self._tcp_socket is None:
-            raise OsefConnectionException("TCP socket has not been initialized")
+            raise OsefConnectionException(
+                f"TCP socket ({self._path.netloc}) has not been initialized"
+            )
 
         try:
             msg = self._tcp_socket.recv(size)
         except socket.timeout:
-            osef_logger.warning("Received timeout. Closing socket.")
+            osef_logger.warning(
+                f"Received timeout. Closing socket ({self._path.netloc})."
+            )
             self.disconnect()
         except ConnectionResetError:
-            osef_logger.warning("Socket reset error. Closing socket.")
+            osef_logger.warning(
+                f"Socket reset error. Closing socket ({self._path.netloc})."
+            )
             self.disconnect()
         return msg
 
     def connect(self) -> None:
         """Try to open the socket
 
         :raises OsefConnectionException: if the connection failed.
@@ -131,15 +137,15 @@
             self._tcp_socket.connect((self._path.hostname, self._path.port or 11120))
             osef_logger.warning(
                 "Connected to %s:%d",
                 self._path.hostname,
                 self._path.port or 11120,
             )
         except OSError as exp:
-            raise OsefConnectionException(exp) from exp
+            raise OsefConnectionException(f"{exp} ({self._path.netloc})") from exp
 
     def disconnect(self) -> None:
         """Close the socket"""
         if self._tcp_socket is not None:
             self._tcp_socket.close()
 
     def open_socket(
@@ -204,15 +210,15 @@
         :raises OsefConnectionException: if the file could not be opened.
         """
         try:
             self._io_stream = open(  # pylint: disable=consider-using-with
                 self._path, "rb"
             )
         except OSError as exp:
-            raise OsefConnectionException(exp) from exp
+            raise OsefConnectionException(f"{exp} ({self._path})") from exp
 
     def disconnect(self) -> None:
         """Close the file"""
         if self._io_stream is not None:
             self._io_stream.close()
 
     def __enter__(self) -> OsefStreamFile:
@@ -230,10 +236,12 @@
         :param size: of binary value to be read
         :raises EOFError: if no value can be read or if it is empty.
         :raises OsefConnectionException: IOStream not opened.
         :return: Read binary value
         """
 
         if self._io_stream is None:
-            raise OsefConnectionException("File IOStream has not been opened")
+            raise OsefConnectionException(
+                f"File IOStream has not been opened ({self._path})"
+            )
 
         return self._io_stream.read(size)
```

### Comparing `osef-3.0.0a4/osef/parsing/parser.py` & `osef-3.1.0a1/osef/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/parsing/scanner.py` & `osef-3.1.0a1/osef/parsing/scanner.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/spec/_formats.py` & `osef-3.1.0a1/osef/spec/_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import numpy as np
 
 # Project imports
 from osef.spec import constants
 
 
 class BinaryValueFormat:
-    """Class to define the bynary format for reading values."""
+    """Class to define the binary format for reading values."""
 
     NB_POINTS = "<L"
     NB_OBJECTS = "<L"
     NB_LAYERS = "<L"
     LIDAR_MODEL = "<B"
     DIVERGENCE = "<f"
     COORDINATES_REFERENCE_SYSTEM = "<B"
+    TIME_DOMAIN = "<L"
 
 
 # Define format for dictionary values.
 # First value is the binary format, then the dict keys.
 ImageDimensionDictFormat = (
     "<LL",
     [constants.ExtraOsefKeys.IMAGE_WIDTH, constants.ExtraOsefKeys.IMAGE_HEIGHT],
```

### Comparing `osef-3.0.0a4/osef/spec/_packers.py` & `osef-3.1.0a1/osef/spec/_packers.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,30 +166,48 @@
 
         return _parse_dict
 
 
 class TimestampPacker(PackerBase):
     """Derived class to pack/unpack timestamp."""
 
-    def __init__(self) -> None:
-        """Constructor."""
+    def __init__(self, sub_seconds_order: int) -> None:
+        """
+        Constructor.
+        `sub_seconds_order` is the order (power of 10) associated to the time decimals.
+        """
         super().__init__()
-        self.pack = TimestampPacker._timestamp_packer
-        self.unpack = TimestampPacker._timestamp_unpacker
+        self.sub_seconds_order = sub_seconds_order
+        self.pack = self._timestamp_packer
+        self.unpack = self._timestamp_unpacker
 
-    @staticmethod
-    def _timestamp_packer(value: float) -> bytes:
+    def _timestamp_packer(self, value: float) -> bytes:
         seconds = int(value)
-        micro_seconds = int(round((value - seconds) * 10**6))
-        return Struct("<LL").pack(seconds, micro_seconds)
+        sub_seconds = int(round((value - seconds) * 10**self.sub_seconds_order))
+        return Struct("<LL").pack(seconds, sub_seconds)
+
+    def _timestamp_unpacker(self, value: bytes) -> float:
+        seconds, sub_seconds = Struct("<LL").unpack(value)
+        return seconds + sub_seconds * 10**-self.sub_seconds_order
+
+
+class TimestampMicroPacker(TimestampPacker):
+    """Derived class to pack/unpack timestamp using microseconds."""
+
+    def __init__(self) -> None:
+        """Constructor."""
+        super().__init__(6)
+
 
-    @staticmethod
-    def _timestamp_unpacker(value: bytes) -> float:
-        seconds, micro_seconds = Struct("<LL").unpack(value)
-        return seconds + micro_seconds * 10**-6
+class TimestampNanoPacker(TimestampPacker):
+    """Derived class to pack/unpack timestamp using nanoseconds."""
+
+    def __init__(self) -> None:
+        """Constructor."""
+        super().__init__(9)
 
 
 class ProcessingBitfieldPacker(PackerBase):
     """Derived class for pack/unpack processing bitfield."""
 
     def __init__(self) -> None:
         """Constructor."""
```

### Comparing `osef-3.0.0a4/osef/spec/_types.py` & `osef-3.1.0a1/osef/spec/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     OsefTypes.NUMBER_OF_OBJECTS: TypeInfo(
         OsefKeys.NUMBER_OF_OBJECTS,
         _packers.ValuePacker(_formats.BinaryValueFormat.NB_OBJECTS),
     ),
     OsefTypes._CLOUD_FRAME: TypeInfo(OsefKeys._CLOUD_FRAME, InternalNodeInfo(dict)),
     OsefTypes.TIMESTAMP_MICROSECOND: TypeInfo(
         OsefKeys.TIMESTAMP_MICROSECOND,
-        _packers.TimestampPacker(),
+        _packers.TimestampMicroPacker(),
     ),
     OsefTypes._AZIMUTHS_COLUMN: TypeInfo(
         OsefKeys._AZIMUTHS_COLUMN,
         _packers.ArrayPacker(np.dtype(np.float32)),
     ),
     OsefTypes.NUMBER_OF_LAYERS: TypeInfo(
         OsefKeys.NUMBER_OF_LAYERS,
@@ -321,14 +321,50 @@
         OsefKeys._CYLINDRICAL_COVARIANCE,
         _packers.ArrayPacker(np.dtype(np.float32)),
     ),
     OsefTypes.COORDINATES_REFERENCE_SYSTEM: TypeInfo(
         OsefKeys.COORDINATES_REFERENCE_SYSTEM,
         _packers.ValuePacker(_formats.BinaryValueFormat.COORDINATES_REFERENCE_SYSTEM),
     ),
+    OsefTypes.START_TIMESTAMP: TypeInfo(
+        OsefKeys.START_TIMESTAMP,
+        _packers.TimestampNanoPacker(),
+    ),
+    OsefTypes.END_TIMESTAMP: TypeInfo(
+        OsefKeys.END_TIMESTAMP,
+        _packers.TimestampNanoPacker(),
+    ),
+    OsefTypes.TIME_DOMAIN: TypeInfo(
+        OsefKeys.TIME_DOMAIN,
+        _packers.ValuePacker(_formats.BinaryValueFormat.TIME_DOMAIN),
+    ),
+    OsefTypes.TIME_INTERVAL: TypeInfo(OsefKeys.TIME_INTERVAL, InternalNodeInfo(dict)),
+    OsefTypes.CLASSIFICATION_CONFIDENCE: TypeInfo(
+        OsefKeys.CLASSIFICATION_CONFIDENCE,
+        _packers.ArrayPacker(np.dtype(np.float32)),
+    ),
+    OsefTypes._CLASS_PROBABILITIES_ARRAY: TypeInfo(
+        OsefKeys._CLASS_PROBABILITIES_ARRAY,
+        _packers.ArrayPacker(np.dtype(np.float32)),
+    ),
+    OsefTypes._CLASSIFIER_DEF: TypeInfo(
+        OsefKeys._CLASSIFIER_DEF, InternalNodeInfo(dict)
+    ),
+    OsefTypes._ENABLED_CLASS_IDS_ARRAY: TypeInfo(
+        OsefKeys._ENABLED_CLASS_IDS_ARRAY,
+        _packers.ArrayPacker(np.dtype(np.uint32)),
+    ),
+    OsefTypes._REFLECTION_FEATURES_ARRAY: TypeInfo(
+        OsefKeys._REFLECTION_FEATURES_ARRAY,
+        _packers.ArrayPacker(np.dtype(np.float32)),
+    ),
+    OsefTypes._REFLECTION_BITS: TypeInfo(
+        OsefKeys._REFLECTION_BITS,
+        _packers.BoolBitfieldPacker(),
+    ),
 }
 
 
 def get_type_info_by_id(type_code: int):
     """Get TypeInfo for a given type code.
 
     :param type_code: Int value in OsefTypes
```

### Comparing `osef-3.0.0a4/osef/spec/constants.py` & `osef-3.1.0a1/osef/spec/constants.py`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/osef/spec/osef_types.py` & `osef-3.1.0a1/osef/spec/osef_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """OSEF private types definition."""
-__version__ = "1.14.0"
+__version__ = "1.17.0"
 
 # Standard imports
 from enum import Enum, IntEnum
 
 # !!! Warning !!!
 # !!! This file has been auto generated, do not attempt to edit it !!!
 # Important: all words use little-endian representation, unless specified otherwise
@@ -96,14 +96,24 @@
     _INSTANTANEOUS_ROTATION_SPEED = 83
     _FILTERED_TRANSLATION_SPEED = 84
     _FILTERED_ROTATION_SPEED = 85
     REFERENCE_MAP_BITS = 86
     _CARTESIAN_COVARIANCE = 87
     _CYLINDRICAL_COVARIANCE = 88
     COORDINATES_REFERENCE_SYSTEM = 89
+    START_TIMESTAMP = 90
+    END_TIMESTAMP = 91
+    TIME_DOMAIN = 92
+    TIME_INTERVAL = 93
+    CLASSIFICATION_CONFIDENCE = 94
+    _CLASS_PROBABILITIES_ARRAY = 95
+    _CLASSIFIER_DEF = 96
+    _ENABLED_CLASS_IDS_ARRAY = 97
+    _REFLECTION_FEATURES_ARRAY = 98
+    _REFLECTION_BITS = 99
 
 
 class OsefKeys(str, Enum):
     """OSEF type keys."""
 
     def __repr__(self) -> str:
         """Override repr method to display OsefKeys directly as strings."""
@@ -121,26 +131,27 @@
     - none or one:     Spherical Coordinates          (SPHERICAL_COORDINATES) [DEPRECATED USAGE]
     - none or one:     Reflectivities                 (REFLECTIVITIES)
     - none or one:     Background Flags               (BACKGROUND_FLAGS) [DEPRECATED USAGE]
     - none or one:     Cartesian Coordinates          (CARTESIAN_COORDINATES)
     - none or one:     BGR Colors                     (BGR_COLORS)
     - none or one:     Azimuths Column                (AZIMUTHS_COLUMN)
     - none or one:     Cloud Processing               (CLOUD_PROCESSING)
-    - none or one:     Percept                        (PERCEPT)
+    - none or one:     Percept                        (PERCEPT) [DEPRECATED USAGE]
     - none or one:     Object ID 32 Bits              (OBJECT_ID_32_BITS)
     - none or one:     Cartesian Coordinates 4F       (CARTESIAN_COORDINATES_4F) [DEPRECATED USAGE]
     - none or one:     Background Bits                (BACKGROUND_BITS)
     - none or one:     Ground Plane Bits              (GROUND_PLANE_BITS)
     - none or one:     Azimuths                       (AZIMUTHS)
     - none or one:     Elevations                     (ELEVATIONS)
     - none or one:     Distances                      (DISTANCES)
-    - none or one:     Road Markings Bits             (ROAD_MARKINGS_BITS)
+    - none or one:     Road Markings Bits             (ROAD_MARKINGS_BITS) [DEPRECATED USAGE]
     - none or one:     Carla Tag Array                (CARLA_TAG_ARRAY)
     - none or one:     Reference Map Bits             (REFERENCE_MAP_BITS)
     - none or one:     Coordinates Reference System   (COORDINATES_REFERENCE_SYSTEM)
+    - none or one:     Reflection Bits                (REFLECTION_BITS)
     """
 
     NUMBER_OF_POINTS = "number_of_points"
     """
     Number of Points
     **Output when**: Augmented Cloud is enabled.
     **Format**: Contains 32 bits unsigned int value.
@@ -316,19 +327,20 @@
     Timestamped Data
     **Output when**: Always.
     Contains following sub-TLVs:
     - exactly one:     Timestamp Microsecond          (TIMESTAMP_MICROSECOND)
     - none or one:     Object Detection Frame         (OBJECT_DETECTION_FRAME)
     - none or one:     Cloud Frame                    (CLOUD_FRAME)
     - none or one:     Scan Frame                     (SCAN_FRAME)
+    - zero to many:    Time interval                  (TIME_INTERVAL)
     """
 
     _PERCEPT = "percept"
     """
-    Percept
+    Percept [DEPRECATED USAGE]
     Contains list of percept classes represented as unsigned 16-bits integer, using enum PERCEPT ID.
     """
 
     _BGR_IMAGE_FRAME = "bgr_image_frame"
     """
     BGR Image Frame
     Contains following sub-TLVs:
@@ -377,14 +389,15 @@
     - none or one:     Geographic Speed               (GEOGRAPHIC_SPEED)
     - none or one:     Ego Motion                     (EGO_MOTION)
     - none or one:     Tracked Objects                (TRACKED_OBJECTS)
     - none or one:     Zones Def                      (ZONES_DEF)
     - none or one:     Zones Objects Binding          (ZONES_OBJECTS_BINDING) [DEPRECATED USAGE]
     - none or one:     Zones Objects Binding 32 Bits  (ZONES_OBJECTS_BINDING_32_BITS)
     - none or one:     Height Map                     (HEIGHT_MAP)
+    - none or one:     Classifier Def                 (CLASSIFIER_DEF)
     """
 
     TRACKED_OBJECTS = "tracked_objects"
     """
     Tracked Objects
     **Output when**: Tracking is enabled.
     **Purpose**: Properties of tracked objects, which includes centroid, bbox, speed...
@@ -397,14 +410,17 @@
     - exactly one:     Bbox Sizes                     (BBOX_SIZES)
     - exactly one:     Speed Vectors                  (SPEED_VECTORS)
     - exactly one:     Pose Array                     (POSE_ARRAY)
     - none or one:     Slam Pose Array                (SLAM_POSE_ARRAY)
     - exactly one:     Object Properties              (OBJECT_PROPERTIES)
     - none or one:     Geographic Pose Array          (GEOGRAPHIC_POSE_ARRAY)
     - none or one:     Geographic Speed Array         (GEOGRAPHIC_SPEED_ARRAY)
+    - none or one:     Classification confidence      (CLASSIFICATION_CONFIDENCE)
+    - none or one:     Class probabilities Array      (CLASS_PROBABILITIES_ARRAY)
+    - none or one:     Reflection features array      (REFLECTION_FEATURES_ARRAY)
     """
 
     BBOX_SIZES = "bbox_sizes"
     """
     Bbox Sizes
     **Output when**: Tracking is enabled.
     **Purpose**: Define bounding boxes around each tracked object.
@@ -538,20 +554,23 @@
 
     OBJECT_PROPERTIES = "object_properties"
     """
     Object Properties
     **Output when**: Tracking is enabled.
     **Purpose**: Properties of the object.
     **Format**: One byte per object, each bit of this can represent different properties.
-    * 1st bit: 1 if the object has a proper orientation (like a cuboid), 0 otherwise (like a cylinder).
-    * 2nd bit: 1 if the object has been seen in the last scan, 0 if it was not seen.
-    * 3rd bit: 1 if the object has a valid slam pose, 0 otherwise. See type 55 (Slam Pose Array) for more information.
-    * 4th bit: 1 if the object is static (e.g. traffic signs, poles...), 0 otherwise
-    * 5th bit: reserved for later use
-    * 6th bit: reserved for later use
+    * 1st bit: is_oriented: 1 if the object has a proper orientation (like a cuboid), 0 otherwise (like a cylinder).
+    * 2nd bit: is_seen: 1 if the object has been seen in the last scan, 0 if it was not seen.
+    * 3rd bit: has_valid_slam_pose: 1 if the object has a valid slam pose, 0 otherwise. See type 55 (Slam Pose Array)
+    for more information.
+    * 4th bit: is_static_object: 1 if the object is static (e.g. traffic signs, poles...), 0 otherwise
+    * 5th bit: has_a_priori_dimensions: 1 if an a priori estimation of the object dimensions has been given as input, 0
+    otherwise
+    * 6th bit: is_controlled: 1 if the object has been declared controlled by a system taking Shift Perception data as
+    input
     * 7th bit: reserved for later use
     * 8th bit: reserved for later use
     """
 
     _IMU_PACKET = "imu_packet"
     """
     IMU Packet
@@ -643,24 +662,27 @@
     GEOGRAPHIC_POSE = "geographic_pose"
     """
     Geographic Pose [DEPRECATED USAGE]
     **Deprecated since**: 5.3
     **Instead, use**: "Geographic Pose Precise" (Type 57)
     **Purpose**: Represents the geographic pose, output from the relocalization processing, expressed in decimal
     degrees notation (latitude, longitude & heading).
-    **Format**: Concatenation of 3 single precision (32 bits) floats [lat, long, heading].
+    **Format**: Concatenation of 3 single-precision (32 bits) floats [lat, long, heading].
     * Single-precision floating-point (float32) : latitude in decimal degrees, range [ -90.0 .. 90.0 ]
     * Single-precision floating-point (float32) : longitude in decimal degrees, range [ -180.0 .. 180.0 ]
     * Single-precision floating-point (float32) : heading in decimal degrees, range [ 0.0 .. 360.0 [
     """
 
     OBJECT_ID_32_BITS = "object_id_32_bits"
     """
     Object ID 32 Bits
     **Output when**: Tracking is enabled.
+    * Standard behavior: output as leaf of Tracked Objects.
+    * Optional & internal behavior: output also as leaf of Augmented Cloud when object_id is listed in
+    cloud_fields_to_stream.
     **Format**: Array of unsigned 32-bits integers. Each element of the array is an Object ID.
     **Purpose**: Give a unique identifier (ID) to each detected object.
     Optionally, this ID can also be used to establish a link between detected objects
     and the defined Zones, or the points from an Augmented Cloud.
     When used as leaf of Tracked Objects:
     - The number of elements of the array is equal to the Number of Objects (type 10).
     - Each ID represents a distinct detected object.
@@ -775,24 +797,24 @@
     GEOGRAPHIC_POSE_PRECISE = "geographic_pose_precise"
     """
     Geographic Pose Precise
     **Output when**: Relocalization in a reference map and georeferencing are enabled.
     So in processing config: slam.enable set to true, slam.reference_map defined and georeferencing.enable set to true.
     **Purpose**: Represents the geographic pose, output from the relocalization processing, expressed in decimal
     degrees notation (latitude, longitude & heading).
-    **Format**: Concatenation of 2 double precision (64 bits) and a single precision (32 bits) floats [lat, long,
+    **Format**: Concatenation of 2 double-precision (64 bits) and a single-precision (32 bits) floats [lat, long,
     heading].
     * Double-precision floating-point (float64) : latitude in decimal degrees, range [ -90.0 .. 90.0 ]
     * Double-precision floating-point (float64) : longitude in decimal degrees, range [ -180.0 .. 180.0 ]
     * Single-precision floating-point (float32) : heading in decimal degrees, range [ 0.0 .. 360.0 [
     """
 
     _ROAD_MARKINGS_BITS = "road_markings_bits"
     """
-    Road Markings Bits
+    Road Markings Bits [DEPRECATED USAGE]
     Contains a padded (up to a byte) list of bits, 1 bit per point of the cloud. If the bit is set, the point belongs
     to a road marking.
     """
 
     SMOOTHED_POSE = "smoothed_pose"
     """
     Smoothed Pose
@@ -926,15 +948,15 @@
     background scene array, in degrees
     """
 
     _BACKGROUND_SCENE_PARAMS_ELEVATIONS = "background_scene_params_elevations"
     """
     Background Scene Params Elevations
     **Output when**: generated by Carla Scenario Generator.
-    **Format**: List of single precision floats, each one representing the elevation of a row in the background scene
+    **Format**: List of single-precision floats, each one representing the elevation of a row in the background scene
     array, in degrees
     """
 
     _BACKGROUND_SCENE_FRAGMENT = "background_scene_fragment"
     """
     Background Scene Fragment
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
@@ -951,25 +973,25 @@
       * cells_number: 32-bites unsigned integer, number of cells contained in the fragment
     """
 
     _BACKGROUND_SCENE_FRAGMENT_DISTANCES = "background_scene_fragment_distances"
     """
     Background Scene Fragment Distances
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
-    **Format**: List of single precision floats, each one representing the farthest background distance for the
+    **Format**: List of single-precision floats, each one representing the farthest background distance for the
     corresponding cell
     """
 
     GEOGRAPHIC_POSE_ARRAY = "geographic_pose_array"
     """
     Geographic Pose Array
     **Output when**: Tracking is enabled and georeferencing is activated.
     **Purpose**: Represents the geographic pose, output from the relocalization processing, expressed in decimal
     degrees notation (latitude, longitude & heading) of each tracked object.
-    **Format**: Concatenation of 2 double precision (64 bits) and a single precision (32 bits) floats [lat, long,
+    **Format**: Concatenation of 2 double-precision (64 bits) and a single-precision (32 bits) floats [lat, long,
     heading], one for each tracked object.
     * Double-precision floating-point (float64): latitude in decimal degrees, range [ -90.0 .. 90.0 ]
     * Double-precision floating-point (float64): longitude in decimal degrees, range [ -180.0 .. 180.0 ]
     * Single-precision floating-point (float32): heading in decimal degrees, range [ 0.0 .. 360.0 [
     """
 
     GEOGRAPHIC_SPEED = "geographic_speed"
@@ -995,41 +1017,41 @@
     """
 
     _INSTANTANEOUS_TRANSLATION_SPEED = "instantaneous_translation_speed"
     """
     Instantaneous Translation Speed
     **Output when**: SLAM is enabled and its speed_measurement module is enabled.
     **Purpose**: Represents the instantaneous translation speed of the device (m/s).
-    **Format**: Array of 3 single precision (32 bits) floats, representing the translation speed on each direction.
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the translation speed on each direction.
     """
 
     _INSTANTANEOUS_ROTATION_SPEED = "instantaneous_rotation_speed"
     """
     Instantaneous Rotation Speed
     **Output when**: SLAM is enabled and its speed_measurement module is enabled.
     **Purpose**: Represents the instantaneous rotation speed of the device (rad/s).
-    **Format**: Array of 3 single precision (32 bits) floats, representing the rotation speed around each axis.
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the rotation speed around each axis.
     """
 
     _FILTERED_TRANSLATION_SPEED = "filtered_translation_speed"
     """
     Filtered Translation Speed
     **Output when**: SLAM is enabled and its speed_measurement module is enabled.
     **Purpose**: Represents the filtered translation speed of the device (m/s). An averaging filter smooths the
     evolution of the speed. A short delay will appear due to the filtering (usually around 1 sec).
-    **Format**: Array of 3 single precision (32 bits) floats, representing the translation speed on each direction.
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the translation speed on each direction.
     """
 
     _FILTERED_ROTATION_SPEED = "filtered_rotation_speed"
     """
     Filtered Rotation Speed
     **Output when**: SLAM is enabled and its speed_measurement module is enabled.
     **Purpose**: Represents the filtered rotation speed of the device (rad/s). An averaging filter smooths the
     evolution of the speed. A short delay will appear due to the filtering (usually around 1 sec).
-    **Format**: Array of 3 single precision (32 bits) floats, representing the rotation speed around each axis.
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the rotation speed around each axis.
     """
 
     REFERENCE_MAP_BITS = "reference_map_bits"
     """
     Reference Map Bits
     **Output when**: SLAM is enabled and its mapping module is enabled.
     **Purpose**: SLAM identifies potential points of interest within the point cloud, and the mapping module selects
@@ -1040,36 +1062,131 @@
 
     _CARTESIAN_COVARIANCE = "cartesian_covariance"
     """
     Cartesian covariance
     **Output when**: SLAM is enabled and compute_covariance option is set to true.
     **Purpose**: Represents the cartesian covariances (m²). It estimates the confidence of the algorithm, and how
     trustworthy is the position.
-    **Format**: Array of 3 single precision (32 bits) floats, representing the covariance of x, y and z measurements.
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the covariance of x, y and z measurements.
     """
 
     _CYLINDRICAL_COVARIANCE = "cylindrical_covariance"
     """
     Cylindrical covariance
     **Output when**: SLAM is enabled and compute_covariance option is set to true.
     **Purpose**: Represents the cylindrical covariances (°²). It estimates the confidence of the algorithm, and how
     trustworthy is the orientation.
-    **Format**: Array of 3 single precision (32 bits) floats, representing the covariance of roll (rotation around X
+    **Format**: Array of 3 single-precision (32 bits) floats, representing the covariance of roll (rotation around X
     axis), pitch (rotation around Y axis) and yaw (rotation around Z axis) measurements.
     """
 
     COORDINATES_REFERENCE_SYSTEM = "coordinates_reference_system"
     """
     Coordinates Reference System
     **Output when**: Augmented Cloud is enabled.
     **Purpose**: The coordinates of the augmented cloud may be expressed in an absolute or relative coordinate system.
-    The latter usually being relative to the the sensor. This field indicates the reference system in use.
+    The latter usually being relative to the sensor. This field indicates the reference system in use.
     **Format**: Enumerate COORDINATES REFERENCE SYSTEM
     """
 
+    START_TIMESTAMP = "start_timestamp"
+    """
+    Start timestamp
+    **Purpose**: Start of the time interval. The start timestamp is included in the interval. Unix timestamp with
+    **nanosecond** precision.
+    **Format**: Contains concatenation of:
+    * UNIX time in seconds, unsigned 32-bits integer, range [ 0 .. 2^32 [
+    * remaining nanoseconds, unsigned 32-bits integer, range [ 0 .. 1'000'000'000 [
+    """
+
+    END_TIMESTAMP = "end_timestamp"
+    """
+    End timestamp
+    **Purpose**: End of the time interval. The end timestamp is not included in the interval. Unix timestamp with
+    **nanosecond** precision.
+    **Format**: Contains concatenation of:
+    * UNIX time in seconds, unsigned 32-bits integer, range [ 0 .. 2^32 [
+    * remaining nanoseconds, unsigned 32-bits integer, range [ 0 .. 1'000'000'000 [
+    """
+
+    TIME_DOMAIN = "time_domain"
+    """
+    Time domain
+    **Purpose**: Time domain used to generate the timestamps:
+       * Reception time: timestamps are generated when the data is received by the system,
+       * Sensor time: timestamps are generated by the LiDAR, when the data is acquired
+    Warning: Mixing timestamps of different domains is not advised.
+    **Format**: Unsigned 32-bits enumerate TIME DOMAIN
+    """
+
+    TIME_INTERVAL = "time_interval"
+    """
+    Time interval
+    **Output when**: Scan Maker is time-based.
+    **Purpose**: A duration between a start timestamp and an end timestamp. Depending on the time domain Sub-TLV, the
+    data is guaranteed to have been either acquired or received during this duration.
+    Contains following sub-TLVs:
+    - exactly one:     Start timestamp                (START_TIMESTAMP)
+    - exactly one:     End timestamp                  (END_TIMESTAMP)
+    - exactly one:     Time domain                    (TIME_DOMAIN)
+    """
+
+    CLASSIFICATION_CONFIDENCE = "classification_confidence"
+    """
+    Classification confidence
+    **Output when**: Tracking is enabled.
+    **Purpose**: Represents a level of confidence, from 0 to 1, regarding the class ID assigned to each tracked object.
+    **Format**: A single-precision (32 bits) float for each tracked object, range [ 0 .. 1 ].
+    """
+
+    _CLASS_PROBABILITIES_ARRAY = "class_probabilities_array"
+    """
+    Class probabilities Array
+    **Output when**: Tracking and class probabilities are enabled.
+    **Purpose**: Normalized distribution over enabled class IDs, expressing, for each tracked object, its
+    classification probability.
+    **Format**: Array containing a single-precision (32 bits) float per class id for each tracked object with range [ 0
+    .. 1 ].
+    """
+
+    _CLASSIFIER_DEF = "classifier_def"
+    """
+    Classifier Def
+    **Output when**: Tracking is enabled.
+    **Purpose**: Definition of classifier settings
+    Contains following sub-TLVs:
+    - exactly one:     Enabled class IDs Array        (ENABLED_CLASS_IDS_ARRAY)
+    """
+
+    _ENABLED_CLASS_IDS_ARRAY = "enabled_class_ids_array"
+    """
+    Enabled class IDs Array
+    **Output when**: Tracking and class probabilities are enabled.
+    **Purpose**: List class IDs that can be assigned to tracked objects.
+    **Format**: Array of signed 32 bits integers, using enum CLASS ID. Use TLV length to determine the number of class
+    IDs.
+    The order is important as it is respected for other fields like type 95.
+    """
+
+    _REFLECTION_FEATURES_ARRAY = "reflection_features_array"
+    """
+    Reflection features array
+    **Output when**: Tracking is enabled and option is enabled in configuration
+    **Purpose**: Internal only: Reflections filtering - values of features for each object used by the reflection
+    filtering. Used for debug and/or retraining.
+    **Format**: Array of single precision floats, 6 per objects, concatenated for all objects.
+    """
+
+    _REFLECTION_BITS = "reflection_bits"
+    """
+    Reflection Bits
+    Contains a padded list of bits, 1 bit per point of the cloud. If the bit is set, the point is an unwanted
+    reflection, generated by ricochet on an overly reflective surface.
+    """
+
 
 class ClassId(IntEnum):
     """Tracked object class ID"""
 
     UNKNOWN = 0
     PERSON = 1
     LUGGAGE = 2
@@ -1080,14 +1197,16 @@
     VAN = 7
     TWO_WHEELER = 8
     MASK = 9
     NO_MASK = 10
     LANDMARK = 11
     TRAILER = 12
     TRACTOR_HEAD = 13
+    GATE = 14
+    TUGGER_TRAIN = 15
 
 
 class PerceptId(IntEnum):
     """Percept class ID"""
 
     DEFAULT = 0
     ROAD = 1
@@ -1169,7 +1288,14 @@
 
 class CoordinatesReferenceSystem(IntEnum):
     """Coordinates Reference System"""
 
     UNDEFINED = 0
     WORLD = 1
     SENSOR = 2
+
+
+class TimeDomain(IntEnum):
+    """Time domain"""
+
+    LOCAL = 0
+    SENSOR = 1
```

### Comparing `osef-3.0.0a4/osef.egg-info/PKG-INFO` & `osef-3.1.0a1/osef.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osef
-Version: 3.0.0a4
+Version: 3.1.0a1
 Summary: Osef python library.
 Author-email: Outsight Developpers <support@outsight.tech>
 Project-URL: Documentation, https://outsight-tech.gitlab.io/common/osef-python-library/
 Project-URL: Support, https://support.outsight.ai
 Project-URL: Changes, https://outsight-tech.gitlab.io/common/osef-python-library/CHANGELOG.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `osef-3.0.0a4/osef.egg-info/SOURCES.txt` & `osef-3.1.0a1/osef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osef-3.0.0a4/pyproject.toml` & `osef-3.1.0a1/pyproject.toml`

 * *Files identical despite different names*

