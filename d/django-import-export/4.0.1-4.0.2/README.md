# Comparing `tmp/django_import_export-4.0.1.tar.gz` & `tmp/django_import_export-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export-4.0.1.tar", last modified: Wed May  8 08:57:18 2024, max compression
+gzip compressed data, was "django_import_export-4.0.2.tar", last modified: Mon May 13 18:47:11 2024, max compression
```

## Comparing `django_import_export-4.0.1.tar` & `django_import_export-4.0.2.tar`

### file list

```diff
@@ -1,335 +1,336 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.552449 django_import_export-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.508449 django_import_export-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-08 08:57:10.000000 django_import_export-4.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-08 08:57:10.000000 django_import_export-4.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 08:57:10.000000 django_import_export-4.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-08 08:57:10.000000 django_import_export-4.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-08 08:57:10.000000 django_import_export-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 08:57:10.000000 django_import_export-4.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-08 08:57:18.552449 django_import_export-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-08 08:57:10.000000 django_import_export-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-08 08:57:10.000000 django_import_export-4.0.1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 08:57:10.000000 django_import_export-4.0.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.552449 django_import_export-4.0.1/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 08:57:18.000000 django_import_export-4.0.1/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.512449 django_import_export-4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.516449 django_import_export-4.0.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30548 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    57619 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.516449 django_import_export-4.0.1/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-08 08:57:10.000000 django_import_export-4.0.1/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 08:57:18.000000 django_import_export-4.0.1/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35221 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.520449 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.496449 django_import_export-4.0.1/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.524449 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    49322 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.528449 django_import_export-4.0.1/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21360 2024-05-08 08:57:10.000000 django_import_export-4.0.1/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-08 08:57:10.000000 django_import_export-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 08:57:10.000000 django_import_export-4.0.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 08:57:10.000000 django_import_export-4.0.1/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-08 08:57:10.000000 django_import_export-4.0.1/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:57:18.552449 django_import_export-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:57:10.000000 django_import_export-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.532449 django_import_export-4.0.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.536449 django_import_export-4.0.1/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.536449 django_import_export-4.0.1/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/0015_withpositiveintegerfields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.500449 django_import_export-4.0.1/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.540449 django_import_export-4.0.1/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_action_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    17599 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    39062 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_model_resource_fields_generate_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.544449 django_import_export-4.0.1/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    26269 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.504449 django_import_export-4.0.1/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:18.548449 django_import_export-4.0.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-08 08:57:10.000000 django_import_export-4.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.700663 django_import_export-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.656663 django_import_export-4.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.656663 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.660663 django_import_export-4.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-13 18:47:07.000000 django_import_export-4.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-13 18:47:07.000000 django_import_export-4.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 18:47:07.000000 django_import_export-4.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 18:47:07.000000 django_import_export-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 18:47:07.000000 django_import_export-4.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 18:47:11.700663 django_import_export-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 18:47:07.000000 django_import_export-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-13 18:47:07.000000 django_import_export-4.0.2/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 18:47:07.000000 django_import_export-4.0.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.664662 django_import_export-4.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.644662 django_import_export-4.0.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.668663 django_import_export-4.0.2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/non-field-specific-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22107 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    58752 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.668663 django_import_export-4.0.2/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:47:11.000000 django_import_export-4.0.2/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.644662 django_import_export-4.0.2/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50781 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 18:47:07.000000 django_import_export-4.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-13 18:47:07.000000 django_import_export-4.0.2/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-13 18:47:07.000000 django_import_export-4.0.2/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:47:11.700663 django_import_export-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:47:07.000000 django_import_export-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0015_withpositiveintegerfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_action_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40988 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_model_resource_fields_generate_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_natural_foreign_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tox.ini
```

### Comparing `django_import_export-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.2/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/.github/stale.yml` & `django_import_export-4.0.2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/.github/workflows/release.yml` & `django_import_export-4.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/.github/workflows/test.yml` & `django_import_export-4.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/AUTHORS` & `django_import_export-4.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/CODE_OF_CONDUCT.md` & `django_import_export-4.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/LICENSE` & `django_import_export-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/Makefile` & `django_import_export-4.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/PKG-INFO` & `django_import_export-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.1
+Version: 4.0.2
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django_import_export-4.0.1/README.rst` & `django_import_export-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/RELEASE.md` & `django_import_export-4.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/django_import_export.egg-info/PKG-INFO` & `django_import_export-4.0.2/django_import_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.1
+Version: 4.0.2
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django_import_export-4.0.1/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.2/django_import_export.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 tests/core/tests/admin_integration/test_import.py
 tests/core/tests/admin_integration/test_views.py
 tests/core/tests/test_resources/__init__.py
 tests/core/tests/test_resources/test_bulk_operations.py
 tests/core/tests/test_resources/test_diffs.py
 tests/core/tests/test_resources/test_import_export.py
 tests/core/tests/test_resources/test_misc.py
+tests/core/tests/test_resources/test_natural_foreign_key.py
 tests/core/tests/test_resources/test_relationships.py
 tests/core/tests/test_resources/test_modelresource/__init__.py
 tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
 tests/core/tests/test_resources/test_modelresource/test_data_handling.py
 tests/core/tests/test_resources/test_modelresource/test_data_import.py
 tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
 tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
```

### Comparing `django_import_export-4.0.1/docs/Makefile` & `django_import_export-4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/change-form-export.png` & `django_import_export-4.0.2/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.2/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.2/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.2/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.2/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.2/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.2/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.2/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/export-button.png` & `django_import_export-4.0.2/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.2/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/import-button.png` & `django_import_export-4.0.2/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.2/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.2/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/_static/images/select-for-export.png` & `django_import_export-4.0.2/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/admin_integration.rst` & `django_import_export-4.0.2/docs/admin_integration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,20 @@
   admin.site.register(Book, BookAdmin)
 
 Note that the above example refers specifically to the :ref:`example application<exampleapp>`, you'll have to modify
 this to refer to your own model instances.  In the example application, the 'Category' model has this functionality.
 
 When 'Go' is clicked for the selected items, the user will be directed to the
 :ref:`export 'confirm' page<export_confirm>`.  It is possible to disable this extra step by setting the
-:ref:`import_export_skip_admin_action_export_ui` flag
+:ref:`import_export_skip_admin_action_export_ui` flag.
+
+.. note::
+
+    If deploying to a multi-tenant environment, you may need to use the to ensure that one set of users cannot export
+    data belonging to another set.  See :meth:`~import_export.admin.ExportMixin.get_valid_export_item_pks`.
 
 Export from model instance change form
 --------------------------------------
 
 When :ref:`export via admin action<export_via_admin_action>` is enabled, then it is also possible to export from a
 model instance change form:
```

### Comparing `django_import_export-4.0.1/docs/advanced_usage.rst` & `django_import_export-4.0.2/docs/advanced_usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,17 @@
         class Meta:
             model = Book
             exclude = ('imported', )
 
 If both ``fields`` and ``exclude`` are declared, the ``fields`` declaration takes precedence, and ``exclude`` is
 ignored.
 
+In cases where a :ref:`custom column name<field_declaration>` is used, declare the name of the model attribute in the
+``fields`` list., not the column alias.
+
 .. _field_ordering:
 
 Field ordering
 --------------
 
 The precedence for the order of fields for import / export is defined as follows:
 
@@ -67,16 +70,14 @@
 Where ``import_order`` or ``export_order`` contains a subset of ``fields`` then the ``import_order`` and
 ``export_order`` fields will be processed first.
 
 If no ``fields``, ``import_order`` or ``export_order`` is defined then fields are created via introspection of the model
 class.  The order of declared fields in the model instance is preserved, and any non-model fields are last in the
 ordering.
 
-.. _field_declaration:
-
 Model relations
 ---------------
 
 When defining :class:`~import_export.resources.ModelResource` fields it is
 possible to follow model relationships::
 
     class BookResource(resources.ModelResource):
@@ -87,14 +88,16 @@
 
 This example declares that the ``Author.name`` value (which has a foreign key relation to ``Book``) will appear in the
 export.
 
 Note that declaring the relationship using this syntax sets ``field`` as readonly, meaning this field will be skipped
 when importing data. To understand how to import model relations, see :ref:`import_model_relations`.
 
+.. _field_declaration:
+
 Explicit field declaration
 --------------------------
 
 We can declare fields explicitly to give us more control over the relationship between the row and the model attribute.
 In the example below, we use the ``attribute`` kwarg to define the model attribute, and ``column_name`` to define the
 column name (i.e. row header)::
```

### Comparing `django_import_export-4.0.1/docs/api_mixins.rst` & `django_import_export-4.0.2/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/api_widgets.rst` & `django_import_export-4.0.2/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/bulk_import.rst` & `django_import_export-4.0.2/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/changelog.rst` & `django_import_export-4.0.2/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.2 (2024-05-13)
+------------------
+
+- fix export with custom column name (`1821 <https://github.com/django-import-export/django-import-export/pull/1821>`_)
+- fix allow ``column_name`` to be declared in ``fields`` list (`1822 <https://github.com/django-import-export/django-import-export/pull/1822>`_)
+- fix clash between ``key_is_id`` and ``use_natural_foreign_keys`` (`1824 <https://github.com/django-import-export/django-import-export/pull/1824>`_)
+- remove unreachable code (`1825 <https://github.com/django-import-export/django-import-export/pull/1825>`_)
+- fix issue with widget assignment for custom ``ForeignKey`` subclasses (`1826 <https://github.com/django-import-export/django-import-export/pull/1826>`_)
+- performance: select of valid pks for export restricted to action exports (`1827 <https://github.com/django-import-export/django-import-export/pull/1827>`_)
+- fix crash on export with custom column name (`1828 <https://github.com/django-import-export/django-import-export/pull/1828>`_)
+- remove outdated datetime formatting logic (`1830 <https://github.com/django-import-export/django-import-export/pull/1830>`_)
+
 4.0.1 (2024-05-08)
 ------------------
 
 - fix crash on export when model has no ``id`` (`1802 <https://github.com/django-import-export/django-import-export/pull/1802>`_)
 - fix Widget crash when django Field subclass is used (`1805 <https://github.com/django-import-export/django-import-export/pull/1805>`_)
 - fix regression: allow imports when default ``import_id_field`` is not present (`1813 <https://github.com/django-import-export/django-import-export/pull/1813>`_)
```

### Comparing `django_import_export-4.0.1/docs/conf.py` & `django_import_export-4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/contributing.rst` & `django_import_export-4.0.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/export_workflow.rst` & `django_import_export-4.0.2/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/faq.rst` & `django_import_export-4.0.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/getting_started.rst` & `django_import_export-4.0.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/image_src/export_workflow.txt` & `django_import_export-4.0.2/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/image_src/import_workflow.txt` & `django_import_export-4.0.2/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/import_workflow.rst` & `django_import_export-4.0.2/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/index.rst` & `django_import_export-4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/installation.rst` & `django_import_export-4.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/make.bat` & `django_import_export-4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/release_notes.rst` & `django_import_export-4.0.2/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/docs/testing.rst` & `django_import_export-4.0.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/admin.py` & `django_import_export-4.0.2/import_export/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from django.template.response import TemplateResponse
 from django.urls import path, reverse
 from django.utils.decorators import method_decorator
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_POST
 
-from import_export import exceptions
-
 from .forms import ConfirmImportForm, ImportForm, SelectableFieldsExportForm
 from .mixins import BaseExportMixin, BaseImportMixin
 from .results import RowResult
 from .signals import post_export, post_import
 from .tmp_storages import TempFolderStorage
 
 logger = logging.getLogger(__name__)
@@ -503,35 +501,28 @@
                     )
                     resources = [resource]
 
                     # prepare additional kwargs for import_data, if needed
                     imp_kwargs = self.get_import_data_kwargs(
                         request=request, form=import_form, **kwargs
                     )
-                    try:
-                        result = resource.import_data(
-                            dataset,
-                            dry_run=True,
-                            raise_errors=False,
-                            file_name=import_file.name,
-                            user=request.user,
-                            **imp_kwargs,
-                        )
-                        context["result"] = result
-
-                        if (
-                            not result.has_errors()
-                            and not result.has_validation_errors()
-                        ):
-                            context["confirm_form"] = self.create_confirm_form(
-                                request, import_form=import_form
-                            )
-                    except exceptions.FieldError as e:
-                        messages.error(request, str(e))
+                    result = resource.import_data(
+                        dataset,
+                        dry_run=True,
+                        raise_errors=False,
+                        file_name=import_file.name,
+                        user=request.user,
+                        **imp_kwargs,
+                    )
+                    context["result"] = result
 
+                    if not result.has_errors() and not result.has_validation_errors():
+                        context["confirm_form"] = self.create_confirm_form(
+                            request, import_form=import_form
+                        )
         else:
             res_kwargs = self.get_import_resource_kwargs(
                 request=request, form=import_form, **kwargs
             )
             resource_classes = self.get_import_resource_classes(request)
             resources = [
                 resource_class(**res_kwargs) for resource_class in resource_classes
@@ -726,19 +717,22 @@
         form_type = self.get_export_form_class()
         formats = self.get_export_formats()
         form = form_type(
             formats,
             self.get_export_resource_classes(request),
             data=request.POST or None,
         )
-        form.fields["export_items"] = MultipleChoiceField(
-            widget=MultipleHiddenInput,
-            required=False,
-            choices=[(o.pk, o.pk) for o in self.model.objects.all()],
-        )
+        if request.POST and "export_items" in request.POST:
+            # this field is instantiated if the export is POSTed from the
+            # 'action' drop down
+            form.fields["export_items"] = MultipleChoiceField(
+                widget=MultipleHiddenInput,
+                required=False,
+                choices=[(pk, pk) for pk in self.get_valid_export_item_pks(request)],
+            )
         if form.is_valid():
             file_format = formats[int(form.cleaned_data["format"])]()
 
             if "export_items" in form.changed_data:
                 # this request has arisen from an Admin UI action
                 # export item pks are stored in form data
                 # so generate the queryset from the stored pks
@@ -767,14 +761,26 @@
             except FieldError as e:
                 messages.error(request, str(e))
 
         context = self.init_request_context_data(request, form)
         request.current_app = self.admin_site.name
         return TemplateResponse(request, [self.export_template_name], context=context)
 
+    def get_valid_export_item_pks(self, request):
+        """
+        Returns a list of valid pks for export.
+        This is used to validate which objects can be exported when exports are
+        triggered from the Admin UI 'action' dropdown.
+        This can be overridden to filter returned pks for performance and/or security
+        reasons.
+        :param request: The request object.
+        :returns: a list of valid pks (by default is all pks in table).
+        """
+        return self.model.objects.all().values_list("pk", flat=True)
+
     def changelist_view(self, request, extra_context=None):
         if extra_context is None:
             extra_context = {}
         extra_context["has_export_permission"] = self.has_export_permission(request)
         return super().changelist_view(request, extra_context)
 
     def get_export_filename(self, request, queryset, file_format):
@@ -840,14 +846,15 @@
             request,
             object_id,
             form_url,
             extra_context=extra_context,
         )
 
     def response_change(self, request, obj):
+        # called if the export is triggered from the instance detail page.
         if "_export-item" in request.POST:
             return self.export_admin_action(
                 request, self.model.objects.filter(id=obj.id)
             )
         return super().response_change(request, obj)
 
     def export_admin_action(self, request, queryset):
@@ -869,24 +876,23 @@
             response["Content-Disposition"] = 'attachment; filename="%s"' % (
                 self.get_export_filename(request, queryset, file_format),
             )
             return response
 
         form_type = self.get_export_form_class()
         formats = self.get_export_formats()
+        export_items = list(queryset.values_list("pk", flat=True))
         form = form_type(
             formats=formats,
             resources=self.get_export_resource_classes(request),
-            initial={"export_items": list(queryset.values_list("pk", flat=True))},
+            initial={"export_items": export_items},
         )
         # selected items are to be stored as a hidden input on the form
         form.fields["export_items"] = MultipleChoiceField(
-            widget=MultipleHiddenInput,
-            required=False,
-            choices=[(str(o), str(o)) for o in queryset.all()],
+            widget=MultipleHiddenInput, required=False, choices=export_items
         )
         context = self.init_request_context_data(request, form)
 
         # this is necessary to render the FORM action correctly
         # i.e. so the POST goes to the correct URL
         export_url = reverse(
             "%s:%s_%s_export"
```

### Comparing `django_import_export-4.0.1/import_export/declarative.py` & `django_import_export-4.0.2/import_export/declarative.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,26 +76,31 @@
 
             # #1693 check the fields explicitly declared as attributes of the Resource
             # class.
             # if 'fields' property is defined, declared fields can only be included
             # if they appear in the 'fields' iterable.
             declared_fields = dict()
             for field_name, field in new_class.fields.items():
-                if opts.fields is not None and field_name not in opts.fields:
+                column_name = field.column_name
+                if (
+                    opts.fields is not None
+                    and field_name not in opts.fields
+                    and column_name not in opts.fields
+                ):
                     continue
                 declared_fields[field_name] = field
 
             field_list = []
             for f in sorted(model_opts.fields + model_opts.many_to_many):
                 if opts.fields is not None and f.name not in opts.fields:
                     continue
                 if opts.exclude and f.name in opts.exclude:
                     continue
 
-                if f.name in declared_fields:
+                if f.name in set(declared_fields.keys()):
                     # If model field is declared in `ModelResource`,
                     # remove it from `declared_fields`
                     # to keep exact order of model fields
                     field = declared_fields.pop(f.name)
                 else:
                     field = new_class.field_from_django_field(f.name, f, readonly=False)
```

### Comparing `django_import_export-4.0.1/import_export/exceptions.py` & `django_import_export-4.0.2/import_export/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 class FieldError(ImportExportError):
     """Raised when a field encounters an error."""
 
     pass
 
 
+class WidgetError(ImportExportError):
+    """Raised when there is a misconfiguration with a Widget."""
+
+    pass
+
+
 class ImportError(ImportExportError):
     def __init__(self, error, number=None, row=None):
         """A wrapper for errors thrown from the import process.
 
         :param error: The underlying error that occurred.
         :param number: The row number of the row containing the error (if obtainable).
         :param row: The row containing the error (if obtainable).
```

### Comparing `django_import_export-4.0.1/import_export/fields.py` & `django_import_export-4.0.2/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/formats/base_formats.py` & `django_import_export-4.0.2/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/forms.py` & `django_import_export-4.0.2/import_export/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/instance_loaders.py` & `django_import_export-4.0.2/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/ru/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/mixins.py` & `django_import_export-4.0.2/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/options.py` & `django_import_export-4.0.2/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/resources.py` & `django_import_export-4.0.2/import_export/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -427,15 +427,26 @@
                 f"skipping field '{field}' "
                 f"- column name '{field.column_name}' is not present in row"
             )
             return
         field.save(instance, row, is_m2m, **kwargs)
 
     def get_import_fields(self):
-        return [self.fields[f] for f in self.get_import_order()]
+        import_fields = []
+        for field_name in self.get_import_order():
+            if field_name in self.fields:
+                import_fields.append(self.fields[field_name])
+                continue
+            # issue 1815
+            # allow for fields to be referenced by column_name in `fields` list
+            for field in self.fields.values():
+                if field.column_name == field_name:
+                    import_fields.append(field)
+                    continue
+        return import_fields
 
     def import_obj(self, obj, data, dry_run, **kwargs):
         warn(
             "The 'import_obj' method is deprecated and will be replaced "
             "with 'import_instance(self, instance, row, **kwargs)' "
             "in a future release.  Refer to Release Notes for details.",
             DeprecationWarning,
@@ -1033,35 +1044,49 @@
 
         method = getattr(self, dehydrate_method, None)
         if method is not None:
             return method(instance)
         return field.export(instance)
 
     def get_export_fields(self):
-        return [self.fields[f] for f in self.get_export_order()]
+        export_fields = []
+        for field_name in self.get_export_order():
+            if field_name in self.fields:
+                export_fields.append(self.fields[field_name])
+                continue
+            # issue 1828
+            # allow for fields to be referenced by column_name in `fields` list
+            for field in self.fields.values():
+                if field.column_name == field_name:
+                    export_fields.append(field)
+                    continue
+        return export_fields
 
     def export_resource(self, instance, fields=None):
         export_fields = self.get_export_fields()
 
         if isinstance(fields, list) and fields:
             return [
                 self.export_field(field, instance)
                 for field in export_fields
-                if field.column_name in fields
+                if field.attribute in fields or field.column_name in fields
             ]
 
         return [self.export_field(field, instance) for field in export_fields]
 
     def get_export_headers(self, fields=None):
-        headers = [force_str(field.column_name) for field in self.get_export_fields()]
-
+        export_fields = self.get_export_fields()
         if isinstance(fields, list) and fields:
-            return [f for f in headers if f in fields]
+            return [
+                f.column_name
+                for f in export_fields
+                if f.attribute in fields or f.column_name in fields
+            ]
 
-        return headers
+        return [force_str(field.column_name) for field in export_fields]
 
     def get_user_visible_fields(self):
         return self.get_fields()
 
     def iter_queryset(self, queryset):
         if not isinstance(queryset, QuerySet):
             yield from queryset
@@ -1093,15 +1118,16 @@
             queryset = self.get_queryset()
         queryset = self.filter_export(queryset, **kwargs)
         export_fields = kwargs.get("export_fields", None)
         headers = self.get_export_headers(fields=export_fields)
         dataset = tablib.Dataset(headers=headers)
 
         for obj in self.iter_queryset(queryset):
-            dataset.append(self.export_resource(obj, fields=export_fields))
+            r = self.export_resource(obj, fields=export_fields)
+            dataset.append(r)
 
         self.after_export(queryset, dataset, **kwargs)
 
         return dataset
 
     def _get_ordered_field_names(self, order_field):
         """
@@ -1110,15 +1136,19 @@
         # get any declared 'order' fields
         order_fields = getattr(self._meta, order_field) or ()
         # get any defined fields
         defined_fields = order_fields + tuple(getattr(self._meta, "fields") or ())
 
         order = list()
         [order.append(f) for f in defined_fields if f not in order]
-        return tuple(order) + tuple(k for k in self.fields if k not in order)
+        declared_fields = []
+        for field_name, field in self.fields.items():
+            if field_name not in order and field.column_name not in order:
+                declared_fields.append(field_name)
+        return tuple(order) + tuple(declared_fields)
 
     def _is_using_transactions(self, kwargs):
         return kwargs.get("using_transactions", False)
 
     def _is_dry_run(self, kwargs):
         return kwargs.get("dry_run", False)
 
@@ -1244,14 +1274,16 @@
             # issue 1804
             # The field class may be in a third party library as a subclass
             # of a standard field class.
             # iterate base classes to determine the correct widget class to use.
             for base_class in inspect.getmro(f.__class__):
                 if base_class.__name__ in cls.WIDGETS_MAP:
                     result = cls.WIDGETS_MAP[base_class.__name__]
+                    if isinstance(result, str):
+                        result = getattr(cls, result)(f)
                     break
 
             try:
                 from django.contrib.postgres.fields import ArrayField
             except ImportError:
                 # ImportError: No module named psycopg2.extras
                 class ArrayField:
@@ -1286,15 +1318,19 @@
 
         FieldWidget = cls.widget_from_django_field(django_field)
         widget_kwargs = cls.widget_kwargs_for_field(field_name, django_field)
 
         attribute = field_name
         column_name = field_name
         # To solve #974
-        if isinstance(django_field, ForeignKey) and "__" not in column_name:
+        if (
+            isinstance(django_field, ForeignKey)
+            and "__" not in column_name
+            and not cls._meta.use_natural_foreign_keys
+        ):
             attribute += "_id"
             widget_kwargs["key_is_id"] = True
 
         field = cls.DEFAULT_RESOURCE_FIELD(
             attribute=attribute,
             column_name=column_name,
             widget=FieldWidget(**widget_kwargs),
```

### Comparing `django_import_export-4.0.1/import_export/results.py` & `django_import_export-4.0.2/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.2/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.2/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/static/import_export/import.css` & `django_import_export-4.0.2/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.2/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.2/import_export/templates/admin/import_export/export.html`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 {% endblock %}
 
 {% block breadcrumbs_last %}
 {% translate "Export" %}
 {% endblock %}
 
 {% block content %}
+{% if form.errors %}
+  {{ form.errors }}
+{% endif %}
 <form action="{{ export_url }}" method="POST">
   {% csrf_token %}
     {# export request has originated from an Admin UI action #}
     {% if form.initial.export_items %}
       <p>
       {% blocktranslate count len=form.initial.export_items|length %}
         Export {{ len }} selected item.
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% extends "admin/import_export/base.html" %} {% load i18n %} {% load
 admin_urls %} {% load import_export_tags %} {% block extrahead %}{{ block.super
 }}
 {{ form.media }} {% endblock %} {% block breadcrumbs_last %} {% translate
-"Export" %} {% endblock %} {% block content %}
+"Export" %} {% endblock %} {% block content %} {% if form.errors %} {
+{ form.errors }} {% endif %}
 {% csrf_token %} {# export request has originated from an Admin UI action #} {%
 if form.initial.export_items %}
 {% blocktranslate count len=form.initial.export_items|length %} Export {{ len
 }} selected item. {% plural %} Export {{ len }} selected items. {%
 endblocktranslate %}
 {% endif %} {# fields list is not required with selectable fields form #} {% if
 not form.is_selectable_fields_form %} {% include "admin/import_export/
```

### Comparing `django_import_export-4.0.1/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.2/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.2/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/tmp_storages.py` & `django_import_export-4.0.2/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/utils.py` & `django_import_export-4.0.2/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/import_export/widgets.py` & `django_import_export-4.0.2/import_export/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils import timezone
 from django.utils.dateparse import parse_duration
 from django.utils.encoding import force_str, smart_str
 from django.utils.formats import number_format
 from django.utils.translation import gettext_lazy as _
 
+from import_export.exceptions import WidgetError
+
 logger = logging.getLogger(__name__)
 
 
 def format_datetime(value, datetime_format):
-    # conditional logic to handle correct formatting of dates
+    # handle correct formatting of dates
     # see https://code.djangoproject.com/ticket/32738
-    if django.VERSION[0] >= 4:
-        format = django.utils.formats.sanitize_strftime_format(datetime_format)
-        return value.strftime(format)
-    else:
-        return django.utils.datetime_safe.new_datetime(value).strftime(datetime_format)
+    format_ = django.utils.formats.sanitize_strftime_format(datetime_format)
+    return value.strftime(format_)
 
 
 class Widget:
     """
     A Widget handles converting between import and export representations.
     """
 
@@ -493,14 +492,18 @@
         key_is_id=False,
         **kwargs,
     ):
         self.model = model
         self.field = field
         self.key_is_id = key_is_id
         self.use_natural_foreign_keys = use_natural_foreign_keys
+        if use_natural_foreign_keys is True and key_is_id is True:
+            raise WidgetError(
+                _("use_natural_foreign_keys and key_is_id cannot both be True")
+            )
         super().__init__(**kwargs)
 
     def get_queryset(self, value, row, *args, **kwargs):
         """
         Returns a queryset of all objects for this Model.
 
         Overwrite this method if you want to limit the pool of objects from
```

### Comparing `django_import_export-4.0.1/pyproject.toml` & `django_import_export-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/runtests.py` & `django_import_export-4.0.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/runtests.sh` & `django_import_export-4.0.2/runtests.sh`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/admin.py` & `django_import_export-4.0.2/tests/core/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.contrib import admin
 
 from import_export.admin import (
     ExportActionModelAdmin,
     ImportExportModelAdmin,
     ImportMixin,
 )
+from import_export.fields import Field
 from import_export.resources import ModelResource
 
 from .forms import CustomConfirmImportForm, CustomExportForm, CustomImportForm
 from .models import Author, Book, Category, Child, EBook, UUIDCategory
 
 
 class ChildAdmin(ImportMixin, admin.ModelAdmin):
@@ -46,31 +47,29 @@
 
 
 class AuthorAdmin(ImportMixin, admin.ModelAdmin):
     pass
 
 
 class EBookResource(ModelResource):
+    published = Field(attribute="published", column_name="published_date")
+
     def __init__(self, **kwargs):
         super().__init__()
         self.author_id = kwargs.get("author_id")
 
     def filter_export(self, queryset, **kwargs):
         return queryset.filter(author_id=self.author_id)
 
     class Meta:
         model = EBook
-        fields = (
-            "id",
-            "author_email",
-            "name",
-        )
+        fields = ("id", "author_email", "name", "published")
 
 
-class CustomBookAdmin(ImportExportModelAdmin):
+class CustomBookAdmin(ExportActionModelAdmin, ImportExportModelAdmin):
     """Example usage of custom import / export forms"""
 
     resource_classes = [EBookResource]
     import_form_class = CustomImportForm
     confirm_form_class = CustomConfirmImportForm
     export_form_class = CustomExportForm
 
@@ -93,18 +92,18 @@
         kwargs.update({"user": request.user})
         return kwargs
 
     def get_export_resource_kwargs(self, request, **kwargs):
         # this is overridden to demonstrate that custom form fields can be used
         # to override the export query.
         # The dict returned here will be passed as kwargs to EBookResource
-        export_form = kwargs["export_form"]
+        export_form = kwargs.get("export_form")
         if export_form:
-            return dict(author_id=export_form.cleaned_data["author"].id)
-        return {}
+            kwargs.update(author_id=export_form.cleaned_data["author"].id)
+        return kwargs
 
 
 admin.site.register(Book, BookAdmin)
 admin.site.register(Category, CategoryAdmin)
 admin.site.register(Author, AuthorAdmin)
 admin.site.register(Child, ChildAdmin)
 admin.site.register(EBook, CustomBookAdmin)
```

### Comparing `django_import_export-4.0.1/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.2/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/exports/books.json` & `django_import_export-4.0.2/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/exports/books.xls` & `django_import_export-4.0.2/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/exports/books.xlsx` & `django_import_export-4.0.2/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/fixtures/book.json` & `django_import_export-4.0.2/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/forms.py` & `django_import_export-4.0.2/tests/core/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from django import forms
 
-from import_export.forms import ConfirmImportForm, ExportForm, ImportForm
+from import_export.forms import (
+    ConfirmImportForm,
+    ImportForm,
+    SelectableFieldsExportForm,
+)
 
 from .models import Author
 
 
 class AuthorFormMixin(forms.Form):
     author = forms.ModelChoiceField(queryset=Author.objects.all(), required=True)
 
@@ -17,11 +21,11 @@
 
 class CustomConfirmImportForm(AuthorFormMixin, ConfirmImportForm):
     """Customized ConfirmImportForm, with author field required"""
 
     pass
 
 
-class CustomExportForm(AuthorFormMixin, ExportForm):
+class CustomExportForm(AuthorFormMixin, SelectableFieldsExportForm):
     """Customized ExportForm, with author field required"""
 
     pass
```

### Comparing `django_import_export-4.0.1/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.2/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.2/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.2/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.2/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.2/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.2/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.2/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.2/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.2/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/migrations/0015_withpositiveintegerfields.py` & `django_import_export-4.0.2/tests/core/migrations/0015_withpositiveintegerfields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/models.py` & `django_import_export-4.0.2/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.2/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/admin_integration/test_action_export.py` & `django_import_export-4.0.2/tests/core/tests/admin_integration/test_action_export.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,14 +124,33 @@
                     "selected_across": "0",
                     "_selected_action": "0",
                 },
             )
             self.assertTrue(200 <= response.status_code <= 399)
             mock_export_admin_action.assert_called()
 
+    def test_export_admin_action_with_restricted_pks(self):
+        data = {
+            "format": "0",
+            "export_items": [str(self.cat1.id)],
+            **self.resource_fields_payload,
+        }
+        # mock returning a set of pks which is not in the submitted range
+        with mock.patch(
+            "import_export.admin.ExportMixin.get_valid_export_item_pks"
+        ) as mock_valid_pks:
+            mock_valid_pks.return_value = [999]
+            response = self.client.post(self.category_export_url, data)
+            self.assertEqual(response.status_code, 200)
+            self.assertIn(
+                "Select a valid choice. "
+                f"{self.cat1.id} is not one of the available choices.",
+                str(response.content),
+            )
+
     def test_get_export_data_raises_PermissionDenied_when_no_export_permission_assigned(
         self,
     ):
         request = MagicMock(spec=HttpRequest)
 
         class TestMixin(ExportMixin):
             model = Book
```

### Comparing `django_import_export-4.0.1/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.2/tests/core/tests/admin_integration/test_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from datetime import datetime
+from datetime import date, datetime
 from io import BytesIO
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 import chardet
 import tablib
-from core.admin import BookAdmin, BookResource
+from core.admin import BookAdmin, BookResource, EBookResource
 from core.models import Author, Book, UUIDCategory
 from core.tests.admin_integration.mixins import AdminTestMixin
 from core.tests.utils import ignore_utcnow_deprecation_warning
 from django.contrib.admin.sites import AdminSite
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.models import User
 from django.core.exceptions import FieldError
@@ -41,15 +41,15 @@
         self.assertNotIn("Export 0 selected items.", str(response.content))
         form = response.context["form"]
         self.assertEqual(2, len(form.fields["resource"].choices))
 
         data = {"format": "0", **self.bookresource_export_fields_payload}
         date_str = datetime.now().strftime("%Y-%m-%d")
         # Should not contain COUNT queries from ModelAdmin.get_results()
-        with self.assertNumQueries(6):
+        with self.assertNumQueries(5):
             response = self.client.post(self.book_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="Book-{}.csv"'.format(date_str),
@@ -304,35 +304,65 @@
     def test_export_model_with_custom_PK(self):
         # issue 1800
         UUIDCategory.objects.create(name="UUIDCategory")
         response = self.client.get(self.uuid_category_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "UUIDCategoryResource")
 
+    def test_export_with_custom_field(self):
+        # issue 1808
+        a = Author.objects.create(id=11, name="Ian Fleming")
+        data = {
+            "format": "0",
+            "author": a.id,
+            "resource": "",
+            "ebookresource_id": True,
+            "ebookresource_author_email": True,
+            "ebookresource_name": True,
+            "ebookresource_published": True,
+        }
+        date_str = datetime.now().strftime("%Y-%m-%d")
+        response = self.client.post(self.ebook_export_url, data)
+        self.assertEqual(response.status_code, 200)
+        self.assertTrue(response.has_header("Content-Disposition"))
+        self.assertEqual(response["Content-Type"], "text/csv")
+        self.assertEqual(
+            response["Content-Disposition"],
+            'attachment; filename="EBook-{}.csv"'.format(date_str),
+        )
+        self.assertEqual(b"id,author_email,name,published_date\r\n", response.content)
+
 
 class FilteredExportAdminIntegrationTest(AdminTestMixin, TestCase):
     fixtures = ["category", "book", "author"]
 
     def test_export_filters_by_form_param(self):
         # issue 1578
         author = Author.objects.get(name="Ian Fleming")
 
-        data = {"format": "0", "author": str(author.id)}
+        data = {
+            "format": "0",
+            "author": str(author.id),
+            "ebookresource_id": True,
+            "ebookresource_author_email": True,
+            "ebookresource_name": True,
+            "ebookresource_published": True,
+        }
         date_str = datetime.now().strftime("%Y-%m-%d")
         response = self.client.post(self.ebook_export_url, data)
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
         self.assertEqual(
-            b"id,author_email,name\r\n"
-            b"5,ian@example.com,The Man with the Golden Gun\r\n",
+            b"id,author_email,name,published_date\r\n"
+            b"5,ian@example.com,The Man with the Golden Gun,1965-04-01\r\n",
             response.content,
         )
 
 
 class TestExportEncoding(TestCase):
     mock_request = MagicMock(spec=HttpRequest)
     mock_request.POST = {"format": 0, "bookresource_id": True}
@@ -431,7 +461,48 @@
 
         for index, resource in enumerate(form_resources):
             resource_fields = resource().get_export_order()
             self.assertEqual(
                 response_content.count(f'resource-index="{index}"'),
                 len(resource_fields),
             )
+
+
+class CustomColumnNameExportTest(AdminTestMixin, TestCase):
+    """Test export ok when column name is defined in fields list (issue 1828)."""
+
+    def setUp(self):
+        super().setUp()
+        EBookResource._meta.fields = ("id", "author_email", "name", "published_date")
+
+    def tearDown(self):
+        super().tearDown()
+        EBookResource._meta.fields = ("id", "author_email", "name", "published")
+
+    def test_export_with_custom_field(self):
+        a = Author.objects.create(id=11, name="Ian Fleming")
+        book = Book.objects.create(
+            name="Moonraker", author=a, published=date(1955, 4, 5)
+        )
+        data = {
+            "format": "0",
+            "author": a.id,
+            "resource": "",
+            "ebookresource_id": True,
+            "ebookresource_author_email": True,
+            "ebookresource_name": True,
+            "ebookresource_published_date": True,
+        }
+        date_str = datetime.now().strftime("%Y-%m-%d")
+        response = self.client.post(self.ebook_export_url, data)
+        self.assertEqual(response.status_code, 200)
+        self.assertTrue(response.has_header("Content-Disposition"))
+        self.assertEqual(response["Content-Type"], "text/csv")
+        self.assertEqual(
+            response["Content-Disposition"],
+            'attachment; filename="EBook-{}.csv"'.format(date_str),
+        )
+        s = (
+            "id,author_email,name,published_date\r\n"
+            f"{book.id},,Moonraker,1955-04-05\r\n"
+        )
+        self.assertEqual(str.encode(s), response.content)
```

### Comparing `django_import_export-4.0.1/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.2/tests/core/tests/admin_integration/test_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import os
 import warnings
 from io import StringIO
 from unittest import mock
 from unittest.mock import patch
 
-from core.admin import AuthorAdmin, BookAdmin, CustomBookAdmin, ImportMixin
+from core.admin import (
+    AuthorAdmin,
+    BookAdmin,
+    CustomBookAdmin,
+    EBookResource,
+    ImportMixin,
+)
 from core.models import Author, Book, EBook, Parent
 from core.tests.admin_integration.mixins import AdminTestMixin
 from django.contrib.admin.models import DELETION, LogEntry
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.models import User
 from django.test import RequestFactory
 from django.test.testcases import TestCase, TransactionTestCase
@@ -928,22 +934,76 @@
             self.ebook_import_url,
             "books.csv",
             input_format="0",
             data={"author": author_id},
         )
         # test header rendered in correct order
         target_header_re = (
-            r"<thead>[\\n\s]+<tr>[\\n\s]+<th></th>[\\n\s]+<th>id</th>"
-            r"[\\n\s]+<th>author_email</th>[\\n\s]+<th>name</th>[\\n\s]+</tr>[\\n\s]+"
+            r"<thead>[\\n\s]+"
+            r"<tr>[\\n\s]+"
+            r"<th></th>[\\n\s]+"
+            r"<th>id</th>[\\n\s]+"
+            r"<th>author_email</th>[\\n\s]+"
+            r"<th>name</th>[\\n\s]+"
+            r"<th>published_date</th>[\\n\s]+"
+            r"</tr>[\\n\s]+"
             "</thead>"
         )
         self.assertRegex(str(response.content), target_header_re)
         # test row rendered in correct order
         target_row_re = (
             r'<tr class="new">[\\n\s]+'
             r'<td class="import-type">[\\n\s]+New[\\n\s]+</td>[\\n\s]+'
             r'<td><ins style="background:#e6ffe6;">1</ins></td>[\\n\s]+'
             r'<td><ins style="background:#e6ffe6;">test@example.com</ins></td>[\\n\s]+'
             r'<td><ins style="background:#e6ffe6;">Some book</ins></td>[\\n\s]+'
+            r"<td><span>None</span></td>[\\n\s]+"
+            "</tr>"
+        )
+        self.assertRegex(str(response.content), target_row_re)
+
+
+class CustomColumnNameImportTest(AdminTestMixin, TestCase):
+    """Handle custom column name import (issue 1822)."""
+
+    fixtures = ["author"]
+
+    def setUp(self):
+        super().setUp()
+        EBookResource._meta.fields = ("id", "author_email", "name", "published_date")
+
+    def tearDown(self):
+        super().tearDown()
+        EBookResource._meta.fields = ("id", "author_email", "name", "published")
+
+    def test_import_preview_order(self):
+        author_id = Author.objects.first().id
+        response = self._do_import_post(
+            self.ebook_import_url,
+            "books.csv",
+            input_format="0",
+            data={"author": author_id},
+        )
+        # test header rendered in correct order
+        target_header_re = (
+            r"<thead>[\\n\s]+"
+            r"<tr>[\\n\s]+"
+            r"<th></th>[\\n\s]+"
+            r"<th>id</th>[\\n\s]+"
+            r"<th>author_email</th>[\\n\s]+"
+            r"<th>name</th>[\\n\s]+"
+            r"<th>published_date</th>[\\n\s]+"
+            r"</tr>[\\n\s]+"
+            "</thead>"
+        )
+        self.assertRegex(str(response.content), target_header_re)
+        # test row rendered in correct order
+        target_row_re = (
+            r'<tr class="new">[\\n\s]+'
+            r'<td class="import-type">[\\n\s]+New[\\n\s]+</td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">1</ins></td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">test@example.com</ins></td>[\\n\s]+'
+            r'<td><ins style="background:#e6ffe6;">Some book</ins></td>[\\n\s]+'
+            r"<td><span>None</span></td>[\\n\s]+"
             "</tr>"
         )
         self.assertRegex(str(response.content), target_row_re)
```

### Comparing `django_import_export-4.0.1/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.2/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/resources.py` & `django_import_export-4.0.2/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.2/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_declarative.py` & `django_import_export-4.0.2/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_fields.py` & `django_import_export-4.0.2/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_forms.py` & `django_import_export-4.0.2/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.2/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.2/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_mixins.py` & `django_import_export-4.0.2/tests/core/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_model_resource_fields_generate_widgets.py` & `django_import_export-4.0.2/tests/core/tests/test_model_resource_fields_generate_widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import django
 from core.models import WithPositiveIntegerFields
 from django.contrib.contenttypes import fields as contenttype_fields
 from django.contrib.postgres import fields as postgres
 from django.contrib.postgres import search as postgres_search
 from django.contrib.postgres.fields import ranges as postgres_ranges
 from django.db import models
-from django.db.models.fields.related import RelatedField
+from django.db.models.fields.related import ForeignKey, RelatedField
 
 from import_export import widgets
 from import_export.resources import ModelResource
+from import_export.widgets import ForeignKeyWidget
 
 
 class ExampleResource(ModelResource):
     class Meta:
         model = WithPositiveIntegerFields
 
 
@@ -184,7 +185,26 @@
             postgres.DecimalRangeField(),
             postgres.HStoreField(),
             postgres.IntegerRangeField(),
             postgres.JSONField(),
             postgres.RangeField(),
         ]
         return fields
+
+    def test_custom_fk_field(self):
+        # issue 1817 - if a 'custom' foreign key field is provided, then this should
+        # be handled when widgets are defined
+        class CustomForeignKey(ForeignKey):
+            def __init__(
+                self,
+                to,
+                on_delete,
+                **kwargs,
+            ):
+                super().__init__(to, on_delete, **kwargs)
+
+        resource_field = ModelResource.field_from_django_field(
+            "custom_fk",
+            CustomForeignKey(WithPositiveIntegerFields, on_delete=models.SET_NULL),
+            False,
+        )
+        self.assertEqual(ForeignKeyWidget, resource_field.widget.__class__)
```

### Comparing `django_import_export-4.0.1/tests/core/tests/test_permissions.py` & `django_import_export-4.0.2/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_import_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import date
 from unittest.mock import patch
 
 import tablib
-from core.models import Author, Book, Category
+from core.models import Author, Book, Category, EBook
 from core.tests.resources import AuthorResource, BookResource
 from django.test import TestCase
 
 from import_export import exceptions, fields, resources, widgets
+from import_export.fields import Field
+from import_export.resources import ModelResource
 
 
 class AfterImportComparisonTest(TestCase):
     class BookResource(resources.ModelResource):
         is_published = False
 
         def after_import_row(self, row, row_result, **kwargs):
@@ -368,7 +370,36 @@
     def test_import_row_with_no_defined_id_field(self):
         """Ensure a row with no id field can be imported (issue 1812)."""
         self.assertEqual(0, Author.objects.count())
         dataset = tablib.Dataset(*[("J. R. R. Tolkien",)], headers=["name"])
         self.resource = AuthorResource()
         self.resource.import_data(dataset)
         self.assertEqual(1, Author.objects.count())
+
+
+class CustomColumnNameImportTest(TestCase):
+    """
+    If a custom field is declared, import should work if either the Field's
+    attribute name or column name is referenced in the ``fields`` list (issue 1815).
+    """
+
+    fixtures = ["author"]
+
+    class _EBookResource(ModelResource):
+        published = Field(attribute="published", column_name="published_date")
+
+        class Meta:
+            model = EBook
+            fields = ("id", "name", "published_date")
+
+    def setUp(self):
+        super().setUp()
+        self.resource = CustomColumnNameImportTest._EBookResource()
+
+    def test_import_with_column_alias_in_fields_list(self):
+        self.assertEqual(0, EBook.objects.count())
+        dataset = tablib.Dataset(
+            *[(1, "Moonraker", "1955-04-05")], headers=["id", "name", "published_date"]
+        )
+        self.resource.import_data(dataset, raise_errors=True)
+        self.assertEqual(1, EBook.objects.count())
+        self.assertEqual(date(1955, 4, 5), EBook.objects.first().published)
```

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import tablib
+from core.admin import BookResource
 from core.models import Author, Book
 from django.test import TestCase
 
-from tests.core.tests.resources import BookResource
-
 
 class ExportFunctionalityTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
@@ -18,15 +17,16 @@
         self.assertEqual(
             headers,
             [
                 "id",
                 "name",
                 "author",
                 "author_email",
-                "published_date",
+                "imported",
+                "published",
                 "published_time",
                 "price",
                 "added",
                 "categories",
             ],
         )
```

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_modelresource/test_widget.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_widget.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.2/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_results.py` & `django_import_export-4.0.2/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.2/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/core/tests/test_widgets.py` & `django_import_export-4.0.2/tests/core/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from core.models import Author, Book, Category
 from core.tests.utils import ignore_utcnow_deprecation_warning
 from django.test import TestCase
 from django.test.utils import override_settings
 from django.utils import timezone
 
 from import_export import widgets
+from import_export.exceptions import WidgetError
 
 
 class WidgetTest(TestCase):
     def setUp(self):
         self.widget = widgets.Widget()
 
     def test_clean(self):
@@ -578,14 +579,24 @@
         can be rendered
         """
         self.assertEqual(
             self.natural_key_book_widget.render(self.book),
             json.dumps(self.book.natural_key()),
         )
 
+    def test_natural_foreign_key_with_key_is_id(self):
+        with self.assertRaises(WidgetError) as e:
+            widgets.ForeignKeyWidget(
+                Author, use_natural_foreign_keys=True, key_is_id=True
+            )
+        self.assertEqual(
+            "use_natural_foreign_keys and key_is_id " "cannot both be True",
+            str(e.exception),
+        )
+
 
 class ManyToManyWidget(TestCase, RowDeprecationTestMixin):
     def setUp(self):
         self.widget = widgets.ManyToManyWidget(Category)
         self.widget_name = widgets.ManyToManyWidget(Category, field="name")
         self.cat1 = Category.objects.create(name="Cat úňíčóďě")
         self.cat2 = Category.objects.create(name="Cat 2")
```

### Comparing `django_import_export-4.0.1/tests/docker-compose.yml` & `django_import_export-4.0.2/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/scripts/bulk_import.py` & `django_import_export-4.0.2/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tests/settings.py` & `django_import_export-4.0.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.1/tox.ini` & `django_import_export-4.0.2/tox.ini`

 * *Files identical despite different names*

