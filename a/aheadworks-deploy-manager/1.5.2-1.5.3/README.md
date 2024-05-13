# Comparing `tmp/aheadworks_deploy_manager-1.5.2.tar.gz` & `tmp/aheadworks_deploy_manager-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aheadworks_deploy_manager-1.5.2.tar", last modified: Thu Mar 28 13:01:54 2024, max compression
+gzip compressed data, was "aheadworks_deploy_manager-1.5.3.tar", last modified: Mon May 13 08:59:12 2024, max compression
```

## Comparing `aheadworks_deploy_manager-1.5.2.tar` & `aheadworks_deploy_manager-1.5.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/
--rw-r--r--   0 root         (0) root         (0)      503 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.643169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7744 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/db_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5205 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    15096 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/version_control_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/console/
--rw-rw-rw-   0 root         (0) root         (0)    10041 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/console/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/bitbucket.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/dockerhub.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/logging.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/parser/
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/parser/php.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/ssh_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8102 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/model/
--rw-rw-rw-   0 root         (0) root         (0)     3227 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/model/extension.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.647169 aheadworks_deploy_manager-1.5.2/aheadworks_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1126 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/composer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/discord_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/file_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/jira_api_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     7962 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/magento_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/api/youtrack_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/console/
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/console/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/cd.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/data/data_object.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/data/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/http/api_request.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.651169 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/parser/
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/parser/json.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_core/model/parser/xml.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)      503 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-28 13:01:54.000000 aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/zip-safe
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/api/
--rw-rw-rw-   0 root         (0) root         (0)     4226 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/api/pipeline_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    27419 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/api/release_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/console/
--rw-rw-rw-   0 root         (0) root         (0)     3553 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/console/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/__main__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/console/
--rw-rw-rw-   0 root         (0) root         (0)     7454 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/console/console.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-28 13:01:54.655169 aheadworks_deploy_manager-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-03-28 13:01:44.000000 aheadworks_deploy_manager-1.5.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.481531 aheadworks_deploy_manager-1.5.3/
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/db_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    15096 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/version_control_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/console/
+-rw-rw-rw-   0 root         (0) root         (0)    10041 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/console/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/bitbucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/dockerhub.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/logging.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.469531 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/parser/php.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/ssh_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8102 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/model/
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/model/extension.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/composer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/discord_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/jira_api_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7962 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/magento_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/api/youtrack_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/console/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/console/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/cd.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/data/data_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/data/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.473531 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/http/api_request.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/parser/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_core/model/parser/xml.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-13 08:59:12.000000 aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/zip-safe
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/api/
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/api/pipeline_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    27457 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/api/release_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/console/
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/console/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/__main__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-13 08:59:12.477532 aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/console/
+-rw-rw-rw-   0 root         (0) root         (0)     7454 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/console/console.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-13 08:59:12.481531 aheadworks_deploy_manager-1.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-13 08:59:00.000000 aheadworks_deploy_manager-1.5.3/setup.py
```

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/bitbucket_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/db_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/db_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/dockerhub_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/file_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/file_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/api/version_control_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/api/version_control_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/console/console.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/bitbucket.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/bitbucket.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/data/dockerhub.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/data/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_bitbucket_manager/model/parser/php.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_bitbucket_manager/model/parser/php.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/__main__.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_composer_manager/model/extension.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_composer_manager/model/extension.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/api/composer_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/api/composer_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/api/file_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/api/file_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/api/jira_api_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/api/jira_api_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/api/magento_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/api/magento_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/api/youtrack_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/api/youtrack_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/console/console.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/model/http/api_request.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/model/http/api_request.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/model/parser/json.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/model/parser/json.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_core/model/parser/xml.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_core/model/parser/xml.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_deploy_manager.egg-info/SOURCES.txt` & `aheadworks_deploy_manager-1.5.3/aheadworks_deploy_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/api/pipeline_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/api/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/api/release_manager.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/api/release_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,16 @@
 
         # module_dependencies = self.magento_manager.get_module_dependencies(path_to_module)
         module_dependencies = self.magento_manager.get_module_dependencies_from_composer(composer_file)
         composer_package_name = ','.join(list(map(lambda x: x['full_module_name'], module_dependencies.values())))
 
         # assign release pack to user
         release_issue = jira_instance.issue(release_task_key)
-        release_issue.update(assignee={'accountId': assign_to})
+        if (not assign_to == ""):
+            release_issue.update(assignee={'accountId': assign_to})
         jira_instance.add_comment(release_issue, f'Composer Package Name:\n{composer_package_name}')
 
         # uncomment if needed check transitions for issue
         # transitions = jira_instance.transitions(release_issue)
         # set done to pd and test issue. transition=31 - Task Done
         # Set PD and TEST to Done
         pd_issue = jira_instance.issue(pd_task_key)
```

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_release_manager/console/console.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_release_manager/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/aheadworks_test_manager/console/console.py` & `aheadworks_deploy_manager-1.5.3/aheadworks_test_manager/console/console.py`

 * *Files identical despite different names*

### Comparing `aheadworks_deploy_manager-1.5.2/setup.py` & `aheadworks_deploy_manager-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='aheadworks_deploy_manager',
-    version='1.5.2',
+    version='1.5.3',
     zip_safe=True,
     packages=[
         'aheadworks_composer_manager',
         'aheadworks_core',
         'aheadworks_bitbucket_manager',
         'aheadworks_release_manager',
         'aheadworks_test_manager'
```

