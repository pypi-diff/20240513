# Comparing `tmp/ce_ui-1.8.1.tar.gz` & `tmp/ce_ui-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_ui-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ce_ui-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ce_ui-1.8.1.tar` & `ce_ui-1.8.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1076 2024-05-13 06:15:16.017562 ce_ui-1.8.1/LICENSE
--rw-r--r--   0        0        0      429 2024-05-13 06:15:16.017562 ce_ui-1.8.1/README.rst
--rw-r--r--   0        0        0       47 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/__init__.py
--rw-r--r--   0        0        0      649 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/apps.py
--rw-r--r--   0        0        0     2550 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/context_processors.py
--rw-r--r--   0        0        0     3478 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/management/commands/import_terms.py
--rw-r--r--   0        0        0    11850 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/serializers.py
--rw-r--r--   0        0        0      415 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/signals.py
--rw-r--r--   0        0        0      167 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/static/images/README.md
--rw-r--r--   0        0        0     8883 2024-05-13 06:15:16.017562 ce_ui-1.8.1/ce_ui/static/images/cc/cc0-1.0.svg
--rw-r--r--   0        0        0    10236 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/cc/ccby-4.0.svg
--rw-r--r--   0        0        0    16462 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/cc/ccbysa-4.0.svg
--rw-r--r--   0        0        0     5067 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/ce_logo.svg
--rw-r--r--   0        0        0    16601 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/erc_logo.png
--rw-r--r--   0        0        0     2407 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/favicons/favicon.png
--rw-r--r--   0        0        0    19728 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/logo_livmats_small.jpg
--rw-r--r--   0        0        0    49148 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/nsf_logo.png
--rw-r--r--   0        0        0    20123 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/pitt_logo.png
--rw-r--r--   0        0        0   156800 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/screenshot_contact_mechanics.jpg
--rw-r--r--   0        0        0   182968 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/screenshot_psd.jpg
--rw-r--r--   0        0        0    51196 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/thumbnail_unavailable.png
--rw-r--r--   0        0        0     3355 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/images/uni_freiburg_logo.png
-lrwxr-xr-x   0        0        0        0 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/other/CHANGELOG.md -> ../../../CHANGELOG.md
--rw-r--r--   0        0        0    24306 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/other/TermsConditions-2.0.md
--rw-r--r--   0        0        0     5086 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/other/TermsConditions.md
--rw-r--r--   0        0        0     2735 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/other/TermsConditionsSupplement.md
--rw-r--r--   0        0        0     2736 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/FileSaver.min.js
--rw-r--r--   0        0        0    10404 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map
--rw-r--r--   0        0        0    23965 2024-05-13 06:15:16.021562 ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js
--rw-r--r--   0        0        0   247016 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon.min.js
--rw-r--r--   0        0        0   301334 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map
--rw-r--r--   0        0        0      573 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/403.html
--rw-r--r--   0        0        0      167 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/403_csrf.html
--rw-r--r--   0        0        0      269 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/404.html
--rw-r--r--   0        0        0      582 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/500.html
--rw-r--r--   0        0        0      242 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/account_inactive.html
--rw-r--r--   0        0        0      254 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/base.html
--rw-r--r--   0        0        0     2622 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/email.html
--rw-r--r--   0        0        0      950 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     1455 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/login.html
--rw-r--r--   0        0        0      540 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/logout.html
--rw-r--r--   0        0        0      490 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_change.html
--rw-r--r--   0        0        0      859 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0      473 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0      957 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      250 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      451 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/password_set.html
--rw-r--r--   0        0        0      688 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/signup.html
--rw-r--r--   0        0        0      263 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      436 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      796 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/account/verified_email_required.html
--rw-r--r--   0        0        0     1102 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/analysis/analyses_detail.html
--rw-r--r--   0        0        0      671 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/analysis/analyses_list.html
--rw-r--r--   0        0        0    25249 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/base.html
--rw-r--r--   0        0        0      149 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/fa5_icon.html
--rw-r--r--   0        0        0     1307 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/file_formats.html
--rw-r--r--   0        0        0     3809 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/select.html
--rw-r--r--   0        0        0      764 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/share.html
--rw-r--r--   0        0        0      722 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/surface_detail.html
--rw-r--r--   0        0        0      752 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/manager/topography_detail.html
--rw-r--r--   0        0        0       26 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/pages/about.html
--rw-r--r--   0        0        0     3958 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/pages/basic_usage.html
--rw-r--r--   0        0        0     1151 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/pages/help.html
--rw-r--r--   0        0        0    11200 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/pages/home.html
--rw-r--r--   0        0        0     2082 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/pages/termsconditions.html
--rw-r--r--   0        0        0      881 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/tabnav/tabs.html
--rw-r--r--   0        0        0     1498 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/users/user_detail.html
--rw-r--r--   0        0        0      474 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/users/user_form.html
--rw-r--r--   0        0        0       69 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/users/user_label.html
--rw-r--r--   0        0        0      426 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templates/users/user_list.html
--rw-r--r--   0        0        0        0 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templatetags/__init__.py
--rw-r--r--   0        0        0      487 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templatetags/icon_tags.py
--rw-r--r--   0        0        0     2253 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/templatetags/tabnav_tags.py
--rw-r--r--   0        0        0        0 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/__init__.py
--rw-r--r--   0        0        0      631 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/conftest.py
--rw-r--r--   0        0        0      234 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/fixtures.py
--rw-r--r--   0        0        0     1441 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/test_anonymous.py
--rw-r--r--   0        0        0      245 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/test_api.py
--rw-r--r--   0        0        0      576 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/test_challenge_redirect.py
--rw-r--r--   0        0        0     2843 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/test_handling.py
--rw-r--r--   0        0        0     1510 2024-05-13 06:15:16.025562 ce_ui-1.8.1/ce_ui/tests/test_prevent_url_guessing.py
--rw-r--r--   0        0        0    53839 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/tests/test_search.py
--rw-r--r--   0        0        0    13579 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/tests/test_select_tab.py
--rw-r--r--   0        0        0     7799 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/tests/test_utils.py
--rw-r--r--   0        0        0     2181 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/tests/test_welcome_page.py
--rw-r--r--   0        0        0      984 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/tests/utils.py
--rw-r--r--   0        0        0     4721 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/urls.py
--rw-r--r--   0        0        0    19875 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/utils.py
--rw-r--r--   0        0        0       86 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/version.py
--rw-r--r--   0        0        0    34148 2024-05-13 06:15:16.029563 ce_ui-1.8.1/ce_ui/views.py
--rw-r--r--   0        0        0     1819 2024-05-13 06:15:16.029563 ce_ui-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 ce_ui-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-13 20:42:24.045601 ce_ui-1.8.2/LICENSE
+-rw-r--r--   0        0        0      429 2024-05-13 20:42:24.045601 ce_ui-1.8.2/README.rst
+-rw-r--r--   0        0        0       47 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/__init__.py
+-rw-r--r--   0        0        0      649 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/apps.py
+-rw-r--r--   0        0        0     2550 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/context_processors.py
+-rw-r--r--   0        0        0     3478 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/management/commands/import_terms.py
+-rw-r--r--   0        0        0    11850 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/serializers.py
+-rw-r--r--   0        0        0      415 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/signals.py
+-rw-r--r--   0        0        0      167 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/README.md
+-rw-r--r--   0        0        0     8883 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/cc/cc0-1.0.svg
+-rw-r--r--   0        0        0    10236 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/cc/ccby-4.0.svg
+-rw-r--r--   0        0        0    16462 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/cc/ccbysa-4.0.svg
+-rw-r--r--   0        0        0     5067 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/ce_logo.svg
+-rw-r--r--   0        0        0    16601 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/erc_logo.png
+-rw-r--r--   0        0        0     2407 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/favicons/favicon.png
+-rw-r--r--   0        0        0    19728 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/logo_livmats_small.jpg
+-rw-r--r--   0        0        0    49148 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/nsf_logo.png
+-rw-r--r--   0        0        0    20123 2024-05-13 20:42:24.045601 ce_ui-1.8.2/ce_ui/static/images/pitt_logo.png
+-rw-r--r--   0        0        0   156800 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/images/screenshot_contact_mechanics.jpg
+-rw-r--r--   0        0        0   182968 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/images/screenshot_psd.jpg
+-rw-r--r--   0        0        0    51196 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/images/thumbnail_unavailable.png
+-rw-r--r--   0        0        0     3355 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/images/uni_freiburg_logo.png
+lrwxr-xr-x   0        0        0        0 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/other/CHANGELOG.md -> ../../../CHANGELOG.md
+-rw-r--r--   0        0        0    24306 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/other/TermsConditions-2.0.md
+-rw-r--r--   0        0        0     5086 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/other/TermsConditions.md
+-rw-r--r--   0        0        0     2735 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/other/TermsConditionsSupplement.md
+-rw-r--r--   0        0        0     2736 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js
+-rw-r--r--   0        0        0    10404 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map
+-rw-r--r--   0        0        0    23965 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js
+-rw-r--r--   0        0        0   247016 2024-05-13 20:42:24.049601 ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js
+-rw-r--r--   0        0        0   301334 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map
+-rw-r--r--   0        0        0      573 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/403.html
+-rw-r--r--   0        0        0      167 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/403_csrf.html
+-rw-r--r--   0        0        0      269 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/404.html
+-rw-r--r--   0        0        0      582 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/500.html
+-rw-r--r--   0        0        0      242 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      254 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/base.html
+-rw-r--r--   0        0        0     2622 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/email.html
+-rw-r--r--   0        0        0      950 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     1455 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/login.html
+-rw-r--r--   0        0        0      540 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      490 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_change.html
+-rw-r--r--   0        0        0      859 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0      473 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0      957 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      250 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      451 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/password_set.html
+-rw-r--r--   0        0        0      688 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      263 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      436 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      796 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/account/verified_email_required.html
+-rw-r--r--   0        0        0     1102 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/analysis/analyses_detail.html
+-rw-r--r--   0        0        0      671 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/analysis/analyses_list.html
+-rw-r--r--   0        0        0    25249 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/base.html
+-rw-r--r--   0        0        0      149 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/fa5_icon.html
+-rw-r--r--   0        0        0     1307 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/file_formats.html
+-rw-r--r--   0        0        0     3809 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/select.html
+-rw-r--r--   0        0        0      764 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/share.html
+-rw-r--r--   0        0        0      722 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/surface_detail.html
+-rw-r--r--   0        0        0      752 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/manager/topography_detail.html
+-rw-r--r--   0        0        0       26 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/pages/about.html
+-rw-r--r--   0        0        0     3958 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/pages/basic_usage.html
+-rw-r--r--   0        0        0     1151 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/pages/help.html
+-rw-r--r--   0        0        0    11200 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/pages/home.html
+-rw-r--r--   0        0        0     2082 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/pages/termsconditions.html
+-rw-r--r--   0        0        0      881 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/tabnav/tabs.html
+-rw-r--r--   0        0        0     1498 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/users/user_detail.html
+-rw-r--r--   0        0        0      474 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/users/user_form.html
+-rw-r--r--   0        0        0       69 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/users/user_label.html
+-rw-r--r--   0        0        0      426 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templates/users/user_list.html
+-rw-r--r--   0        0        0        0 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templatetags/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templatetags/icon_tags.py
+-rw-r--r--   0        0        0     2253 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/templatetags/tabnav_tags.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/conftest.py
+-rw-r--r--   0        0        0      234 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/fixtures.py
+-rw-r--r--   0        0        0     1441 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_anonymous.py
+-rw-r--r--   0        0        0      245 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_api.py
+-rw-r--r--   0        0        0      576 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_challenge_redirect.py
+-rw-r--r--   0        0        0     2843 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_handling.py
+-rw-r--r--   0        0        0     1510 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_prevent_url_guessing.py
+-rw-r--r--   0        0        0    53839 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_search.py
+-rw-r--r--   0        0        0    13579 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_select_tab.py
+-rw-r--r--   0        0        0     7799 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_utils.py
+-rw-r--r--   0        0        0     2181 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/test_welcome_page.py
+-rw-r--r--   0        0        0      984 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/tests/utils.py
+-rw-r--r--   0        0        0     4721 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/urls.py
+-rw-r--r--   0        0        0    19875 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/utils.py
+-rw-r--r--   0        0        0       86 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/version.py
+-rw-r--r--   0        0        0    34148 2024-05-13 20:42:24.053601 ce_ui-1.8.2/ce_ui/views.py
+-rw-r--r--   0        0        0     1819 2024-05-13 20:42:24.057601 ce_ui-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 ce_ui-1.8.2/PKG-INFO
```

### Comparing `ce_ui-1.8.1/LICENSE` & `ce_ui-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/apps.py` & `ce_ui-1.8.2/ce_ui/apps.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/context_processors.py` & `ce_ui-1.8.2/ce_ui/context_processors.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/management/commands/import_terms.py` & `ce_ui-1.8.2/ce_ui/management/commands/import_terms.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/serializers.py` & `ce_ui-1.8.2/ce_ui/serializers.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/cc/cc0-1.0.svg` & `ce_ui-1.8.2/ce_ui/static/images/cc/cc0-1.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/cc/ccby-4.0.svg` & `ce_ui-1.8.2/ce_ui/static/images/cc/ccby-4.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/cc/ccbysa-4.0.svg` & `ce_ui-1.8.2/ce_ui/static/images/cc/ccbysa-4.0.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/ce_logo.svg` & `ce_ui-1.8.2/ce_ui/static/images/ce_logo.svg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/erc_logo.png` & `ce_ui-1.8.2/ce_ui/static/images/erc_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/favicons/favicon.png` & `ce_ui-1.8.2/ce_ui/static/images/favicons/favicon.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/logo_livmats_small.jpg` & `ce_ui-1.8.2/ce_ui/static/images/logo_livmats_small.jpg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/nsf_logo.png` & `ce_ui-1.8.2/ce_ui/static/images/nsf_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/pitt_logo.png` & `ce_ui-1.8.2/ce_ui/static/images/pitt_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/screenshot_contact_mechanics.jpg` & `ce_ui-1.8.2/ce_ui/static/images/screenshot_contact_mechanics.jpg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/screenshot_psd.jpg` & `ce_ui-1.8.2/ce_ui/static/images/screenshot_psd.jpg`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/thumbnail_unavailable.png` & `ce_ui-1.8.2/ce_ui/static/images/thumbnail_unavailable.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/images/uni_freiburg_logo.png` & `ce_ui-1.8.2/ce_ui/static/images/uni_freiburg_logo.png`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/other/TermsConditions-2.0.md` & `ce_ui-1.8.2/ce_ui/static/other/TermsConditions-2.0.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/other/TermsConditions.md` & `ce_ui-1.8.2/ce_ui/static/other/TermsConditions.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/other/TermsConditionsSupplement.md` & `ce_ui-1.8.2/ce_ui/static/other/TermsConditionsSupplement.md`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/FileSaver.min.js` & `ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map` & `ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/FileSaver.min.js.map`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js` & `ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon-scalebar.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon.min.js` & `ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map` & `ce_ui-1.8.2/ce_ui/static/vendor/openseadragon/openseadragon.min.js.map`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/403.html` & `ce_ui-1.8.2/ce_ui/templates/403.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/500.html` & `ce_ui-1.8.2/ce_ui/templates/500.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/email.html` & `ce_ui-1.8.2/ce_ui/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/email_confirm.html` & `ce_ui-1.8.2/ce_ui/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/login.html` & `ce_ui-1.8.2/ce_ui/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/logout.html` & `ce_ui-1.8.2/ce_ui/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/password_reset.html` & `ce_ui-1.8.2/ce_ui/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/password_reset_from_key.html` & `ce_ui-1.8.2/ce_ui/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/signup.html` & `ce_ui-1.8.2/ce_ui/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/account/verified_email_required.html` & `ce_ui-1.8.2/ce_ui/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/analysis/analyses_detail.html` & `ce_ui-1.8.2/ce_ui/templates/analysis/analyses_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/analysis/analyses_list.html` & `ce_ui-1.8.2/ce_ui/templates/analysis/analyses_list.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/base.html` & `ce_ui-1.8.2/ce_ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/manager/file_formats.html` & `ce_ui-1.8.2/ce_ui/templates/manager/file_formats.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/manager/select.html` & `ce_ui-1.8.2/ce_ui/templates/manager/select.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/manager/share.html` & `ce_ui-1.8.2/ce_ui/templates/manager/share.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/manager/surface_detail.html` & `ce_ui-1.8.2/ce_ui/templates/manager/surface_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/manager/topography_detail.html` & `ce_ui-1.8.2/ce_ui/templates/manager/topography_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/pages/basic_usage.html` & `ce_ui-1.8.2/ce_ui/templates/pages/basic_usage.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/pages/help.html` & `ce_ui-1.8.2/ce_ui/templates/pages/help.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/pages/home.html` & `ce_ui-1.8.2/ce_ui/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/pages/termsconditions.html` & `ce_ui-1.8.2/ce_ui/templates/pages/termsconditions.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/tabnav/tabs.html` & `ce_ui-1.8.2/ce_ui/templates/tabnav/tabs.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templates/users/user_detail.html` & `ce_ui-1.8.2/ce_ui/templates/users/user_detail.html`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/templatetags/tabnav_tags.py` & `ce_ui-1.8.2/ce_ui/templatetags/tabnav_tags.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/conftest.py` & `ce_ui-1.8.2/ce_ui/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_anonymous.py` & `ce_ui-1.8.2/ce_ui/tests/test_anonymous.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_challenge_redirect.py` & `ce_ui-1.8.2/ce_ui/tests/test_challenge_redirect.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_handling.py` & `ce_ui-1.8.2/ce_ui/tests/test_handling.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_prevent_url_guessing.py` & `ce_ui-1.8.2/ce_ui/tests/test_prevent_url_guessing.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_search.py` & `ce_ui-1.8.2/ce_ui/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_select_tab.py` & `ce_ui-1.8.2/ce_ui/tests/test_select_tab.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_utils.py` & `ce_ui-1.8.2/ce_ui/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/test_welcome_page.py` & `ce_ui-1.8.2/ce_ui/tests/test_welcome_page.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/tests/utils.py` & `ce_ui-1.8.2/ce_ui/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/urls.py` & `ce_ui-1.8.2/ce_ui/urls.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/utils.py` & `ce_ui-1.8.2/ce_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/ce_ui/views.py` & `ce_ui-1.8.2/ce_ui/views.py`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/pyproject.toml` & `ce_ui-1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ce_ui-1.8.1/PKG-INFO` & `ce_ui-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ce-ui
-Version: 1.8.1
+Version: 1.8.2
 Summary: The user-facing interface of contact.engineering.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

