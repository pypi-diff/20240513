# Comparing `tmp/simpledomcontrol-0.4.6.tar.gz` & `tmp/simpledomcontrol-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpledomcontrol-0.4.6.tar", max compression
+gzip compressed data, was "simpledomcontrol-0.4.8.tar", max compression
```

## Comparing `simpledomcontrol-0.4.6.tar` & `simpledomcontrol-0.4.8.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rwxr-xr-x   0        0        0       18 2023-09-13 12:39:11.659921 simpledomcontrol-0.4.6/README.md
--rwxr-xr-x   0        0        0     1082 2023-12-15 08:41:43.223803 simpledomcontrol-0.4.6/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.166975 simpledomcontrol-0.4.6/sdc_core/__init__.py
--rwxr-xr-x   0        0        0       98 2023-09-21 08:45:54.656855 simpledomcontrol-0.4.6/sdc_core/apps.py
--rw-r--r--   0        0        0    18645 2023-12-13 14:34:04.092799 simpledomcontrol-0.4.6/sdc_core/consumers.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.6/sdc_core/management/__init__.py
--rw-r--r--   0        0        0      164 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.6/sdc_core/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      176 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.6/sdc_core/management/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.6/sdc_core/management/commands/__init__.py
--rw-r--r--   0        0        0      173 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      185 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      185 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/_private.cpython-39.pyc
--rw-r--r--   0        0        0     3111 2023-11-16 20:41:41.244279 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_cc.cpython-310.pyc
--rw-r--r--   0        0        0     3235 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_cc.cpython-39.pyc
--rw-r--r--   0        0        0     3278 2023-11-15 14:57:12.955993 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_controller_infos.cpython-310.pyc
--rw-r--r--   0        0        0      967 2023-11-15 07:20:44.934088 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_controller_url.cpython-310.pyc
--rw-r--r--   0        0        0     2669 2023-11-07 13:16:56.062974 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_model_infos.cpython-310.pyc
--rw-r--r--   0        0        0     2302 2023-11-24 09:37:56.060620 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_init.cpython-310.pyc
--rw-r--r--   0        0        0     2368 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_init.cpython-39.pyc
--rw-r--r--   0        0        0     2777 2023-11-16 20:24:39.232107 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-310.pyc
--rw-r--r--   0        0        0     2785 2023-04-04 10:33:03.270414 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-39.pyc
--rw-r--r--   0        0        0     3134 2023-11-24 08:07:05.791278 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_links.cpython-310.pyc
--rw-r--r--   0        0        0     2033 2023-09-21 08:46:16.872860 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-310.pyc
--rw-r--r--   0        0        0     2048 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-39.pyc
--rw-r--r--   0        0        0     5905 2023-03-31 13:46:19.184969 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-310.pyc
--rw-r--r--   0        0        0     5940 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-39.pyc
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.6/sdc_core/management/commands/_private.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__init__.py
--rw-r--r--   0        0        0      182 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      194 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8592 2023-11-24 08:07:06.275254 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-310.pyc
--rw-r--r--   0        0        0     8033 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4225 2023-09-21 08:46:16.120859 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4205 2023-04-04 10:50:54.427002 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-39.pyc
--rw-r--r--   0        0        0     1515 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/options.cpython-310.pyc
--rw-r--r--   0        0        0     1545 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     1793 2023-09-21 08:46:13.508859 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4789 2023-11-16 20:45:13.741182 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4479 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2641 2023-09-14 07:32:05.325796 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     2665 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/utils.cpython-39.pyc
--rwxr-xr-x   0        0        0    11256 2023-11-24 06:39:15.995849 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/add_controller_manager.py
--rw-r--r--   0        0        0     4591 2023-09-21 08:45:54.636855 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/add_model_manager.py
--rwxr-xr-x   0        0        0     1217 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/options.py
--rwxr-xr-x   0        0        0     1889 2023-09-21 08:45:54.644855 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/sdc_core_manager.py
--rwxr-xr-x   0        0        0     4472 2023-11-16 20:45:12.821178 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/settings_manager.py
--rwxr-xr-x   0        0        0     2157 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/utils.py
--rwxr-xr-x   0        0        0     3251 2023-11-16 20:25:56.852389 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_cc.py
--rw-r--r--   0        0        0     3694 2023-11-15 14:56:59.559480 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_get_controller_infos.py
--rw-r--r--   0        0        0      507 2023-11-15 07:20:42.554086 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_get_controller_url.py
--rw-r--r--   0        0        0     2665 2023-11-07 13:16:45.855370 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_get_model_infos.py
--rwxr-xr-x   0        0        0     2711 2023-11-24 09:32:19.797721 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_init.py
--rw-r--r--   0        0        0      703 2023-10-12 09:29:35.938805 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_is_installed.py
--rwxr-xr-x   0        0        0     2642 2023-11-16 20:24:23.716052 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_new_model.py
--rwxr-xr-x   0        0        0     3608 2023-11-24 06:25:48.207532 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_update_links.py
--rwxr-xr-x   0        0        0     1933 2023-09-21 08:45:54.588855 simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_update_url.py
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__init__.py
--rw-r--r--   0        0        0      165 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1322 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/forms.cpython-310.pyc
--rw-r--r--   0        0        0      605 2023-11-15 08:32:34.682753 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/import_manager.cpython-310.pyc
--rw-r--r--   0        0        0     2508 2023-10-11 13:59:42.076794 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     2201 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     1280 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/search.cpython-310.pyc
--rw-r--r--   0        0        0     2597 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/views.cpython-310.pyc
--rwxr-xr-x   0        0        0     1174 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/forms.py
--rwxr-xr-x   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/import_manager.py
--rw-r--r--   0        0        0     2234 2023-10-11 13:59:37.053640 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/models.py
--rwxr-xr-x   0        0        0     2458 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/response.py
--rwxr-xr-x   0        0        0     1838 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/search.py
--rwxr-xr-x   0        0        0     2380 2023-09-21 08:45:54.668855 simpledomcontrol-0.4.6/sdc_core/sdc_extentions/views.py
--rw-r--r--   0        0        0      107 2023-12-12 08:17:05.980843 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/.babelrc
--rw-r--r--   0        0        0     4673 2023-12-15 08:40:53.567934 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/gulpfile.jsx
--rwxr-xr-x   0        0        0      399 2023-12-12 12:31:17.861882 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/src/index.organizer.js
--rw-r--r--   0        0        0      324 2023-11-24 09:54:39.300747 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/src/index.style.scss
--rw-r--r--   0        0        0      429 2023-11-24 09:34:33.772197 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/tests/pre-test-setup.js
--rw-r--r--   0        0        0      212 2023-12-12 12:31:17.893882 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/tests/test-setup.js
--rw-r--r--   0        0        0     1139 2023-09-22 07:43:59.149945 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
--rw-r--r--   0        0        0      432 2023-09-22 07:54:08.342934 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
--rw-r--r--   0        0        0      677 2023-09-22 07:54:40.070948 simpledomcontrol-0.4.6/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
--rwxr-xr-x   0        0        0     1228 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
--rwxr-xr-x   0        0        0     2464 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/index.html
--rwxr-xr-x   0        0        0     2328 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/server_call.txt
--rwxr-xr-x   0        0        0      895 2023-11-17 10:42:24.806725 simpledomcontrol-0.4.6/sdc_core/template_files/asgi.py.txt
--rwxr-xr-x   0        0        0       82 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/controller/templade_view.html
--rwxr-xr-x   0        0        0     1337 2023-12-12 12:31:17.885882 simpledomcontrol-0.4.6/sdc_core/template_files/controller/template_controller.js.txt
--rwxr-xr-x   0        0        0       18 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/controller/template_css.scss
--rw-r--r--   0        0        0      535 2023-11-24 10:09:44.297249 simpledomcontrol-0.4.6/sdc_core/template_files/controller/template_test.js.text
--rw-r--r--   0        0        0      278 2023-12-12 12:31:17.897882 simpledomcontrol-0.4.6/sdc_core/template_files/js_test.js.txt
--rw-r--r--   0        0        0     1633 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/models/detail.html
--rw-r--r--   0        0        0     2303 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/models/list.html
--rwxr-xr-x   0        0        0     1635 2023-12-12 12:32:29.273766 simpledomcontrol-0.4.6/sdc_core/template_files/package.json
--rwxr-xr-x   0        0        0      357 2023-09-21 08:45:54.596855 simpledomcontrol-0.4.6/sdc_core/template_files/routing.py.txt
--rwxr-xr-x   0        0        0      149 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/sdc_urls.py.txt
--rwxr-xr-x   0        0        0       90 2023-09-21 08:45:54.608855 simpledomcontrol-0.4.6/sdc_core/template_files/sdc_views.py.txt
--rwxr-xr-x   0        0        0      936 2023-11-24 11:35:47.297156 simpledomcontrol-0.4.6/sdc_core/template_files/settings_extension.py.txt
--rwxr-xr-x   0        0        0      989 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/templates/base.html
--rwxr-xr-x   0        0        0      427 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/templates/index.html
--rwxr-xr-x   0        0        0      289 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_core/template_files/urls.py.txt
--rw-r--r--   0        0        0     2847 2023-12-12 12:31:17.821882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
--rw-r--r--   0        0        0     1178 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
--rw-r--r--   0        0        0     2454 2023-12-12 12:31:17.869882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
--rw-r--r--   0        0        0     1833 2023-12-12 12:31:17.901882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
--rw-r--r--   0        0        0       23 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
--rw-r--r--   0        0        0     1318 2023-12-12 12:31:17.793882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
--rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
--rw-r--r--   0        0        0     3046 2023-12-13 13:46:40.556259 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
--rw-r--r--   0        0        0      103 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
--rw-r--r--   0        0        0     3267 2023-12-12 12:31:17.909881 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
--rw-r--r--   0        0        0      180 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
--rw-r--r--   0        0        0     1457 2023-12-12 12:31:17.829882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
--rw-r--r--   0        0        0    20079 2023-12-13 15:05:52.501451 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
--rw-r--r--   0        0        0     1019 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
--rw-r--r--   0        0        0     4914 2023-12-12 12:31:17.837882 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
--rw-r--r--   0        0        0     2238 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
--rw-r--r--   0        0        0     2819 2023-12-12 12:31:17.961881 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
--rw-r--r--   0        0        0      668 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
--rw-r--r--   0        0        0      364 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
--rw-r--r--   0        0        0      462 2023-12-12 12:31:17.945881 simpledomcontrol-0.4.6/sdc_tools/Assets/tests/sdc_tools.test.js
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_tools/__init__.py
--rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.6/sdc_tools/admin.py
--rwxr-xr-x   0        0        0       97 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/apps.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/migrations/__init__.py
--rw-r--r--   0        0        0      233 2023-09-14 07:34:03.056641 simpledomcontrol-0.4.6/sdc_tools/migrations/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       60 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/models.py
--rwxr-xr-x   0        0        0      804 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/sdc_urls.py
--rwxr-xr-x   0        0        0     1485 2023-09-21 08:45:54.640855 simpledomcontrol-0.4.6/sdc_tools/sdc_views.py
--rwxr-xr-x   0        0        0     2110 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/elements/form.html
--rwxr-xr-x   0        0        0     1866 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/elements/inline_form.html
--rwxr-xr-x   0        0        0     1132 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/email/base.html
--rw-r--r--   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
--rw-r--r--   0        0        0       36 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
--rw-r--r--   0        0        0      136 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
--rw-r--r--   0        0        0       37 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
--rw-r--r--   0        0        0      338 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
--rwxr-xr-x   0        0        0      141 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
--rw-r--r--   0        0        0      496 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templatetags/__init__.py
--rw-r--r--   0        0        0      164 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1061 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/addclass.cpython-310.pyc
--rw-r--r--   0        0        0      667 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/indexfilter.cpython-310.pyc
--rw-r--r--   0        0        0     1481 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/sdc_filter.cpython-310.pyc
--rwxr-xr-x   0        0        0      825 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templatetags/addclass.py
--rwxr-xr-x   0        0        0      357 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templatetags/indexfilter.py
--rwxr-xr-x   0        0        0     1135 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/templatetags/sdc_filter.py
--rwxr-xr-x   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/tests.py
--rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_tools/views.py
--rw-r--r--   0        0        0     1453 2023-12-12 12:31:17.865882 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
--rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
--rw-r--r--   0        0        0     1424 2023-12-12 12:31:17.797882 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
--rw-r--r--   0        0        0       18 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
--rw-r--r--   0        0        0      110 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
--rw-r--r--   0        0        0       49 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
--rw-r--r--   0        0        0      456 2023-12-12 12:31:17.813882 simpledomcontrol-0.4.6/sdc_user/Assets/tests/sdc_user.test.js
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_user/__init__.py
--rw-r--r--   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_user/admin.py
--rw-r--r--   0        0        0      147 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_user/apps.py
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_user/migrations/__init__.py
--rw-r--r--   0        0        0      232 2023-09-14 07:34:03.060642 simpledomcontrol-0.4.6/sdc_user/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.6/sdc_user/models.py
--rw-r--r--   0        0        0      304 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.6/sdc_user/sdc_urls.py
--rw-r--r--   0        0        0     2140 2023-09-21 08:45:54.648855 simpledomcontrol-0.4.6/sdc_user/sdc_views.py
--rw-r--r--   0        0        0      401 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.6/sdc_user/templates/sdc_user/sdc/sdc_login.html
--rw-r--r--   0        0        0      327 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.6/sdc_user/templates/sdc_user/sdc/sdc_logout.html
--rw-r--r--   0        0        0       60 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.6/sdc_user/tests.py
--rw-r--r--   0        0        0       63 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.6/sdc_user/views.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 simpledomcontrol-0.4.6/PKG-INFO
+-rwxr-xr-x   0        0        0       18 2023-09-13 12:39:11.659921 simpledomcontrol-0.4.8/README.md
+-rwxr-xr-x   0        0        0     1082 2023-12-15 08:45:39.702665 simpledomcontrol-0.4.8/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.166975 simpledomcontrol-0.4.8/sdc_core/__init__.py
+-rwxr-xr-x   0        0        0       98 2023-09-21 08:45:54.656855 simpledomcontrol-0.4.8/sdc_core/apps.py
+-rw-r--r--   0        0        0    18645 2023-12-13 14:34:04.092799 simpledomcontrol-0.4.8/sdc_core/consumers.py
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/__init__.py
+-rw-r--r--   0        0        0      164 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      176 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.8/sdc_core/management/__pycache__/__init__.cpython-39.pyc
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/__init__.py
+-rw-r--r--   0        0        0      173 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      185 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      185 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/_private.cpython-39.pyc
+-rw-r--r--   0        0        0     3111 2023-11-16 20:41:41.244279 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-310.pyc
+-rw-r--r--   0        0        0     3235 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-39.pyc
+-rw-r--r--   0        0        0     3278 2023-11-15 14:57:12.955993 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_infos.cpython-310.pyc
+-rw-r--r--   0        0        0      967 2023-11-15 07:20:44.934088 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_url.cpython-310.pyc
+-rw-r--r--   0        0        0     2669 2023-11-07 13:16:56.062974 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_model_infos.cpython-310.pyc
+-rw-r--r--   0        0        0     2302 2023-11-24 09:37:56.060620 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-310.pyc
+-rw-r--r--   0        0        0     2368 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-39.pyc
+-rw-r--r--   0        0        0     2777 2023-11-16 20:24:39.232107 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-310.pyc
+-rw-r--r--   0        0        0     2785 2023-04-04 10:33:03.270414 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3134 2023-11-24 08:07:05.791278 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_links.cpython-310.pyc
+-rw-r--r--   0        0        0     2033 2023-09-21 08:46:16.872860 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-310.pyc
+-rw-r--r--   0        0        0     2048 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-39.pyc
+-rw-r--r--   0        0        0     5905 2023-03-31 13:46:19.184969 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-310.pyc
+-rw-r--r--   0        0        0     5940 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-39.pyc
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/_private.py
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__init__.py
+-rw-r--r--   0        0        0      182 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      194 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8592 2023-11-24 08:07:06.275254 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     8033 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     4225 2023-09-21 08:46:16.120859 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4205 2023-04-04 10:50:54.427002 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     1515 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-310.pyc
+-rw-r--r--   0        0        0     1545 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-39.pyc
+-rw-r--r--   0        0        0     1793 2023-09-21 08:46:13.508859 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     4789 2023-11-16 20:45:13.741182 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4479 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2641 2023-09-14 07:32:05.325796 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2665 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-39.pyc
+-rwxr-xr-x   0        0        0    11256 2023-11-24 06:39:15.995849 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_controller_manager.py
+-rw-r--r--   0        0        0     4591 2023-09-21 08:45:54.636855 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_model_manager.py
+-rwxr-xr-x   0        0        0     1217 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/options.py
+-rwxr-xr-x   0        0        0     1889 2023-09-21 08:45:54.644855 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/sdc_core_manager.py
+-rwxr-xr-x   0        0        0     4472 2023-11-16 20:45:12.821178 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/settings_manager.py
+-rwxr-xr-x   0        0        0     2157 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/utils.py
+-rwxr-xr-x   0        0        0     3251 2023-11-16 20:25:56.852389 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_cc.py
+-rw-r--r--   0        0        0     3694 2023-11-15 14:56:59.559480 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_infos.py
+-rw-r--r--   0        0        0      507 2023-11-15 07:20:42.554086 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_url.py
+-rw-r--r--   0        0        0     2665 2023-11-07 13:16:45.855370 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_model_infos.py
+-rwxr-xr-x   0        0        0     2711 2023-11-24 09:32:19.797721 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_init.py
+-rw-r--r--   0        0        0      703 2023-10-12 09:29:35.938805 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_is_installed.py
+-rwxr-xr-x   0        0        0     2642 2023-11-16 20:24:23.716052 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_new_model.py
+-rwxr-xr-x   0        0        0     3608 2023-11-24 06:25:48.207532 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_links.py
+-rwxr-xr-x   0        0        0     1933 2023-09-21 08:45:54.588855 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_url.py
+-rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__init__.py
+-rw-r--r--   0        0        0      165 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1322 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/forms.cpython-310.pyc
+-rw-r--r--   0        0        0      605 2023-11-15 08:32:34.682753 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/import_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     2508 2023-10-11 13:59:42.076794 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0        0        0     2201 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     1280 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/search.cpython-310.pyc
+-rw-r--r--   0        0        0     2597 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/views.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1174 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/forms.py
+-rwxr-xr-x   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/import_manager.py
+-rw-r--r--   0        0        0     2234 2023-10-11 13:59:37.053640 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/models.py
+-rwxr-xr-x   0        0        0     2458 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/response.py
+-rwxr-xr-x   0        0        0     1838 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/search.py
+-rwxr-xr-x   0        0        0     2380 2023-09-21 08:45:54.668855 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/views.py
+-rw-r--r--   0        0        0      107 2023-12-12 08:17:05.980843 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/.babelrc
+-rw-r--r--   0        0        0     4673 2023-12-15 08:40:53.567934 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/gulpfile.jsx
+-rwxr-xr-x   0        0        0      399 2023-12-12 12:31:17.861882 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/src/index.organizer.js
+-rw-r--r--   0        0        0      324 2023-11-24 09:54:39.300747 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/src/index.style.scss
+-rw-r--r--   0        0        0      429 2023-11-24 09:34:33.772197 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/tests/pre-test-setup.js
+-rw-r--r--   0        0        0      212 2023-12-12 12:31:17.893882 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/tests/test-setup.js
+-rw-r--r--   0        0        0     1139 2023-09-22 07:43:59.149945 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
+-rw-r--r--   0        0        0      432 2023-09-22 07:54:08.342934 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
+-rw-r--r--   0        0        0      677 2023-09-22 07:54:40.070948 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
+-rwxr-xr-x   0        0        0     1228 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
+-rwxr-xr-x   0        0        0     2464 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/index.html
+-rwxr-xr-x   0        0        0     2328 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/server_call.txt
+-rwxr-xr-x   0        0        0      895 2023-11-17 10:42:24.806725 simpledomcontrol-0.4.8/sdc_core/template_files/asgi.py.txt
+-rwxr-xr-x   0        0        0       82 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/controller/templade_view.html
+-rwxr-xr-x   0        0        0     1337 2023-12-12 12:31:17.885882 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_controller.js.txt
+-rwxr-xr-x   0        0        0       18 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_css.scss
+-rw-r--r--   0        0        0      535 2023-11-24 10:09:44.297249 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_test.js.text
+-rw-r--r--   0        0        0      278 2023-12-12 12:31:17.897882 simpledomcontrol-0.4.8/sdc_core/template_files/js_test.js.txt
+-rw-r--r--   0        0        0     1633 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/models/detail.html
+-rw-r--r--   0        0        0     2303 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/models/list.html
+-rwxr-xr-x   0        0        0     1635 2023-12-15 08:45:07.802861 simpledomcontrol-0.4.8/sdc_core/template_files/package.json
+-rwxr-xr-x   0        0        0      357 2023-09-21 08:45:54.596855 simpledomcontrol-0.4.8/sdc_core/template_files/routing.py.txt
+-rwxr-xr-x   0        0        0      149 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/sdc_urls.py.txt
+-rwxr-xr-x   0        0        0       90 2023-09-21 08:45:54.608855 simpledomcontrol-0.4.8/sdc_core/template_files/sdc_views.py.txt
+-rwxr-xr-x   0        0        0      936 2023-11-24 11:35:47.297156 simpledomcontrol-0.4.8/sdc_core/template_files/settings_extension.py.txt
+-rwxr-xr-x   0        0        0      989 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/templates/base.html
+-rwxr-xr-x   0        0        0      427 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/templates/index.html
+-rwxr-xr-x   0        0        0      289 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/urls.py.txt
+-rw-r--r--   0        0        0     2847 2023-12-12 12:31:17.821882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
+-rw-r--r--   0        0        0     1178 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
+-rw-r--r--   0        0        0     2454 2023-12-12 12:31:17.869882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
+-rw-r--r--   0        0        0     1833 2023-12-12 12:31:17.901882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
+-rw-r--r--   0        0        0       23 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
+-rw-r--r--   0        0        0     1318 2023-12-12 12:31:17.793882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
+-rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
+-rw-r--r--   0        0        0     3046 2023-12-13 13:46:40.556259 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
+-rw-r--r--   0        0        0      103 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
+-rw-r--r--   0        0        0     3267 2023-12-12 12:31:17.909881 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
+-rw-r--r--   0        0        0      180 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
+-rw-r--r--   0        0        0     1457 2023-12-12 12:31:17.829882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
+-rw-r--r--   0        0        0    20079 2023-12-13 15:05:52.501451 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
+-rw-r--r--   0        0        0     1019 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
+-rw-r--r--   0        0        0     4914 2023-12-12 12:31:17.837882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
+-rw-r--r--   0        0        0     2238 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
+-rw-r--r--   0        0        0     2819 2023-12-12 12:31:17.961881 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
+-rw-r--r--   0        0        0      668 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
+-rw-r--r--   0        0        0      364 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
+-rw-r--r--   0        0        0      462 2023-12-12 12:31:17.945881 simpledomcontrol-0.4.8/sdc_tools/Assets/tests/sdc_tools.test.js
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_tools/__init__.py
+-rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_tools/admin.py
+-rwxr-xr-x   0        0        0       97 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/apps.py
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/migrations/__init__.py
+-rw-r--r--   0        0        0      233 2023-09-14 07:34:03.056641 simpledomcontrol-0.4.8/sdc_tools/migrations/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       60 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/models.py
+-rwxr-xr-x   0        0        0      804 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/sdc_urls.py
+-rwxr-xr-x   0        0        0     1485 2023-09-21 08:45:54.640855 simpledomcontrol-0.4.8/sdc_tools/sdc_views.py
+-rwxr-xr-x   0        0        0     2110 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/elements/form.html
+-rwxr-xr-x   0        0        0     1866 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/elements/inline_form.html
+-rwxr-xr-x   0        0        0     1132 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/email/base.html
+-rw-r--r--   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
+-rw-r--r--   0        0        0       36 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
+-rw-r--r--   0        0        0      136 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
+-rw-r--r--   0        0        0       37 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
+-rw-r--r--   0        0        0      338 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
+-rwxr-xr-x   0        0        0      141 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
+-rw-r--r--   0        0        0      496 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
+-rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/__init__.py
+-rw-r--r--   0        0        0      164 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1061 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/addclass.cpython-310.pyc
+-rw-r--r--   0        0        0      667 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/indexfilter.cpython-310.pyc
+-rw-r--r--   0        0        0     1481 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/sdc_filter.cpython-310.pyc
+-rwxr-xr-x   0        0        0      825 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/addclass.py
+-rwxr-xr-x   0        0        0      357 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/indexfilter.py
+-rwxr-xr-x   0        0        0     1135 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/sdc_filter.py
+-rwxr-xr-x   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/tests.py
+-rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/views.py
+-rw-r--r--   0        0        0     1453 2023-12-12 12:31:17.865882 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
+-rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
+-rw-r--r--   0        0        0     1424 2023-12-12 12:31:17.797882 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
+-rw-r--r--   0        0        0       18 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
+-rw-r--r--   0        0        0      110 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
+-rw-r--r--   0        0        0       49 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
+-rw-r--r--   0        0        0      456 2023-12-12 12:31:17.813882 simpledomcontrol-0.4.8/sdc_user/Assets/tests/sdc_user.test.js
+-rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/__init__.py
+-rw-r--r--   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/admin.py
+-rw-r--r--   0        0        0      147 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/apps.py
+-rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/migrations/__init__.py
+-rw-r--r--   0        0        0      232 2023-09-14 07:34:03.060642 simpledomcontrol-0.4.8/sdc_user/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       57 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/models.py
+-rw-r--r--   0        0        0      304 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/sdc_urls.py
+-rw-r--r--   0        0        0     2140 2023-09-21 08:45:54.648855 simpledomcontrol-0.4.8/sdc_user/sdc_views.py
+-rw-r--r--   0        0        0      401 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/templates/sdc_user/sdc/sdc_login.html
+-rw-r--r--   0        0        0      327 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/templates/sdc_user/sdc/sdc_logout.html
+-rw-r--r--   0        0        0       60 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/tests.py
+-rw-r--r--   0        0        0       63 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/views.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 simpledomcontrol-0.4.8/PKG-INFO
```

### Comparing `simpledomcontrol-0.4.6/pyproject.toml` & `simpledomcontrol-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimpleDomControl"
-version = "0.4.6"
+version = "0.4.8"
 authors = [ "Martin Starman <private@martin-starman.com>", ]
 description = "Simple DOM control -> a django MVC framework"
 readme = "README.md"
 license = 'Apache License 2.0'
 
 packages = [{include = "sdc_core"}, {include = "sdc_user"}, {include = "sdc_tools"}]
 keywords = ["django", "MVC",]
```

### Comparing `simpledomcontrol-0.4.6/sdc_core/consumers.py` & `simpledomcontrol-0.4.8/sdc_core/consumers.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_cc.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_cc.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_controller_infos.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_infos.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_controller_url.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_get_model_infos.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_model_infos.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_init.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_init.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_links.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_links.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/options.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/options.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/utils.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/__pycache__/utils.cpython-39.pyc` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/add_controller_manager.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_controller_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/add_model_manager.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_model_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/options.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/options.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/sdc_core_manager.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/sdc_core_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/settings_manager.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/settings_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/init_add/utils.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/utils.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_cc.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_cc.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_get_controller_infos.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_infos.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_get_model_infos.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_model_infos.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_init.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_init.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_is_installed.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_is_installed.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_new_model.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_new_model.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_update_links.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_links.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/management/commands/sdc_update_url.py` & `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_url.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/forms.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/forms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/import_manager.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/import_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/models.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/response.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/search.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/search.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/__pycache__/views.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/forms.py` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/forms.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/models.py` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/models.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/response.py` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/response.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/search.py` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/search.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/sdc_extentions/views.py` & `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/Assets/gulpfile.jsx` & `simpledomcontrol-0.4.8/sdc_core/template_files/Assets/gulpfile.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx` & `simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx` & `simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt` & `simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/index.html` & `simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/index.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/apps/sdc_examples/server_call.txt` & `simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/server_call.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/asgi.py.txt` & `simpledomcontrol-0.4.8/sdc_core/template_files/asgi.py.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/controller/template_controller.js.txt` & `simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_controller.js.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/controller/template_test.js.text` & `simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_test.js.text`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/models/detail.html` & `simpledomcontrol-0.4.8/sdc_core/template_files/models/detail.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/models/list.html` & `simpledomcontrol-0.4.8/sdc_core/template_files/models/list.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/package.json` & `simpledomcontrol-0.4.8/sdc_core/template_files/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'dependencies'": "{'sdc_client': '^0.3.8'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "",
     "dependencies": {
         "bootstrap": "^5.3.2",
         "jquery": "^3.7.1",
         "lodash": "^4.17.21",
-        "sdc_client": "^0.3.7"
+        "sdc_client": "^0.3.8"
     },
     "description": "",
     "devDependencies": {
         "@babel/core": "^7.23.3",
         "@babel/preset-react": "^7.23.3",
         "@babel/register": "^7.22.15",
         "babel-jest": "^29.7.0",
```

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/settings_extension.py.txt` & `simpledomcontrol-0.4.8/sdc_core/template_files/settings_extension.py.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_core/template_files/templates/base.html` & `simpledomcontrol-0.4.8/sdc_core/template_files/templates/base.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js` & `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/sdc_urls.py` & `simpledomcontrol-0.4.8/sdc_tools/sdc_urls.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/sdc_views.py` & `simpledomcontrol-0.4.8/sdc_tools/sdc_views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templates/elements/form.html` & `simpledomcontrol-0.4.8/sdc_tools/templates/elements/form.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templates/elements/inline_form.html` & `simpledomcontrol-0.4.8/sdc_tools/templates/elements/inline_form.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templates/email/base.html` & `simpledomcontrol-0.4.8/sdc_tools/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/addclass.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/addclass.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/indexfilter.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/indexfilter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templatetags/__pycache__/sdc_filter.cpython-310.pyc` & `simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/sdc_filter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templatetags/addclass.py` & `simpledomcontrol-0.4.8/sdc_tools/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_tools/templatetags/sdc_filter.py` & `simpledomcontrol-0.4.8/sdc_tools/templatetags/sdc_filter.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js` & `simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js` & `simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/sdc_user/sdc_views.py` & `simpledomcontrol-0.4.8/sdc_user/sdc_views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.6/PKG-INFO` & `simpledomcontrol-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpledomcontrol
-Version: 0.4.6
+Version: 0.4.8
 Summary: Simple DOM control -> a django MVC framework
 Home-page: https://github.com/StarmanMartin/sdc
 License: Apache-2.0
 Keywords: django,MVC
 Author: Martin Starman
 Author-email: private@martin-starman.com
 Requires-Python: >=3.9,<4.0
```

