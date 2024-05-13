# Comparing `tmp/core_website_app-2.8.0.tar.gz` & `tmp/core_website_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_website_app-2.8.0.tar", last modified: Tue Mar 12 19:07:32 2024, max compression
+gzip compressed data, was "core_website_app-2.9.0.tar", last modified: Mon May 13 16:12:49 2024, max compression
```

## Comparing `core_website_app-2.8.0.tar` & `core_website_app-2.9.0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.247366 core_website_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:07:23.000000 core_website_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2024-03-12 19:07:23.000000 core_website_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2024-03-12 19:07:32.240834 core_website_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2024-03-12 19:07:23.000000 core_website_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.832262 core_website_app-2.8.0/core_website_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3597 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/admin.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.990691 core_website_app-2.8.0/core_website_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/commons/enums.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.010277 core_website_app-2.8.0/core_website_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       24 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.067552 core_website_app-2.8.0/core_website_app/components/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/account_request/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/account_request/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.125225 core_website_app-2.8.0/core_website_app/components/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2177 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/contact_message/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      938 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/contact_message/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.162512 core_website_app-2.8.0/core_website_app/components/help/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/help/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      780 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/help/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.202775 core_website_app-2.8.0/core_website_app/components/privacy_policy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/privacy_policy/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/privacy_policy/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.248532 core_website_app-2.8.0/core_website_app/components/rules_of_behavior/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/rules_of_behavior/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/rules_of_behavior/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.300983 core_website_app-2.8.0/core_website_app/components/terms_of_use/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/terms_of_use/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/components/terms_of_use/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2449 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.336205 core_website_app-2.8.0/core_website_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.375661 core_website_app-2.8.0/core_website_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.489830 core_website_app-2.8.0/core_website_app/rest/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2934 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/account_request/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1553 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/account_request/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/account_request/tests.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5445 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/account_request/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.566471 core_website_app-2.8.0/core_website_app/rest/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      457 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/contact_message/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/contact_message/tests.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5620 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/contact_message/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.361826 core_website_app-2.8.0/core_website_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.381735 core_website_app-2.8.0/core_website_app/static/core_website_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.374921 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.596069 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 19:07:23.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/css/messages.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.668212 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/messages.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/messages.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4034 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/user_requests.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      273 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/user_requests.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.391793 core_website_app-2.8.0/core_website_app/static/core_website_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.693685 core_website_app-2.8.0/core_website_app/static/core_website_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/user/css/list.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.713853 core_website_app-2.8.0/core_website_app/static/core_website_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/static/core_website_app/user/js/user_account_req.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.411934 core_website_app-2.8.0/core_website_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.491124 core_website_app-2.8.0/core_website_app/templates/core_website_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.836833 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.857380 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.879026 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2116 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1577 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.902923 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:30.923802 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      687 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.016362 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      422 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/contact_message_for_admin.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      385 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/request_account_approved.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/request_account_denied.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/request_account_for_admin.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      331 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/email/request_account_for_user.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/help.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.484169 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.077349 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/confirm_delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/read.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.136294 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/user_requests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/user_requests/accept.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/user_requests/deny.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/modals/user_requests/error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/privacy_policy.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/rules_of_behavior.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/terms_of_use.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/user_requests.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.281244 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1034 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/contact.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/footer_menu.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3418 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/help.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      330 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/privacy-policy.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      239 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/request_error.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1280 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/request_new_account.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      436 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/rules_of_behavior.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/templates/core_website_app/user/terms-of-use.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.331896 core_website_app-2.8.0/core_website_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      341 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/utils/custom_context_processors.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.354991 core_website_app-2.8.0/core_website_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.414808 core_website_app-2.8.0/core_website_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4935 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1997 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.511904 core_website_app-2.8.0/core_website_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7550 2024-03-12 19:07:24.000000 core_website_app-2.8.0/core_website_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:29.934335 core_website_app-2.8.0/core_website_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2024-03-12 19:07:28.000000 core_website_app-2.8.0/core_website_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6059 2024-03-12 19:07:29.000000 core_website_app-2.8.0/core_website_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:07:28.000000 core_website_app-2.8.0/core_website_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-03-12 19:07:28.000000 core_website_app-2.8.0/core_website_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-03-12 19:07:28.000000 core_website_app-2.8.0/core_website_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:07:25.000000 core_website_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 19:07:25.000000 core_website_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-03-12 19:07:25.000000 core_website_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:07:32.250095 core_website_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2024-03-12 19:07:25.000000 core_website_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.555752 core_website_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.576865 core_website_app-2.8.0/tests/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.601246 core_website_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.650296 core_website_app-2.8.0/tests/components/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8580 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/account_request/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.712886 core_website_app-2.8.0/tests/components/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/contact_message/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5239 2024-03-12 19:07:25.000000 core_website_app-2.8.0/tests/components/contact_message/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.784230 core_website_app-2.8.0/tests/components/help/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/help/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1443 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/help/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.829250 core_website_app-2.8.0/tests/components/privacy_policy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/privacy_policy/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1676 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/privacy_policy/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.884485 core_website_app-2.8.0/tests/components/rules_of_behavior/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/rules_of_behavior/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1787 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/rules_of_behavior/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.926433 core_website_app-2.8.0/tests/components/terms_of_use/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/terms_of_use/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/terms_of_use/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.966514 core_website_app-2.8.0/tests/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3566 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/components/web_page/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:31.987528 core_website_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.035633 core_website_app-2.8.0/tests/rest/account_request/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/rest/account_request/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8169 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/rest/account_request/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.081459 core_website_app-2.8.0/tests/rest/contact_message/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/rest/contact_message/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7339 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/rest/contact_message/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.104801 core_website_app-2.8.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2229 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.131758 core_website_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.158458 core_website_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.185626 core_website_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:32.214829 core_website_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:26.000000 core_website_app-2.8.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.152245 core_website_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:12:35.000000 core_website_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2024-05-13 16:12:35.000000 core_website_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2024-05-13 16:12:49.146321 core_website_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2024-05-13 16:12:35.000000 core_website_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.440865 core_website_app-2.9.0/core_website_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3597 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/admin.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.590441 core_website_app-2.9.0/core_website_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      225 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/commons/enums.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.612557 core_website_app-2.9.0/core_website_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       24 2024-05-13 16:12:35.000000 core_website_app-2.9.0/core_website_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.664934 core_website_app-2.9.0/core_website_app/components/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/account_request/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/account_request/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.724216 core_website_app-2.9.0/core_website_app/components/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2177 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/contact_message/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      938 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/contact_message/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.763603 core_website_app-2.9.0/core_website_app/components/help/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/help/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      780 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/help/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.802167 core_website_app-2.9.0/core_website_app/components/privacy_policy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/privacy_policy/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      913 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/privacy_policy/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.844883 core_website_app-2.9.0/core_website_app/components/rules_of_behavior/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/rules_of_behavior/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/rules_of_behavior/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.882564 core_website_app-2.9.0/core_website_app/components/terms_of_use/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/terms_of_use/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      875 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/components/terms_of_use/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2449 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.920185 core_website_app-2.9.0/core_website_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:36.000000 core_website_app-2.9.0/core_website_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.983977 core_website_app-2.9.0/core_website_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.089165 core_website_app-2.9.0/core_website_app/rest/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2934 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/account_request/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1553 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/account_request/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/account_request/tests.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5445 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/account_request/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.169570 core_website_app-2.9.0/core_website_app/rest/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:38.000000 core_website_app-2.9.0/core_website_app/rest/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      457 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/rest/contact_message/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/rest/contact_message/tests.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5620 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/rest/contact_message/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:45.963824 core_website_app-2.9.0/core_website_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:45.986890 core_website_app-2.9.0/core_website_app/static/core_website_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:45.979063 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.201998 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/css/messages.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.275969 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/messages.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/messages.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4034 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/user_requests.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      273 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/user_requests.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.008275 core_website_app-2.9.0/core_website_app/static/core_website_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.299686 core_website_app-2.9.0/core_website_app/static/core_website_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/user/css/list.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.320952 core_website_app-2.9.0/core_website_app/static/core_website_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/static/core_website_app/user/js/user_account_req.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.022137 core_website_app-2.9.0/core_website_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.104223 core_website_app-2.9.0/core_website_app/templates/core_website_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.450601 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.472064 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.494605 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2116 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1577 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.514831 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.535179 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      687 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.915052 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      422 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/contact_message_for_admin.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      385 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/request_account_approved.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/request_account_denied.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/request_account_for_admin.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      331 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/email/request_account_for_user.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/help.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.099286 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:47.975030 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/confirm_delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      212 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/contact_messages/read.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.035640 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/user_requests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      213 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/user_requests/accept.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/user_requests/deny.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/modals/user_requests/error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/privacy_policy.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/rules_of_behavior.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/terms_of_use.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/user_requests.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.220844 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1034 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/contact.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/footer_menu.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     3418 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/help.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      330 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/privacy-policy.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      239 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/request_error.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1280 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/request_new_account.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      436 2024-05-13 16:12:40.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/rules_of_behavior.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/templates/core_website_app/user/terms-of-use.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      978 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.264381 core_website_app-2.9.0/core_website_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      341 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/utils/custom_context_processors.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.285896 core_website_app-2.9.0/core_website_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.365067 core_website_app-2.9.0/core_website_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4935 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1997 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.458779 core_website_app-2.9.0/core_website_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1377 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7550 2024-05-13 16:12:41.000000 core_website_app-2.9.0/core_website_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:46.531892 core_website_app-2.9.0/core_website_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1240 2024-05-13 16:12:45.000000 core_website_app-2.9.0/core_website_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6059 2024-05-13 16:12:45.000000 core_website_app-2.9.0/core_website_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:12:45.000000 core_website_app-2.9.0/core_website_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-05-13 16:12:45.000000 core_website_app-2.9.0/core_website_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-05-13 16:12:45.000000 core_website_app-2.9.0/core_website_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:12:42.000000 core_website_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:12:42.000000 core_website_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-05-13 16:12:42.000000 core_website_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:12:49.154470 core_website_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1451 2024-05-13 16:12:42.000000 core_website_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.503414 core_website_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.525124 core_website_app-2.9.0/tests/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.550960 core_website_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.599529 core_website_app-2.9.0/tests/components/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8580 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/account_request/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.657039 core_website_app-2.9.0/tests/components/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/contact_message/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5239 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/contact_message/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.698184 core_website_app-2.9.0/tests/components/help/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/help/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1443 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/help/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.739608 core_website_app-2.9.0/tests/components/privacy_policy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/privacy_policy/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1676 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/privacy_policy/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.783592 core_website_app-2.9.0/tests/components/rules_of_behavior/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/rules_of_behavior/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1787 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/rules_of_behavior/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.826951 core_website_app-2.9.0/tests/components/terms_of_use/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/terms_of_use/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/terms_of_use/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.880249 core_website_app-2.9.0/tests/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3566 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/components/web_page/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.900031 core_website_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.943399 core_website_app-2.9.0/tests/rest/account_request/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/rest/account_request/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8169 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/rest/account_request/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:48.985631 core_website_app-2.9.0/tests/rest/contact_message/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/rest/contact_message/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7339 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/rest/contact_message/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.005550 core_website_app-2.9.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2229 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.034288 core_website_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.072775 core_website_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.098511 core_website_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:49.122355 core_website_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:42.000000 core_website_app-2.9.0/tests/views/user/__init__.py
```

### Comparing `core_website_app-2.8.0/LICENSE.md` & `core_website_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/PKG-INFO` & `core_website_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_website_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Basic web functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_website_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ================
         Core Website App
```

### Comparing `core_website_app-2.8.0/README.rst` & `core_website_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/admin.py` & `core_website_app-2.9.0/core_website_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/account_request/api.py` & `core_website_app-2.9.0/core_website_app/components/account_request/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/account_request/models.py` & `core_website_app-2.9.0/core_website_app/components/account_request/models.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/contact_message/api.py` & `core_website_app-2.9.0/core_website_app/components/contact_message/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/contact_message/models.py` & `core_website_app-2.9.0/core_website_app/components/contact_message/models.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/help/api.py` & `core_website_app-2.9.0/core_website_app/components/help/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/privacy_policy/api.py` & `core_website_app-2.9.0/core_website_app/components/privacy_policy/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/rules_of_behavior/api.py` & `core_website_app-2.9.0/core_website_app/components/rules_of_behavior/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/components/terms_of_use/api.py` & `core_website_app-2.9.0/core_website_app/components/terms_of_use/api.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/menus.py` & `core_website_app-2.9.0/core_website_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/migrations/0001_initial.py` & `core_website_app-2.9.0/core_website_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/rest/account_request/abstract_views.py` & `core_website_app-2.9.0/core_website_app/rest/account_request/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/rest/account_request/serializers.py` & `core_website_app-2.9.0/core_website_app/rest/account_request/serializers.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/rest/account_request/views.py` & `core_website_app-2.9.0/core_website_app/rest/account_request/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/rest/contact_message/views.py` & `core_website_app-2.9.0/core_website_app/rest/contact_message/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/rest/urls.py` & `core_website_app-2.9.0/core_website_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/settings.py` & `core_website_app-2.9.0/core_website_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/messages.js` & `core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/messages.js`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/static/core_website_app/admin/js/user_requests.js` & `core_website_app-2.9.0/core_website_app/static/core_website_app/admin/js/user_requests.js`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/modals/deny_request.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/account_requests/pending.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/list.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/admin/contact_messages/modals/delete_message.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/user/contact.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/user/contact.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/user/help.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/user/help.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/templates/core_website_app/user/request_new_account.html` & `core_website_app-2.9.0/core_website_app/templates/core_website_app/user/request_new_account.html`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/urls.py` & `core_website_app-2.9.0/core_website_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/views/admin/ajax.py` & `core_website_app-2.9.0/core_website_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/views/admin/views.py` & `core_website_app-2.9.0/core_website_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/views/user/forms.py` & `core_website_app-2.9.0/core_website_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app/views/user/views.py` & `core_website_app-2.9.0/core_website_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/core_website_app.egg-info/PKG-INFO` & `core_website_app-2.9.0/core_website_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-website-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Basic web functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_website_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ================
         Core Website App
```

### Comparing `core_website_app-2.8.0/core_website_app.egg-info/SOURCES.txt` & `core_website_app-2.9.0/core_website_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/setup.py` & `core_website_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_website_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Basic web functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_website_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_website_app-2.8.0/tests/components/account_request/tests_unit.py` & `core_website_app-2.9.0/tests/components/account_request/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/contact_message/tests_int.py` & `core_website_app-2.9.0/tests/components/contact_message/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/contact_message/tests_unit.py` & `core_website_app-2.9.0/tests/components/contact_message/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/help/tests_unit.py` & `core_website_app-2.9.0/tests/components/help/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/privacy_policy/tests_unit.py` & `core_website_app-2.9.0/tests/components/privacy_policy/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/rules_of_behavior/tests_unit.py` & `core_website_app-2.9.0/tests/components/rules_of_behavior/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/terms_of_use/tests_unit.py` & `core_website_app-2.9.0/tests/components/terms_of_use/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/components/web_page/tests_unit.py` & `core_website_app-2.9.0/tests/components/web_page/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/rest/account_request/tests_permission.py` & `core_website_app-2.9.0/tests/rest/account_request/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/rest/contact_message/tests_permission.py` & `core_website_app-2.9.0/tests/rest/contact_message/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_website_app-2.8.0/tests/test_settings.py` & `core_website_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

