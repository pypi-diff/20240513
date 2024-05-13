# Comparing `tmp/lunes-cms-2023.7.0.tar.gz` & `tmp/lunes-cms-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunes-cms-2023.7.0.tar", last modified: Wed Jul 26 15:50:40 2023, max compression
+gzip compressed data, was "lunes-cms-2024.5.0.tar", last modified: Mon May 13 08:32:43 2024, max compression
```

## Comparing `lunes-cms-2023.7.0.tar` & `lunes-cms-2024.5.0.tar`

### file list

```diff
@@ -1,148 +1,156 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1485 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/permissions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/api/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/templates/swagger_ui.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4970 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/discipline_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/feedback_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1180 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/group_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/training_set_serializer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2011 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.702255 lunes-cms-2023.7.0/lunes_cms/api/v1/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1708 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1130 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/feedback_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1412 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/group_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/sponsors_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_viewset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/api/v1/views/word_viewset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1927 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/admins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/alternative_word_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11922 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/discipline_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7099 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/document_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/document_image_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/feedback_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      313 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/group_api_key_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/sponsor_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13090 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/admins/training_set_admin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/apps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2854 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/forms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10273 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/list_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.706255 lunes-cms-2023.7.0/lunes_cms/cms/migrations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12781 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0001_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1787 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0002_modify_group_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2813 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0004_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1431 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0005_auto_create_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3244 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2476 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0009_sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0010_sponsor_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/0011_document_example_sentence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/migrations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/alternative_word.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/content_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/discipline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3885 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/document_image.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2891 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4574 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/group_api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/sponsor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3027 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/static.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/models/training_set.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/cms/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/discipline_filter.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/object_delete_summary.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/templatetags/admin_filter_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1519 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4543 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/validators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/cms/widgets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/context_processors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/logging_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/urls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/core/wsgi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/apps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5641 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/templates/public_upload.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/urls.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.710255 lunes-cms-2023.7.0/lunes_cms/help/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/views/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2128 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/help/views/public_upload.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/locale/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/locale/de/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10631 2023-07-26 15:50:29.000000 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2023-07-26 15:50:29.000000 lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/lunes-cms-cli
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/static/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6573 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/css/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/corporate_identity.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/feedback.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/css/overlay.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/guidelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/guidelines/fotoguide.pdf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/fallback-icon.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes-dark.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/images/logo.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.714255 lunes-cms-2023.7.0/lunes_cms/static/js/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/corporate_identity.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/image_preview.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/manytomany_overlay.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/lunes_cms/static/js/overlay.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:50:40.698255 lunes-cms-2023.7.0/lunes_cms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3005 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4504 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-07-26 15:50:40.000000 lunes-cms-2023.7.0/lunes_cms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2428 2023-07-26 15:50:40.718255 lunes-cms-2023.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2023-07-26 15:50:37.000000 lunes-cms-2023.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1136 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/NOTICE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1577 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/permissions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/templates/swagger_ui.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4961 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.209021 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      433 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/alternative_word_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_list_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      540 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      812 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/feedback_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/group_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/sponsor_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      543 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1902 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.213021 lunes-cms-2024.5.0/lunes_cms/api/v1/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1870 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/feedback_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/group_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/sponsors_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1591 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_viewset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1858 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/api/v1/views/word_viewset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.213021 lunes-cms-2024.5.0/lunes_cms/cms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      128 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admin.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.217022 lunes-cms-2024.5.0/lunes_cms/cms/admins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/alternative_word_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12953 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/discipline_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8083 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/document_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/document_image_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/feedback_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/group_api_key_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/sponsor_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14258 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/admins/training_set_admin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/apps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2797 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/forms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10231 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/list_filter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.217022 lunes-cms-2024.5.0/lunes_cms/cms/migrations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12826 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0001_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0003_remove_documentimage_name.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2868 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0004_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3316 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2571 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0009_sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0010_sponsor_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0011_document_example_sentence.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0012_add_additional_field.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0013_add_plural_field.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2500 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/migrations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/alternative_word.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/content_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3035 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/discipline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4461 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/document_image.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4886 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/group_api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/sponsor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3332 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/static.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3390 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/models/training_set.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/cms/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3954 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/discipline_filter.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/object_delete_summary.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.221022 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/templatetags/admin_filter_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/validators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/cms/widgets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/context_processors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/logging_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17883 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1690 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/urls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/core/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      320 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/apps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5641 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/templates/public_upload.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      353 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/urls.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/help/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/views/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/help/views/public_upload.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/locale/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/locale/de/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10993 2024-05-13 08:32:34.000000 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-13 08:32:34.000000 lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      983 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/lunes-cms-cli
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.205021 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.225021 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6573 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/css/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/corporate_identity.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/document_form.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/feedback.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1384 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/css/overlay.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/guidelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1447497 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/guidelines/fotoguide.pdf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.229021 lunes-cms-2024.5.0/lunes_cms/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/fallback-icon.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes-dark.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      933 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/images/logo.svg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/lunes_cms/static/js/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      705 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/color_unread_feedback.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/corporate_identity.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1430 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/image_preview.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/manytomany_overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/overlay.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/lunes_cms/static/js/toggle_plural_field.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:32:43.233021 lunes-cms-2024.5.0/lunes_cms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4345 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4873 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-05-13 08:32:43.000000 lunes-cms-2024.5.0/lunes_cms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2024-05-13 08:32:43.237022 lunes-cms-2024.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      187 2024-05-13 08:32:40.000000 lunes-cms-2024.5.0/setup.py
```

### Comparing `lunes-cms-2023.7.0/LICENSE.txt` & `lunes-cms-2024.5.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -171,33 +170,7 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
```

### Comparing `lunes-cms-2023.7.0/MANIFEST.in` & `lunes-cms-2024.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/README.md` & `lunes-cms-2024.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![CircleCI](https://circleci.com/gh/digitalfabrik/lunes-cms.svg?style=shield)](https://circleci.com/gh/digitalfabrik/lunes-cms)
 ![Coverage](https://img.shields.io/codeclimate/coverage/digitalfabrik/lunes-cms)
 [![Documentation Status](https://readthedocs.org/projects/lunes-cms/badge/?version=latest)](https://lunes-cms.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/github/license/digitalfabrik/lunes-cms)](https://opensource.org/licenses/Apache-2.0)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Pylint](https://img.shields.io/badge/pylint-10.00-brightgreen)](https://www.pylint.org/)
 
 # Lunes CMS
 
 [![Logo](https://lunes.tuerantuer.org/static/images/logo-lunes.svg)](https://www.lunes.app)
 
 [Lunes - Vocabulary for your profession.](https://www.lunes.app)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/permissions.py` & `lunes-cms-2024.5.0/lunes_cms/api/permissions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from django.core.exceptions import PermissionDenied
-from django.db.models import Q
-from django.utils.timezone import now
-
 from rest_framework import permissions
 
 from ..cms.models import GroupAPIKey
 from .utils import get_key
 
 
 class VerifyGroupKey(permissions.AllowAny):
-    """Simple permissions class that blocks
+    """
+    Simple permissions class that blocks
     requests if no valid API-Token is delivered.
     Inherits from `permissions.AllowAny`.
     """
 
     def has_permission(self, request, view):
-        """Checks whether a valid API-Key is send
+        """
+        Checks whether a valid API-Key is send
         by the user in the authorization header
 
         :param request: http request
         :type request: HttpRequest
         :param view: restframework view
         :type view: viewsets.ModelViewSet
         :return: False if user doesn't send a API-key
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/utils.py` & `lunes-cms-2024.5.0/lunes_cms/api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A collection of helper methods and classes
 """
 
 from django.core.exceptions import PermissionDenied
 from django.db.models import Count, Q
-
 from rest_framework import routers
 
 from ..cms.models import Discipline, GroupAPIKey
 from ..cms.utils import get_child_count
 
 
 class OptionalSlashRouter(routers.DefaultRouter):
@@ -34,15 +33,15 @@
     :return: api key in authorization header
     :rtype: str
     """
     authorization = request.META.get("HTTP_AUTHORIZATION")
     if not authorization:
         return None
     try:
-        _, key = authorization.split("{} ".format(keyword))
+        _, key = authorization.split(f"{keyword} ")
     except ValueError:
         key = None
     return key
 
 
 def get_filtered_discipline_queryset(discipline_view_set):
     """
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/__init__.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 from .alternative_word_serializer import AlternativeWordSerializer
 from .discipline_serializer import DisciplineSerializer
 from .document_image_list_serializer import DocumentImageListSerializer
 from .document_image_serializer import DocumentImageSerializer
 from .document_serializer import DocumentSerializer
 from .feedback_serializer import FeedbackSerializer
 from .group_serializer import GroupSerializer
-from .training_set_serializer import TrainingSetSerializer
 from .sponsor_serializer import SponsorSerializer
+from .training_set_serializer import TrainingSetSerializer
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/discipline_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/discipline_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 
     def get_total_discipline_children(self, obj):
         """Returns the total child count by calling
         utils.get_child_count(obj).
 
 
         :param disc: Discipline instance
-        :type disc: models.Discipline
+        :type disc: ~lunes_cms.cms.models.discipline.Discipline
         :return: sum of children
         :rtype: int
         """
         return get_child_count(obj)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_image_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_image_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/document_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/document_serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         Define model and the corresponding fields
         """
 
         model = Document
         fields = (
             "id",
             "word",
-            "article",
+            "singular_article",
             "audio",
             "word_type",
             "alternatives",
             "document_image",
             "example_sentence",
         )
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/fallback_icon_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/group_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/group_serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,14 @@
 
     def get_total_discipline_children(self, obj):
         """Returns the total child count of a group.
         A child itself or one of its sub-children needs to
         contain at least one training set.
 
         :param disc: Discipline instance
-        :type disc: models.Discipline
+        :type disc: ~lunes_cms.cms.models.discipline.Discipline
         :return: sum of children
         :rtype: int
         """
         queryset = Discipline.objects.filter(released=True, created_by=obj.id)
         queryset = [obj for obj in queryset if obj.is_root_node() and obj.is_valid()]
         return len(queryset)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/serializers/training_set_serializer.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/serializers/training_set_serializer.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/urls.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """
 URL patterns for the first version of the Lunes API
 """
-from django.urls import include, path, re_path
-
-from rest_framework import permissions
-from rest_framework.versioning import NamespaceVersioning
-
+from django.urls import include, path
 from drf_spectacular.views import SpectacularAPIView, SpectacularSwaggerView
 
 from ..utils import OptionalSlashRouter
 from . import views
 
-
 #: The namespace for this URL config (see :attr:`django.urls.ResolverMatch.app_name`)
 app_name = "v1"
 
 #: Router for dynamic url patterns
 router = OptionalSlashRouter()
 router.register(r"disciplines", views.DisciplineViewSet, "disciplines")
 router.register(
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_filtered_viewset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from rest_framework import mixins, viewsets
 
 from ....cms.models import Discipline
 from ...utils import (
-    get_filtered_discipline_queryset,
+    check_group_object_permissions,
     get_discipline_by_group_queryset,
+    get_filtered_discipline_queryset,
     get_overview_discipline_queryset,
-    check_group_object_permissions,
 )
 from ..serializers import DisciplineSerializer
 
 
 class DisciplineFilteredViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     """
     Defines a view set for the Discipline module, optionally filtered respected to
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/discipline_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/discipline_viewset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from django.core.exceptions import PermissionDenied
-from django.db.models import Q, Count
-
+from django.db.models import Count, Q
 from rest_framework import viewsets
 
 from ....cms.models import Discipline, GroupAPIKey
 from ...utils import get_key
 from ..serializers import DisciplineSerializer
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_by_id_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_by_id_viewset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from rest_framework import viewsets
-from rest_framework.authentication import SessionAuthentication, BasicAuthentication
+from rest_framework.authentication import BasicAuthentication, SessionAuthentication
 from rest_framework.permissions import IsAuthenticated
 
 from ....cms.models import Document
 from ..serializers import DocumentSerializer
 
 
 class DocumentByIdViewSet(viewsets.ModelViewSet):
@@ -26,10 +26,9 @@
         :type self: class
 
         :return: (filtered) queryset
         :rtype: QuerySet
         """
         if getattr(self, "swagger_fake_view", False):
             return Document.objects.none()
-        user = self.request.user
         queryset = Document.objects.filter(id=self.kwargs["document_id"])
         return queryset
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/document_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/document_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/group_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/group_viewset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from django.contrib.auth.models import Group
 from django.core.exceptions import PermissionDenied
-
 from rest_framework import viewsets
 
 from ....cms.models import GroupAPIKey, TrainingSet
 from ...permissions import VerifyGroupKey
 from ...utils import get_key
 from ..serializers import GroupSerializer
 
@@ -34,13 +33,13 @@
         if getattr(self, "swagger_fake_view", False):
             return TrainingSet.objects.none()
         key = get_key(self.request)
         if not key:
             raise PermissionDenied()
         try:
             api_key_object = GroupAPIKey.get_from_token(key)
-        except GroupAPIKey.DoesNotExist:
-            raise PermissionDenied()
+        except GroupAPIKey.DoesNotExist as e:
+            raise PermissionDenied() from e
         if not api_key_object:
             raise PermissionDenied()
         queryset = Group.objects.filter(id=api_key_object.group_id)
         return queryset
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/sponsors_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/sponsors_viewset.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_by_id_viewset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from rest_framework import viewsets
-from django.core.exceptions import PermissionDenied
 from django.db.models import Count, Q
+from rest_framework import viewsets
 
-from ....cms.models import TrainingSet, GroupAPIKey
+from ....cms.models import GroupAPIKey, TrainingSet
 from ...utils import get_key
 from ..serializers import TrainingSetSerializer
 
 
 class TrainingSetByIdViewSet(viewsets.ReadOnlyModelViewSet):
     """
     Defines a view set for a TrainingSet module of a given id.
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/training_set_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/training_set_viewset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.db.models import Count, Q
-
 from rest_framework import viewsets
 
 from ....cms.models import Discipline, TrainingSet
 from ...utils import check_group_object_permissions
 from ..serializers import TrainingSetSerializer
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/api/v1/views/word_viewset.py` & `lunes-cms-2024.5.0/lunes_cms/api/v1/views/word_viewset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.db.models import Q
-
 from rest_framework import viewsets
-from rest_framework.authentication import SessionAuthentication, BasicAuthentication
+from rest_framework.authentication import BasicAuthentication, SessionAuthentication
 
 from ....cms.models import Document, GroupAPIKey
 from ...utils import get_key
 from ..serializers import DocumentSerializer
 
 
 class WordViewSet(viewsets.ModelViewSet):
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 specify autocomplete_fields, search_fields and nested modules
 """
 from __future__ import absolute_import, unicode_literals
 
 from django.contrib import admin
 from django.utils.translation import ugettext_lazy as _
 
-from .models import Discipline, TrainingSet, Document, GroupAPIKey, Feedback, Sponsor
-from .admins import DisciplineAdmin
-from .admins import TrainingSetAdmin
-from .admins import DocumentAdmin
-from .admins import GroupAPIKeyAdmin
-from .admins import FeedbackAdmin
-from .admins import SponsorAdmin
+from .admins import (
+    DisciplineAdmin,
+    DocumentAdmin,
+    FeedbackAdmin,
+    GroupAPIKeyAdmin,
+    SponsorAdmin,
+    TrainingSetAdmin,
+)
+from .models import Discipline, Document, Feedback, GroupAPIKey, Sponsor, TrainingSet
 
 
 def get_app_list(self, request):
     """
     Function that returns a sorted list of all the installed apps that have been
     registered in this site.
 
@@ -32,14 +34,16 @@
     ordering = {
         _("disciplines").capitalize(): 1,
         _("training sets").capitalize(): 2,
         _("vocabulary").capitalize(): 3,
         _("api keys").capitalize(): 4,
         _("feedback").capitalize(): 5,
     }
+
+    # pylint: disable=protected-access
     app_dict = self._build_app_dict(request)
 
     # Sort the apps alphabetically.
     app_list = sorted(app_dict.values(), key=lambda x: x["name"].lower())
 
     # Sort the respective modules according the defined order
     for app in app_list:
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/discipline_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/discipline_admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.contrib import admin
-from django.db.models import Count, F, Q
+from django.db.models import Count, Q
 from django.db.models.functions import Greatest
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
-
 from mptt.admin import DraggableMPTTAdmin
 
-from ..models import Static, Discipline
+from ..models import Discipline, Static
 
 
 class DisciplineAdmin(DraggableMPTTAdmin):
     """
     Admin Interface to for the Discipline module.
     Inheriting from `mptt.admin.DraggableMPTTAdmin`.
     """
@@ -52,41 +51,41 @@
         """
         Overwrite django built-in function to save
         user group and admin status of model
 
         :param request: current user request
         :type request: django.http.request
         :param obj: discipline object
-        :type obj: models.Discipline
+        :type obj: ~lunes_cms.cms.models.discipline.Discipline
         :param form: employed model form
         :type form: ModelForm
         :param change: True if change on existing model
         :type change: bool
         :raises IndexError: Error when user is not superuser and doesn't belong to any group
         """
         if not change:
             if len(request.user.groups.all()) >= 1:
                 obj.created_by = request.user.groups.all()[0]
             elif not request.user.is_superuser:
                 raise IndexError("No group assigned. Please add the user to a group")
             obj.creator_is_admin = request.user.is_superuser
         obj.save()
 
-    def get_action_choices(self, request):
+    def get_action_choices(self, request, default_choices=""):
         """
         Overwrite django built-in function to modify action choices. The first
         option is dropped since it is a place holder.
 
         :param request: current user request
         :type request: django.http.request
 
         :return: modified action choices
         :rtype: dict
         """
-        choices = super(DisciplineAdmin, self).get_action_choices(request)
+        choices = super().get_action_choices(request)
         choices.pop(0)
         return choices
 
     def get_queryset(self, request):
         """
         Overwrite django built-in function to modify queryset according to user.
         Users that are not superusers only see disciplines of their groups.
@@ -203,15 +202,15 @@
                 "modules_released", "children_modules_released"
             ),
             modules_unreleased_order=Greatest(
                 "modules_unreleased", "children_modules_unreleased"
             ),
         )
 
-    def get_form(self, request, obj=None, **kwargs):
+    def get_form(self, request, obj=None, change=False, **kwargs):
         """
         Overwrite django built-in function to define custom choices
         in MPTT many to many selector for parent disciplines,
         e.g. users should not see disciplines by superusers.
         The function modifies the querysets of the
         corresponding base fields dynamically.
 
@@ -219,15 +218,15 @@
         :type request: django.http.request
         :param obj: django model object, defaults to None
         :type obj: django.db.models, optional
 
         :return: model form with adjusted querysets
         :rtype: ModelForm
         """
-        form = super(DisciplineAdmin, self).get_form(request, obj, **kwargs)
+        form = super().get_form(request, obj, **kwargs)
         if not request.user.is_superuser:
             form.base_fields["parent"].queryset = (
                 Discipline.objects.filter(
                     created_by__in=request.user.groups.all(),
                     training_sets__isnull=True,
                 )
                 .order_by("title")
@@ -271,38 +270,65 @@
         queryset.update(released=False)
 
     @admin.display(
         description=_("released modules"),
         ordering="modules_released_order",
     )
     def modules_released(self, obj):
+        """
+        returns HTML Tag of the link to released training sets related to the discipline
+
+        :param obj: Discipline object
+        :type obj: ~lunes_cms.cms.models.discipline.Discipline
+
+        :return: HTML Tag of the link to released training sets related to the discipline
+        :rtype: str
+        """
         if not obj.is_leaf_node():
             return obj.children_modules_released
         trainingset_list = reverse("admin:cms_trainingset_changelist")
         return mark_safe(
             f"<a href={trainingset_list}?disciplines={obj.id}&released__exact=1>{obj.modules_released}</a>"
         )
 
     @admin.display(
         description=_("unreleased modules"),
         ordering="modules_unreleased_order",
     )
     def modules_unreleased(self, obj):
+        """
+        returns HTML Tag of the link to unreleased training sets related to the discipline
+
+        :param obj: Discipline object
+        :type obj: ~lunes_cms.cms.models.discipline.Discipline
+
+        :return: HTML Tag of the link to unreleased training sets related to the discipline
+        :rtype: str
+        """
         if not obj.is_leaf_node():
             return obj.children_modules_unreleased
         trainingset_list = reverse("admin:cms_trainingset_changelist")
         return mark_safe(
             f"<a href={trainingset_list}?disciplines={obj.id}&released__exact=0>{obj.modules_unreleased}</a>"
         )
 
     @admin.display(
         description=_("published words in released modules"),
         ordering="-words_released_order",
     )
     def words_released(self, obj):
+        """
+        returns HTML Tag of the link to released words in the relased training sets related to the descipline
+
+        :param obj: Discipline object
+        :type obj: ~lunes_cms.cms.models.discipline.Discipline
+
+        :return:
+        :rtype: str
+        """
         if not obj.is_leaf_node():
             return obj.children_words_released
         document_list = reverse("admin:cms_document_changelist")
         return mark_safe(
             f"<a href={document_list}?disciplines={obj.id}&assigned=released&images=approved>{obj.words_released}</a>"
         )
 
@@ -310,21 +336,24 @@
         description=_("creator group"),
     )
     def creator_group(self, obj):
         """
         Include creator group of discipline in list display
 
         :param obj: Discipline object
-        :type obj: models.Discipline
+        :type obj: ~lunes_cms.cms.models.discipline.Discipline
 
         :return: Either static admin group or user group
         :rtype: str
         """
         if obj.creator_is_admin:
             return Static.admin_group
-        elif obj.created_by:
+        if obj.created_by:
             return obj.created_by
-        else:
-            return None
+        return None
 
     class Media:
+        """
+        Media class for admin interface for disciplines
+        """
+
         js = ("js/image_preview.js",)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/document_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/document_admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.contrib import admin
 from django.db.models import Case, Exists, IntegerField, OuterRef, Value, When
 from django.utils.translation import ugettext_lazy as _
 
 from ..list_filter import (
-    DocumentDisciplineListFilter,
-    DocumentTrainingSetListFilter,
     ApprovedImageListFilter,
     AssignedListFilter,
+    DocumentDisciplineListFilter,
+    DocumentTrainingSetListFilter,
 )
-from ..models import Static, DocumentImage
-from .document_image_admin import DocumentImageAdmin
+from ..models import DocumentImage, Static
 from .alternative_word_admin import AlternativeWordAdmin
-
+from .document_image_admin import DocumentImageAdmin
 
 SUPERUSER_ONLY_LIST_FILTERS = [ApprovedImageListFilter]
 
 
 class DocumentAdmin(admin.ModelAdmin):
     """
     Admin Interface to for the Document module.
     Inheriting from `admin.ModelAdmin`.
     """
 
-    exclude = ("article_plural", "creator_is_admin")
+    fields = (
+        "word_type",
+        "grammatical_gender",
+        ("singular_article", "word"),
+        ("plural_article", "plural"),
+        "audio",
+        "definition",
+        "additional_meaning_1",
+        "additional_meaning_2",
+    )
     readonly_fields = ("created_by",)
     search_fields = ["word", "alternatives__alt_word"]
     inlines = [DocumentImageAdmin, AlternativeWordAdmin]
     ordering = ["word", "creation_date"]
     list_display = (
         "word",
         "word_type",
-        "article_display",
+        "singular_article_display",
         "related_training_set",
+        "related_disciplines",
         "has_audio",
         "has_image",
         "creator_group",
         "creation_date",
     )
     list_filter = (
         DocumentDisciplineListFilter,
@@ -66,25 +75,25 @@
             if len(request.user.groups.all()) >= 1:
                 obj.created_by = request.user.groups.all()[0]
             elif not request.user.is_superuser:
                 raise IndexError("No group assigned. Please add the user to a group")
             obj.creator_is_admin = request.user.is_superuser
         obj.save()
 
-    def get_action_choices(self, request):
+    def get_action_choices(self, request, default_choices=""):
         """
         Overwrite django built-in function to modify action choices. The first
         option is dropped since it is a place holder.
 
         :param request: current user request
         :type request: django.http.request
         :return: modified action choices
         :rtype: dict
         """
-        choices = super(DocumentAdmin, self).get_action_choices(request)
+        choices = super().get_action_choices(request)
         choices.pop(0)
         return choices
 
     def get_queryset(self, request):
         """
         Overwrite django built-in function to modify queryset according to user.
         Users that are not superusers only see documents of their groups.
@@ -92,15 +101,15 @@
         :param request: current user request
         :type request: django.http.request
 
         :return: adjusted queryset
         :rtype: QuerySet
         """
         qs = (
-            super(DocumentAdmin, self)
+            super()
             .get_queryset(request)
             .annotate(
                 has_image=Exists(DocumentImage.objects.filter(document=OuterRef("pk"))),
                 has_confirmed_image=Exists(
                     DocumentImage.objects.filter(
                         document=OuterRef("pk"), confirmed=True
                     )
@@ -126,29 +135,48 @@
         :return: comma seperated list of related training sets
         :rtype: str
         """
         return ", ".join([child.title for child in obj.training_sets.all()])
 
     related_training_set.short_description = _("training set")
 
+    def related_disciplines(self, obj):
+        """
+        Display related desciplines in list display
+
+        :param obj: Document object
+        :type obj: models.Document
+        :return: comma seperated list of related training sets
+        :rtype: str
+        """
+        disciplines = []
+
+        for training_set in obj.training_sets.all():
+            disciplines += [
+                discipline.title for discipline in training_set.discipline.all()
+            ]
+
+        return ", ".join(disciplines)
+
+    related_disciplines.short_description = _("disciplines")
+
     def creator_group(self, obj):
         """
         Include creator group of discipline in list display
 
         :param obj: Document object
         :type obj: models.Document
         :return: Either static admin group or user group
         :rtype: str
         """
         if obj.creator_is_admin:
             return Static.admin_group
-        elif obj.created_by:
+        if obj.created_by:
             return obj.created_by
-        else:
-            return None
+        return None
 
     creator_group.short_description = _("creator group")
     creator_group.admin_order_field = "created_by"
 
     def has_audio(self, obj):
         """
         Include in list display whether a document has an audio file.
@@ -156,16 +184,15 @@
         :param obj: Document object
         :type obj: models.Document
         :return: Either static admin group or user group
         :rtype: str
         """
         if obj.audio:
             return True
-        else:
-            return False
+        return False
 
     has_audio.boolean = True
     has_audio.short_description = _("audio")
     has_audio.admin_order_field = "audio"
 
     def has_image(self, obj):
         """
@@ -183,27 +210,27 @@
             return None
         return False
 
     has_image.boolean = True
     has_image.short_description = _("image")
     has_image.admin_order_field = "image_sort"
 
-    def article_display(self, obj):
+    def singular_article_display(self, obj):
         """
         Include article of document in list display
 
         :param obj: Document object
         :type obj: models.Document
 
         :return: Either static admin group or user group
         :rtype: str
         """
-        return obj.get_article_display()
+        return obj.get_singular_article_display()
 
-    article_display.short_description = _("article")
+    singular_article_display.short_description = _("singular article")
 
     def get_list_filter(self, request):
         """
         Override djangos get_list_filter function
         to remove specific list filters that are only relevant
         for super users.
 
@@ -218,8 +245,16 @@
         if request.user.is_superuser:
             return self.list_filter
         # remove filters that are only relevant for super users
         filters = [f for f in self.list_filter if f not in SUPERUSER_ONLY_LIST_FILTERS]
         return tuple(filters)
 
     class Media:
-        js = ("js/image_preview.js",)
+        """
+        Media class of admin interface for documents
+        """
+
+        css = {"all": ("css/document_form.css",)}
+        js = (
+            "js/image_preview.js",
+            "js/toggle_plural_field.js",
+        )
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/document_image_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/document_image_admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         :type obj: django.db.models, optional
 
         :return: custom fields list
         :rtype: list[str]
         """
         if request.user.is_superuser and self.superuser_fields:
             return (self.fields or tuple()) + self.superuser_fields
-        return super(DocumentImageAdmin, self).get_fields(request, obj)
+        return super().get_fields(request, obj)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/feedback_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/feedback_admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,8 +64,13 @@
             request,
             _(
                 "The selected feedback entries were successfully marked as unread.",
             ),
         )
 
     class Media:
+        """
+        Media class for Feedback Admin
+        """
+
         css = {"all": ("css/feedback.css",)}
+        js = ("js/color_unread_feedback.js",)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/sponsor_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/sponsor_admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.contrib import admin
-
 from django.utils.translation import ugettext_lazy as _
 
 from ..utils import get_image_tag
 
 
 class SponsorAdmin(admin.ModelAdmin):
     """
@@ -44,8 +43,12 @@
         :rtype: str
         """
         return get_image_tag(obj.logo)
 
     image_tag.short_description = ""
 
     class Media:
+        """
+        Media class of Sponsor Admin
+        """
+
         js = ("js/image_preview.js",)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/admins/training_set_admin.py` & `lunes-cms-2024.5.0/lunes_cms/cms/admins/training_set_admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import absolute_import, unicode_literals
 
 from django.conf import settings
 from django.contrib import admin, messages
 from django.db.models import Count, F, Q
 from django.urls import reverse
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _, ngettext
-
+from django.utils.translation import ngettext
+from django.utils.translation import ugettext_lazy as _
 from mptt.admin import DraggableMPTTAdmin
 
-from ..list_filter import DisciplineListFilter
 from ..forms import TrainingSetForm
-from ..models import Static, Document, Discipline
+from ..list_filter import DisciplineListFilter
+from ..models import Discipline, Document, Static
 from ..utils import iter_to_string
 
 
 class TrainingSetAdmin(DraggableMPTTAdmin):
     """
     Admin Interface to for the TrainigSet module.
     Inheriting from `mptt.admin.DraggableMPTTAdmin`.
@@ -65,40 +65,40 @@
         """
         Overwrite django built-in function to save
         user group and admin status of model
 
         :param request: current user request
         :type request: django.http.request
         :param obj: training set object
-        :type obj: models.TrainingSet
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
         :param form: employed model form
         :type form: ModelForm
         :param change: True if change on existing model
         :type change: bool
         :raises IndexError: Error when user is not superuser and doesn't belong to any group
         """
         if not change:
             if len(request.user.groups.all()) >= 1:
                 obj.created_by = request.user.groups.all()[0]
             elif not request.user.is_superuser:
                 raise IndexError("No group assigned. Please add the user to a group")
             obj.creator_is_admin = request.user.is_superuser
         obj.save()
 
-    def get_action_choices(self, request):
+    def get_action_choices(self, request, default_choices=""):
         """
         Overwrite django built-in function to modify action choices. The first
         option is dropped since it is a place holder.
 
         :param request: current user request
         :type request: django.http.request
         :return: modified action choices
         :rtype: dict
         """
-        choices = super(TrainingSetAdmin, self).get_action_choices(request)
+        choices = super().get_action_choices(request)
         choices.pop(0)
         return choices
 
     def get_queryset(self, request):
         """
         Overwrite django built-in function to modify queryset according to user.
         Users that are not superusers only see training set of their groups.
@@ -133,29 +133,29 @@
             words=Count(
                 "documents",
                 filter=Q(documents__created_by__in=user_groups),
                 distinct=True,
             ),
         )
 
-    def get_form(self, request, obj=None, **kwargs):
+    def get_form(self, request, obj=None, change=False, **kwargs):
         """
         Overwrite django built-in function to define custom choices
         in many to many selectors, e.g. users should not see documents
         by superusers. The function modifies the querysets of the
         corresponding base fields dynamically.
 
         :param request: current user request
         :type request: django.http.request
         :param obj: django model object, defaults to None
         :type obj: django.db.models, optional
         :return: model form with adjusted querysets
         :rtype: ModelForm
         """
-        form = super(TrainingSetAdmin, self).get_form(request, obj, **kwargs)
+        form = super().get_form(request, obj, **kwargs)
         if not request.user.is_superuser:
             form.base_fields["discipline"].queryset = (
                 Discipline.objects.filter(
                     created_by__in=request.user.groups.all(), lft=F("rght") - 1
                 )
                 .order_by("title")
                 .order_by("level")
@@ -292,65 +292,92 @@
             )
 
     @admin.display(
         description=_("words"),
         ordering="-words",
     )
     def words(self, obj):
+        """
+        returns HTML tag of the link to the list of words related to the training set
+
+        :param obj: Training set object
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
+        :return: HTML tag of the link to the list of words related to the training set
+        :rtype: str
+        """
         document_list = reverse("admin:cms_document_changelist")
         return mark_safe(
             f"<a href={document_list}?training+set={obj.id}>{obj.words}</a>"
         )
 
     @admin.display(
         description=_("published words"),
         ordering="-words_released",
     )
     def words_released(self, obj):
+        """
+        returns HTML tag of the link to the list of released words related to the training set
+
+        :param obj: Training set object
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
+        :return: HTML tag of the link to the list of released words related to the training set
+        :rtype: str
+        """
         document_list = reverse("admin:cms_document_changelist")
         return mark_safe(
             f"<a href={document_list}?training+set={obj.id}&images=approved>{obj.words_released}</a>"
         )
 
     @admin.display(
         description=_("unpublished words"),
         ordering="-words_unreleased",
     )
     def words_unreleased(self, obj):
+        """
+        returns HTML tag of the Link to the list of unreleased words related to the training set
+
+        :param obj: Training set object
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
+        :return: HTML tag of the Link to the list of unreleased words related to the training set
+        :rtype: str
+        """
         document_list = reverse("admin:cms_document_changelist")
         return mark_safe(
             f"<a href={document_list}?training+set={obj.id}&images=no-approved>{obj.words_unreleased}</a>"
         )
 
     def related_disciplines(self, obj):
         """
         Display related disciplines in list display
 
         :param obj: Training set object
-        :type obj: models.TrainingSet
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
         :return: comma separated list of related disciplines
         :rtype: str
         """
         return ", ".join([child.title for child in obj.discipline.all()])
 
     related_disciplines.short_description = _("disciplines")
 
     def creator_group(self, obj):
         """
         Include creator group of discipline in list display
 
         :param obj: Training set object
-        :type obj: models.TrainingSet
+        :type obj: ~lunes_cms.cms.models.training_set.TrainingSet
         :return: Either static admin group or user group
         :rtype: str
         """
         if obj.creator_is_admin:
             return Static.admin_group
-        elif obj.created_by:
+        if obj.created_by:
             return obj.created_by
-        else:
-            return None
+        return None
 
     creator_group.short_description = _("creator group")
 
     class Media:
+        """
+        Media class of Training Set Admin
+        """
+
         js = ("js/image_preview.js",)
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/forms.py` & `lunes-cms-2024.5.0/lunes_cms/cms/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django import forms
 from django.conf import settings
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
-from mptt.models import TreeForeignKey
 
-from .models import Document, TrainingSet, Discipline
+from .models import Discipline, Document, TrainingSet
 from .widgets import ManyToManyOverlay
 
 
 class DisciplineChoiceField(forms.ModelMultipleChoiceField):
     """
     Custom form field in order to include parent nodes in string representation.
     Inherits from `forms.ModelMultipleChocieField`.
@@ -18,16 +17,15 @@
     def label_from_instance(self, obj):
         if obj.parent:
             ancestors = [
                 node.title for node in obj.parent.get_ancestors(include_self=True)
             ]
             ancestors.append(obj.title)
             return " \u2794 ".join(ancestors)
-        else:
-            return obj.title
+        return obj.title
 
 
 class TrainingSetForm(forms.ModelForm):
     """
     Defining custom form for the training set admin interface.
     Inherits from `forms.ModelForm`.
     """
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/list_filter.py` & `lunes-cms-2024.5.0/lunes_cms/cms/list_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from collections import defaultdict
-
 from django.contrib import admin
 from django.db.models import F
 from django.utils.translation import ugettext_lazy as _
+
 from .models import Discipline, TrainingSet
 
 
 class DisciplineListFilter(admin.SimpleListFilter):
     """
     Generic Filter for models that have a direct relationship to disciplines.
     Inherits from `admin.SimpleListFilter`.
@@ -201,19 +200,19 @@
         :return: filtered queryset based on the value provided in the query string
         :rtype: QuerySet
         """
 
         if self.value():
             if self.value() == NONE:
                 return queryset.filter(document_image__isnull=True).distinct()
-            elif self.value() == PENDING:
+            if self.value() == PENDING:
                 return queryset.filter(document_image__confirmed=False).distinct()
-            elif self.value() == APPROVED:
+            if self.value() == APPROVED:
                 return queryset.filter(document_image__confirmed=True).distinct()
-            elif self.value() == NO_APPROVED:
+            if self.value() == NO_APPROVED:
                 return queryset.exclude(document_image__confirmed=True).distinct()
         return queryset
 
 
 NONE = "none"
 AT_LEAST_ONE = "at-least-one"
 RELEASED = "released"
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0001_initial.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # Generated by Django 3.2.13 on 2022-04-15 17:27
 
-from django.db import migrations, models
 import django.db.models.deletion
+import mptt.fields
+from django.db import migrations, models
+
 import lunes_cms.cms.models.static
 import lunes_cms.cms.validators
-import mptt.fields
 
 
 class Migration(migrations.Migration):
+    """
+    Initial Migration file
+    """
+
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Discipline",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0002_modify_group_model.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0002_modify_group_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from django.db import migrations, models
+
 import lunes_cms.cms.models.static
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file for changing group model
+    """
+
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
         ("cms", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
@@ -25,23 +30,23 @@
         This is a workaround that allows to store ``auth``
         migration outside the directory it should be stored.
         Takes a ProjectState and returns a new one with the migration's operations applied to it.
         Preserves the original object state by default and will return a mutated state from a copy.
         """
         app_label = self.app_label
         self.app_label = "auth"
-        state = super(Migration, self).mutate_state(project_state, preserve)
+        state = super().mutate_state(project_state, preserve)
         self.app_label = app_label
         return state
 
     def apply(self, project_state, schema_editor, collect_sql=False):
         """
         Same workaround as described in ``mutate_state`` method.
         Takes a project_state representing all migrations prior to this one
         and a schema_editor for a live database and applies the migration in a forwards order.
         Returns the resulting project state for efficient re-use by following Migrations.
         """
         app_label = self.app_label
         self.app_label = "auth"
-        state = super(Migration, self).apply(project_state, schema_editor, collect_sql)
+        state = super().apply(project_state, schema_editor, collect_sql)
         self.app_label = app_label
         return state
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0004_feedback.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0004_feedback.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Generated by Django 3.2.13 on 2022-06-13 08:20
 
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file to enable feedback
+    """
+
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("cms", "0003_remove_documentimage_name"),
     ]
 
     operations = [
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0005_auto_create_id.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0005_auto_create_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Generated by Django 3.2.13 on 2022-07-25 14:26
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file to add auto field for ids
+    """
+
     dependencies = [
         ("cms", "0004_feedback"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="alternativeword",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0006_convert_group_api_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Generated by Django 3.2.13 on 2022-07-24 19:33
 
 import django.core.validators
 from django.db import migrations, models
+
 import lunes_cms.cms.models.group_api_key
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file to convert fields of group api key
+    """
+
     dependencies = [
         ("cms", "0005_auto_create_id"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="groupapikey",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0007_document_created_by_link.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0007_document_created_by_link.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by Django 3.2.13 on 2022-07-05 11:32
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
-# pylint: disable=unused-argument
+# pylint: disable=unused-argument, unused-variable
 def link_created_by(apps, schema_editor):
     """
     Convert the ``created_by`` char field to a foreign key
 
     :param apps: The configuration of installed applications
     :type apps: ~django.apps.registry.Apps
 
@@ -19,15 +19,15 @@
     Group = apps.get_model("auth", "Group")
     for document in Document.objects.filter(created_by__isnull=False):
         group, created = Group.objects.get_or_create(name=document.created_by)
         document.created_by_link = group
         document.save()
 
 
-# pylint: disable=unused-argument
+# pylint: disable=unused-argument,unused-variable
 def reverse_created_by(apps, schema_editor):
     """
     Convert the ``created_by`` field from foreign key to a char field
 
     :param apps: The configuration of installed applications
     :type apps: ~django.apps.registry.Apps
 
@@ -39,14 +39,18 @@
     for document in Document.objects.filter(created_by_link__isnull=False):
         group, created = Group.objects.get_or_create(id=document.created_by_link.id)
         document.created_by = group.name
         document.save()
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file to rename created_by_link
+    """
+
     dependencies = [
         ("cms", "0006_convert_group_api_key"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="document",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/migrations/0009_sponsor.py` & `lunes-cms-2024.5.0/lunes_cms/cms/migrations/0009_sponsor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Generated by Django 3.2.16 on 2023-02-20 10:29
 
 from django.db import migrations, models
+
 import lunes_cms.cms.models.static
 import lunes_cms.cms.validators
 
 
 class Migration(migrations.Migration):
+    """
+    Migration file to add sponsors
+    """
+
     dependencies = [
         ("cms", "0008_add_numerals_adverbs_and_pronouns_as_word_types"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="Sponsor",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/__init__.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from . import content_type, group
 from .alternative_word import AlternativeWord
 from .discipline import Discipline
 from .document import Document
 from .document_image import DocumentImage
-from .static import Static, convert_umlaute_images, convert_umlaute_audio
-from .training_set import TrainingSet
-from .group_api_key import GroupAPIKey
 from .feedback import Feedback
+from .group_api_key import GroupAPIKey
 from .sponsor import Sponsor
-from . import group, content_type
+from .static import Static, convert_umlaute_audio, convert_umlaute_images
+from .training_set import TrainingSet
 
 __all__ = [
     "AlternativeWord",
     "Discipline",
     "Document",
     "DocumentImage",
     "Static",
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/discipline.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/discipline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from django.db import models
-from django.db.models.deletion import CASCADE
 from django.contrib.auth.models import Group
 from django.contrib.contenttypes.fields import GenericRelation
+from django.db import models
+from django.db.models.deletion import CASCADE
 from django.utils.translation import ugettext_lazy as _
-
 from mptt.models import MPTTModel, TreeForeignKey
 
 from ..utils import get_child_count, get_image_tag
 from .feedback import Feedback
 from .static import convert_umlaute_images
 
 
@@ -87,15 +86,15 @@
     def __str__(self):
         """
         String representation of Discipline instance
 
         :return: title of discipline instance
         :rtype: str
         """
-        return self.title
+        return str(self.title)
 
     class Meta:
         """
         Define user readable name of Field
         """
 
         verbose_name = _("discipline")
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/document.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/document.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
-
 from pathlib import Path
-from django.core.files import File
+
 from django.contrib.contenttypes.fields import GenericRelation
+from django.core.files import File
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
-
 from pydub import AudioSegment
 
 from ..utils import document_to_string
 from ..validators import (
     validate_file_extension,
     validate_file_size,
     validate_multiple_extensions,
@@ -28,18 +27,36 @@
     word_type = models.CharField(
         max_length=255,
         choices=Static.word_type_choices,
         default="",
         verbose_name=_("word type"),
     )
     word = models.CharField(max_length=255, verbose_name=_("word"))
-    article = models.IntegerField(
-        choices=Static.article_choices,
+    grammatical_gender = models.IntegerField(
+        choices=Static.grammatical_genders,
+        verbose_name=_("Grammatical gender"),
+        blank=True,
+        null=True,
+    )
+    singular_article = models.IntegerField(
+        choices=Static.singular_article_choices,
+        default="",
+        verbose_name=_("singular article"),
+    )
+    plural = models.CharField(
+        max_length=255,
+        verbose_name=_("plural"),
+        blank=True,
         default="",
-        verbose_name=_("article"),
+    )
+    plural_article = models.IntegerField(
+        choices=Static.plural_article_choices,
+        verbose_name=_("plural article"),
+        blank=True,
+        null=True,
     )
     audio = models.FileField(
         upload_to=convert_umlaute_audio,
         validators=[
             validate_file_extension,
             validate_file_size,
             validate_multiple_extensions,
@@ -48,60 +65,76 @@
         null=True,
         verbose_name=_("audio"),
     )
     example_sentence = models.TextField(verbose_name=_("example sentence"), blank=True)
     creation_date = models.DateTimeField(
         auto_now_add=True, verbose_name=_("creation date")
     )
+    definition = models.TextField(
+        max_length=256,
+        blank=True,
+        null=True,
+        verbose_name=_("definition"),
+    )
+    additional_meaning_1 = models.CharField(
+        max_length=256,
+        blank=True,
+        null=True,
+        verbose_name=_("additional meaning 1"),
+    )
+    additional_meaning_2 = models.CharField(
+        max_length=256,
+        blank=True,
+        null=True,
+        verbose_name=_("additional meaning 2"),
+    )
     created_by = models.ForeignKey(
         max_length=255,
         null=True,
         blank=True,
         verbose_name=_("created by"),
         to=Group,
         on_delete=models.CASCADE,
     )
     creator_is_admin = models.BooleanField(default=True, verbose_name=_("admin"))
     feedback = GenericRelation(Feedback)
 
     @property
-    def converted(self, content_type="audio/mpeg"):
+    def converted(self):
         """
         Function that converts the uploaded audio to .mp3 and
         returns the converted file
 
         :param self: A handle to the :class:`models.Document`
         :type self: class: `models.Document`
-        :param content_type: content type of the converted file, defaults to "audio/mpeg"
-        :type request: content_type
 
         :return: File containing .mp3 audio
         :rtype: .mp3 File
         """
-        super(Document, self).save()
+        super().save()
         file_path = self.audio.path
         original_extension = file_path.split(".")[-1]
         mp3_converted_file = AudioSegment.from_file(file_path, original_extension)
         new_path = file_path[:-4] + "-conv.mp3"
         mp3_converted_file.export(new_path, format="mp3", bitrate="44.1k")
 
         converted_audiofile = File(file=open(new_path, "rb"), name=Path(new_path))
         converted_audiofile.name = Path(new_path).name
-        converted_audiofile.content_type = content_type
+        converted_audiofile.content_type = "audio/mpeg"
         converted_audiofile.size = os.path.getsize(new_path)
         os.remove(new_path)
         return converted_audiofile
 
     def save(self, *args, **kwargs):
         """Overwrite djangos save function to convert audio files
         to mp3 format (original file is saved as backup).
         """
         if self.audio:
             self.audio = self.converted
-        super(Document, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
 
     def __str__(self):
         """String representation of Document instance
 
         :return: title of document instance
         :rtype: str
         """
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/document_image.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/document_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
-
 from PIL import Image, ImageFilter
 
 from ..utils import get_image_tag
 from ..validators import validate_multiple_extensions
-from .static import Static, convert_umlaute_images
 from .document import Document
+from .static import Static, convert_umlaute_images
 
 
 class DocumentImage(models.Model):
     """
     Contains images and its titles that can be linked to a document object.
     """
 
@@ -108,15 +107,15 @@
         """
         return self.document.word
 
     def save(self, *args, **kwargs):
         """Overwrite djangos save function to scale images into a
         uniform size that is defined in the Static module.
         """
-        super(DocumentImage, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
         self.save_original_img()
         self.crop_img()
 
     class Meta:
         """
         Define user readable name of TrainingSet
         """
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/feedback.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/feedback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from html import escape
 
 from django.conf import settings
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.urls import reverse
-from django.utils.translation import gettext_lazy as _
 from django.utils.safestring import mark_safe
 from django.utils.text import Truncator
+from django.utils.translation import gettext_lazy as _
 
 
 class Feedback(models.Model):
     """
     Model to store feedback about disciplines, training sets and vocabulary words
     """
 
@@ -77,11 +77,15 @@
 
         :return: Truncated feedback comment
         :rtype: str
         """
         return Truncator(self.comment).chars(80)
 
     class Meta:
+        """
+        Meta class of feedback model
+        """
+
         #: The verbose name of the model
         verbose_name = _("feedback")
         #: The plural verbose name of the model
         verbose_name_plural = _("feedback entries")
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/group_api_key.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/group_api_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from html import escape
-from string import digits, ascii_uppercase
+from string import ascii_uppercase, digits
 
 from django.contrib.auth.models import Group
 from django.core.exceptions import PermissionDenied
 from django.core.validators import MinLengthValidator, RegexValidator
 from django.db import models
 from django.db.models import Q
 from django.utils.crypto import get_random_string
 from django.utils.html import mark_safe
-from django.utils.translation import ugettext_lazy as _
 from django.utils.timezone import now
-
+from django.utils.translation import ugettext_lazy as _
 from qr_code.qrcode.maker import make_qr_code_url_with_args
 
 
 def generate_default_token():
     """
     Generate a default random token of upper case letters and digits
 
@@ -128,25 +127,38 @@
             else "-"
         )
 
     qr_code.short_description = _("QR code")
 
     @classmethod
     def get_from_token(cls, token):
+        """
+        returns a group api which maches to the given token
+
+        :param token: token
+        :type token: str
+
+        :return: Group API Key object
+        :rtype: ~lunes_cms.cms.models.group_api_key.GroupAPIKey
+        """
         try:
             return cls.objects.get(
                 Q(token=token, revoked=False)
                 & (Q(expiry_date__isnull=True) | Q(expiry_date__gt=now()))
             )
-        except cls.DoesNotExist:
-            raise PermissionDenied()
+        except cls.DoesNotExist as e:
+            raise PermissionDenied() from e
 
     def __str__(self):
         """
         :return: The canonical string representation of an API key
         :rtype: str
         """
         return _('{}: Token for the group "{}"').format(self.token, self.group)
 
     class Meta:
+        """
+        Meta class for GroupAPIKey
+        """
+
         verbose_name = _("API Key")
         verbose_name_plural = _("API Keys")
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/sponsor.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/sponsor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import models
 from django.utils.translation import ugettext_lazy as _
 
-from .static import upload_sponsor_logos
 from ..validators import validate_multiple_extensions
+from .static import upload_sponsor_logos
 
 
 class Sponsor(models.Model):
     """
     Model to manage our sponsors that are shown in the app.
     """
 
@@ -29,15 +29,15 @@
     def __str__(self):
         """
         String representation of sponsor name
 
         :return: name of the sponsor
         :rtype: str
         """
-        return self.name
+        return str(self.name)
 
     class Meta:
         """
         Define user readable name of sponsors
         """
 
         verbose_name = _("sponsor")
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/static.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/static.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-from django.contrib.auth.models import User, Group
+from django.contrib.auth.models import Group, User
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
 from ..utils import create_resource_path
 
 
 class Static:
     """
     Module for static and global variables
     """
 
     # Possible articles
-    article_choices = [
+    singular_article_choices = [
         (0, "keiner"),
         (1, "der"),
         (2, "die"),
         (3, "das"),
         (4, "die (Plural)"),
     ]
+    plural_article_choices = [
+        (0, "keiner"),
+        (1, "die (Plural)"),
+    ]
 
     # Possible word types
     word_type_choices = [
         ("Nomen", "Substantiv"),
         ("Verb", "Verb"),
         ("Adjektiv", "Adjektiv"),
         ("Numeral", "Numeral"),
         ("Pronomen", "Pronomen"),
         ("Adverb", "Adverb"),
     ]
 
+    # Possible grammatical genders
+    grammatical_genders = [
+        (0, "kein"),
+        (1, "Maskulinum"),
+        (2, "Femininum"),
+        (3, "Neutrum"),
+        (4, "Plural"),
+    ]
+
     # number of pixels used for box blur
     blurr_radius = 30
     # maximum (width, height) of images
     img_size = (1024, 768)
 
     # super admin group name
     admin_group = "Lunes"
@@ -106,7 +119,8 @@
     :rtype: bool
     """
     if Static.default_group_name:
         default_group = Group.objects.filter(name=Static.default_group_name)
         if not created or not default_group:
             return False
         instance.groups.add(Group.objects.get(name=Static.default_group_name))
+    return True
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/models/training_set.py` & `lunes-cms-2024.5.0/lunes_cms/cms/models/training_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from django.db import models
-from mptt.models import MPTTModel, TreeForeignKey
 from django.contrib.auth.models import Group
 from django.contrib.contenttypes.fields import GenericRelation
 from django.core.exceptions import ValidationError
+from django.db import models
 from django.db.models.deletion import CASCADE
-from django.utils.translation import ugettext_lazy as _
 from django.utils.html import format_html
+from django.utils.translation import ugettext_lazy as _
+from mptt.models import MPTTModel, TreeForeignKey
 
 from ..utils import get_image_tag
+from .discipline import Discipline
+from .document import Document
 from .feedback import Feedback
 from .static import convert_umlaute_images
-from .document import Document
-from .discipline import Discipline
 
 
-class TrainingSet(MPTTModel):  # pylint: disable=R0903
+class TrainingSet(MPTTModel):
     """
     Training sets are part of disciplines, have a title, a description
     an icon and relates to documents and disciplines.
     Inherits from `mptt.models.MPTTModel`.
     """
 
     released = models.BooleanField(default=False, verbose_name=_("released"))
@@ -62,38 +62,43 @@
 
     def __str__(self):
         """String representation of TrainingSet instance
 
         :return: title of training set instance
         :rtype: str
         """
-        return self.title
+        return str(self.title)
 
     def save(self, *args, **kwargs):
         """Overwrite djangos save function to assure
         that no child elements are created.
 
         :raises ValidationError: Exception if child training set is created
         """
         if self.parent:
             msg = _(
                 "It is not possible to create child elements for training sets (unlike disciplines)."
             )
             raise ValidationError(msg)
-        super(TrainingSet, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
 
     # pylint: disable=R0903
     class Meta:
         """
         Define user readable name of TrainingSet
         """
 
         verbose_name = _("training set")
         verbose_name_plural = _("training sets")
 
     def style_description_field(self):
+        """
+        This function adds css classes to description field
+        :return: description field HTML code incl. CSS classes
+        :rtype: str
+        """
         return format_html(
             '<div style="overflow-wrap: break-word; max-width: 150px;" >{}</div>',
             self.description,
         )
 
     style_description_field.short_description = "description"
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/base.html` & `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_confirmation.html` & `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html` & `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/templates/admin/discipline_filter.html` & `lunes-cms-2024.5.0/lunes_cms/cms/templates/admin/discipline_filter.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/templatetags/admin_filter_tags.py` & `lunes-cms-2024.5.0/lunes_cms/cms/templatetags/admin_filter_tags.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This is a collection of admin filter tags and filters
 """
-from collections import defaultdict
 import logging
+from collections import defaultdict
 
 from django import template
 
 logger = logging.getLogger(__name__)
 register = template.Library()
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/urls.py` & `lunes-cms-2024.5.0/lunes_cms/cms/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,18 @@
 Map paths to view functions.
 Defines custom schema views and a router that
 handles the url patterns described in the `README.md` file
 """
 
 from django.contrib import admin
 from django.contrib.auth import views as auth_views
-from django.urls import path, include
-from django.conf.urls.static import static
-from django.conf import settings
-from django.conf.urls.i18n import i18n_patterns
-from django.conf.urls import url
-from django.templatetags.static import static as get_static_url
-from django.urls import path, reverse_lazy
+from django.urls import path
 from django.utils.translation import ugettext_lazy as _
-from django.views.generic.base import RedirectView
 from django.views.i18n import JavaScriptCatalog
 
-
 #: The url patterns of this module (see :doc:`django:topics/http/urls`)
 urlpatterns = [
     path(
         "admin/password_reset/",
         auth_views.PasswordResetView.as_view(),
         name="admin_password_reset",
     ),
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/utils.py` & `lunes-cms-2024.5.0/lunes_cms/cms/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 A collection of helper methods and classes
 """
 
 import os
-import uuid
-import string
 import pathlib
-
+import string
+import uuid
 from html import escape
 
 from django.utils.crypto import get_random_string
 from django.utils.html import mark_safe
 from django.utils.translation import ugettext as _
 
 
@@ -25,27 +24,29 @@
 
     :return: full file path
     :rtype: str
     """
     return os.path.join(parent_dir, str(uuid.uuid1()) + pathlib.Path(filename).suffix)
 
 
-def get_random_key(length: int = 10, excluded_chars: list = []) -> str:
+def get_random_key(length: int = 10, excluded_chars: list = None) -> str:
     """
     Auxiliary function that creates a random key based on latin letters and digits using
     the passed length. Optionally, it is possible to exclude characters like l and 1.
 
     :param length: key length, defaults to 10
     :type length: int, optional
-    :param excluded_chars: list of characters to be excluded (mixed dtypes possible), defaults to []
+    :param excluded_chars: list of characters to be excluded (mixed dtypes possible), defaults to None
     :type excluded_chars: list, optional
 
     :return: key
     :rtype: str
     """
+    if excluded_chars is None:
+        excluded_chars = []
     choices = string.ascii_letters + string.digits
     for char in excluded_chars:
         choices = choices.replace(str(char), "")
     key = get_random_string(length, choices)
     return key
 
 
@@ -56,30 +57,39 @@
     :param doc: Document object
     :type doc: models.Document
 
     :return: String representation of document image
     :rtype: str
     """
     alt_words = [str(elem) for elem in doc.alternatives.all()]
+    has_foto = "\U0001F4F7" if doc.document_image.all() else "\U000026A0"
 
     if len(alt_words) > 0:
         alt_words = "(" + ", ".join(alt_words) + ")"
-        return "(" + doc.get_article_display() + ") " + doc.word + " " + alt_words
-    else:
-        return "(" + doc.get_article_display() + ") " + doc.word
+        return (
+            has_foto
+            + " "
+            + "("
+            + doc.get_singular_article_display()
+            + ") "
+            + doc.word
+            + " "
+            + alt_words
+        )
+    return has_foto + " " + "(" + doc.get_singular_article_display() + ") " + doc.word
 
 
 def get_child_count(disc):
     """
     Returns the number of children of a discipline.
     Every child contains at least one training set or is a direct/indirect
     parent of a discipline that contains one.
 
     :param disc: Discipline instance
-    :type disc: models.Discipline
+    :type disc: ~lunes_cms.cms.models.discipline.Discipline
 
     :return: sum of children
     :rtype: int
     """
     children_counter = 0
     for child in disc.get_children():
         if child.released and get_training_set_count(child) > 0:
@@ -89,15 +99,15 @@
 
 def get_training_set_count(disc):
     """
     Returns the total number of training sets of a discipline and all its
     child elements.
 
     :param disc: Discipline instance
-    :type disc: models.Discipline
+    :type disc: ~lunes_cms.cms.models.discipline.Discipline
 
     :return: sum of training sets
     :rtype: int
     """
     training_set_counter = 0
     for child in disc.get_descendants(include_self=True):
         training_set_counter += child.training_sets.count()
@@ -126,14 +136,15 @@
         src = escape(f"/media/{image}")
     # Hide preview if image is empty or has invalid type
     html_cls = "" if src else 'class="hidden"'
     # HTML image tag for previews
     return mark_safe(f'<img src="{src}" width={width} height="auto" {html_cls} />')
 
 
+# pylint: disable=redefined-builtin
 def iter_to_string(iter):
     """
     Convert an iterable of objects to a readable string.
     It joins the first elements with commas and separates the last element by "and".
 
     :param iter: The input iterable
     :type iter: ~collections.abc.Iterable
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/cms/validators.py` & `lunes-cms-2024.5.0/lunes_cms/cms/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from django.utils.translation import ugettext_lazy as _
-from django.core.exceptions import ValidationError
 import os
 
+from django.core.exceptions import ValidationError
+from django.utils.translation import ugettext_lazy as _
+
 
 def validate_file_extension(value):
     """
     Function to validate the audio file format
 
     :param value: audio file returned by a `models.FileField`
     :type value: audio file
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/core/context_processors.py` & `lunes-cms-2024.5.0/lunes_cms/core/context_processors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Context processors pass additional variables to templates (see :ref:`context-processors`).
 """
 from ..cms.models import Feedback
 
 
-# pylint: disable=unused-variable
 def feedback_processor(request):
     """
     This context processor injects the number of unread feedback entries into the template context.
 
     :param request: The current http request
     :type request: ~django.http.HttpRequest
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/core/logging_formatter.py` & `lunes-cms-2024.5.0/lunes_cms/core/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/core/settings.py` & `lunes-cms-2024.5.0/lunes_cms/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 https://docs.djangoproject.com/en/2.2/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/2.2/ref/settings/
 """
 
 import os
+
 from distutils.util import strtobool
 
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.translation import ugettext_lazy as _
 
 from .logging_formatter import ColorFormatter
 
-
 ###################
 # CUSTOM SETTINGS #
 ###################
 
 #: Build paths inside the project like this: ``os.path.join(BASE_DIR, ...)``
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
@@ -413,16 +413,14 @@
     "DEFAULT_SCHEMA_CLASS": "drf_spectacular.openapi.AutoSchema",
     "DEFAULT_VERSIONING_CLASS": "rest_framework.versioning.NamespaceVersioning",
     "ALLOWED_VERSIONS": ("v1", "v2"),
     "DEFAULT_VERSION": "default",
     "DEFAULT_API_URL": "http://localhost:8080/api/",
 }
 
-from django.templatetags.static import static
-
 SPECTACULAR_SETTINGS = {
     "TITLE": "Lunes API",
     "DESCRIPTION": "The API documentation for the Lunes CMS",
     "VERSION": None,
     "SCHEMA_PATH_PREFIX": "/api(/v[0-9])?",
     "CONTACT": {"email": "tech@integreat-app.de"},
     "LICENSE": {
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/core/urls.py` & `lunes-cms-2024.5.0/lunes_cms/core/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,22 @@
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 
 """
-from django.contrib import admin
-from django.contrib.auth import views as auth_views
-from django.urls import path, include
-from django.conf.urls.static import static
 from django.conf import settings
-from django.conf.urls.i18n import i18n_patterns
 from django.conf.urls import url
+from django.conf.urls.i18n import i18n_patterns
+from django.conf.urls.static import static
 from django.templatetags.static import static as get_static_url
-from django.urls import path, reverse_lazy
+from django.urls import include, path, reverse_lazy
 from django.utils.translation import ugettext_lazy as _
 from django.views.generic.base import RedirectView
-from django.views.i18n import JavaScriptCatalog
-
 
 #: The url patterns of this module (see :doc:`django:topics/http/urls`)
 urlpatterns = [
     path("", RedirectView.as_view(url=reverse_lazy("admin:login"))),
     path(
         "favicon.ico",
         RedirectView.as_view(url=get_static_url("images/logo.svg")),
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/core/wsgi.py` & `lunes-cms-2024.5.0/lunes_cms/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/help/templates/public_upload.html` & `lunes-cms-2024.5.0/lunes_cms/help/templates/public_upload.html`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/help/views/public_upload.py` & `lunes-cms-2024.5.0/lunes_cms/help/views/public_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from django.shortcuts import render
 
-from ...cms.models import TrainingSet, Document, DocumentImage, Discipline
+from ...cms.models import Discipline, Document, DocumentImage, TrainingSet
 
 
 def public_upload(request):
     """Public form to upload missing images
 
     :param request: current user request
     :type request: django.http.request
@@ -23,15 +23,15 @@
                     document=document,
                     image=uploaded_image,
                     confirmed=False,
                 )
                 image.save()
                 upload_success = True
     missing_images = Document.objects.values_list(
-        "id", "word", "article", "training_sets"
+        "id", "word", "singular_article", "training_sets"
     ).filter(document_image__isnull=True)
     training_sets = (
         TrainingSet.objects.values_list("id", "title")
         .filter(documents__document_image__isnull=True)
         .distinct()
     )
     disciplines = (
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/django.mo` & `lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -105,14 +105,17 @@
 
 msgid "File type not supported! Use: .mp3 .aac .wav .m4a .wma .ogg"
 msgstr "Unerlaubtes Dateiformat! Erlaubt: .mp3 .aac .wav .m4a .wma .ogg"
 
 msgid "German"
 msgstr "Deutsch"
 
+msgid "Grammatical gender"
+msgstr "Genus"
+
 msgid "Home"
 msgstr "Home"
 
 msgid "If the API key is revoked, clients cannot use it anymore."
 msgstr ""
 "Wenn der API-Schlüssel widerrufen wird, können Clients ihn nicht mehr "
 "verwenden."
@@ -260,14 +263,20 @@
 msgid ""
 "You can only release a training set that contains at least {} vocabulary "
 "words with confirmed images."
 msgstr ""
 "Sie können nur Module veröffentlichen, die mindestens {} Vokabeln mit "
 "bestätigten Bildern enthalten."
 
+msgid "additional meaning 1"
+msgstr "Zusätzliche Bedeutung 1"
+
+msgid "additional meaning 2"
+msgstr "Zusätzliche Bedeutung 2"
+
 msgid "admin"
 msgstr "Admin"
 
 msgid "alternative word"
 msgstr "Alternatives Wort"
 
 msgid "alternative words"
@@ -275,17 +284,14 @@
 
 msgid "and"
 msgstr "und"
 
 msgid "api keys"
 msgstr "API Keys"
 
-msgid "article"
-msgstr "Artikel"
-
 msgid "audio"
 msgstr "Audio"
 
 msgid "comment"
 msgstr "Kommentar"
 
 msgid "content type"
@@ -296,14 +302,17 @@
 
 msgid "creation date"
 msgstr "Erstellt am"
 
 msgid "creator group"
 msgstr "Besitzergruppe"
 
+msgid "definition"
+msgstr "Definition"
+
 msgid "description"
 msgstr "Beschreibung"
 
 msgid "discipline"
 msgstr "Modulgruppe"
 
 msgid "disciplines"
@@ -320,14 +329,17 @@
 
 msgid "feedback"
 msgstr "Feedback"
 
 msgid "feedback entries"
 msgstr "Feedback-Einträge"
 
+msgid "grammatical gender"
+msgstr "Genus"
+
 msgid "group"
 msgstr "Gruppe"
 
 msgid "help"
 msgstr "Hilfe"
 
 msgid "icon"
@@ -350,14 +362,20 @@
 
 msgid "object id"
 msgstr "Objekt-ID"
 
 msgid "parent"
 msgstr "Übergeordnete Modulgruppe"
 
+msgid "plural"
+msgstr "Plural"
+
+msgid "plural article"
+msgstr "Plural-Artikel"
+
 msgid "published words"
 msgstr "veröffentlichte Vokabeln"
 
 msgid "published words in released modules"
 msgstr "veröffentlichte Vokabeln in veröffentlichten Modulen"
 
 msgid "refers to"
@@ -368,14 +386,17 @@
 
 msgid "released modules"
 msgstr "veröffentlichte Module"
 
 msgid "revoked"
 msgstr "widerrufen"
 
+msgid "singular article"
+msgstr "Singular-Artikel"
+
 msgid "sponsor"
 msgstr "Sponsor"
 
 msgid "sponsors"
 msgstr "Sponsoren"
 
 msgid "submitted on"
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo` & `lunes-cms-2024.5.0/lunes_cms/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/lunes-cms-cli` & `lunes-cms-2024.5.0/lunes_cms/lunes-cms-cli`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/bootstrap/css/bootstrap.min.css` & `lunes-cms-2024.5.0/lunes_cms/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/css/corporate_identity.css` & `lunes-cms-2024.5.0/lunes_cms/static/css/corporate_identity.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/css/feedback.css` & `lunes-cms-2024.5.0/lunes_cms/static/css/feedback.css`

 * *Files 22% similar despite different names*

```diff
@@ -4,42 +4,56 @@
 /* Additional CSS for styling the feedback table */
   width: 100%;
   table-layout: fixed;
   overflow-wrap: break-word;
   min-width: 1000px;
 }
 
+
+.table-striped tbody tr:nth-of-type(odd){
+  background-color: #ffffff;
+}
+
+thead th .text{
+  color: #001f3f;
+}
+
+thead tr {
+  background-color: #e2e1e1;
+  font-weight: bold;
+}
+
 /* Checkbox column */
 thead th:nth-child(1) {
-  width: 40px;
+  width: 3%;
 }
 
 /* Comment column */
 thead th:nth-child(2) {
-  width: auto;
+  width: 25%;
 }
 
 /* Related object column */
 thead th:nth-child(3) {
-  width: 250px;
+  width: 19%;
 }
 
 /* Related object type column */
 thead th:nth-child(4) {
-  width: 140px;
+  width: 15%;
 }
 
 /* Submission date column */
 thead th:nth-child(5) {
-  width: 185px;
+  width: 19%;
 }
 
 /* Read by column */
 thead th:nth-child(6) {
-  width: 230px;
+  width: 19%;
 }
 
 /* Truncate long comments and content object links */
 .field-comment a,
 .field-content_object_link a {
   display: block;
   white-space: nowrap;
```

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/css/overlay.css` & `lunes-cms-2024.5.0/lunes_cms/static/css/overlay.css`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/guidelines/fotoguide.pdf` & `lunes-cms-2024.5.0/lunes_cms/static/guidelines/fotoguide.pdf`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes-dark.svg` & `lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes-dark.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/images/logo-lunes.svg` & `lunes-cms-2024.5.0/lunes_cms/static/images/logo-lunes.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/images/logo.svg` & `lunes-cms-2024.5.0/lunes_cms/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/js/image_preview.js` & `lunes-cms-2024.5.0/lunes_cms/static/js/image_preview.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/js/manytomany_overlay.js` & `lunes-cms-2024.5.0/lunes_cms/static/js/manytomany_overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms/static/js/overlay.js` & `lunes-cms-2024.5.0/lunes_cms/static/js/overlay.js`

 * *Files identical despite different names*

### Comparing `lunes-cms-2023.7.0/lunes_cms.egg-info/SOURCES.txt` & `lunes-cms-2024.5.0/lunes_cms.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-LICENSE.txt
+LICENSE
 MANIFEST.in
+NOTICE.md
 README.md
 setup.cfg
 setup.py
 lunes_cms/__init__.py
 lunes_cms/lunes-cms-cli
 lunes_cms.egg-info/PKG-INFO
 lunes_cms.egg-info/SOURCES.txt
@@ -65,14 +66,18 @@
 lunes_cms/cms/migrations/0005_auto_create_id.py
 lunes_cms/cms/migrations/0006_convert_group_api_key.py
 lunes_cms/cms/migrations/0007_document_created_by_link.py
 lunes_cms/cms/migrations/0008_add_numerals_adverbs_and_pronouns_as_word_types.py
 lunes_cms/cms/migrations/0009_sponsor.py
 lunes_cms/cms/migrations/0010_sponsor_url.py
 lunes_cms/cms/migrations/0011_document_example_sentence.py
+lunes_cms/cms/migrations/0012_add_additional_field.py
+lunes_cms/cms/migrations/0013_add_plural_field.py
+lunes_cms/cms/migrations/0014_add_plural_field_and_plural_article.py
+lunes_cms/cms/migrations/0015_add_grammatical_gender_fields.py
 lunes_cms/cms/migrations/__init__.py
 lunes_cms/cms/models/__init__.py
 lunes_cms/cms/models/alternative_word.py
 lunes_cms/cms/models/content_type.py
 lunes_cms/cms/models/discipline.py
 lunes_cms/cms/models/document.py
 lunes_cms/cms/models/document_image.py
@@ -101,18 +106,21 @@
 lunes_cms/help/templates/public_upload.html
 lunes_cms/help/views/__init__.py
 lunes_cms/help/views/public_upload.py
 lunes_cms/locale/de/LC_MESSAGES/django.mo
 lunes_cms/locale/de/LC_MESSAGES/djangojs.mo
 lunes_cms/static/bootstrap/css/bootstrap.min.css
 lunes_cms/static/css/corporate_identity.css
+lunes_cms/static/css/document_form.css
 lunes_cms/static/css/feedback.css
 lunes_cms/static/css/overlay.css
 lunes_cms/static/guidelines/fotoguide.pdf
 lunes_cms/static/images/fallback-icon.svg
 lunes_cms/static/images/logo-lunes-dark.svg
 lunes_cms/static/images/logo-lunes.svg
 lunes_cms/static/images/logo.svg
+lunes_cms/static/js/color_unread_feedback.js
 lunes_cms/static/js/corporate_identity.js
 lunes_cms/static/js/image_preview.js
 lunes_cms/static/js/manytomany_overlay.js
-lunes_cms/static/js/overlay.js
+lunes_cms/static/js/overlay.js
+lunes_cms/static/js/toggle_plural_field.js
```

### Comparing `lunes-cms-2023.7.0/lunes_cms.egg-info/requires.txt` & `lunes-cms-2024.5.0/lunes_cms.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-django==3.2.20
+django==3.2.21
 django-jazzmin==2.6.0
-django-mptt==0.14.0
+django-mptt==0.15.0
 django-qr-code==3.1.1
 djangorestframework==3.14.0
-drf-spectacular==0.26.3
-ipython==8.14.0
-pillow==10.0.0
-psycopg2==2.9.6
+drf-spectacular==0.26.5
+ipython==8.16.0
+pillow==10.0.1
+psycopg2==2.9.8
 pydub==0.25.1
 
 [dev]
-black==23.7.0
-bumpver==2023.1125
-pre-commit==3.3.3
+black==23.9.1
+bumpver==2023.1126
+pre-commit==3.4.0
 pyjwt==2.8.0
 pylint-django==2.5.3
 pylint-runner==0.6.0
-shellcheck-py==0.9.0.5
+shellcheck-py==0.9.0.6
 twine==4.0.2
 
 [doc]
-sphinx==6.2.1
-sphinx-rtd-theme==1.2.2
-sphinx-last-updated-by-git==0.3.5
-sphinxcontrib-django==2.4
+sphinx==7.2.6
+sphinx-rtd-theme==1.3.0
+sphinx-last-updated-by-git==0.3.6
+sphinxcontrib-django==2.5
 
 [test]
 pytest-circleci-parallelized==0.1.0
 pytest-cov==4.1.0
 pytest-django==4.5.2
-pytest-icdiff==0.6
+pytest-icdiff==0.8
 pytest-xdist==3.3.1
```

### Comparing `lunes-cms-2023.7.0/setup.cfg` & `lunes-cms-2024.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [metadata]
 name = lunes-cms
-version = 2023.7.0
+version = 2024.5.0
 author = Tür an Tür – Digitalfabrik gGmbH
 author_email = tech@integreat-app.de
 description = Content Management System for the Lunes Vocabulary Trainer App
 url = https://lunes.app/
 project_urls = 
 	Documentation=https://lunes-cms.rtfd.io
 	Issues=https://github.com/digitalfabrik/lunes-cms/issues
 	Source Code=https://github.com/digitalfabrik/lunes-cms
 	Release Notes=https://digitalfabrik.github.io/integreat-cms/changelog.html
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
-license_file = LICENSE.txt
+license_files = 
+	LICENSE
+	NOTICE.md
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
@@ -39,52 +41,52 @@
 	vocabulary-trainer
 	visual-vocabulary-trainer
 
 [options]
 packages = 
 	lunes_cms
 install_requires = 
-	django==3.2.20
+	django==3.2.21
 	django-jazzmin==2.6.0
-	django-mptt==0.14.0
+	django-mptt==0.15.0
 	django-qr-code==3.1.1
 	djangorestframework==3.14.0
-	drf-spectacular==0.26.3
-	ipython==8.14.0
-	pillow==10.0.0
-	psycopg2==2.9.6
+	drf-spectacular==0.26.5
+	ipython==8.16.0
+	pillow==10.0.1
+	psycopg2==2.9.8
 	pydub==0.25.1
 python_requires = >=3.8
 include_package_data = True
 scripts = lunes_cms/lunes-cms-cli
 
 [options.extras_require]
 dev = 
-	black==23.7.0
-	bumpver==2023.1125
-	pre-commit==3.3.3
+	black==23.9.1
+	bumpver==2023.1126
+	pre-commit==3.4.0
 	pyjwt==2.8.0
 	pylint-django==2.5.3
 	pylint-runner==0.6.0
-	shellcheck-py==0.9.0.5
+	shellcheck-py==0.9.0.6
 	twine==4.0.2
 doc = 
-	sphinx==6.2.1
-	sphinx-rtd-theme==1.2.2
-	sphinx-last-updated-by-git==0.3.5
-	sphinxcontrib-django==2.4
+	sphinx==7.2.6
+	sphinx-rtd-theme==1.3.0
+	sphinx-last-updated-by-git==0.3.6
+	sphinxcontrib-django==2.5
 test = 
 	pytest-circleci-parallelized==0.1.0
 	pytest-cov==4.1.0
 	pytest-django==4.5.2
-	pytest-icdiff==0.6
+	pytest-icdiff==0.8
 	pytest-xdist==3.3.1
 
 [bumpver]
-current_version = 2023.7.0
+current_version = 2024.5.0
 version_pattern = YYYY.MM.INC0[-TAG]
 commit_message = 
 	Bump version to {new_version}
 	[skip ci]
 commit = True
 tag = False
 push = False
```

