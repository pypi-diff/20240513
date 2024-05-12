# Comparing `tmp/django-audit-events-0.3.0.tar.gz` & `tmp/django-audit-events-0.3.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-audit-events-0.3.0.tar", last modified: Mon May  6 06:52:16 2024, max compression
+gzip compressed data, was "dist/django-audit-events-0.3.1.dev0.tar", last modified: Sun May 12 22:25:28 2024, max compression
```

## Comparing `django-audit-events-0.3.0.tar` & `django-audit-events-0.3.1.dev0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      220 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/.editorconfig
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      101 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/.gitignore
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      113 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/.isort.cfg
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       27 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/CHANGELOG.md
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1050 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/LICENSE.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3505 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/PKG-INFO
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1714 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/README.md
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2612 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/bitbucket-pipelines.yml
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      380 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      396 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/admin.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      447 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/apps.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      733 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/conf.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4523 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/context.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1842 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/filters.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1544 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/django.po
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      843 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/middleware.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/migrations/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1984 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0001_initial.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2207 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0002_archivedauditevent.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      712 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0003_auto_20201218_1113.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      650 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0004_auto_20210127_2021.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      768 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/0005_auto_20220215_0756.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      669 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/migrations/0006_auto_20220920_1327.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/migrations/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      857 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/mixin.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4659 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/models.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      476 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/serializers.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1675 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tasks.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/tests/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      290 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_conf.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     6001 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_context.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1362 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/tests/test_middleware.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1539 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_mixin.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2062 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/test_models.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2548 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/tests/test_tasks.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       58 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/urls.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       65 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      160 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/tests/utils/models.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      205 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/django_audit_events/urls.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      917 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/django_audit_events/utils.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       22 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events/version.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1060 2023-11-29 08:37:50.000000 django-audit-events-0.3.0/django_audit_events/views.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3505 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/PKG-INFO
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1798 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/SOURCES.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/dependency_links.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:50:27.000000 django-audit-events-0.3.0/django_audit_events.egg-info/not-zip-safe
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       20 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/django_audit_events.egg-info/top_level.txt
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/docs/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      634 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/Makefile
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1609 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/advanced.rst
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2080 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/conf.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1533 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/configuration.rst
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      944 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/index.rst
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1252 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/introduction.rst
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      795 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/make.bat
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2265 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/docs/quickstart.rst
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      310 2022-09-16 07:00:53.000000 django-audit-events-0.3.0/pyproject.toml
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      396 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/requirements.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2337 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/runtests.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       38 2024-05-06 06:52:16.000000 django-audit-events-0.3.0/setup.cfg
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2628 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/setup.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1819 2024-05-06 06:51:16.000000 django-audit-events-0.3.0/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/filters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/middleware.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0002_archivedauditevent.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0003_auto_20201218_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0004_auto_20210127_2021.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0005_auto_20220215_0756.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0006_auto_20220920_1327.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      857 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/urls.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/tox.ini
```

### Comparing `django-audit-events-0.3.0/LICENSE.txt` & `django-audit-events-0.3.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/PKG-INFO` & `django-audit-events-0.3.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.3.0
+Version: 0.3.1.dev0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -73,7 +73,9 @@
 
 ```
 >>> event.content
 {"something": "done", "bar: "baz"}
 ```
 
 For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
+
+
```

### Comparing `django-audit-events-0.3.0/README.md` & `django-audit-events-0.3.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/bitbucket-pipelines.yml` & `django-audit-events-0.3.1.dev0/bitbucket-pipelines.yml`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,14 @@
       - step:
           name: Publish to PyPI
           image: python:3.7-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
             - CRYPTOGRAPHY_DONT_BUILD_RUST=1 pip install setuptools setuptools_scm twine
             - python setup.py sdist bdist_wheel
-            - twine upload -u $PYPI_USERNAME -p $PYPI_PASSWORD dist/*
+            - twine upload -u __token__ -p $PYPI_TOKEN --skip-existing dist/*
 definitions:
   services:
     postgres:
       image: postgres
       variables:
         POSTGRES_PASSWORD: postgres
```

### Comparing `django-audit-events-0.3.0/django_audit_events/conf.py` & `django-audit-events-0.3.1.dev0/django_audit_events/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/context.py` & `django-audit-events-0.3.1.dev0/django_audit_events/context.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/filters.py` & `django-audit-events-0.3.1.dev0/django_audit_events/filters.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/locale/tr/LC_MESSAGES/django.po` & `django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/middleware.py` & `django-audit-events-0.3.1.dev0/django_audit_events/middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0001_initial.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0002_archivedauditevent.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0002_archivedauditevent.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0003_auto_20201218_1113.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0003_auto_20201218_1113.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0004_auto_20210127_2021.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0004_auto_20210127_2021.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0005_auto_20220215_0756.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0005_auto_20220215_0756.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/migrations/0006_auto_20220920_1327.py` & `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0006_auto_20220920_1327.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/mixin.py` & `django-audit-events-0.3.1.dev0/django_audit_events/mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/models.py` & `django-audit-events-0.3.1.dev0/django_audit_events/models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tasks.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tasks.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tests/test_context.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tests/test_middleware.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tests/test_mixin.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tests/test_models.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/tests/test_tasks.py` & `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/utils.py` & `django-audit-events-0.3.1.dev0/django_audit_events/utils.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events/views.py` & `django-audit-events-0.3.1.dev0/django_audit_events/views.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/django_audit_events.egg-info/PKG-INFO` & `django-audit-events-0.3.1.dev0/django_audit_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.3.0
+Version: 0.3.1.dev0
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
@@ -73,7 +73,9 @@
 
 ```
 >>> event.content
 {"something": "done", "bar: "baz"}
 ```
 
 For more information about installation and usage, check out the [documentation](https://django-audit-events.readthedocs.io/)!
+
+
```

### Comparing `django-audit-events-0.3.0/django_audit_events.egg-info/SOURCES.txt` & `django-audit-events-0.3.1.dev0/django_audit_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/Makefile` & `django-audit-events-0.3.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/advanced.rst` & `django-audit-events-0.3.1.dev0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/conf.py` & `django-audit-events-0.3.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/configuration.rst` & `django-audit-events-0.3.1.dev0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/index.rst` & `django-audit-events-0.3.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/introduction.rst` & `django-audit-events-0.3.1.dev0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/make.bat` & `django-audit-events-0.3.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/docs/quickstart.rst` & `django-audit-events-0.3.1.dev0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/runtests.py` & `django-audit-events-0.3.1.dev0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/setup.py` & `django-audit-events-0.3.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.0/tox.ini` & `django-audit-events-0.3.1.dev0/tox.ini`

 * *Files identical despite different names*

