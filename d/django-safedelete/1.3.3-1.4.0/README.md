# Comparing `tmp/django-safedelete-1.3.3.tar.gz` & `tmp/django_safedelete-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-safedelete-1.3.3.tar", last modified: Mon Nov 13 09:40:26 2023, max compression
+gzip compressed data, was "django_safedelete-1.4.0.tar", last modified: Mon May 13 11:59:22 2024, max compression
```

## Comparing `django-safedelete-1.3.3.tar` & `django_safedelete-1.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.040761 django-safedelete-1.3.3/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       91 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/AUTHORS
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5681 2023-11-13 09:35:48.000000 django-safedelete-1.3.3/CHANGES
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1479 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/LICENSE
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      227 2022-08-17 08:58:50.000000 django-safedelete-1.3.3/MANIFEST.in
--rw-r--r--   0 gagaro    (1000) gagaro    (1000)    11083 2023-11-13 09:40:26.040761 django-safedelete-1.3.3/PKG-INFO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4285 2023-11-13 09:35:18.000000 django-safedelete-1.3.3/README.rst
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/django_safedelete.egg-info/
--rw-r--r--   0 gagaro    (1000) gagaro    (1000)    11083 2023-11-13 09:40:26.000000 django-safedelete-1.3.3/django_safedelete.egg-info/PKG-INFO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1554 2023-11-13 09:40:26.000000 django-safedelete-1.3.3/django_safedelete.egg-info/SOURCES.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2023-11-13 09:40:26.000000 django-safedelete-1.3.3/django_safedelete.egg-info/dependency_links.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        7 2023-11-13 09:40:26.000000 django-safedelete-1.3.3/django_safedelete.egg-info/requires.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       11 2023-11-13 09:40:26.000000 django-safedelete-1.3.3/django_safedelete.egg-info/top_level.txt
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/safedelete/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      456 2023-11-13 09:35:48.000000 django-safedelete-1.3.3/safedelete/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    10916 2023-11-13 09:35:18.000000 django-safedelete-1.3.3/safedelete/admin.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      164 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/apps.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      430 2022-08-16 15:43:13.000000 django-safedelete-1.3.3/safedelete/config.py
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.028761 django-safedelete-1.3.3/safedelete/locale/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.028761 django-safedelete-1.3.3/safedelete/locale/de/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/safedelete/locale/de/LC_MESSAGES/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1417 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.028761 django-safedelete-1.3.3/safedelete/locale/fr/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/safedelete/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1436 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     6715 2022-09-12 13:15:59.000000 django-safedelete-1.3.3/safedelete/managers.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    15110 2023-01-30 08:45:11.000000 django-safedelete-1.3.3/safedelete/models.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        7 2022-08-17 08:58:50.000000 django-safedelete-1.3.3/safedelete/py.typed
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     3470 2022-09-12 13:44:44.000000 django-safedelete-1.3.3/safedelete/query.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4673 2023-04-05 07:16:43.000000 django-safedelete-1.3.3/safedelete/queryset.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      191 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/signals.py
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.028761 django-safedelete-1.3.3/safedelete/static/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/safedelete/static/safedelete/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       90 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/static/safedelete/admin.css
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.028761 django-safedelete-1.3.3/safedelete/templates/
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.036761 django-safedelete-1.3.3/safedelete/templates/safedelete/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      832 2023-11-13 09:35:18.000000 django-safedelete-1.3.3/safedelete/templates/safedelete/hard_delete_selected_confirmation.html
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      823 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/templates/safedelete/undelete_selected_confirmation.html
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2023-11-13 09:40:26.040761 django-safedelete-1.3.3/safedelete/tests/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      980 2022-08-16 14:17:12.000000 django-safedelete-1.3.3/safedelete/tests/models.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2026 2022-05-03 13:05:57.000000 django-safedelete-1.3.3/safedelete/tests/settings.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7302 2023-11-13 09:35:18.000000 django-safedelete-1.3.3/safedelete/tests/test_admin.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2855 2023-04-05 07:16:43.000000 django-safedelete-1.3.3/safedelete/tests/test_custom_queryset.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1220 2022-09-12 13:02:38.000000 django-safedelete-1.3.3/safedelete/tests/test_foreignkey.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1853 2022-05-03 13:20:29.000000 django-safedelete-1.3.3/safedelete/tests/test_hard_delete.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1432 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_invisible.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1719 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_lookups.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2369 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_many2many.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2124 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_no_cascade.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1026 2022-05-03 13:20:29.000000 django-safedelete-1.3.3/safedelete/tests/test_no_delete.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1953 2023-01-27 14:11:40.000000 django-safedelete-1.3.3/safedelete/tests/test_prefetch_related.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    10847 2022-09-12 13:54:22.000000 django-safedelete-1.3.3/safedelete/tests/test_queryset.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      664 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_refresh_from_db.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2143 2022-05-03 13:05:57.000000 django-safedelete-1.3.3/safedelete/tests/test_single_delete_call_on_inheritance.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7391 2022-05-03 13:20:29.000000 django-safedelete-1.3.3/safedelete/tests/test_soft_delete.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    11836 2023-10-30 08:28:58.000000 django-safedelete-1.3.3/safedelete/tests/test_soft_delete_cascade.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1352 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_subquery.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2735 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/test_visible_by_pk.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5062 2022-05-03 13:20:29.000000 django-safedelete-1.3.3/safedelete/tests/testcase.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      544 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/safedelete/tests/urls.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1055 2023-01-09 09:00:31.000000 django-safedelete-1.3.3/safedelete/utils.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       80 2023-11-13 09:40:26.044761 django-safedelete-1.3.3/setup.cfg
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2049 2022-05-03 12:18:26.000000 django-safedelete-1.3.3/setup.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.596334 django_safedelete-1.4.0/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       91 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/AUTHORS
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5798 2024-05-13 11:55:57.000000 django_safedelete-1.4.0/CHANGES
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1479 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/LICENSE
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      227 2022-08-17 08:58:50.000000 django_safedelete-1.4.0/MANIFEST.in
+-rw-r--r--   0 gagaro    (1000) gagaro    (1000)    11225 2024-05-13 11:59:22.596334 django_safedelete-1.4.0/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4285 2023-11-13 09:35:18.000000 django_safedelete-1.4.0/README.rst
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.596334 django_safedelete-1.4.0/django_safedelete.egg-info/
+-rw-r--r--   0 gagaro    (1000) gagaro    (1000)    11225 2024-05-13 11:59:22.000000 django_safedelete-1.4.0/django_safedelete.egg-info/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1554 2024-05-13 11:59:22.000000 django_safedelete-1.4.0/django_safedelete.egg-info/SOURCES.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2024-05-13 11:59:22.000000 django_safedelete-1.4.0/django_safedelete.egg-info/dependency_links.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       17 2024-05-13 11:59:22.000000 django_safedelete-1.4.0/django_safedelete.egg-info/requires.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       11 2024-05-13 11:59:22.000000 django_safedelete-1.4.0/django_safedelete.egg-info/top_level.txt
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.592333 django_safedelete-1.4.0/safedelete/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      456 2024-05-13 11:56:07.000000 django_safedelete-1.4.0/safedelete/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    10929 2024-05-13 09:42:27.000000 django_safedelete-1.4.0/safedelete/admin.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      164 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/apps.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      430 2022-08-16 15:43:13.000000 django_safedelete-1.4.0/safedelete/config.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.588333 django_safedelete-1.4.0/safedelete/locale/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.584334 django_safedelete-1.4.0/safedelete/locale/de/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.592333 django_safedelete-1.4.0/safedelete/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1417 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.588333 django_safedelete-1.4.0/safedelete/locale/fr/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.592333 django_safedelete-1.4.0/safedelete/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1436 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     6715 2022-09-12 13:15:59.000000 django_safedelete-1.4.0/safedelete/managers.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    15110 2023-01-30 08:45:11.000000 django_safedelete-1.4.0/safedelete/models.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        7 2022-08-17 08:58:50.000000 django_safedelete-1.4.0/safedelete/py.typed
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     3470 2022-09-12 13:44:44.000000 django_safedelete-1.4.0/safedelete/query.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4673 2023-04-05 07:16:43.000000 django_safedelete-1.4.0/safedelete/queryset.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      191 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/signals.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.588333 django_safedelete-1.4.0/safedelete/static/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.592333 django_safedelete-1.4.0/safedelete/static/safedelete/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       90 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/static/safedelete/admin.css
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.588333 django_safedelete-1.4.0/safedelete/templates/
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.592333 django_safedelete-1.4.0/safedelete/templates/safedelete/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      832 2023-11-13 09:35:18.000000 django_safedelete-1.4.0/safedelete/templates/safedelete/hard_delete_selected_confirmation.html
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      823 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/templates/safedelete/undelete_selected_confirmation.html
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 11:59:22.596334 django_safedelete-1.4.0/safedelete/tests/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      980 2022-08-16 14:17:12.000000 django_safedelete-1.4.0/safedelete/tests/models.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2026 2022-05-03 13:05:57.000000 django_safedelete-1.4.0/safedelete/tests/settings.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7302 2023-11-13 09:35:18.000000 django_safedelete-1.4.0/safedelete/tests/test_admin.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2855 2023-04-05 07:16:43.000000 django_safedelete-1.4.0/safedelete/tests/test_custom_queryset.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1220 2022-09-12 13:02:38.000000 django_safedelete-1.4.0/safedelete/tests/test_foreignkey.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1853 2022-05-03 13:20:29.000000 django_safedelete-1.4.0/safedelete/tests/test_hard_delete.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1432 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_invisible.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1719 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_lookups.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2369 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_many2many.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2124 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_no_cascade.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1026 2022-05-03 13:20:29.000000 django_safedelete-1.4.0/safedelete/tests/test_no_delete.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1953 2023-01-27 14:11:40.000000 django_safedelete-1.4.0/safedelete/tests/test_prefetch_related.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    10847 2022-09-12 13:54:22.000000 django_safedelete-1.4.0/safedelete/tests/test_queryset.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      664 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_refresh_from_db.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2143 2022-05-03 13:05:57.000000 django_safedelete-1.4.0/safedelete/tests/test_single_delete_call_on_inheritance.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7391 2022-05-03 13:20:29.000000 django_safedelete-1.4.0/safedelete/tests/test_soft_delete.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    11836 2023-10-30 08:28:58.000000 django_safedelete-1.4.0/safedelete/tests/test_soft_delete_cascade.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1352 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_subquery.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2735 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/test_visible_by_pk.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5062 2022-05-03 13:20:29.000000 django_safedelete-1.4.0/safedelete/tests/testcase.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      544 2022-05-03 12:18:26.000000 django_safedelete-1.4.0/safedelete/tests/urls.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1055 2023-01-09 09:00:31.000000 django_safedelete-1.4.0/safedelete/utils.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       80 2024-05-13 11:59:22.596334 django_safedelete-1.4.0/setup.cfg
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2062 2024-05-13 09:28:53.000000 django_safedelete-1.4.0/setup.py
```

### Comparing `django-safedelete-1.3.3/CHANGES` & `django_safedelete-1.4.0/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 CHANGELOG
 =========
 
+1.4.0 (2024-05-13)
+==================
+
+- Support Python 3.11 / Django 5.0
+- Drop support for Django 3.2 / 4.0 / 4.1
+
 1.3.3 (2023-11-13)
 ==================
 
 - Add Hard Delete Action to SafeDeleteAdmin #236 
 
 1.3.2 (2023-04-05)
 ==================
```

### Comparing `django-safedelete-1.3.3/LICENSE` & `django_safedelete-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/PKG-INFO` & `django_safedelete-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-safedelete
-Version: 1.3.3
+Version: 1.4.0
 Summary: Mask your objects instead of deleting them from your database.
 Home-page: https://github.com/makinacorpus/django-safedelete
-Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/1.3.3
+Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/1.4.0
 Author: Korantin Auguste
 Author-email: contact@palkeo.com
 License: BSD
 Keywords: django,delete,safedelete,softdelete
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: Django
+Requires-Dist: packaging
 
 Django safedelete
 =================
 
 .. image:: https://github.com/makinacorpus/django-safedelete/workflows/Python%20application/badge.svg
     :target: https://github.com/makinacorpus/django-safedelete/actions?query=workflow%3A%22Python+application%22
 
@@ -173,14 +174,20 @@
     :target: http://www.makina-corpus.com
 
 
 =========
 CHANGELOG
 =========
 
+1.4.0 (2024-05-13)
+==================
+
+- Support Python 3.11 / Django 5.0
+- Drop support for Django 3.2 / 4.0 / 4.1
+
 1.3.3 (2023-11-13)
 ==================
 
 - Add Hard Delete Action to SafeDeleteAdmin #236 
 
 1.3.2 (2023-04-05)
 ==================
```

### Comparing `django-safedelete-1.3.3/README.rst` & `django_safedelete-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/django_safedelete.egg-info/PKG-INFO` & `django_safedelete-1.4.0/django_safedelete.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-safedelete
-Version: 1.3.3
+Version: 1.4.0
 Summary: Mask your objects instead of deleting them from your database.
 Home-page: https://github.com/makinacorpus/django-safedelete
-Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/1.3.3
+Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/1.4.0
 Author: Korantin Auguste
 Author-email: contact@palkeo.com
 License: BSD
 Keywords: django,delete,safedelete,softdelete
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: Django
+Requires-Dist: packaging
 
 Django safedelete
 =================
 
 .. image:: https://github.com/makinacorpus/django-safedelete/workflows/Python%20application/badge.svg
     :target: https://github.com/makinacorpus/django-safedelete/actions?query=workflow%3A%22Python+application%22
 
@@ -173,14 +174,20 @@
     :target: http://www.makina-corpus.com
 
 
 =========
 CHANGELOG
 =========
 
+1.4.0 (2024-05-13)
+==================
+
+- Support Python 3.11 / Django 5.0
+- Drop support for Django 3.2 / 4.0 / 4.1
+
 1.3.3 (2023-11-13)
 ==================
 
 - Add Hard Delete Action to SafeDeleteAdmin #236 
 
 1.3.2 (2023-04-05)
 ==================
```

### Comparing `django-safedelete-1.3.3/django_safedelete.egg-info/SOURCES.txt` & `django_safedelete-1.4.0/django_safedelete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/admin.py` & `django_safedelete-1.4.0/safedelete/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import PermissionDenied
 from django.db.models import F
 from django.template.response import TemplateResponse
 from django.utils.encoding import force_str
 from django.utils.html import conditional_escape, format_html
 from django.utils.translation import gettext_lazy as _
-from pkg_resources import parse_version
+from packaging.version import parse as parse_version
 
 from .config import FIELD_NAME
 from .utils import related_objects
 from .models import HARD_DELETE
 
 # Django 3.0 compatibility
 try:
```

### Comparing `django-safedelete-1.3.3/safedelete/locale/de/LC_MESSAGES/django.po` & `django_safedelete-1.4.0/safedelete/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/locale/fr/LC_MESSAGES/django.po` & `django_safedelete-1.4.0/safedelete/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/managers.py` & `django_safedelete-1.4.0/safedelete/managers.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/models.py` & `django_safedelete-1.4.0/safedelete/models.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/query.py` & `django_safedelete-1.4.0/safedelete/query.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/queryset.py` & `django_safedelete-1.4.0/safedelete/queryset.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/templates/safedelete/hard_delete_selected_confirmation.html` & `django_safedelete-1.4.0/safedelete/templates/safedelete/hard_delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/templates/safedelete/undelete_selected_confirmation.html` & `django_safedelete-1.4.0/safedelete/templates/safedelete/undelete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/models.py` & `django_safedelete-1.4.0/safedelete/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/settings.py` & `django_safedelete-1.4.0/safedelete/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_admin.py` & `django_safedelete-1.4.0/safedelete/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_custom_queryset.py` & `django_safedelete-1.4.0/safedelete/tests/test_custom_queryset.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_foreignkey.py` & `django_safedelete-1.4.0/safedelete/tests/test_foreignkey.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_hard_delete.py` & `django_safedelete-1.4.0/safedelete/tests/test_hard_delete.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_invisible.py` & `django_safedelete-1.4.0/safedelete/tests/test_invisible.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_lookups.py` & `django_safedelete-1.4.0/safedelete/tests/test_lookups.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_many2many.py` & `django_safedelete-1.4.0/safedelete/tests/test_many2many.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_no_cascade.py` & `django_safedelete-1.4.0/safedelete/tests/test_no_cascade.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_no_delete.py` & `django_safedelete-1.4.0/safedelete/tests/test_no_delete.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_prefetch_related.py` & `django_safedelete-1.4.0/safedelete/tests/test_prefetch_related.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_queryset.py` & `django_safedelete-1.4.0/safedelete/tests/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_refresh_from_db.py` & `django_safedelete-1.4.0/safedelete/tests/test_refresh_from_db.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_single_delete_call_on_inheritance.py` & `django_safedelete-1.4.0/safedelete/tests/test_single_delete_call_on_inheritance.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_soft_delete.py` & `django_safedelete-1.4.0/safedelete/tests/test_soft_delete.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_soft_delete_cascade.py` & `django_safedelete-1.4.0/safedelete/tests/test_soft_delete_cascade.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_subquery.py` & `django_safedelete-1.4.0/safedelete/tests/test_subquery.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/test_visible_by_pk.py` & `django_safedelete-1.4.0/safedelete/tests/test_visible_by_pk.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/testcase.py` & `django_safedelete-1.4.0/safedelete/tests/testcase.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/tests/urls.py` & `django_safedelete-1.4.0/safedelete/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/safedelete/utils.py` & `django_safedelete-1.4.0/safedelete/utils.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-1.3.3/setup.py` & `django_safedelete-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,10 +49,10 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Development Status :: 4 - Beta',
     ],
     license='BSD',
-    install_requires=['Django'],
+    install_requires=['Django', 'packaging'],
     include_package_data=True,
 )
```

