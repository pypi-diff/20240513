# Comparing `tmp/android-cli-1.0.9.tar.gz` & `tmp/android_cli-1.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-cli-1.0.9.tar", last modified: Thu Apr 25 12:25:16 2024, max compression
+gzip compressed data, was "android_cli-1.10.0.tar", last modified: Mon May 13 21:04:41 2024, max compression
```

## Comparing `android-cli-1.0.9.tar` & `android_cli-1.10.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.745930 android-cli-1.0.9/
--rw-r--r--   0 juan       (501) staff       (20)      236 2024-04-25 12:25:16.745703 android-cli-1.0.9/PKG-INFO
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.731128 android-cli-1.0.9/android_cli.egg-info/
--rw-r--r--   0 juan       (501) staff       (20)      236 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/PKG-INFO
--rw-r--r--   0 juan       (501) staff       (20)     1963 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/SOURCES.txt
--rw-r--r--   0 juan       (501) staff       (20)        1 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/dependency_links.txt
--rw-r--r--   0 juan       (501) staff       (20)       51 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/entry_points.txt
--rw-r--r--   0 juan       (501) staff       (20)       91 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/requires.txt
--rw-r--r--   0 juan       (501) staff       (20)        4 2024-04-25 12:25:16.000000 android-cli-1.0.9/android_cli.egg-info/top_level.txt
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.731381 android-cli-1.0.9/cli/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:14:42.000000 android-cli-1.0.9/cli/__init__.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.734681 android-cli-1.0.9/cli/entities/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 02:21:04.000000 android-cli-1.0.9/cli/entities/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     6252 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/entities/app.py
--rw-r--r--   0 juan       (501) staff       (20)     2954 2024-03-08 20:33:40.000000 android-cli-1.0.9/cli/entities/aws.py
--rw-r--r--   0 juan       (501) staff       (20)     5858 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/bitrise.py
--rw-r--r--   0 juan       (501) staff       (20)     2090 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/fcm.py
--rw-r--r--   0 juan       (501) staff       (20)     2600 2024-01-24 19:37:08.000000 android-cli-1.0.9/cli/entities/git.py
--rw-r--r--   0 juan       (501) staff       (20)    13647 2024-03-04 20:18:55.000000 android-cli-1.0.9/cli/entities/jira.py
--rw-r--r--   0 juan       (501) staff       (20)     8314 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/entities/lokalise.py
--rw-r--r--   0 juan       (501) staff       (20)     9699 2024-03-18 12:31:54.000000 android-cli-1.0.9/cli/entities/menu.py
--rw-r--r--   0 juan       (501) staff       (20)     6495 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/entities/setting.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.735052 android-cli-1.0.9/cli/form/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 22:20:43.000000 android-cli-1.0.9/cli/form/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      682 2024-01-24 18:46:20.000000 android-cli-1.0.9/cli/form/_form_confirm.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.736474 android-cli-1.0.9/cli/form/bitrise/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:13:23.000000 android-cli-1.0.9/cli/form/bitrise/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     2258 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/branch_form.py
--rw-r--r--   0 juan       (501) staff       (20)      676 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/build_type_form.py
--rw-r--r--   0 juan       (501) staff       (20)     1489 2024-02-09 17:02:00.000000 android-cli-1.0.9/cli/form/bitrise/release_notes_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2542 2024-01-29 12:48:34.000000 android-cli-1.0.9/cli/form/bitrise/version_code_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2368 2024-01-24 14:18:20.000000 android-cli-1.0.9/cli/form/bitrise/version_name_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.737023 android-cli-1.0.9/cli/form/code_gen/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/form/code_gen/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      657 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/form/code_gen/code_gen_form.py
--rw-r--r--   0 juan       (501) staff       (20)     3698 2024-04-25 12:24:19.000000 android-cli-1.0.9/cli/form/code_gen/create_new_screen.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.738021 android-cli-1.0.9/cli/form/fcm/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     1194 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_firebase_id_form.py
--rw-r--r--   0 juan       (501) staff       (20)      456 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_body_form.py
--rw-r--r--   0 juan       (501) staff       (20)      514 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_deeplink_form.py
--rw-r--r--   0 juan       (501) staff       (20)      460 2024-03-05 20:01:57.000000 android-cli-1.0.9/cli/form/fcm/fcm_notification_title_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.740012 android-cli-1.0.9/cli/form/git/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-24 12:50:52.000000 android-cli-1.0.9/cli/form/git/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     3035 2024-01-24 18:46:20.000000 android-cli-1.0.9/cli/form/git/_new_branch_form.py
--rw-r--r--   0 juan       (501) staff       (20)     4193 2024-01-24 20:09:48.000000 android-cli-1.0.9/cli/form/git/_pull_request_form.py
--rw-r--r--   0 juan       (501) staff       (20)     2242 2024-01-24 19:15:46.000000 android-cli-1.0.9/cli/form/git/create_new_branch.py
--rw-r--r--   0 juan       (501) staff       (20)     4012 2024-02-01 20:35:53.000000 android-cli-1.0.9/cli/form/git/create_new_pull_request.py
--rw-r--r--   0 juan       (501) staff       (20)      673 2024-01-24 19:45:29.000000 android-cli-1.0.9/cli/form/git/git_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.741778 android-cli-1.0.9/cli/form/jira/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-23 15:51:10.000000 android-cli-1.0.9/cli/form/jira/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      458 2024-02-01 18:44:37.000000 android-cli-1.0.9/cli/form/jira/jira_description_form.py
--rw-r--r--   0 juan       (501) staff       (20)      611 2024-03-05 20:02:08.000000 android-cli-1.0.9/cli/form/jira/jira_issue_form.py
--rw-r--r--   0 juan       (501) staff       (20)      791 2024-02-14 12:28:45.000000 android-cli-1.0.9/cli/form/jira/jira_release_start_date_form.py
--rw-r--r--   0 juan       (501) staff       (20)      749 2024-02-14 12:27:50.000000 android-cli-1.0.9/cli/form/jira/jira_release_version_form.py
--rw-r--r--   0 juan       (501) staff       (20)      640 2024-02-01 20:23:20.000000 android-cli-1.0.9/cli/form/jira/jira_title_form.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.742857 android-cli-1.0.9/cli/form/lokalise/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-20 15:15:41.000000 android-cli-1.0.9/cli/form/lokalise/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)      638 2024-03-18 12:31:54.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_add_strings_form.py
--rw-r--r--   0 juan       (501) staff       (20)      625 2024-01-24 14:20:55.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_get_strings_form.py
--rw-r--r--   0 juan       (501) staff       (20)      859 2024-01-24 14:20:55.000000 android-cli-1.0.9/cli/form/lokalise/lokalise_menu_form.py
--rw-r--r--   0 juan       (501) staff       (20)      349 2024-03-05 14:11:11.000000 android-cli-1.0.9/cli/main.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.744311 android-cli-1.0.9/cli/utils/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-01-14 01:48:56.000000 android-cli-1.0.9/cli/utils/__init__.py
-drwxr-xr-x   0 juan       (501) staff       (20)        0 2024-04-25 12:25:16.745372 android-cli-1.0.9/cli/utils/code_templates/
--rw-r--r--   0 juan       (501) staff       (20)        0 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/utils/code_templates/__init__.py
--rw-r--r--   0 juan       (501) staff       (20)     4141 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/fragment_template.py
--rw-r--r--   0 juan       (501) staff       (20)      768 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/mock_preview_template.py
--rw-r--r--   0 juan       (501) staff       (20)      879 2024-03-04 16:53:48.000000 android-cli-1.0.9/cli/utils/code_templates/update_di.py
--rw-r--r--   0 juan       (501) staff       (20)     3204 2024-03-15 19:00:19.000000 android-cli-1.0.9/cli/utils/code_templates/viewmodel_template.py
--rw-r--r--   0 juan       (501) staff       (20)      950 2024-01-24 14:46:30.000000 android-cli-1.0.9/cli/utils/configs.py
--rw-r--r--   0 juan       (501) staff       (20)      598 2024-01-24 19:37:08.000000 android-cli-1.0.9/cli/utils/editor.py
--rw-r--r--   0 juan       (501) staff       (20)     1637 2024-01-20 02:02:53.000000 android-cli-1.0.9/cli/utils/shell.py
--rw-r--r--   0 juan       (501) staff       (20)      217 2024-01-14 01:53:54.000000 android-cli-1.0.9/cli/utils/singleton.py
--rw-r--r--   0 juan       (501) staff       (20)     4891 2024-02-20 19:19:46.000000 android-cli-1.0.9/cli/utils/ui.py
--rw-r--r--   0 juan       (501) staff       (20)     1652 2024-02-19 18:53:53.000000 android-cli-1.0.9/cli/utils/ui_menu.py
--rw-r--r--   0 juan       (501) staff       (20)       38 2024-04-25 12:25:16.745976 android-cli-1.0.9/setup.cfg
--rw-r--r--   0 juan       (501) staff       (20)      445 2024-04-25 12:24:19.000000 android-cli-1.0.9/setup.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.082062 android_cli-1.10.0/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      237 2024-05-13 21:04:41.081618 android_cli-1.10.0/PKG-INFO
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.081210 android_cli-1.10.0/android_cli.egg-info/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      237 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     1963 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        1 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)       51 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)       91 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/requires.txt
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        4 2024-05-13 21:04:41.000000 android_cli-1.10.0/android_cli.egg-info/top_level.txt
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.058368 android_cli-1.10.0/cli/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/__init__.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.062254 android_cli-1.10.0/cli/entities/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/entities/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     6253 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/app.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2954 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/entities/aws.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     5858 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/bitrise.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2090 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/fcm.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2600 2024-02-24 20:04:21.000000 android_cli-1.10.0/cli/entities/git.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)    13647 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/jira.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     8314 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/lokalise.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     9699 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/menu.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     6495 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/entities/setting.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.062834 android_cli-1.10.0/cli/form/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      682 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/_form_confirm.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.072356 android_cli-1.10.0/cli/form/bitrise/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/bitrise/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2258 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/bitrise/branch_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      676 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/bitrise/build_type_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     1489 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/bitrise/release_notes_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2542 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/bitrise/version_code_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2368 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/bitrise/version_name_form.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.073187 android_cli-1.10.0/cli/form/code_gen/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-03-19 15:30:03.000000 android_cli-1.10.0/cli/form/code_gen/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      657 2024-03-19 15:30:03.000000 android_cli-1.10.0/cli/form/code_gen/code_gen_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     3698 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/code_gen/create_new_screen.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.074113 android_cli-1.10.0/cli/form/fcm/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/fcm/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     1194 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/fcm/fcm_firebase_id_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      456 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/fcm/fcm_notification_body_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      514 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/fcm/fcm_notification_deeplink_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      460 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/fcm/fcm_notification_title_form.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.075658 android_cli-1.10.0/cli/form/git/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     3035 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/_new_branch_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     4193 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/_pull_request_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     2242 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/create_new_branch.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     4012 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/create_new_pull_request.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      673 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/git/git_form.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.076902 android_cli-1.10.0/cli/form/jira/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/jira/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      458 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/jira/jira_description_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      611 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/jira/jira_issue_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      791 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/jira/jira_release_start_date_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      749 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/form/jira/jira_release_version_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      640 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/jira/jira_title_form.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.077988 android_cli-1.10.0/cli/form/lokalise/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/lokalise/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      638 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/lokalise/lokalise_add_strings_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      625 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/lokalise/lokalise_get_strings_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      859 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/form/lokalise/lokalise_menu_form.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      349 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/main.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.079602 android_cli-1.10.0/cli/utils/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/utils/__init__.py
+drwxr-xr-x   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-05-13 21:04:41.080881 android_cli-1.10.0/cli/utils/code_templates/
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)        0 2024-03-19 15:30:03.000000 android_cli-1.10.0/cli/utils/code_templates/__init__.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     4135 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/utils/code_templates/fragment_template.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      768 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/utils/code_templates/mock_preview_template.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      879 2024-03-19 15:30:03.000000 android_cli-1.10.0/cli/utils/code_templates/update_di.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     3204 2024-05-13 21:04:30.000000 android_cli-1.10.0/cli/utils/code_templates/viewmodel_template.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      950 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/utils/configs.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      598 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/utils/editor.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     1637 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/utils/shell.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      217 2024-02-19 19:39:08.000000 android_cli-1.10.0/cli/utils/singleton.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     4891 2024-03-03 03:15:02.000000 android_cli-1.10.0/cli/utils/ui.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)     1652 2024-03-19 15:25:58.000000 android_cli-1.10.0/cli/utils/ui_menu.py
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)       38 2024-05-13 21:04:41.082157 android_cli-1.10.0/setup.cfg
+-rw-r--r--   0 ignaciodeandreisdenis   (501) staff       (20)      446 2024-05-13 21:04:30.000000 android_cli-1.10.0/setup.py
```

### Comparing `android-cli-1.0.9/android_cli.egg-info/SOURCES.txt` & `android_cli-1.10.0/android_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/app.py` & `android_cli-1.10.0/cli/entities/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cli.entities.setting import Settings
 from cli.utils.singleton import singleton
 import questionary
 
 
 @singleton
 class App:
-    version: str = "1.0.9"
+    version: str = "1.10.0"
 
     def init(self):
         os.system('printf "\033c"')
         os.system('cls' if os.name == 'nt' else 'clear')
 
         print(f"Press [enter] to start GIT-CLI {self.version}")
```

### Comparing `android-cli-1.0.9/cli/entities/aws.py` & `android_cli-1.10.0/cli/entities/aws.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/bitrise.py` & `android_cli-1.10.0/cli/entities/bitrise.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/fcm.py` & `android_cli-1.10.0/cli/entities/fcm.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/git.py` & `android_cli-1.10.0/cli/entities/git.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/jira.py` & `android_cli-1.10.0/cli/entities/jira.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 JIRA_TRANSITIONS = {
     'BACKLOG': '11',
     'BLOCKED': '111',
     'DISCARDED': '121',
     'PLANNING': '241',
     'DEVELOPMENT': '171',
     'TESTING': '271',
-    'IMPLEMENTATION': '281',
+    'READY_FOR_PROD': '321',
     'PRE_PROD': '291',
-    'LIVE': '261'
+    'DONE': '341'
 }
 
 
 def show_loading_spinner(is_loading, message="Loading, please wait ..."):
     spinner = ['⠋', '⠙', '⠹', '⠸', '⠼', '⠴', '⠦', '⠧', '⠇', '⠏']
     while is_loading.is_set():
         for char in spinner:
@@ -387,15 +387,15 @@
             active_release = self.get_release_active_android_release()
             ticket_key = self.search_key_in_description(active_release.get('description'))
             ticket = self.get_ticket_by_key(ticket_key)[0].get('fields')
             due_date = ticket.get('duedate')
             issues = self.get_issues_by_due_date(due_date, project_keys=['PR', 'NPR', 'BUG'])
             for issue in issues:
                 ticket_key = issue.get('key')
-                transition = self.make_transition(self, issue_key=ticket_key, transition_id=JIRA_TRANSITIONS['LIVE'])
+                transition = self.make_transition(self, issue_key=ticket_key, transition_id=JIRA_TRANSITIONS['DONE'])
                 print(transition)
         finally:
             is_loading.clear()
             spinner_thread.join()
             return "Tickets updated"
 
     @staticmethod
```

### Comparing `android-cli-1.0.9/cli/entities/lokalise.py` & `android_cli-1.10.0/cli/entities/lokalise.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/menu.py` & `android_cli-1.10.0/cli/entities/menu.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/entities/setting.py` & `android_cli-1.10.0/cli/entities/setting.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/_form_confirm.py` & `android_cli-1.10.0/cli/form/_form_confirm.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/bitrise/branch_form.py` & `android_cli-1.10.0/cli/form/bitrise/branch_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/bitrise/build_type_form.py` & `android_cli-1.10.0/cli/form/bitrise/build_type_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/bitrise/release_notes_form.py` & `android_cli-1.10.0/cli/form/bitrise/release_notes_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/bitrise/version_code_form.py` & `android_cli-1.10.0/cli/form/bitrise/version_code_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/bitrise/version_name_form.py` & `android_cli-1.10.0/cli/form/bitrise/version_name_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/code_gen/code_gen_form.py` & `android_cli-1.10.0/cli/form/code_gen/code_gen_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/code_gen/create_new_screen.py` & `android_cli-1.10.0/cli/form/code_gen/create_new_screen.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/fcm/fcm_firebase_id_form.py` & `android_cli-1.10.0/cli/form/fcm/fcm_firebase_id_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/fcm/fcm_notification_deeplink_form.py` & `android_cli-1.10.0/cli/form/fcm/fcm_notification_deeplink_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/git/_new_branch_form.py` & `android_cli-1.10.0/cli/form/git/_new_branch_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/git/_pull_request_form.py` & `android_cli-1.10.0/cli/form/git/_pull_request_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/git/create_new_branch.py` & `android_cli-1.10.0/cli/form/git/create_new_branch.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/git/create_new_pull_request.py` & `android_cli-1.10.0/cli/form/git/create_new_pull_request.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/git/git_form.py` & `android_cli-1.10.0/cli/form/git/git_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/jira/jira_issue_form.py` & `android_cli-1.10.0/cli/form/jira/jira_issue_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/jira/jira_release_start_date_form.py` & `android_cli-1.10.0/cli/form/jira/jira_release_start_date_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/jira/jira_release_version_form.py` & `android_cli-1.10.0/cli/form/jira/jira_release_version_form.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 import questionary
 
 
 def ask_for_release_version():
     try:
-        message = f'Add release version (ex. 4.29): '
+        message = f'Add release version (ex. 4.41): '
         title = questionary.unsafe_prompt(
             {
                 'type': 'text',
                 'name': 'value',
                 'message': message,
                 'default': '',
                 'validate': lambda val: 'Invalid format. Format should be like 4.22, 4.22.1' if not
```

### Comparing `android-cli-1.0.9/cli/form/jira/jira_title_form.py` & `android_cli-1.10.0/cli/form/jira/jira_title_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/lokalise/lokalise_add_strings_form.py` & `android_cli-1.10.0/cli/form/lokalise/lokalise_add_strings_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/lokalise/lokalise_get_strings_form.py` & `android_cli-1.10.0/cli/form/lokalise/lokalise_get_strings_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/form/lokalise/lokalise_menu_form.py` & `android_cli-1.10.0/cli/form/lokalise/lokalise_menu_form.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/code_templates/fragment_template.py` & `android_cli-1.10.0/cli/utils/code_templates/fragment_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import androidx.compose.ui.Modifier
 import androidx.compose.ui.tooling.preview.PreviewParameter
 import androidx.navigation.fragment.navArgs
 import com.astropaycard.android.core.base.BaseFragment
 import com.astropaycard.android.core.base.extensions.navigateBack
 import com.astropaycard.android.core.design_system.previews.DefaultPreview
 import com.astropaycard.android.core.design_system.texts.BodyTextDefault
-import com.astropaycard.android.core.design_system.theme.AstroPayTheme
+import com.astropaycard.android.core.design_system.theme.ElviraTheme
 import com.astropaycard.android.core.ui.databinding.FragmentComposeBinding
 import com.astropaycard.android.core.ui.toolbar.DefaultToolBar
 import com.astropaycard.android.core.ui.view_state.ContentState
 import {package}.mock_preview.{name}PreviewProvider
 import org.koin.androidx.viewmodel.ext.android.viewModel
 
 class {name}Fragment :
@@ -43,15 +43,15 @@
     }}
 
     override fun onViewCreated(view: View, savedInstanceState: Bundle?) {{
         super.onViewCreated(view, savedInstanceState)
 
         binding.apply {{
             composeView.setContent {{
-                AstroPayTheme {{
+                ElviraTheme {{
                     val screenState by viewModel.stateLiveData.observeAsState(
                         initial = {name}ViewModel.ViewState()
                     )
                     Screen(
                         screenState = screenState,
                         eventReducer = ::onUIEvent,
                     )
@@ -118,15 +118,15 @@
     }}
 
     @Composable
     @DefaultPreview
     private fun ScreenPreview(
         @PreviewParameter({name}PreviewProvider::class) state: {name}ViewModel.ViewState
     ) {{
-        AstroPayTheme {{
+        ElviraTheme {{
             Screen(state)
         }}
     }}
 }}
 '''
     with open(file_name, "w") as file:
         file.write(file_content)
```

### Comparing `android-cli-1.0.9/cli/utils/code_templates/mock_preview_template.py` & `android_cli-1.10.0/cli/utils/code_templates/mock_preview_template.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/code_templates/update_di.py` & `android_cli-1.10.0/cli/utils/code_templates/update_di.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/code_templates/viewmodel_template.py` & `android_cli-1.10.0/cli/utils/code_templates/viewmodel_template.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/configs.py` & `android_cli-1.10.0/cli/utils/configs.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/editor.py` & `android_cli-1.10.0/cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/shell.py` & `android_cli-1.10.0/cli/utils/shell.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/ui.py` & `android_cli-1.10.0/cli/utils/ui.py`

 * *Files identical despite different names*

### Comparing `android-cli-1.0.9/cli/utils/ui_menu.py` & `android_cli-1.10.0/cli/utils/ui_menu.py`

 * *Files identical despite different names*

