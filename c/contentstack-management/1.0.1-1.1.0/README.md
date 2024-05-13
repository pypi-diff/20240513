# Comparing `tmp/contentstack-management-1.0.1.tar.gz` & `tmp/contentstack_management-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentstack-management-1.0.1.tar", last modified: Wed Dec 13 05:01:02 2023, max compression
+gzip compressed data, was "contentstack_management-1.1.0.tar", last modified: Mon May 13 11:53:19 2024, max compression
```

## Comparing `contentstack-management-1.0.1.tar` & `contentstack_management-1.1.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/aliases/aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28780 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/assets/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/auditlogs/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/auditlogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/auditlogs/auditlog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/branches/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/branches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/branches/branches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/bulk_operations/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/bulk_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/bulk_operations/bulk_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/content_types/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/content_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/content_types/content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/contentstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/delivery_token/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/delivery_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/delivery_token/delivery_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/entries/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20214 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/entries/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.030278 contentstack-management-1.0.1/contentstack_management/environments/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/environments/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/extensions/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/global_fields/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/global_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/global_fields/global_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/labels/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/labels/label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/locale/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/locale/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/management_token/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/management_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/management_token/management_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/organizations/organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/publish_queue/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/publish_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/publish_queue/publish_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/release_items/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/release_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/release_items/release_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/releases/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/releases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/releases/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/roles/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/stack/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14399 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/stack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/taxonomies/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/taxonomies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/taxonomies/taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.034278 contentstack-management-1.0.1/contentstack_management/terms/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/terms/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/contentstack_management/user_session/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/user_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/user_session/user_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/contentstack_management/users/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/users/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/contentstack_management/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13473 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/webhooks/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/contentstack_management/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25869 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/contentstack_management/workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/contentstack_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2023-12-13 05:01:02.000000 contentstack-management-1.0.1/contentstack_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-12-13 05:01:02.000000 contentstack-management-1.0.1/contentstack_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 05:01:02.000000 contentstack-management-1.0.1/contentstack_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-13 05:01:02.000000 contentstack-management-1.0.1/contentstack_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-13 05:01:02.000000 contentstack-management-1.0.1/contentstack_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 05:01:02.038278 contentstack-management-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-12-13 05:00:50.000000 contentstack-management-1.0.1/tests/test_contentstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.239761 contentstack_management-1.1.0/contentstack_management/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.239761 contentstack_management-1.1.0/contentstack_management/aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/aliases/aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.239761 contentstack_management-1.1.0/contentstack_management/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28780 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/assets/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.239761 contentstack_management-1.1.0/contentstack_management/auditlogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/auditlogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/auditlogs/auditlog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.239761 contentstack_management-1.1.0/contentstack_management/branches/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/branches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/branches/branches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/bulk_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/bulk_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/bulk_operations/bulk_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/content_types/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/content_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/content_types/content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/contentstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/delivery_token/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/delivery_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/delivery_token/delivery_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20214 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/entries/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/environments/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/extensions/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/global_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/global_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/global_fields/global_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/labels/label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/locale/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/management_token/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/management_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/management_token/management_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.243761 contentstack_management-1.1.0/contentstack_management/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/organizations/organization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/publish_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/publish_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/publish_queue/publish_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/release_items/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/release_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/release_items/release_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/releases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/releases/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/stack/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14399 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/stack/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/taxonomies/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/taxonomies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/taxonomies/taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/terms/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/terms/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/user_session/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/user_session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/user_session/user_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/users/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.247762 contentstack_management-1.1.0/contentstack_management/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13473 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/webhooks/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/contentstack_management/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/contentstack_management/workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/contentstack_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-13 11:53:19.000000 contentstack_management-1.1.0/contentstack_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-13 11:53:19.000000 contentstack_management-1.1.0/contentstack_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:53:19.000000 contentstack_management-1.1.0/contentstack_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 11:53:19.000000 contentstack_management-1.1.0/contentstack_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 11:53:19.000000 contentstack_management-1.1.0/contentstack_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:53:19.251762 contentstack_management-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-13 11:53:15.000000 contentstack_management-1.1.0/tests/test_contentstack.py
```

### Comparing `contentstack-management-1.0.1/LICENSE` & `contentstack_management-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2012 - 2023 Contentstack. All rights reserved.
+Copyright (c) 2012 - 2024 Contentstack. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `contentstack-management-1.0.1/PKG-INFO` & `contentstack_management-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentstack-management
-Version: 1.0.1
+Version: 1.1.0
 Summary: Contentstack API Client Library for Python
 Home-page: https://github.com/contentstack/contentstack-management-python
 Author: ishaileshmishra
 Author-email: mobile@contentstack.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `contentstack-management-1.0.1/README.md` & `contentstack_management-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/__init__.py` & `contentstack_management-1.1.0/contentstack_management/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,14 @@
 "Extension"
 )
 
 __title__ = 'contentstack-management-python'
 __author__ = 'ishaileshmishra'
 __status__ = 'debug'
 __region__ = 'na'
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 __host__ = 'api.contentstack.io'
 __protocol__ = 'https://'
 __api_version__ = 'v3'
 __endpoint__ = 'https://api.contentstack.io/v3/'
 __email__ = 'mobile@contentstack.com'
 __issues__ = 'support@contentstack.com'
```

### Comparing `contentstack-management-1.0.1/contentstack_management/_api_client.py` & `contentstack_management-1.1.0/contentstack_management/_api_client.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/_constant.py` & `contentstack_management-1.1.0/contentstack_management/_constant.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/aliases/aliases.py` & `contentstack_management-1.1.0/contentstack_management/aliases/aliases.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/assets/assets.py` & `contentstack_management-1.1.0/contentstack_management/assets/assets.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/auditlogs/auditlog.py` & `contentstack_management-1.1.0/contentstack_management/auditlogs/auditlog.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/branches/branches.py` & `contentstack_management-1.1.0/contentstack_management/branches/branches.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/bulk_operations/bulk_operation.py` & `contentstack_management-1.1.0/contentstack_management/bulk_operations/bulk_operation.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/content_types/content_type.py` & `contentstack_management-1.1.0/contentstack_management/content_types/content_type.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/contentstack.py` & `contentstack_management-1.1.0/contentstack_management/contentstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class Region(Enum):
     US = "us"
     EU = "eu"
     AZURE_EU = "azure-eu"
     AZURE_NA = "azure-na"
+    GCP_NA = "gcp-na"
 
 
 def user_agents(headers=None):
     if headers is None:
         headers = {}
     local_headers = {'X-User-Agent': f'contentstack-management-python/v{version}',
                      "Content-Type": "application/json"}
@@ -31,14 +32,17 @@
     def __init__(self, host: str = 'api.contentstack.io', scheme: str = 'https://',
                  authtoken: str = None , management_token=None, headers: dict = None,
                  region: Region = Region.US.value, version='v3', timeout=2, max_retries: int = 18,
                  **kwargs):
         self.endpoint = 'https://api.contentstack.io/v3/'
         if region is not None and host is not None and region is not Region.US.value:
             self.endpoint = f'{scheme}{region}-{host}/{version}/'
+        if region is not None and host is None and region is not Region.US.value:
+            host = 'api.contentstack.com'
+            self.endpoint = f'{scheme}{region}-{host}/{version}/'
         if host is not None and region is None:
             self.endpoint = f'{scheme}{host}/{version}/'
         if headers is None:
             headers = {}
         if authtoken is not None:
             headers['authtoken'] = authtoken
```

### Comparing `contentstack-management-1.0.1/contentstack_management/delivery_token/delivery_token.py` & `contentstack_management-1.1.0/contentstack_management/delivery_token/delivery_token.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/entries/entry.py` & `contentstack_management-1.1.0/contentstack_management/entries/entry.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/environments/environment.py` & `contentstack_management-1.1.0/contentstack_management/environments/environment.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/extensions/extension.py` & `contentstack_management-1.1.0/contentstack_management/extensions/extension.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/global_fields/global_fields.py` & `contentstack_management-1.1.0/contentstack_management/global_fields/global_fields.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/labels/label.py` & `contentstack_management-1.1.0/contentstack_management/labels/label.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/locale/locale.py` & `contentstack_management-1.1.0/contentstack_management/locale/locale.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/management_token/management_token.py` & `contentstack_management-1.1.0/contentstack_management/management_token/management_token.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/metadata/metadata.py` & `contentstack_management-1.1.0/contentstack_management/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/organizations/organization.py` & `contentstack_management-1.1.0/contentstack_management/organizations/organization.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/publish_queue/publish_queue.py` & `contentstack_management-1.1.0/contentstack_management/publish_queue/publish_queue.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/release_items/release_item.py` & `contentstack_management-1.1.0/contentstack_management/release_items/release_item.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/releases/release.py` & `contentstack_management-1.1.0/contentstack_management/releases/release.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/roles/roles.py` & `contentstack_management-1.1.0/contentstack_management/roles/roles.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/stack/stack.py` & `contentstack_management-1.1.0/contentstack_management/stack/stack.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/taxonomies/taxonomy.py` & `contentstack_management-1.1.0/contentstack_management/taxonomies/taxonomy.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/terms/terms.py` & `contentstack_management-1.1.0/contentstack_management/terms/terms.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/user_session/user_session.py` & `contentstack_management-1.1.0/contentstack_management/user_session/user_session.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/users/user.py` & `contentstack_management-1.1.0/contentstack_management/users/user.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/webhooks/webhook.py` & `contentstack_management-1.1.0/contentstack_management/webhooks/webhook.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management/workflows/workflows.py` & `contentstack_management-1.1.0/contentstack_management/workflows/workflows.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/contentstack_management.egg-info/PKG-INFO` & `contentstack_management-1.1.0/contentstack_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentstack-management
-Version: 1.0.1
+Version: 1.1.0
 Summary: Contentstack API Client Library for Python
 Home-page: https://github.com/contentstack/contentstack-management-python
 Author: ishaileshmishra
 Author-email: mobile@contentstack.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `contentstack-management-1.0.1/contentstack_management.egg-info/SOURCES.txt` & `contentstack_management-1.1.0/contentstack_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/setup.py` & `contentstack_management-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `contentstack-management-1.0.1/tests/test_contentstack.py` & `contentstack_management-1.1.0/tests/test_contentstack.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,18 @@
         self.client = contentstack_management.Client(host=host)
         self.client.login(username, password)
 
     def test_client(self):
         client = contentstack_management.Client(authtoken='your_authtoken')
         self.assertEqual('https://api.contentstack.io/v3/', client.endpoint) # Default host 'api.contentstack.io'
 
+    def test_gcp_na_region(self):
+        client = contentstack_management.Client(authtoken='your_authtoken', region='gcp-na')
+        self.assertEqual('https://gcp-na-api.contentstack.com/v3/', client.endpoint)
+
     def test_successful_get_login(self):
         client = contentstack_management.Client(host=host)
         response = client.login(username, password)
         self.assertEqual(response.request.url, f"{self.client.endpoint}user-session")
         self.assertEqual(response.request.method, "POST")
         self.assertEqual(response.request.headers["Content-Type"], "application/json")
```

