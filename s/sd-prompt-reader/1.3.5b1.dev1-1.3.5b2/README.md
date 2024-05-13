# Comparing `tmp/sd_prompt_reader-1.3.5b1.dev1.tar.gz` & `tmp/sd_prompt_reader-1.3.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_prompt_reader-1.3.5b1.dev1.tar", max compression
+gzip compressed data, was "sd_prompt_reader-1.3.5b2.tar", max compression
```

## Comparing `sd_prompt_reader-1.3.5b1.dev1.tar` & `sd_prompt_reader-1.3.5b2.tar`

### file list

```diff
@@ -1,86 +1,77 @@
--rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.5b1.dev1/LICENSE
--rw-r--r--   0        0        0    16866 2024-04-30 16:03:46.478493 sd_prompt_reader-1.3.5b1.dev1/README.md
--rw-r--r--   0        0        0     1038 2024-04-30 17:30:43.564510 sd_prompt_reader-1.3.5b1.dev1/pyproject.toml
--rw-r--r--   0        0        0    10244 2024-04-30 17:28:30.413726 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/.DS_Store
--rw-r--r--   0        0        0      119 2023-09-11 15:13:17.041022 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/__init__.py
--rw-r--r--   0        0        0       25 2024-04-30 17:36:25.240898 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/__version__.py
--rw-r--r--   0        0        0    33371 2024-04-24 20:33:49.648741 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/app.py
--rw-r--r--   0        0        0     4464 2023-09-30 12:48:42.979786 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/button.py
--rw-r--r--   0        0        0    12797 2024-04-30 17:33:37.852795 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/cli.py
--rw-r--r--   0        0        0     4997 2024-03-21 13:25:50.368703 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/constants.py
--rw-r--r--   0        0        0      374 2023-09-11 15:13:17.044406 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/ctkdnd.py
--rw-r--r--   0        0        0     6148 2024-04-25 20:30:42.459491 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/.DS_Store
--rw-r--r--   0        0        0      404 2024-03-21 13:25:50.369729 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__init__.py
--rw-r--r--   0        0        0      856 2024-03-21 13:26:30.452091 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6324 2024-03-21 15:43:43.619025 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/a1111.cpython-311.pyc
--rw-r--r--   0        0        0     5475 2024-04-24 20:23:00.680145 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/base_format.cpython-311.pyc
--rw-r--r--   0        0        0    23302 2024-04-24 20:31:35.569124 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/comfyui.cpython-311.pyc
--rw-r--r--   0        0        0     2713 2024-03-21 13:26:30.470550 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/drawthings.cpython-311.pyc
--rw-r--r--   0        0        0     4959 2024-03-21 13:26:30.460509 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/easydiffusion.cpython-311.pyc
--rw-r--r--   0        0        0     3184 2024-03-21 13:26:30.473931 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/fooocus.cpython-311.pyc
--rw-r--r--   0        0        0    10740 2024-04-30 10:39:44.586436 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/invokeai.cpython-311.pyc
--rw-r--r--   0        0        0     8920 2024-04-30 15:51:34.852164 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/novelai.cpython-311.pyc
--rw-r--r--   0        0        0     3766 2024-03-21 13:26:30.472344 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/__pycache__/swarmui.cpython-311.pyc
--rw-r--r--   0        0        0     4208 2024-03-21 15:43:32.269504 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/a1111.py
--rw-r--r--   0        0        0     2601 2024-04-23 19:14:30.193953 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/base_format.py
--rw-r--r--   0        0        0    20917 2024-04-24 20:26:31.436939 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/comfyui.py
--rw-r--r--   0        0        0     1004 2024-03-21 13:25:50.372554 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/drawthings.py
--rw-r--r--   0        0        0     2738 2024-03-21 13:25:50.373098 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/easydiffusion.py
--rw-r--r--   0        0        0     1402 2024-03-21 13:25:50.373744 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/fooocus.py
--rw-r--r--   0        0        0     6178 2024-04-25 09:51:40.283772 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/invokeai.py
--rw-r--r--   0        0        0     4464 2024-04-30 15:51:30.127491 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/novelai.py
--rw-r--r--   0        0        0     1876 2024-03-21 13:25:50.375371 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/swarmui.py
--rw-r--r--   0        0        0    13157 2024-04-30 15:51:30.109283 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/image_data_reader.py
--rw-r--r--   0        0        0     2401 2024-04-23 19:14:30.194590 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/logger.py
--rw-r--r--   0        0        0     6126 2023-09-30 23:12:04.290329 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/parameter_viewer.py
--rw-r--r--   0        0        0    19582 2023-09-30 12:48:42.987332 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/prompt_viewer.py
--rw-r--r--   0        0        0     6148 2023-09-20 15:11:02.029930 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/.DS_Store
--rw-r--r--   0        0        0      119 2023-09-11 15:13:17.048711 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/__init__.py
--rw-r--r--   0        0        0      334 2023-09-11 15:22:09.298003 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3239 2023-08-29 22:10:08.112057 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/check_circle_24.png
--rw-r--r--   0        0        0     2076 2023-08-29 22:10:08.112671 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/check_circle_24_alpha.png
--rw-r--r--   0        0        0     1293 2023-08-29 22:10:08.113243 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/cleaning_services_24.png
--rw-r--r--   0        0        0     1036 2023-08-29 22:10:08.113737 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/cleaning_services_24_alpha.png
--rw-r--r--   0        0        0      602 2023-08-29 22:10:08.114163 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_20.png
--rw-r--r--   0        0        0      550 2023-08-29 22:10:08.114647 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_20_alpha.png
--rw-r--r--   0        0        0      739 2023-08-29 22:10:08.115173 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_24.png
--rw-r--r--   0        0        0      621 2023-08-29 22:10:08.115591 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_24_alpha.png
--rw-r--r--   0        0        0      751 2023-08-29 22:10:08.116121 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/description_24.png
--rw-r--r--   0        0        0      637 2023-08-29 22:10:08.116635 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/description_24_alpha.png
--rw-r--r--   0        0        0     1226 2023-08-29 22:10:08.117090 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_24.png
--rw-r--r--   0        0        0      905 2023-08-29 22:10:08.117558 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_24_alpha.png
--rw-r--r--   0        0        0     2016 2023-08-29 22:10:08.117987 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_off_24.png
--rw-r--r--   0        0        0     1368 2023-08-29 22:10:08.118427 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_off_24_alpha.png
--rw-r--r--   0        0        0     3062 2023-08-29 22:10:08.118883 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/error_24.png
--rw-r--r--   0        0        0     1964 2023-08-29 22:10:08.119345 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/error_24_alpha.png
--rw-r--r--   0        0        0      589 2023-08-29 22:10:08.119873 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/expand_more_24.png
--rw-r--r--   0        0        0      585 2023-08-29 22:10:08.120398 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/expand_more_24_alpha.png
--rw-r--r--   0        0        0     4510 2023-08-29 22:10:08.120632 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/gray.json
--rw-r--r--   0        0        0  1377264 2023-08-29 22:10:08.128049 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/icon.icns
--rw-r--r--   0        0        0   612157 2023-08-29 22:10:08.132165 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/icon.ico
--rw-r--r--   0        0        0   810239 2023-08-29 22:10:08.136339 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/icon.png
--rw-r--r--   0        0        0     3042 2023-08-29 22:10:08.136928 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/info_24.png
--rw-r--r--   0        0        0     1966 2023-08-29 22:10:08.137427 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/info_24_alpha.png
--rw-r--r--   0        0        0     1683 2023-08-29 22:10:08.138125 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/lightbulb_20.png
--rw-r--r--   0        0        0     1453 2023-08-29 22:10:08.138711 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/lightbulb_20_alpha.png
--rw-r--r--   0        0        0     1426 2023-08-29 22:10:08.139223 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/mop_24.png
--rw-r--r--   0        0        0     1109 2023-08-29 22:10:08.139580 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/mop_24_alpha.png
--rw-r--r--   0        0        0     1740 2023-08-29 22:10:08.139870 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/place_item_48.png
--rw-r--r--   0        0        0     1334 2023-08-29 22:10:08.140198 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/place_item_48_alpha.png
--rw-r--r--   0        0        0     1241 2023-08-29 22:10:08.140544 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/save_24.png
--rw-r--r--   0        0        0      946 2023-08-29 22:10:08.140887 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/save_24_alpha.png
--rw-r--r--   0        0        0     1619 2023-08-29 22:10:08.141189 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/sort_by_alpha_20.png
--rw-r--r--   0        0        0     1377 2023-08-29 22:10:08.141490 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
--rw-r--r--   0        0        0     2732 2023-08-29 22:10:08.141811 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/update_24.png
--rw-r--r--   0        0        0     1937 2023-08-29 22:10:08.142161 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/update_24_alpha.png
--rw-r--r--   0        0        0      632 2023-09-11 15:13:17.048912 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_sidebar_20.png
--rw-r--r--   0        0        0      615 2023-09-11 15:13:17.049108 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_sidebar_20_alpha.png
--rw-r--r--   0        0        0      560 2023-09-11 15:13:17.049302 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_week_20.png
--rw-r--r--   0        0        0      545 2023-09-11 15:13:17.049498 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_week_20_alpha.png
--rw-r--r--   0        0        0     2258 2023-08-29 22:10:08.144127 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/warning_24.png
--rw-r--r--   0        0        0     1658 2023-08-29 22:10:08.144441 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/warning_24_alpha.png
--rw-r--r--   0        0        0     2917 2024-03-21 13:25:50.376674 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/status_bar.py
--rw-r--r--   0        0        0     3985 2023-09-30 12:48:42.988373 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/textbox.py
--rw-r--r--   0        0        0     1171 2024-03-21 13:25:50.377123 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/update_checker.py
--rw-r--r--   0        0        0     4323 2024-03-21 13:25:50.377815 sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/utility.py
--rw-r--r--   0        0        0    17811 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.5b1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-09 14:16:43.184257 sd_prompt_reader-1.3.5b2/LICENSE
+-rw-r--r--   0        0        0    17363 2024-05-10 13:39:30.045211 sd_prompt_reader-1.3.5b2/README.md
+-rw-r--r--   0        0        0     1444 2024-05-13 12:11:42.728951 sd_prompt_reader-1.3.5b2/pyproject.toml
+-rw-r--r--   0        0        0    10244 2024-05-10 13:09:59.850225 sd_prompt_reader-1.3.5b2/sd_prompt_reader/.DS_Store
+-rw-r--r--   0        0        0      119 2023-09-11 15:13:17.041022 sd_prompt_reader-1.3.5b2/sd_prompt_reader/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-13 12:10:24.963140 sd_prompt_reader-1.3.5b2/sd_prompt_reader/__version__.py
+-rw-r--r--   0        0        0    33472 2024-05-10 13:27:30.272606 sd_prompt_reader-1.3.5b2/sd_prompt_reader/app.py
+-rw-r--r--   0        0        0     4464 2023-09-30 12:48:42.979786 sd_prompt_reader-1.3.5b2/sd_prompt_reader/button.py
+-rw-r--r--   0        0        0    12797 2024-04-30 17:33:37.852795 sd_prompt_reader-1.3.5b2/sd_prompt_reader/cli.py
+-rw-r--r--   0        0        0     5054 2024-05-10 13:07:21.765463 sd_prompt_reader-1.3.5b2/sd_prompt_reader/constants.py
+-rw-r--r--   0        0        0      374 2023-09-11 15:13:17.044406 sd_prompt_reader-1.3.5b2/sd_prompt_reader/ctkdnd.py
+-rw-r--r--   0        0        0     6148 2024-05-05 18:00:15.193918 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/.DS_Store
+-rw-r--r--   0        0        0      404 2024-03-21 13:25:50.369729 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/__init__.py
+-rw-r--r--   0        0        0     4208 2024-03-21 15:43:32.269504 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/a1111.py
+-rw-r--r--   0        0        0     2601 2024-04-23 19:14:30.193953 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/base_format.py
+-rw-r--r--   0        0        0    21405 2024-05-05 16:41:33.743134 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/comfyui.py
+-rw-r--r--   0        0        0     1004 2024-03-21 13:25:50.372554 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/drawthings.py
+-rw-r--r--   0        0        0     2738 2024-03-21 13:25:50.373098 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/easydiffusion.py
+-rw-r--r--   0        0        0     1402 2024-03-21 13:25:50.373744 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/fooocus.py
+-rw-r--r--   0        0        0     6178 2024-04-25 09:51:40.283772 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/invokeai.py
+-rw-r--r--   0        0        0     4464 2024-05-07 18:20:18.870275 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/novelai.py
+-rw-r--r--   0        0        0     1876 2024-03-21 13:25:50.375371 sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/swarmui.py
+-rw-r--r--   0        0        0    13968 2024-05-07 18:19:35.093912 sd_prompt_reader-1.3.5b2/sd_prompt_reader/image_data_reader.py
+-rw-r--r--   0        0        0     2401 2024-04-23 19:14:30.194590 sd_prompt_reader-1.3.5b2/sd_prompt_reader/logger.py
+-rw-r--r--   0        0        0     6126 2024-05-07 17:14:09.040147 sd_prompt_reader-1.3.5b2/sd_prompt_reader/parameter_viewer.py
+-rw-r--r--   0        0        0    19582 2023-09-30 12:48:42.987332 sd_prompt_reader-1.3.5b2/sd_prompt_reader/prompt_viewer.py
+-rw-r--r--   0        0        0     6148 2023-09-20 15:11:02.029930 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/.DS_Store
+-rw-r--r--   0        0        0      119 2023-09-11 15:13:17.048711 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/__init__.py
+-rw-r--r--   0        0        0     3239 2023-08-29 22:10:08.112057 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/check_circle_24.png
+-rw-r--r--   0        0        0     2076 2023-08-29 22:10:08.112671 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/check_circle_24_alpha.png
+-rw-r--r--   0        0        0     1293 2023-08-29 22:10:08.113243 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/cleaning_services_24.png
+-rw-r--r--   0        0        0     1036 2023-08-29 22:10:08.113737 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/cleaning_services_24_alpha.png
+-rw-r--r--   0        0        0      602 2023-08-29 22:10:08.114163 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_20.png
+-rw-r--r--   0        0        0      550 2023-08-29 22:10:08.114647 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_20_alpha.png
+-rw-r--r--   0        0        0      739 2023-08-29 22:10:08.115173 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_24.png
+-rw-r--r--   0        0        0      621 2023-08-29 22:10:08.115591 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_24_alpha.png
+-rw-r--r--   0        0        0      751 2023-08-29 22:10:08.116121 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/description_24.png
+-rw-r--r--   0        0        0      637 2023-08-29 22:10:08.116635 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/description_24_alpha.png
+-rw-r--r--   0        0        0     1226 2023-08-29 22:10:08.117090 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_24.png
+-rw-r--r--   0        0        0      905 2023-08-29 22:10:08.117558 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_24_alpha.png
+-rw-r--r--   0        0        0     2016 2023-08-29 22:10:08.117987 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_off_24.png
+-rw-r--r--   0        0        0     1368 2023-08-29 22:10:08.118427 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_off_24_alpha.png
+-rw-r--r--   0        0        0     3062 2023-08-29 22:10:08.118883 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/error_24.png
+-rw-r--r--   0        0        0     1964 2023-08-29 22:10:08.119345 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/error_24_alpha.png
+-rw-r--r--   0        0        0      589 2023-08-29 22:10:08.119873 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/expand_more_24.png
+-rw-r--r--   0        0        0      585 2023-08-29 22:10:08.120398 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/expand_more_24_alpha.png
+-rw-r--r--   0        0        0     4510 2023-08-29 22:10:08.120632 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/gray.json
+-rw-r--r--   0        0        0   529564 2024-05-09 12:03:50.257473 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/icon-cli.ico
+-rw-r--r--   0        0        0   757699 2024-05-09 12:01:19.547764 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/icon-cube.png
+-rw-r--r--   0        0        0   636668 2024-05-09 12:03:26.284448 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/icon-gui.ico
+-rw-r--r--   0        0        0  1286854 2024-05-10 13:02:27.795579 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/icon.icns
+-rw-r--r--   0        0        0   765111 2024-05-10 13:02:09.389546 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/icon.png
+-rw-r--r--   0        0        0     3042 2023-08-29 22:10:08.136928 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/info_24.png
+-rw-r--r--   0        0        0     1966 2023-08-29 22:10:08.137427 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/info_24_alpha.png
+-rw-r--r--   0        0        0     1683 2023-08-29 22:10:08.138125 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/lightbulb_20.png
+-rw-r--r--   0        0        0     1453 2023-08-29 22:10:08.138711 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/lightbulb_20_alpha.png
+-rw-r--r--   0        0        0     1426 2023-08-29 22:10:08.139223 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/mop_24.png
+-rw-r--r--   0        0        0     1109 2023-08-29 22:10:08.139580 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/mop_24_alpha.png
+-rw-r--r--   0        0        0     1740 2023-08-29 22:10:08.139870 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/place_item_48.png
+-rw-r--r--   0        0        0     1334 2023-08-29 22:10:08.140198 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/place_item_48_alpha.png
+-rw-r--r--   0        0        0     1241 2023-08-29 22:10:08.140544 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/save_24.png
+-rw-r--r--   0        0        0      946 2023-08-29 22:10:08.140887 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/save_24_alpha.png
+-rw-r--r--   0        0        0     1619 2023-08-29 22:10:08.141189 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/sort_by_alpha_20.png
+-rw-r--r--   0        0        0     1377 2023-08-29 22:10:08.141490 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png
+-rw-r--r--   0        0        0     2732 2023-08-29 22:10:08.141811 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/update_24.png
+-rw-r--r--   0        0        0     1937 2023-08-29 22:10:08.142161 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/update_24_alpha.png
+-rw-r--r--   0        0        0      632 2023-09-11 15:13:17.048912 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_sidebar_20.png
+-rw-r--r--   0        0        0      615 2023-09-11 15:13:17.049108 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_sidebar_20_alpha.png
+-rw-r--r--   0        0        0      560 2023-09-11 15:13:17.049302 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_week_20.png
+-rw-r--r--   0        0        0      545 2023-09-11 15:13:17.049498 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_week_20_alpha.png
+-rw-r--r--   0        0        0     2258 2023-08-29 22:10:08.144127 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/warning_24.png
+-rw-r--r--   0        0        0     1658 2023-08-29 22:10:08.144441 sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/warning_24_alpha.png
+-rw-r--r--   0        0        0     2917 2024-03-21 13:25:50.376674 sd_prompt_reader-1.3.5b2/sd_prompt_reader/status_bar.py
+-rw-r--r--   0        0        0     3985 2023-09-30 12:48:42.988373 sd_prompt_reader-1.3.5b2/sd_prompt_reader/textbox.py
+-rw-r--r--   0        0        0     1171 2024-03-21 13:25:50.377123 sd_prompt_reader-1.3.5b2/sd_prompt_reader/update_checker.py
+-rw-r--r--   0        0        0     4323 2024-03-21 13:25:50.377815 sd_prompt_reader-1.3.5b2/sd_prompt_reader/utility.py
+-rw-r--r--   0        0        0    18862 1970-01-01 00:00:00.000000 sd_prompt_reader-1.3.5b2/PKG-INFO
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/LICENSE` & `sd_prompt_reader-1.3.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/README.md` & `sd_prompt_reader-1.3.5b2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-    <img alt="icon" src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/sd_prompt_reader/resources/icon.png" width=20% height=20%>
+    <img alt="icon" src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/sd_prompt_reader/resources/icon-cube.png" width=20% height=20%>
     <h1>Stable Diffusion Prompt Reader</h1>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest">
         <img alt="GitHub releases" src="https://img.shields.io/github/downloads/receyuki/stable-diffusion-prompt-reader/total"></a>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/blob/master/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/github/license/receyuki/stable-diffusion-prompt-reader"></a>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest">
         <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/receyuki/stable-diffusion-prompt-reader"></a>
@@ -19,28 +19,30 @@
 A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
     <br>
   <p>
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
-    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
     <a href="#cli">CLI</a> •
+    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
     <a href="#api">API</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
     <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v134.png">
 </div>
 
->The SD Prompt Reader is now available as a ComfyUI node. Check out 
->the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) for more information.
+> [!TIP]
+> The SD Prompt Reader is now available as a ComfyUI node. Check out 
+> the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) for more information.
 
 ## Features
 - Support macOS, Windows and Linux.
+- Provides both GUI and CLI
 - Simple drag and drop interaction.
 - Copy prompt to clipboard.
 - Remove prompt from image.
 - Export prompt to text file.
 - Edit or import prompt to images
 - Vertical orientation display and sorting by alphabet
 - Detect generation tool.
@@ -51,31 +53,33 @@
 |                                                                                        | PNG | JPEG | WEBP | TXT* |
 |----------------------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
 | [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui)               |  ✅  |  ✅   |  ✅   |  ✅   |
 | [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)                       |  ✅  |  ✅   |  ✅   |      |
 | [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*                        |  ✅  |  ✅   |      |      |
 | [StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* |  ✅  |  ✅   |      |      |
 | [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*                             |  ✅  |  ✅   |      |      |
+| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |  ✅   |      |
+| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
 | [InvokeAI](https://github.com/invoke-ai/InvokeAI)                                      |  ✅  |      |      |      |
 | [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI)              |  ✅  |      |      |      |
 | [InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI)                      |  ✅  |      |      |      |
 | [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                                  |  ✅  |      |      |      |
 | [Draw Things](https://drawthings.ai/)                                                  |  ✅  |      |      |      |
-| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |      |      |
-| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
 | Naifu(4chan)                                                                           |  ✅  |      |      |      |
 
 \* Limitations apply. See [format limitations](#TXT).
 
-If you are using a tool or format that is not on this list, please help me to support your format 
-by uploading the original file generated by your tool to the issues, thx.
-
-For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
-The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a subproject 
-of this project, and it is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+> [!NOTE]
+> If you are using a tool or format that is not on this list, please help me to support your format 
+> by uploading the original file generated by your tool to the issues, thx.
+
+> [!TIP]
+> For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
+> The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a subproject 
+> of this project, and it is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
 
 ## Download
 ### For Windows users
 Download executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
 ### For macOS users
 Download executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
 #### Install via Homebrew Cask
@@ -135,15 +139,18 @@
 ### Remove prompt from image
 - Click "Clear" will generate a new image file with suffix "_data_removed" alongside the original image file.
 - To save to another location, click the expand arrow and click "select directory".
 - To overwrite the original image file, click the expand arrow and click "overwrite the original image".  
 ![remove](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/remove.png)
 
 ### Edit image
-***Please note that the edited image will be written in A1111 format, it meaning that image in any format will become A1111 format after editing.***
+> [!NOTE]
+> The edited image will be written in A1111 format, meaning that image in any format 
+> will become A1111 format after editing.
+
 - Click "Edit" to enter edit mode.
 - Edit the prompt directly in the textbox or import a metadata file in txt format.
 - Click "Save" will generate a edited image file with suffix "_edited" alongside the original image file.
 - To save to another location, click the expand arrow and click "select directory".
 - To overwrite the original image file, click the expand arrow and click "overwrite the original image".  
 ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/save.png)
 
@@ -165,24 +172,37 @@
 | Face restoration        | --restore_faces      |
 
 - Click the expand arrow and click "single line prompt".
 - Paste it into the textbox below the webui script "Prompts from file or textbox".  
 ![single line prompt](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/single_line_prompt.png)
 
 ### ComfyUI SDXL workflow
-***The SDXL workflow does not support editing. 
-If necessary, please remove prompts from image before edit.***  
+> [!NOTE]
+> The SDXL workflow does not support editing. 
+> If necessary, please remove prompts from image before edit. 
+
 If the image's workflow includes multiple sets of SDXL prompts, 
 namely Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt display mode as shown in the image below. 
 There are two interface options available for the multi-set prompt display mode, and you can switch between them using buttons.  
 ![comfyui_sdxl.png](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png)
 
 ## CLI
 A CLI tool for reading, modifying, and clearing metadata is provided. 
-In order to use the CLI tool, please [install SD Prompt Reader via pip](#for-linux-users-not-regularly-tested).
+### Platforms
+#### For Windows users
+`SD Prompt Reader CLI.exe` will be placed in the zip package as a separate executable.   
+Examples:
+`"SD Prompt Reader CLI.exe" -i example.png`  
+#### For macOS users
+The executable is located at `SD Prompt Reader.app/Contents/MacOS/SD Prompt Reader`.  
+Examples:
+`/Applications/SD\ Prompt\ Reader.app/Contents/MacOS/SD\ Prompt\ Reader -i example.png`  
+#### For pip users
+Examples:
+`sd-prompt-reader-cli -i example.png`
 ### Modes and Options
 #### Modes
 - Read Mode: Activated by `-r` or `--read` flag.
 - Write Mode: Activated by `-w` or `--write` flag.
 - Clear Mode: Activated by `-c` or `--clear` flag.
 #### General Options
 - `-i`, `--input-path`: Path to the input image file or directory containing image files, required parameter.
@@ -239,40 +259,45 @@
 ```
 
 ## Format Limitations
 ### TXT
 1. Importing txt file is only allowed in edit mode.
 2. Only A1111 format txt files are supported. You can use txt files generated by the A1111 webui or use the SD prompt reader to export txt from A1111 images
 ### StableSwarmUI
-StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
+> [!IMPORTANT]
+> StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
 ### ComfyUI
-1. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
-This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
-It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
-2. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
-3. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
+> [!IMPORTANT]
+> When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
+> This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
+> It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+
+1. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
+2. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
 (e.g. output hires. fixed image and original image simultaneously in a single flowchart)
 SD Prompt Reader will traverse all flowcharts and branches and display the longest branch with complete input and output.  
-4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
+3. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
 ### Easy Diffusion
 By default, Easy Diffusion does not write metadata to images. Please change the _Metadata format_ in settings to _embed_ to write the metadata to images
 ### Fooocus-MRE
 Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support writing metadata to image files, 
 SD Prompt Reader only supports images generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE).
 
 ## FAQ
 ### Malware Alert
-The false positive reported by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a common issue for _pyinstaller_ users. 
-I spent a lot of time trying to fix the Windows Defender false positive before, but I couldn't do it for every antivirus software. 
-So, you can either trust Windows Defender or use the instruction for Linux users to use this app.
+> [!WARNING]
+> The false positive reported by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a common issue for _pyinstaller_ users. 
+> I spent a lot of time trying to fix the Windows Defender false positive before, but I couldn't do it for every antivirus software. 
+> So, you can either trust Windows Defender or use the instruction for Linux users to use this app.
 ### "SD Prompt Reader.app" is damaged and can't be opened. You should move it to the Trash
-This is a very common macOS issue when you run unsigned non-appstore apps, 
-and developers must pay $99 per year to Apple to eliminate this issue. 
-You can choose to **Allow Apps from Anywhere** in **security & privacy** settings which can be dangerous. 
-The way I prefer is to remove the quarantine attributes. 
+> [!IMPORTANT]
+> This is a very common macOS issue when you run unsigned non-appstore apps, 
+> and developers must pay $99 per year to Apple to eliminate this issue. 
+> You can choose to **Allow Apps from Anywhere** in **security & privacy** settings which can be dangerous. 
+> The way I prefer is to remove the quarantine attributes. 
 1. Open Terminal from the Applications folder. 
 2. Type in the following command and hit Enter. 
 
     `xattr -r -d com.apple.quarantine /path/to/app.app`
 
     In my case it's
```

#### html2text {}

```diff
@@ -3,55 +3,56 @@
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_s_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:
                                _b_l_a_c_k_][platform]
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
     reading prompt from Stable Diffusion generated image outside the webui.
-_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_o_m_f_y_U_I_ _N_o_d_e â¢ _C_L_I
+_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_L_I â¢ _C_o_m_f_y_U_I_ _N_o_d_e
                           â¢ _A_P_I â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
                              screenshot_v134.png]
->The SD Prompt Reader is now available as a ComfyUI node. Check out >the
-[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
-node) for more information. ## Features - Support macOS, Windows and Linux. -
-Simple drag and drop interaction. - Copy prompt to clipboard. - Remove prompt
-from image. - Export prompt to text file. - Edit or import prompt to images -
-Vertical orientation display and sorting by alphabet - Detect generation tool.
-- Multiple formats support. - Dark and light mode support. ## Supported Formats
-| | PNG | JPEG | WEBP | TXT* | |-----------------------------------------------
------------------------------------------|:---:|:----:|:----:|:----:| |
-[A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â
-| â | â | â | | [Easy Diffusion](https://github.com/easydiffusion/
-easydiffusion) | â | â | â | | | [StableSwarmUI](https://github.com/
-Stability-AI/StableSwarmUI)* | â | â | | | | [StableSwarmUI (prior to
-0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* | â | â | | |
-| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)* | â | â | | |
-| [InvokeAI](https://github.com/invoke-ai/InvokeAI) | â | | | | | [InvokeAI
-(prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI) | â | | | | |
-[InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI) | â | | | |
-| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)* | â | | | | | [Draw
-Things](https://drawthings.ai/) | â | | | | | [NovelAI (stealth pnginfo)]
-(https://novelai.net/) | â | | | | | [NovelAI (legacy)](https://novelai.net/
+> [!TIP] > The SD Prompt Reader is now available as a ComfyUI node. Check out >
+the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-
+reader-node) for more information. ## Features - Support macOS, Windows and
+Linux. - Provides both GUI and CLI - Simple drag and drop interaction. - Copy
+prompt to clipboard. - Remove prompt from image. - Export prompt to text file.
+- Edit or import prompt to images - Vertical orientation display and sorting by
+alphabet - Detect generation tool. - Multiple formats support. - Dark and light
+mode support. ## Supported Formats | | PNG | JPEG | WEBP | TXT* | |------------
+----------------------------------------------------------------------------|:-
+--:|:----:|:----:|:----:| | [A1111's webUI](https://github.com/AUTOMATIC1111/
+stable-diffusion-webui) | â | â | â | â | | [Easy Diffusion](https://
+github.com/easydiffusion/easydiffusion) | â | â | â | | | [StableSwarmUI]
+(https://github.com/Stability-AI/StableSwarmUI)* | â | â | | | |
+[StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/
+StableSwarmUI)* | â | â | | | | [Fooocus-MRE](https://github.com/
+MoonRide303/Fooocus-MRE)* | â | â | | | | [NovelAI (stealth pnginfo)]
+(https://novelai.net/) | â | | â | | | [NovelAI (legacy)](https://
+novelai.net/) | â | | | | | [InvokeAI](https://github.com/invoke-ai/InvokeAI)
+| â | | | | | [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-
+ai/InvokeAI) | â | | | | | [InvokeAI (prior to 1.15)](https://github.com/
+invoke-ai/InvokeAI) | â | | | | | [ComfyUI](https://github.com/
+comfyanonymous/ComfyUI)* | â | | | | | [Draw Things](https://drawthings.ai/
 ) | â | | | | | Naifu(4chan) | â | | | | \* Limitations apply. See [format
-limitations](#TXT). If you are using a tool or format that is not on this list,
-please help me to support your format by uploading the original file generated
-by your tool to the issues, thx. For ComfyUI users, the SD Prompt Reader is now
-available as a ComfyUI node. The [ComfyUI Prompt Reader Node](https://
-github.com/receyuki/comfyui-prompt-reader-node) is a subproject of this
-project, and it is recommended to embed the [Prompt Saver node](https://
-github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
-receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
-compatibility. ## Download ### For Windows users Download executable from
-[GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/
-releases/latest) ### For macOS users Download executable from [GitHub Releases]
-(https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
-#### Install via Homebrew Cask You may also install SD Prompt Reader via
-[Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
+limitations](#TXT). > [!NOTE] > If you are using a tool or format that is not
+on this list, please help me to support your format > by uploading the original
+file generated by your tool to the issues, thx. > [!TIP] > For ComfyUI users,
+the SD Prompt Reader is now available as a ComfyUI node. > The [ComfyUI Prompt
+Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a
+subproject > of this project, and it is recommended to embed the [Prompt Saver
+node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node-
+-parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://
+github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure
+maximum compatibility. ## Download ### For Windows users Download executable
+from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-
+reader/releases/latest) ### For macOS users Download executable from [GitHub
+Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/
+latest) #### Install via Homebrew Cask You may also install SD Prompt Reader
+via [Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
 receyuki/sd-prompt-reader/sd-prompt-reader ``` The parameter `--no-quarantine`
 is used since the SD Prompt Reader is currently unsigned as I mentioned [here]
 (https://github.com/receyuki/stable-diffusion-prompt-reader#sd-prompt-
 readerapp-is-damaged-and-cant-be-opened-you-should-move-it-to-the-trash) ###
 For Linux users (not regularly tested) ~~I'm pretty sure linux users can figure
 things out without an executable.~~ - The minimum version of Python required is
 3.10 - Make sure you have the tkinter package installed in your Python. If not,
@@ -72,64 +73,68 @@
 arrow and click "select directory". ![export](https://github.com/receyuki/
 stable-diffusion-prompt-reader/raw/master/images/export.png) ### Remove prompt
 from image - Click "Clear" will generate a new image file with suffix
 "_data_removed" alongside the original image file. - To save to another
 location, click the expand arrow and click "select directory". - To overwrite
 the original image file, click the expand arrow and click "overwrite the
 original image". ![remove](https://github.com/receyuki/stable-diffusion-prompt-
-reader/raw/master/images/remove.png) ### Edit image ***Please note that the
-edited image will be written in A1111 format, it meaning that image in any
-format will become A1111 format after editing.*** - Click "Edit" to enter edit
-mode. - Edit the prompt directly in the textbox or import a metadata file in
-txt format. - Click "Save" will generate a edited image file with suffix
-"_edited" alongside the original image file. - To save to another location,
-click the expand arrow and click "select directory". - To overwrite the
-original image file, click the expand arrow and click "overwrite the original
-image". ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/
-master/images/save.png) ### Copy as single line prompt Copy image prompt and
-setting in a format that can be read by [Prompts from file or textbox](https://
-github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Features#prompts-from-
-file-or-textbox) The following parameters are supported: | Setting | Parameter
-| |-------------------------|----------------------| | Seed | --seed | |
-Variation seed strength | --subseed_strength | | Seed resize from | --
-seed_resize_from_h | | Seed resize from | --seed_resize_from_w | | Sampler | --
-sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | | Size | --width
-| | Size | --height | | Face restoration | --restore_faces | - Click the expand
-arrow and click "single line prompt". - Paste it into the textbox below the
-webui script "Prompts from file or textbox". ![single line prompt](https://
-github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
-single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow does not
-support editing. If necessary, please remove prompts from image before edit.***
-If the image's workflow includes multiple sets of SDXL prompts, namely Clip G
-(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the
-multi-set prompt display mode as shown in the image below. There are two
-interface options available for the multi-set prompt display mode, and you can
-switch between them using buttons. ![comfyui_sdxl.png](https://github.com/
-receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ##
-CLI A CLI tool for reading, modifying, and clearing metadata is provided. In
-order to use the CLI tool, please [install SD Prompt Reader via pip](#for-
-linux-users-not-regularly-tested). ### Modes and Options #### Modes - Read
-Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated by `-w` or `-
--write` flag. - Clear Mode: Activated by `-c` or `--clear` flag. #### General
-Options - `-i`, `--input-path`: Path to the input image file or directory
-containing image files, required parameter. - `-o`, `--output-path`: Path to
-the output file or directory where the processed files will be saved. - `-l`,
-`--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
-#### Read Options - `-f`, `--format-type`: Specifies the output metadata
-format, choices are "TXT" or "JSON". Default format is "TXT" #### Write Options
-- `-m`, `--metadata`: Provides a metadata file for writing. - `-p`, `--
-positive`: Provides a positive prompt string for writing. - `-n`, `--negative`:
-Provides a negative prompt string for writing. - `-s`, `--setting`: Provides a
-setting string for writing. ### Basic Usage - If no output path is specified,
-the modified image will be saved in the current directory with a suffix added
-to the original filename. - To overwrite the source file, set the output path
-equal to the input path. - The write mode only supports modifications to a
-single image. #### Read Mode - Read metadata from an image. - Usage: `sd-
-prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-prompt-
-reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
+reader/raw/master/images/remove.png) ### Edit image > [!NOTE] > The edited
+image will be written in A1111 format, meaning that image in any format > will
+become A1111 format after editing. - Click "Edit" to enter edit mode. - Edit
+the prompt directly in the textbox or import a metadata file in txt format. -
+Click "Save" will generate a edited image file with suffix "_edited" alongside
+the original image file. - To save to another location, click the expand arrow
+and click "select directory". - To overwrite the original image file, click the
+expand arrow and click "overwrite the original image". ![save](https://
+github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/save.png)
+### Copy as single line prompt Copy image prompt and setting in a format that
+can be read by [Prompts from file or textbox](https://github.com/AUTOMATIC1111/
+stable-diffusion-webui/wiki/Features#prompts-from-file-or-textbox) The
+following parameters are supported: | Setting | Parameter | |------------------
+-------|----------------------| | Seed | --seed | | Variation seed strength | -
+-subseed_strength | | Seed resize from | --seed_resize_from_h | | Seed resize
+from | --seed_resize_from_w | | Sampler | --sampler_name | | Steps | --steps |
+| CFG scale | --cfg_scale | | Size | --width | | Size | --height | | Face
+restoration | --restore_faces | - Click the expand arrow and click "single line
+prompt". - Paste it into the textbox below the webui script "Prompts from file
+or textbox". ![single line prompt](https://github.com/receyuki/stable-
+diffusion-prompt-reader/raw/master/images/single_line_prompt.png) ### ComfyUI
+SDXL workflow > [!NOTE] > The SDXL workflow does not support editing. > If
+necessary, please remove prompts from image before edit. If the image's
+workflow includes multiple sets of SDXL prompts, namely Clip G(text_g), Clip L
+(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt
+display mode as shown in the image below. There are two interface options
+available for the multi-set prompt display mode, and you can switch between
+them using buttons. ![comfyui_sdxl.png](https://github.com/receyuki/stable-
+diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ## CLI A CLI tool
+for reading, modifying, and clearing metadata is provided. ### Platforms ####
+For Windows users `SD Prompt Reader CLI.exe` will be placed in the zip package
+as a separate executable. Examples: `"SD Prompt Reader CLI.exe" -i example.png`
+#### For macOS users The executable is located at `SD Prompt Reader.app/
+Contents/MacOS/SD Prompt Reader`. Examples: `/Applications/SD\ Prompt\
+Reader.app/Contents/MacOS/SD\ Prompt\ Reader -i example.png` #### For pip users
+Examples: `sd-prompt-reader-cli -i example.png` ### Modes and Options ####
+Modes - Read Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated
+by `-w` or `--write` flag. - Clear Mode: Activated by `-c` or `--clear` flag.
+#### General Options - `-i`, `--input-path`: Path to the input image file or
+directory containing image files, required parameter. - `-o`, `--output-path`:
+Path to the output file or directory where the processed files will be saved. -
+`-l`, `--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN,
+ERROR). #### Read Options - `-f`, `--format-type`: Specifies the output
+metadata format, choices are "TXT" or "JSON". Default format is "TXT" ####
+Write Options - `-m`, `--metadata`: Provides a metadata file for writing. - `-
+p`, `--positive`: Provides a positive prompt string for writing. - `-n`, `--
+negative`: Provides a negative prompt string for writing. - `-s`, `--setting`:
+Provides a setting string for writing. ### Basic Usage - If no output path is
+specified, the modified image will be saved in the current directory with a
+suffix added to the original filename. - To overwrite the source file, set the
+output path equal to the input path. - The write mode only supports
+modifications to a single image. #### Read Mode - Read metadata from an image.
+- Usage: `sd-prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-
+prompt-reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
 o metadata.txt` `sd-prompt-reader-cli -r -i example.png -f TXT -
 o output_folder/` `sd-prompt-reader-cli -r -i input_folder/ -f JSON -
 o output_folder/` #### Write Mode - Write metadata to an image. - Usage: `sd-
 prompt-reader-cli -w -i -m [-o ]` - Examples: `sd-prompt-reader-cli -w -
 i example.png -m new_metadata.txt` `sd-prompt-reader-cli -w -i example.png -
 m new_metadata.txt -o output.png` `sd-prompt-reader-cli -w -i example.png -
 m new_metadata.json -o output_folder/` #### Clear Mode - Remove all metadata
@@ -138,51 +143,52 @@
 o output.png` `sd-prompt-reader-cli -c -i example.png -o output_folder/` `sd-
 prompt-reader-cli -c -i input_folder/ -o output_folder/` ## API ```Python from
 sd_prompt_reader.image_data_reader import ImageDataReader with open(image_path,
 "rb+") as f: image_metadata = ImageDataReader(f) # WIP ``` ## Format
 Limitations ### TXT 1. Importing txt file is only allowed in edit mode. 2. Only
 A1111 format txt files are supported. You can use txt files generated by the
 A1111 webui or use the SD prompt reader to export txt from A1111 images ###
-StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its format
-may change in the future. I will keep track of upcoming updates of
-StableSwarmUI. ### ComfyUI 1. When custom nodes are used or when the workflow
-becomes overly complex, there is a high probability that metadata may not be
-correctly read. This is because ComfyUI does not store metadata but only the
-complete workflow. SD Prompt Reader can only handle basic workflows. It is
-recommended to embed the [Prompt Saver node](https://github.com/receyuki/
-comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the
-[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
-node) within your workflow to ensure maximum compatibility. 2. If there are
-multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means
-that there are multiple KSampler nodes in the flowchart. 3. Due to the nature
-of ComfyUI, all nodes and flowcharts in the workflow are stored in the image,
-including those that are not being used. Also, a flowchart can have multiple
-branches, inputs and outputs. (e.g. output hires. fixed image and original
-image simultaneously in a single flowchart) SD Prompt Reader will traverse all
-flowcharts and branches and display the longest branch with complete input and
-output. 4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-
-diffusion-prompt-reader#comfyui-sdxl-workflow) ### Easy Diffusion By default,
-Easy Diffusion does not write metadata to images. Please change the _Metadata
-format_ in settings to _embed_ to write the metadata to images ### Fooocus-MRE
-Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus)
-does not support writing metadata to image files, SD Prompt Reader only
-supports images generated by [Fooocus MoonRide Edition](https://github.com/
-MoonRide303/Fooocus-MRE). ## FAQ ### Malware Alert The false positive reported
-by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a
-common issue for _pyinstaller_ users. I spent a lot of time trying to fix the
-Windows Defender false positive before, but I couldn't do it for every
-antivirus software. So, you can either trust Windows Defender or use the
-instruction for Linux users to use this app. ### "SD Prompt Reader.app" is
-damaged and can't be opened. You should move it to the Trash This is a very
-common macOS issue when you run unsigned non-appstore apps, and developers must
-pay $99 per year to Apple to eliminate this issue. You can choose to **Allow
-Apps from Anywhere** in **security & privacy** settings which can be dangerous.
-The way I prefer is to remove the quarantine attributes. 1. Open Terminal from
-the Applications folder. 2. Type in the following command and hit Enter. `xattr
--r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
+StableSwarmUI > [!IMPORTANT] > StableSwarmUI is still in the Alpha testing
+phase, and its format may change in the future. I will keep track of upcoming
+updates of StableSwarmUI. ### ComfyUI > [!IMPORTANT] > When custom nodes are
+used or when the workflow becomes overly complex, there is a high probability
+that metadata may not be correctly read. > This is because ComfyUI does not
+store metadata but only the complete workflow. SD Prompt Reader can only handle
+basic workflows. > It is recommended to embed the [Prompt Saver node](https://
+github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
+generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
+receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
+compatibility. 1. If there are multiple sets of data (seed, steps, CFG, etc.)
+in the setting box, this means that there are multiple KSampler nodes in the
+flowchart. 2. Due to the nature of ComfyUI, all nodes and flowcharts in the
+workflow are stored in the image, including those that are not being used.
+Also, a flowchart can have multiple branches, inputs and outputs. (e.g. output
+hires. fixed image and original image simultaneously in a single flowchart) SD
+Prompt Reader will traverse all flowcharts and branches and display the longest
+branch with complete input and output. 3. [ComfyUI SDXL workflow](https://
+github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow) ###
+Easy Diffusion By default, Easy Diffusion does not write metadata to images.
+Please change the _Metadata format_ in settings to _embed_ to write the
+metadata to images ### Fooocus-MRE Since the original version of [Fooocus]
+(https://github.com/lllyasviel/Fooocus) does not support writing metadata to
+image files, SD Prompt Reader only supports images generated by [Fooocus
+MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE). ## FAQ ###
+Malware Alert > [!WARNING] > The false positive reported by some anti-malwares
+is caused by the packaging tool _pyinstaller_ which is a common issue for
+_pyinstaller_ users. > I spent a lot of time trying to fix the Windows Defender
+false positive before, but I couldn't do it for every antivirus software. > So,
+you can either trust Windows Defender or use the instruction for Linux users to
+use this app. ### "SD Prompt Reader.app" is damaged and can't be opened. You
+should move it to the Trash > [!IMPORTANT] > This is a very common macOS issue
+when you run unsigned non-appstore apps, > and developers must pay $99 per year
+to Apple to eliminate this issue. > You can choose to **Allow Apps from
+Anywhere** in **security & privacy** settings which can be dangerous. > The way
+I prefer is to remove the quarantine attributes. 1. Open Terminal from the
+Applications folder. 2. Type in the following command and hit Enter. `xattr -
+r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
 d com.apple.quarantine /Applications/SD\ Prompt\ Reader.app` If you are still
 concerned about the security of the app you can use the instruction for Linux
 users to use this app. ## TODO - Batch image processing tool - Gallery/Folder
 view - User preference ## Credits - Inspired by [Stable Diffusion web UI]
 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/) - App icon generated
 using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-
 AppIconsModelforSD) - Special thanks to [Azusachan](https://github.com/
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/pyproject.toml` & `sd_prompt_reader-1.3.5b2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sd-prompt-reader"
-version = "1.3.5b1.dev1"
+version = "1.3.5b2"
 description = "A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui."
 authors = ["receyuki <receyuki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 repository = "https://github.com/receyuki/stable-diffusion-prompt-reader"
 documentation = "https://github.com/receyuki/stable-diffusion-prompt-reader"
@@ -17,14 +17,26 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/receyuki/stable-diffusion-prompt-reader/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
+pillow = "10.3.0"
+tkinterdnd2-universal = ">=1.7.3,<1.8.0"
+pyperclip = ">=1.8.2,<1.9.0"
+customtkinter = ">=5.2.2,<5.3.0"
+pyobjus = {version = ">=1.2.3,<1.3.0", platform = "darwin"}
+pyobjc-framework-cocoa = {version = "10.2", platform = "darwin"}
+piexif = ">=1.1.3,<1.2.0"
+pefile = ">=2023.2.7,<2023.3.0"
+requests = ">=2.31.0,<2.32.0"
+toml = ">=0.10.2,<0.11.0"
+ctktooltip = ">=0.8,<1.0"
+click = ">=8.1.7,<8.2.0"
 
 [tool.poetry.scripts]
 sd-prompt-reader = "sd_prompt_reader.app:main"
 sd-prompt-reader-cli = "sd_prompt_reader.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/.DS_Store` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -253,184 +253,184 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0011 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0002 cb27 0000 000b 005f 005f 0070  .....'....._._.p
+00001030: 0000 0003 06c2 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 b22c 9c38  moDDblob.....,.8
-00001060: a4f0 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 1ea8 f41c  moDDblob........
+00001060: 54f5 c541 0000 000b 005f 005f 0070 0079  T..A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 b22c 9c38 a4f0  dDblob.....,.8..
+00001080: 6444 626c 6f62 0000 0008 1ea8 f41c 54f5  dDblob........T.
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0003 6000 0000 0006  comp......`.....
+000010b0: 636f 6d70 0000 0000 0003 a000 0000 0006  comp............
 000010c0: 0066 006f 0072 006d 0061 0074 6c67 3153  .f.o.r.m.a.tlg1S
-000010d0: 636f 6d70 0000 0000 0001 dd43 0000 0006  comp.......C....
+000010d0: 636f 6d70 0000 0000 0001 e206 0000 0006  comp............
 000010e0: 0066 006f 0072 006d 0061 0074 6d6f 4444  .f.o.r.m.a.tmoDD
-000010f0: 626c 6f62 0000 0008 3e54 1081 a5f0 c541  blob....>T.....A
+000010f0: 626c 6f62 0000 0008 0e68 6f31 54f5 c541  blob.....ho1T..A
 00001100: 0000 0006 0066 006f 0072 006d 0061 0074  .....f.o.r.m.a.t
-00001110: 6d6f 6444 626c 6f62 0000 0008 380f 23f4  modDblob....8.#.
-00001120: 82f0 c541 0000 0006 0066 006f 0072 006d  ...A.....f.o.r.m
+00001110: 6d6f 6444 626c 6f62 0000 0008 0e68 6f31  modDblob.....ho1
+00001120: 54f5 c541 0000 0006 0066 006f 0072 006d  T..A.....f.o.r.m
 00001130: 0061 0074 7068 3153 636f 6d70 0000 0000  .a.tph1Scomp....
 00001140: 0002 a000 0000 0009 0072 0065 0073 006f  .........r.e.s.o
 00001150: 0075 0072 0063 0065 0073 6277 7370 626c  .u.r.c.e.sbwspbl
-00001160: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
-00001170: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00001160: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
+00001170: 0203 0405 0607 0808 080b 085d 5368 6f77  ...........]Show
 00001180: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00001190: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000011a0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000011b0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 000011c0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000011d0: 7208 0908 095f 1018 7b7b 3433 362c 2035  r...._..{{436, 5
-000011e0: 3135 7d2c 207b 3932 302c 2034 3336 7d7d  15}, {920, 436}}
-000011f0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-00001200: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-00001210: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-00001220: 0009 0072 0065 0073 006f 0075 0072 0063  ...r.e.s.o.u.r.c
-00001230: 0065 0073 6963 7670 626c 6f62 0000 01be  .e.sicvpblob....
-00001240: 6270 6c69 7374 3030 df10 1001 0203 0405  bplist00........
-00001250: 0607 0809 0a0b 0c0d 0e0f 1011 1213 1114  ................
-00001260: 1115 1615 1718 1519 1a1a 1c5f 1013 6261  ..........._..ba
-00001270: 636b 6772 6f75 6e64 436f 6c6f 7242 6c75  ckgroundColorBlu
-00001280: 6558 6963 6f6e 5369 7a65 5874 6578 7453  eXiconSizeXtextS
-00001290: 697a 655f 1012 6261 636b 6772 6f75 6e64  ize_..background
-000012a0: 436f 6c6f 7252 6564 5e62 6163 6b67 726f  ColorRed^backgro
-000012b0: 756e 6454 7970 655f 1014 6261 636b 6772  undType_..backgr
-000012c0: 6f75 6e64 436f 6c6f 7247 7265 656e 5b67  oundColorGreen[g
-000012d0: 7269 644f 6666 7365 7458 5f10 0f73 6372  ridOffsetX_..scr
-000012e0: 6f6c 6c50 6f73 6974 696f 6e59 5b67 7269  ollPositionY[gri
-000012f0: 644f 6666 7365 7459 5c73 686f 7749 7465  dOffsetY\showIte
-00001300: 6d49 6e66 6f5f 1012 7669 6577 4f70 7469  mInfo_..viewOpti
-00001310: 6f6e 7356 6572 7369 6f6e 5f10 0f73 6372  onsVersion_..scr
-00001320: 6f6c 6c50 6f73 6974 696f 6e58 5961 7272  ollPositionXYarr
-00001330: 616e 6765 4279 5d6c 6162 656c 4f6e 426f  angeBy]labelOnBo
-00001340: 7474 6f6d 5f10 0f73 686f 7749 636f 6e50  ttom_..showIconP
-00001350: 7265 7669 6577 5b67 7269 6453 7061 6369  review[gridSpaci
-00001360: 6e67 233f f000 0000 0000 0023 4050 0000  ng#?.......#@P..
-00001370: 0000 0000 2340 2800 0000 0000 0010 0023  ....#@(........#
-00001380: 0000 0000 0000 0000 2340 7990 0000 0000  ........#@y.....
-00001390: 0008 1001 546e 616d 6509 0923 404b 0000  ....Tname..#@K..
-000013a0: 0000 0000 0008 002b 0041 004a 0053 0068  .......+.A.J.S.h
-000013b0: 0077 008e 009a 00ac 00b8 00c5 00da 00ec  .w..............
-000013c0: 00f6 0104 0116 0122 012b 0134 013d 013f  .......".+.4.=.?
-000013d0: 0148 0151 0152 0154 0159 015a 015b 0000  .H.Q.R.T.Y.Z.[..
-000013e0: 0000 0000 0201 0000 0000 0000 001d 0000  ................
-000013f0: 0000 0000 0000 0000 0000 0000 0164 0000  .............d..
-00001400: 0009 0072 0065 0073 006f 0075 0072 0063  ...r.e.s.o.u.r.c
-00001410: 0065 0073 6c67 3153 636f 6d70 0000 0000  .e.slg1Scomp....
-00001420: 002b b31f 0000 0009 0072 0065 0073 006f  .+.......r.e.s.o
-00001430: 0075 0072 0063 0065 0073 6c73 7643 626c  .u.r.c.e.slsvCbl
-00001440: 6f62 0000 0324 6270 6c69 7374 3030 da01  ob...$bplist00..
-00001450: 0203 0405 0607 0809 0a0b 0b0d 0b54 5554  .............TUT
-00001460: 5657 585f 1010 7573 6552 656c 6174 6976  VWX_..useRelativ
-00001470: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
-00001480: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00001490: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-000014a0: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
-000014b0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
-000014c0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-000014d0: 585a 736f 7274 436f 6c75 6d6e 5869 636f  XZsortColumnXico
-000014e0: 6e53 697a 655f 1012 7669 6577 4f70 7469  nSize_..viewOpti
-000014f0: 6f6e 7356 6572 7369 6f6e 0909 ae0e 171c  onsVersion......
-00001500: 2125 2a2f 3439 3e42 464b 4fd4 0f10 1112  !%*/49>BFKO.....
-00001510: 1314 0b0b 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00001520: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00001530: 7669 7369 626c 6554 6e61 6d65 1101 9909  visibleTname....
-00001540: 09d4 0f10 1112 1819 1a1a 5875 6269 7175  ..........Xubiqu
-00001550: 6974 7910 2308 08d4 1211 100f 0b1a 1f20  ity.#.......... 
-00001560: 0908 10b0 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00001570: 64d4 1211 100f 1a1a 1f24 0808 5b64 6174  d........$..[dat
-00001580: 6543 7265 6174 6564 d40f 1011 1226 271a  eCreated.....&'.
-00001590: 0b54 7369 7a65 1061 0809 d40f 1011 122b  .Tsize.a.......+
-000015a0: 2c0b 0b54 6b69 6e64 1073 0909 d40f 1011  ,..Tkind.s......
-000015b0: 1230 310b 1a55 6c61 6265 6c10 6409 08d4  .01..Ulabel.d...
-000015c0: 0f10 1112 3536 0b1a 5776 6572 7369 6f6e  ....56..Wversion
-000015d0: 104b 0908 d40f 1011 123a 3b0b 1a58 636f  .K.......:;..Xco
-000015e0: 6d6d 656e 7473 1101 2c09 08d4 1211 100f  mments..,.......
-000015f0: 1a1a 1f41 0808 5e64 6174 654c 6173 744f  ...A..^dateLastO
-00001600: 7065 6e65 64d4 1211 100f 1a1a 1f45 0808  pened........E..
-00001610: 5964 6174 6541 6464 6564 d412 1110 0f1a  YdateAdded......
-00001620: 1a49 4a08 0810 d25a 7368 6172 654f 776e  .IJ....ZshareOwn
-00001630: 6572 d412 1110 0f1a 1a49 4e08 085f 100f  er.......IN.._..
-00001640: 7368 6172 654c 6173 7445 6469 746f 72d4  shareLastEditor.
-00001650: 1211 100f 1a1a 4952 0808 5f10 1069 6e76  ......IR.._..inv
-00001660: 6974 6174 696f 6e53 7461 7475 7309 2300  itationStatus.#.
-00001670: 0000 0000 0000 0023 4028 0000 0000 0000  .......#@(......
-00001680: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
-00001690: 0000 0000 0000 1001 0008 001d 0030 0042  .............0.B
-000016a0: 004a 005e 0070 0079 008b 0096 009f 00b4  .J.^.p.y........
-000016b0: 00b5 00b6 00c5 00ce 00d9 00df 00e9 00f1  ................
-000016c0: 00f6 00f9 00fa 00fb 0104 010d 010f 0110  ................
-000016d0: 0111 011a 011b 011c 011e 012b 0134 0135  ...........+.4.5
-000016e0: 0136 0142 014b 0150 0152 0153 0154 015d  .6.B.K.P.R.S.T.]
-000016f0: 0162 0164 0165 0166 016f 0175 0177 0178  .b.d.e.f.o.u.w.x
-00001700: 0179 0182 018a 018c 018d 018e 0197 01a0  .y..............
-00001710: 01a3 01a4 01a5 01ae 01af 01b0 01bf 01c8  ................
-00001720: 01c9 01ca 01d4 01dd 01de 01df 01e1 01ec  ................
-00001730: 01f5 01f6 01f7 0209 0212 0213 0214 0227  ...............'
-00001740: 0228 0231 023a 0247 0250 0000 0000 0000  .(.1.:.G.P......
-00001750: 0201 0000 0000 0000 0059 0000 0000 0000  .........Y......
-00001760: 0000 0000 0000 0000 0252 0000 0009 0072  .........R.....r
-00001770: 0065 0073 006f 0075 0072 0063 0065 0073  .e.s.o.u.r.c.e.s
-00001780: 6c73 7670 626c 6f62 0000 0299 6270 6c69  lsvpblob....bpli
-00001790: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-000017a0: 0b0d 0b47 4847 494a 355f 1010 7573 6552  ...GHGIJ5_..useR
-000017b0: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-000017c0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000017d0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000017e0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-000017f0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-00001800: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-00001810: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-00001820: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
-00001830: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00001840: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-00001850: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
-00001860: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
-00001870: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
-00001880: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
-00001890: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
-000018a0: 6e65 64d4 1819 1a1b 1c1d 0b1f 5776 6973  ned.........Wvis
-000018b0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000018c0: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-000018d0: 07d4 1819 1a1b 1c22 0b24 0810 6409 1005  .......".$..d...
-000018e0: d418 191a 1b1c 270b 2908 104b 0910 06d4  ......'.)..K....
-000018f0: 1b1a 1918 2b1c 2d1c 1002 0810 b008 d418  ....+.-.........
-00001900: 191a 1b0b 311c 3309 1061 0810 03d4 1b1a  ....1.3..a......
-00001910: 1918 351c 2d0b 1001 0809 d418 191a 1b0b  ..5.-...........
-00001920: 3a0b 3c09 1073 0910 04d4 1819 1a1b 0b3f  :.<..s.........?
-00001930: 0b41 0911 0199 0910 00d4 1b1a 1918 431c  .A............C.
-00001940: 2d1c 1008 0808 0923 0000 0000 0000 0000  -......#........
+000011d0: 7208 0909 095f 1019 7b7b 3331 352c 2034  r...._..{{315, 4
+000011e0: 3337 7d2c 207b 3130 3938 2c20 3532 317d  37}, {1098, 521}
+000011f0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
+00001200: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+00001210: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
+00001220: 0000 0900 7200 6500 7300 6f00 7500 7200  ....r.e.s.o.u.r.
+00001230: 6300 6500 7369 6376 7062 6c6f 6200 0001  c.e.sicvpblob...
+00001240: be62 706c 6973 7430 30df 1010 0102 0304  .bplist00.......
+00001250: 0506 0708 090a 0b0c 0d0e 0f10 1112 1311  ................
+00001260: 1411 1516 1517 1815 191a 1a1c 5f10 1362  ............_..b
+00001270: 6163 6b67 726f 756e 6443 6f6c 6f72 426c  ackgroundColorBl
+00001280: 7565 5869 636f 6e53 697a 6558 7465 7874  ueXiconSizeXtext
+00001290: 5369 7a65 5f10 1262 6163 6b67 726f 756e  Size_..backgroun
+000012a0: 6443 6f6c 6f72 5265 645e 6261 636b 6772  dColorRed^backgr
+000012b0: 6f75 6e64 5479 7065 5f10 1462 6163 6b67  oundType_..backg
+000012c0: 726f 756e 6443 6f6c 6f72 4772 6565 6e5b  roundColorGreen[
+000012d0: 6772 6964 4f66 6673 6574 585f 100f 7363  gridOffsetX_..sc
+000012e0: 726f 6c6c 506f 7369 7469 6f6e 595b 6772  rollPositionY[gr
+000012f0: 6964 4f66 6673 6574 595c 7368 6f77 4974  idOffsetY\showIt
+00001300: 656d 496e 666f 5f10 1276 6965 774f 7074  emInfo_..viewOpt
+00001310: 696f 6e73 5665 7273 696f 6e5f 100f 7363  ionsVersion_..sc
+00001320: 726f 6c6c 506f 7369 7469 6f6e 5859 6172  rollPositionXYar
+00001330: 7261 6e67 6542 795d 6c61 6265 6c4f 6e42  rangeBy]labelOnB
+00001340: 6f74 746f 6d5f 100f 7368 6f77 4963 6f6e  ottom_..showIcon
+00001350: 5072 6576 6965 775b 6772 6964 5370 6163  Preview[gridSpac
+00001360: 696e 6723 3ff0 0000 0000 0000 2340 5000  ing#?.......#@P.
+00001370: 0000 0000 0023 4028 0000 0000 0000 1000  .....#@(........
+00001380: 2300 0000 0000 0000 0023 4079 9000 0000  #........#@y....
+00001390: 0000 0810 0154 6e61 6d65 0909 2340 4b00  .....Tname..#@K.
+000013a0: 0000 0000 0000 0800 2b00 4100 4a00 5300  ........+.A.J.S.
+000013b0: 6800 7700 8e00 9a00 ac00 b800 c500 da00  h.w.............
+000013c0: ec00 f601 0401 1601 2201 2b01 3401 3d01  ........".+.4.=.
+000013d0: 3f01 4801 5101 5201 5401 5901 5a01 5b00  ?.H.Q.R.T.Y.Z.[.
+000013e0: 0000 0000 0002 0100 0000 0000 0000 1d00  ................
+000013f0: 0000 0000 0000 0000 0000 0000 0001 6400  ..............d.
+00001400: 0000 0900 7200 6500 7300 6f00 7500 7200  ....r.e.s.o.u.r.
+00001410: 6300 6500 736c 6731 5363 6f6d 7000 0000  c.e.slg1Scomp...
+00001420: 0000 3da5 cb00 0000 0900 7200 6500 7300  ..=.......r.e.s.
+00001430: 6f00 7500 7200 6300 6500 736c 7376 4362  o.u.r.c.e.slsvCb
+00001440: 6c6f 6200 0003 2462 706c 6973 7430 30da  lob...$bplist00.
+00001450: 0102 0304 0506 0708 090a 0b0c 0d0c 5455  ..............TU
+00001460: 5456 570c 5f10 1276 6965 774f 7074 696f  TVW._..viewOptio
+00001470: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00001480: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00001490: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+000014a0: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
+000014b0: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
+000014c0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
+000014d0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e58  ionXZsortColumnX
+000014e0: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
+000014f0: 6c61 7469 7665 4461 7465 7310 0109 ae0e  lativeDates.....
+00001500: 171c 2125 2a2f 3439 3e42 464b 4fd4 0f10  ..!%*/49>BFKO...
+00001510: 1112 0c14 0c16 5776 6973 6962 6c65 5577  ......WvisibleUw
+00001520: 6964 7468 5961 7363 656e 6469 6e67 5a69  idthYascendingZi
+00001530: 6465 6e74 6966 6965 7209 1101 9909 546e  dentifier.....Tn
+00001540: 616d 65d4 0f10 1112 1819 181b 0810 2308  ame...........#.
+00001550: 5875 6269 7175 6974 79d4 1211 100f 1d18  Xubiquity.......
+00001560: 1f0c 5c64 6174 654d 6f64 6966 6965 6408  ..\dateModified.
+00001570: 10b0 09d4 1211 100f 2218 1f18 5b64 6174  ........"...[dat
+00001580: 6543 7265 6174 6564 0808 d40f 1011 120c  eCreated........
+00001590: 2718 2909 1061 0854 7369 7a65 d40f 1011  '.)..a.Tsize....
+000015a0: 120c 2c0c 2e09 1073 0954 6b69 6e64 d40f  ..,....s.Tkind..
+000015b0: 1011 1218 310c 3308 1064 0955 6c61 6265  ....1.3..d.Ulabe
+000015c0: 6cd4 0f10 1112 1836 0c38 0810 4b09 5776  l......6.8..K.Wv
+000015d0: 6572 7369 6f6e d40f 1011 1218 3b0c 3d08  ersion......;.=.
+000015e0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 1211  ..,.Xcomments...
+000015f0: 100f 3f18 1f18 5e64 6174 654c 6173 744f  ..?...^dateLastO
+00001600: 7065 6e65 6408 08d4 1211 100f 4318 1f18  pened.......C...
+00001610: 5964 6174 6541 6464 6564 0808 d412 1110  YdateAdded......
+00001620: 0f47 1849 185a 7368 6172 654f 776e 6572  .G.I.ZshareOwner
+00001630: 0810 d208 d412 1110 0f4c 1849 185f 100f  .........L.I._..
+00001640: 7368 6172 654c 6173 7445 6469 746f 7208  shareLastEditor.
+00001650: 08d4 1211 100f 5018 4918 5f10 1069 6e76  ......P.I._..inv
+00001660: 6974 6174 696f 6e53 7461 7475 7308 0809  itationStatus...
+00001670: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
+00001680: 0000 5c64 6174 654d 6f64 6966 6965 6423  ..\dateModified#
+00001690: 4030 0000 0000 0000 0900 0800 1d00 3200  @0............2.
+000016a0: 4400 4c00 6000 7200 7b00 8d00 9800 a100  D.L.`.r.{.......
+000016b0: b400 b600 b700 c600 cf00 d700 dd00 e700  ................
+000016c0: f200 f300 f600 f700 fc01 0501 0601 0801  ................
+000016d0: 0901 1201 1b01 2801 2901 2b01 2c01 3501  ......(.).+.,.5.
+000016e0: 4101 4201 4301 4c01 4d01 4f01 5001 5501  A.B.C.L.M.O.P.U.
+000016f0: 5e01 5f01 6101 6201 6701 7001 7101 7301  ^._.a.b.g.p.q.s.
+00001700: 7401 7a01 8301 8401 8601 8701 8f01 9801  t.z.............
+00001710: 9901 9c01 9d01 a601 af01 be01 bf01 c001  ................
+00001720: c901 d301 d401 d501 de01 e901 ea01 ec01  ................
+00001730: ed01 f602 0802 0902 0a02 1302 2602 2702  ............&.'.
+00001740: 2802 2902 3202 3b02 4802 5100 0000 0000  (.).2.;.H.Q.....
+00001750: 0002 0100 0000 0000 0000 5900 0000 0000  ..........Y.....
+00001760: 0000 0000 0000 0000 0002 5200 0000 0900  ..........R.....
+00001770: 7200 6500 7300 6f00 7500 7200 6300 6500  r.e.s.o.u.r.c.e.
+00001780: 736c 7376 7062 6c6f 6200 0002 9962 706c  slsvpblob....bpl
+00001790: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
+000017a0: 0b0c 0d0c 4647 4648 490c 5f10 1276 6965  ....FGFHI._..vie
+000017b0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+000017c0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+000017d0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+000017e0: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
+000017f0: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
+00001800: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
+00001810: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
+00001820: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
+00001830: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+00001840: 7310 0109 d90e 0f10 1112 1314 1516 1720  s.............. 
+00001850: 252a 2f34 373c 4158 636f 6d6d 656e 7473  %*/47<AXcomments
+00001860: 556c 6162 656c 5776 6572 7369 6f6e 5b64  UlabelWversion[d
+00001870: 6174 6543 7265 6174 6564 5473 697a 655c  ateCreatedTsize\
+00001880: 6461 7465 4d6f 6469 6669 6564 546b 696e  dateModifiedTkin
+00001890: 6454 6e61 6d65 5e64 6174 654c 6173 744f  dTname^dateLastO
+000018a0: 7065 6e65 64d4 1819 1a1b 1c1d 0c1f 5569  pened.........Ui
+000018b0: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
+000018c0: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
+000018d0: 2c09 08d4 1819 1a1b 2122 0c1f 1005 1064  ,.......!".....d
+000018e0: 0908 d418 191a 1b26 270c 1f10 0610 4b09  .......&'.....K.
+000018f0: 08d4 1b1a 1918 1f1f 2d2e 0808 10b0 1002  ........-.......
+00001900: d418 191a 1b30 311f 0c10 0310 6108 09d4  .....01.....a...
+00001910: 1b1a 1918 0c1f 2d0b 0908 d418 191a 1b38  ......-........8
+00001920: 390c 0c10 0410 7309 09d4 1819 1a1b 3d3e  9.....s.......=>
+00001930: 0c0c 1000 1101 9909 09d4 1b1a 1918 1f1f  ................
+00001940: 2d44 0808 1008 0923 0000 0000 0000 0000  -D.....#........
 00001950: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
-00001960: 6469 6669 6564 2340 3000 0000 0000 0000  dified#@0.......
-00001970: 0800 1d00 3000 4200 4a00 5e00 7000 7900  ....0.B.J.^.p.y.
-00001980: 8b00 9600 9f00 b400 b500 b600 c900 d200  ................
-00001990: d800 e000 ec00 f100 fe01 0301 0801 1701  ................
-000019a0: 2001 2801 2e01 3801 3e01 3f01 4201 4301   .(...8.>.?.B.C.
-000019b0: 4501 4e01 4f01 5101 5201 5401 5d01 5e01  E.N.O.Q.R.T.].^.
-000019c0: 6001 6101 6301 6c01 6e01 6f01 7101 7201  `.a.c.l.n.o.q.r.
-000019d0: 7b01 7c01 7e01 7f01 8101 8a01 8c01 8d01  {.|.~...........
-000019e0: 8e01 9701 9801 9a01 9b01 9d01 a601 a701  ................
-000019f0: aa01 ab01 ad01 b601 b801 b901 ba01 bb01  ................
-00001a00: c401 cd01 da00 0000 0000 0002 0100 0000  ................
-00001a10: 0000 0000 4b00 0000 0000 0000 0000 0000  ....K...........
-00001a20: 0000 0001 e300 0000 0900 7200 6500 7300  ..........r.e.s.
-00001a30: 6f00 7500 7200 6300 6500 736d 6f44 4462  o.u.r.c.e.smoDDb
-00001a40: 6c6f 6200 0000 0846 8ad9 20ad 65c5 4100  lob....F.. .e.A.
-00001a50: 0000 0900 7200 6500 7300 6f00 7500 7200  ....r.e.s.o.u.r.
-00001a60: 6300 6500 736d 6f64 4462 6c6f 6200 0000  c.e.smodDblob...
-00001a70: 0846 8ad9 20ad 65c5 4100 0000 0900 7200  .F.. .e.A.....r.
-00001a80: 6500 7300 6f00 7500 7200 6300 6500 7370  e.s.o.u.r.c.e.sp
-00001a90: 6831 5363 6f6d 7000 0000 0000 2d90 0000  h1Scomp.....-...
-00001aa0: 0000 0900 7200 6500 7300 6f00 7500 7200  ....r.e.s.o.u.r.
-00001ab0: 6300 6500 7376 5372 6e6c 6f6e 6700 0000  c.e.svSrnlong...
-00001ac0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00001960: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
+00001970: 0008 001d 0032 0044 004c 0060 0072 007b  .....2.D.L.`.r.{
+00001980: 008d 0098 00a1 00b4 00b6 00b7 00ca 00d3  ................
+00001990: 00d9 00e1 00ed 00f2 00ff 0104 0109 0118  ................
+000019a0: 0121 0127 012d 0137 013f 0141 0144 0145  .!.'.-.7.?.A.D.E
+000019b0: 0146 014f 0151 0153 0154 0155 015e 0160  .F.O.Q.S.T.U.^.`
+000019c0: 0162 0163 0164 016d 016e 016f 0171 0173  .b.c.d.m.n.o.q.s
+000019d0: 017c 017e 0180 0181 0182 018b 018c 018d  .|.~............
+000019e0: 0196 0198 019a 019b 019c 01a5 01a7 01aa  ................
+000019f0: 01ab 01ac 01b5 01b6 01b7 01b9 01ba 01c3  ................
+00001a00: 01cc 01d9 01e2 0000 0000 0000 0201 0000  ................
+00001a10: 0000 0000 004b 0000 0000 0000 0000 0000  .....K..........
+00001a20: 0000 0000 01e3 0000 0009 0072 0065 0073  ...........r.e.s
+00001a30: 006f 0075 0072 0063 0065 0073 6d6f 4444  .o.u.r.c.e.smoDD
+00001a40: 626c 6f62 0000 0008 9ce8 de46 29f7 c541  blob.......F)..A
+00001a50: 0000 0009 0072 0065 0073 006f 0075 0072  .....r.e.s.o.u.r
+00001a60: 0063 0065 0073 6d6f 6444 626c 6f62 0000  .c.e.smodDblob..
+00001a70: 0008 9ce8 de46 29f7 c541 0000 0009 0072  .....F)..A.....r
+00001a80: 0065 0073 006f 0075 0072 0063 0065 0073  .e.s.o.u.r.c.e.s
+00001a90: 7068 3153 636f 6d70 0000 0000 003f 9000  ph1Scomp.....?..
+00001aa0: 0000 0009 0072 0065 0073 006f 0075 0072  .....r.e.s.o.u.r
+00001ab0: 0063 0065 0073 7653 726e 6c6f 6e67 0000  .c.e.svSrnlong..
+00001ac0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0025 2a2f 3439 3e42 464b 4fd4 0f10 1112  .%*/49>BFKO.....
-00002510: 1314 0b0b 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00002520: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00002530: 7669 7369 626c 6554 6e61 6d65 1101 9909  visibleTname....
-00002540: 09d4 0f10 1112 1819 1a1a 5875 6269 7175  ..........Xubiqu
-00002550: 6974 7910 2308 08d4 1211 100f 0b1a 1f20  ity.#.......... 
-00002560: 0908 10b0 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00002570: 64d4 1211 100f 1a1a 1f24 0808 5b64 6174  d........$..[dat
-00002580: 6543 7265 6174 6564 d40f 1011 1226 271a  eCreated.....&'.
-00002590: 0b54 7369 7a65 1061 0809 d40f 1011 122b  .Tsize.a.......+
-000025a0: 2c0b 0b54 6b69 6e64 1073 0909 d40f 1011  ,..Tkind.s......
-000025b0: 1230 310b 1a55 6c61 6265 6c10 6409 08d4  .01..Ulabel.d...
-000025c0: 0f10 1112 3536 0b1a 5776 6572 7369 6f6e  ....56..Wversion
-000025d0: 104b 0908 d40f 1011 123a 3b0b 1a58 636f  .K.......:;..Xco
-000025e0: 6d6d 656e 7473 1101 2c09 08d4 1211 100f  mments..,.......
-000025f0: 1a1a 1f41 0808 5e64 6174 654c 6173 744f  ...A..^dateLastO
-00002600: 7065 6e65 64d4 1211 100f 1a1a 1f45 0808  pened........E..
-00002610: 5964 6174 6541 6464 6564 d412 1110 0f1a  YdateAdded......
-00002620: 1a49 4a08 0810 d25a 7368 6172 654f 776e  .IJ....ZshareOwn
-00002630: 6572 d412 1110 0f1a 1a49 4e08 085f 100f  er.......IN.._..
-00002640: 7368 6172 654c 6173 7445 6469 746f 72d4  shareLastEditor.
-00002650: 1211 100f 1a1a 4952 0808 5f10 1069 6e76  ......IR.._..inv
-00002660: 6974 6174 696f 6e53 7461 7475 7309 2300  itationStatus.#.
-00002670: 0000 0000 0000 0023 4028 0000 0000 0000  .......#@(......
-00002680: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
-00002690: 0000 0000 0000 1001 0008 001d 0030 0042  .............0.B
-000026a0: 004a 005e 0070 0079 008b 0096 009f 00b4  .J.^.p.y........
-000026b0: 00b5 00b6 00c5 00ce 00d9 00df 00e9 00f1  ................
-000026c0: 00f6 00f9 00fa 00fb 0104 010d 010f 0110  ................
-000026d0: 0111 011a 011b 011c 011e 012b 0134 0135  ...........+.4.5
-000026e0: 0136 0142 014b 0150 0152 0153 0154 015d  .6.B.K.P.R.S.T.]
-000026f0: 0162 0164 0165 0166 016f 0175 0177 0178  .b.d.e.f.o.u.w.x
-00002700: 0179 0182 018a 018c 018d 018e 0197 01a0  .y..............
-00002710: 01a3 01a4 01a5 01ae 01af 01b0 01bf 01c8  ................
-00002720: 01c9 01ca 01d4 01dd 01de 01df 01e1 01ec  ................
-00002730: 01f5 01f6 01f7 0209 0212 0213 0214 0227  ...............'
-00002740: 0228 0231 023a 0247 0250 0000 0000 0000  .(.1.:.G.P......
-00002750: 0201 0000 0000 0000 0059 0000 0000 0000  .........Y......
-00002760: 0000 0000 0000 0000 0252 0000 0009 0072  .........R.....r
-00002770: 0065 0073 006f 0075 0072 0063 0065 0073  .e.s.o.u.r.c.e.s
-00002780: 6c73 7670 626c 6f62 0000 0299 6270 6c69  lsvpblob....bpli
-00002790: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-000027a0: 0b0d 0b47 4847 494a 355f 1010 7573 6552  ...GHGIJ5_..useR
-000027b0: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-000027c0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000027d0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000027e0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-000027f0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-00002800: 7453 697a                                tSiz
+00002500: 001c 2125 2a2f 3439 3e42 464b 4fd4 0f10  ..!%*/49>BFKO...
+00002510: 1112 0c14 0c16 5776 6973 6962 6c65 5577  ......WvisibleUw
+00002520: 6964 7468 5961 7363 656e 6469 6e67 5a69  idthYascendingZi
+00002530: 6465 6e74 6966 6965 7209 1101 9909 546e  dentifier.....Tn
+00002540: 616d 65d4 0f10 1112 1819 181b 0810 2308  ame...........#.
+00002550: 5875 6269 7175 6974 79d4 1211 100f 1d18  Xubiquity.......
+00002560: 1f0c 5c64 6174 654d 6f64 6966 6965 6408  ..\dateModified.
+00002570: 10b0 09d4 1211 100f 2218 1f18 5b64 6174  ........"...[dat
+00002580: 6543 7265 6174 6564 0808 d40f 1011 120c  eCreated........
+00002590: 2718 2909 1061 0854 7369 7a65 d40f 1011  '.)..a.Tsize....
+000025a0: 120c 2c0c 2e09 1073 0954 6b69 6e64 d40f  ..,....s.Tkind..
+000025b0: 1011 1218 310c 3308 1064 0955 6c61 6265  ....1.3..d.Ulabe
+000025c0: 6cd4 0f10 1112 1836 0c38 0810 4b09 5776  l......6.8..K.Wv
+000025d0: 6572 7369 6f6e d40f 1011 1218 3b0c 3d08  ersion......;.=.
+000025e0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 1211  ..,.Xcomments...
+000025f0: 100f 3f18 1f18 5e64 6174 654c 6173 744f  ..?...^dateLastO
+00002600: 7065 6e65 6408 08d4 1211 100f 4318 1f18  pened.......C...
+00002610: 5964 6174 6541 6464 6564 0808 d412 1110  YdateAdded......
+00002620: 0f47 1849 185a 7368 6172 654f 776e 6572  .G.I.ZshareOwner
+00002630: 0810 d208 d412 1110 0f4c 1849 185f 100f  .........L.I._..
+00002640: 7368 6172 654c 6173 7445 6469 746f 7208  shareLastEditor.
+00002650: 08d4 1211 100f 5018 4918 5f10 1069 6e76  ......P.I._..inv
+00002660: 6974 6174 696f 6e53 7461 7475 7308 0809  itationStatus...
+00002670: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
+00002680: 0000 5c64 6174 654d 6f64 6966 6965 6423  ..\dateModified#
+00002690: 4030 0000 0000 0000 0900 0800 1d00 3200  @0............2.
+000026a0: 4400 4c00 6000 7200 7b00 8d00 9800 a100  D.L.`.r.{.......
+000026b0: b400 b600 b700 c600 cf00 d700 dd00 e700  ................
+000026c0: f200 f300 f600 f700 fc01 0501 0601 0801  ................
+000026d0: 0901 1201 1b01 2801 2901 2b01 2c01 3501  ......(.).+.,.5.
+000026e0: 4101 4201 4301 4c01 4d01 4f01 5001 5501  A.B.C.L.M.O.P.U.
+000026f0: 5e01 5f01 6101 6201 6701 7001 7101 7301  ^._.a.b.g.p.q.s.
+00002700: 7401 7a01 8301 8401 8601 8701 8f01 9801  t.z.............
+00002710: 9901 9c01 9d01 a601 af01 be01 bf01 c001  ................
+00002720: c901 d301 d401 d501 de01 e901 ea01 ec01  ................
+00002730: ed01 f602 0802 0902 0a02 1302 2602 2702  ............&.'.
+00002740: 2802 2902 3202 3b02 4802 5100 0000 0000  (.).2.;.H.Q.....
+00002750: 0002 0100 0000 0000 0000 5900 0000 0000  ..........Y.....
+00002760: 0000 0000 0000 0000 0002 5200 0000 0900  ..........R.....
+00002770: 7200 6500 7300 6f00 7500 7200 6300 6500  r.e.s.o.u.r.c.e.
+00002780: 736c 7376 7062 6c6f 6200 0002 9962 706c  slsvpblob....bpl
+00002790: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
+000027a0: 0b0c 0d0c 4647 4648 490c 5f10 1276 6965  ....FGFHI._..vie
+000027b0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+000027c0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+000027d0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+000027e0: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
+000027f0: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
+00002800: 7465 7874                                text
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/app.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self.edit_image = self.load_icon(EDIT_FILE, (24, 24))
         self.edit_off_image = self.load_icon(EDIT_OFF_FILE, (24, 24))
         self.save_image = self.load_icon(SAVE_FILE, (24, 24))
         self.expand_image = self.load_icon(EXPAND_FILE, (12, 24))
         self.sort_image = self.load_icon(SORT_FILE, (20, 20))
         self.view_image = self.load_icon(LIGHTBULB_FILE, (20, 20))
         self.icon_image = CTkImage(Image.open(ICON_FILE), size=(100, 100))
+        self.icon_cube_image = CTkImage(Image.open(ICON_CUBE_FILE), size=(100, 100))
 
         self.icon_image_pi = PhotoImage(file=ICON_FILE)
         self.iconphoto(False, self.icon_image_pi)
         if platform.system() == "Windows":
             self.iconbitmap(ICO_FILE)
 
         # configure layout
@@ -89,16 +90,16 @@
         self.image_frame.grid(
             row=0, column=0, rowspan=4, sticky="news", padx=20, pady=20
         )
 
         self.image_label = CTkLabel(
             self.image_frame,
             width=560,
-            text=VERSION + "\n\n" + MESSAGE["drop"][0],
-            image=self.icon_image,
+            text="\n" + VERSION + "\n\n" + MESSAGE["drop"][0],
+            image=self.icon_cube_image,
             compound="top",
             text_color=ACCESSIBLE_GRAY,
         )
         self.image_label.pack(fill="both", expand=True)
         self.image_label.bind(
             "<Button-1>",
             lambda e: self.display_info(self.select_image(), is_selected=True),
@@ -131,19 +132,19 @@
         self.negative_box = PromptViewer(self, self.status_bar, "Negative Prompt")
         self.negative_box.viewer_frame.grid(
             row=1, column=1, columnspan=6, sticky="news", padx=(0, 20), pady=(0, 20)
         )
 
         self.setting_box = STkTextbox(self, wrap="word", height=80)
         self.setting_box.grid(
-            row=2, column=1, columnspan=6, sticky="news", padx=(0, 20), pady=(0, 20)
+            row=2, column=1, columnspan=6, sticky="news", padx=(0, 20), pady=(1, 21)
         )
         self.setting_box.text = "Setting"
 
-        # textbox simple mode
+        # setting box simple mode
         self.setting_box_simple = CTkFrame(
             self, height=80, fg_color=self.textbox_fg_color
         )
         self.setting_box_parameter = CTkFrame(
             self.setting_box_simple, fg_color="transparent"
         )
         self.setting_box_parameter = ParameterViewer(
@@ -810,27 +811,27 @@
                 self.button_view_setting.mode = SettingMode.SIMPLE
                 self.setting_box_simple.grid(
                     row=2,
                     column=1,
                     columnspan=6,
                     sticky="news",
                     padx=(0, 20),
-                    pady=(0, 20),
+                    pady=(1, 21),
                 )
                 self.setting_box.grid_forget()
                 self.status_bar.info(MESSAGE["view_setting"][0])
             case SettingMode.SIMPLE:
                 self.button_view_setting.mode = SettingMode.NORMAL
                 self.setting_box.grid(
                     row=2,
                     column=1,
                     columnspan=6,
                     sticky="news",
                     padx=(0, 20),
-                    pady=(0, 20),
+                    pady=(1, 21),
                 )
                 self.setting_box_simple.grid_forget()
                 self.status_bar.info(MESSAGE["view_setting"][-1])
 
     @staticmethod
     def mode_update(button: STkButton, textbox: STkTextbox, sort_button: STkButton):
         match button.mode:
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/button.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/button.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/cli.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/cli.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/constants.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     Path(RESOURCE_DIR, "view_week_20_alpha.png"),
 )
 VIEW_TAB_FILE = (
     Path(RESOURCE_DIR, "view_sidebar_20.png"),
     Path(RESOURCE_DIR, "view_sidebar_20_alpha.png"),
 )
 ICON_FILE = Path(RESOURCE_DIR, "icon.png")
-ICO_FILE = Path(RESOURCE_DIR, "icon.ico")
+ICON_CUBE_FILE = Path(RESOURCE_DIR, "icon-cube.png")
+ICO_FILE = Path(RESOURCE_DIR, "icon-gui.ico")
 MESSAGE = {
     "drop": ["Drop image here or click to select"],
     "default": ["Drag and drop your image file into the window"],
     "success": ["Voilà!"],
     "format_error": ["", "No data detected or unsupported format"],
     "suffix_error": ["Unsupported format"],
     "clipboard": ["Copied to the clipboard"],
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/.DS_Store` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0001 1118 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0000 014e 0000 000b 005f 005f 0070  .....N....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 08e0 c8d3  moDDblob........
-00000160: d1ec c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 2a2e a610  moDDblob....*...
+00000160: b457 c541 0000 000b 005f 005f 0070 0079  .W.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 08e0 c8d3 d1ec  dDblob..........
+00000180: 6444 626c 6f62 0000 0008 2a2e a610 b457  dDblob....*....W
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 6000 0000 0000  comp......`.....
+000001b0: 636f 6d70 0000 0000 0000 1000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/a1111.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/a1111.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/base_format.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/base_format.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/comfyui.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/comfyui.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..format.base_format import BaseFormat
 from ..utility import remove_quotes, merge_dict
 
 
 class ComfyUI(BaseFormat):
     # comfyui node types
-    KSAMPLER_TYPES = ["KSampler", "KSamplerAdvanced"]
+    KSAMPLER_TYPES = ["KSampler", "KSamplerAdvanced", "KSampler (Efficient)"]
     VAE_ENCODE_TYPE = ["VAEEncode", "VAEEncodeForInpaint"]
     CHECKPOINT_LOADER_TYPE = [
         "CheckpointLoader",
         "CheckpointLoaderSimple",
         "unCLIPCheckpointLoader",
         "Checkpoint Loader (Simple)",
     ]
@@ -202,14 +202,24 @@
                     self._parameter[p] = str(longest_flow.get(s))
 
         if self._is_sdxl:
             if not self._positive and self.positive_sdxl:
                 self._positive = self.merge_clip(self.positive_sdxl)
             if not self._negative and self.negative_sdxl:
                 self._negative = self.merge_clip(self.negative_sdxl)
+            empty_prompt = (0 if self._positive_sdxl else 1) + (
+                0 if self._negative_sdxl else 1
+            )
+        else:
+            empty_prompt = (0 if self._positive else 1) + (0 if self._negative else 1)
+
+        empty_param = sum(1 for x in self._parameter.values() if x == "None")
+
+        if empty_prompt + empty_param > (6 + 2) / 2 or empty_prompt == 2:
+            raise ValueError("More than half of the parameters cannot be parsed")
 
     @staticmethod
     def merge_clip(data: dict):
         clip_g = data.get("Clip G").strip(" ,")
         clip_l = data.get("Clip L").strip(" ,")
 
         if clip_g == clip_l:
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/drawthings.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/drawthings.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/easydiffusion.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/easydiffusion.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/fooocus.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/fooocus.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/invokeai.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/invokeai.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/novelai.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/novelai.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/format/swarmui.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/swarmui.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/image_data_reader.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/image_data_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     DrawThings,
     SwarmUI,
     Fooocus,
 )
 
 
 class ImageDataReader:
+    NOVELAI_MAGIC = "stealth_pngcomp"
+
     def __init__(self, file, is_txt: bool = False):
         self._height = None
         self._width = None
         self._info = {}
         self._positive = ""
         self._negative = ""
         self._positive_sdxl = {}
@@ -141,20 +143,19 @@
                         else:
                             self._tool = "Draw Things"
                             self._parser = DrawThings(info=data_json)
                     # novelai stealth pnginfo format
                     elif f.mode == "RGBA":
                         try:
                             reader = NovelAI.LSBExtractor(f)
-                            magic = "stealth_pngcomp"
-                            read_magic = reader.get_next_n_bytes(len(magic)).decode(
-                                "utf-8"
-                            )
+                            read_magic = reader.get_next_n_bytes(
+                                len(self.NOVELAI_MAGIC)
+                            ).decode("utf-8")
                             assert (
-                                magic == read_magic
+                                self.NOVELAI_MAGIC == read_magic
                             ), "NovelAI stealth png info magic number error"
                         except Exception as e:
                             self._logger.warn(e)
                             self._status = BaseFormat.Status.FORMAT_ERROR
                         else:
                             self._tool = "NovelAI"
                             self._parser = NovelAI(extractor=reader)
@@ -165,14 +166,29 @@
                             self._tool = "Fooocus"
                             self._parser = Fooocus(
                                 info=json.loads(self._info.get("comment"))
                             )
                         except Exception:
                             self._logger.warn("Fooocus format error")
                             self._status = BaseFormat.Status.FORMAT_ERROR
+                    elif f.mode == "RGBA":
+                        try:
+                            reader = NovelAI.LSBExtractor(f)
+                            read_magic = reader.get_next_n_bytes(
+                                len(self.NOVELAI_MAGIC)
+                            ).decode("utf-8")
+                            assert (
+                                self.NOVELAI_MAGIC == read_magic
+                            ), "NovelAI stealth png info magic number error"
+                        except Exception as e:
+                            self._logger.warn(e)
+                            self._status = BaseFormat.Status.FORMAT_ERROR
+                        else:
+                            self._tool = "NovelAI"
+                            self._parser = NovelAI(extractor=reader)
                     else:
                         try:
                             exif = piexif.load(self._info.get("exif")) or {}
                             user_comment = exif.get("Exif").get(
                                 piexif.ExifIFD.UserComment
                             )
                         except TypeError:
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/logger.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/logger.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/parameter_viewer.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/parameter_viewer.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/prompt_viewer.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/prompt_viewer.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/.DS_Store` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/format/.DS_Store`

 * *Files 23% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 014e 0000 000b 005f 005f 0070  .....N....._._.p
+00000130: 0000 0001 153a 0000 000b 005f 005f 0070  .....:....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 2a2e a610  moDDblob....*...
-00000160: b457 c541 0000 000b 005f 005f 0070 0079  .W.A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 619b 25bd  moDDblob....a.%.
+00000160: f7f3 c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 2a2e a610 b457  dDblob....*....W
+00000180: 6444 626c 6f62 0000 0008 619b 25bd f7f3  dDblob....a.%...
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0000 1000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0001 6000 0000 0000  comp......`.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/check_circle_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/check_circle_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/check_circle_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/check_circle_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/cleaning_services_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/cleaning_services_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/cleaning_services_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/cleaning_services_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_20.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_20_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/content_copy_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/content_copy_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/description_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/description_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/description_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/description_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_off_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_off_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/edit_off_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/edit_off_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/error_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/error_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/error_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/error_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/expand_more_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/expand_more_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/expand_more_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/expand_more_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/gray.json` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/gray.json`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/info_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/info_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/info_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/info_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/lightbulb_20.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/lightbulb_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/lightbulb_20_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/lightbulb_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/mop_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/mop_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/mop_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/mop_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/place_item_48.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/place_item_48.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/place_item_48_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/place_item_48_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/save_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/save_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/save_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/save_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/sort_by_alpha_20.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/sort_by_alpha_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/sort_by_alpha_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/update_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/update_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/update_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/update_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_sidebar_20.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_sidebar_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_sidebar_20_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_sidebar_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_week_20.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_week_20.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/view_week_20_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/view_week_20_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/warning_24.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/warning_24.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/resources/warning_24_alpha.png` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/resources/warning_24_alpha.png`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/status_bar.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/status_bar.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/textbox.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/textbox.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/update_checker.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/update_checker.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/sd_prompt_reader/utility.py` & `sd_prompt_reader-1.3.5b2/sd_prompt_reader/utility.py`

 * *Files identical despite different names*

### Comparing `sd_prompt_reader-1.3.5b1.dev1/PKG-INFO` & `sd_prompt_reader-1.3.5b2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 Metadata-Version: 2.1
 Name: sd-prompt-reader
-Version: 1.3.5b1.dev1
+Version: 1.3.5b2
 Summary: A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
 Home-page: https://github.com/receyuki/stable-diffusion-prompt-reader
 License: MIT
 Author: receyuki
 Author-email: receyuki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<8.2.0)
+Requires-Dist: ctktooltip (>=0.8,<1.0)
+Requires-Dist: customtkinter (>=5.2.2,<5.3.0)
+Requires-Dist: pefile (>=2023.2.7,<2023.3.0)
+Requires-Dist: piexif (>=1.1.3,<1.2.0)
+Requires-Dist: pillow (==10.3.0)
+Requires-Dist: pyobjc-framework-cocoa (==10.2) ; sys_platform == "darwin"
+Requires-Dist: pyobjus (>=1.2.3,<1.3.0) ; sys_platform == "darwin"
+Requires-Dist: pyperclip (>=1.8.2,<1.9.0)
+Requires-Dist: requests (>=2.31.0,<2.32.0)
+Requires-Dist: tkinterdnd2-universal (>=1.7.3,<1.8.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Bug Tracker, https://github.com/receyuki/stable-diffusion-prompt-reader/issues
 Project-URL: Documentation, https://github.com/receyuki/stable-diffusion-prompt-reader
 Project-URL: Repository, https://github.com/receyuki/stable-diffusion-prompt-reader
 Description-Content-Type: text/markdown
 
 <div align="center">
-    <img alt="icon" src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/sd_prompt_reader/resources/icon.png" width=20% height=20%>
+    <img alt="icon" src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/sd_prompt_reader/resources/icon-cube.png" width=20% height=20%>
     <h1>Stable Diffusion Prompt Reader</h1>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest">
         <img alt="GitHub releases" src="https://img.shields.io/github/downloads/receyuki/stable-diffusion-prompt-reader/total"></a>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/blob/master/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/github/license/receyuki/stable-diffusion-prompt-reader"></a>
     <a href="https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest">
         <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/receyuki/stable-diffusion-prompt-reader"></a>
@@ -39,28 +51,30 @@
 A simple standalone viewer for reading prompt from Stable Diffusion generated image outside the webui.
     <br>
   <p>
     <a href="#features">Features</a> •
     <a href="#supported-formats">Supported Formats</a> •
     <a href="#download">Download</a> •
     <a href="#usage">Usage</a> •
-    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
     <a href="#cli">CLI</a> •
+    <a href="https://github.com/receyuki/comfyui-prompt-reader-node">ComfyUI Node</a> •
     <a href="#api">API</a> •
     <a href="#faq">FAQ</a> •
     <a href="#credits">Credits</a>
   </p>
     <img src="https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/screenshot_v134.png">
 </div>
 
->The SD Prompt Reader is now available as a ComfyUI node. Check out 
->the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) for more information.
+> [!TIP]
+> The SD Prompt Reader is now available as a ComfyUI node. Check out 
+> the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) for more information.
 
 ## Features
 - Support macOS, Windows and Linux.
+- Provides both GUI and CLI
 - Simple drag and drop interaction.
 - Copy prompt to clipboard.
 - Remove prompt from image.
 - Export prompt to text file.
 - Edit or import prompt to images
 - Vertical orientation display and sorting by alphabet
 - Detect generation tool.
@@ -71,31 +85,33 @@
 |                                                                                        | PNG | JPEG | WEBP | TXT* |
 |----------------------------------------------------------------------------------------|:---:|:----:|:----:|:----:|
 | [A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui)               |  ✅  |  ✅   |  ✅   |  ✅   |
 | [Easy Diffusion](https://github.com/easydiffusion/easydiffusion)                       |  ✅  |  ✅   |  ✅   |      |
 | [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)*                        |  ✅  |  ✅   |      |      |
 | [StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* |  ✅  |  ✅   |      |      |
 | [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)*                             |  ✅  |  ✅   |      |      |
+| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |  ✅   |      |
+| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
 | [InvokeAI](https://github.com/invoke-ai/InvokeAI)                                      |  ✅  |      |      |      |
 | [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI)              |  ✅  |      |      |      |
 | [InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI)                      |  ✅  |      |      |      |
 | [ComfyUI](https://github.com/comfyanonymous/ComfyUI)*                                  |  ✅  |      |      |      |
 | [Draw Things](https://drawthings.ai/)                                                  |  ✅  |      |      |      |
-| [NovelAI (stealth pnginfo)](https://novelai.net/)                                      |  ✅  |      |      |      |
-| [NovelAI (legacy)](https://novelai.net/)                                               |  ✅  |      |      |      |
 | Naifu(4chan)                                                                           |  ✅  |      |      |      |
 
 \* Limitations apply. See [format limitations](#TXT).
 
-If you are using a tool or format that is not on this list, please help me to support your format 
-by uploading the original file generated by your tool to the issues, thx.
-
-For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
-The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a subproject 
-of this project, and it is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+> [!NOTE]
+> If you are using a tool or format that is not on this list, please help me to support your format 
+> by uploading the original file generated by your tool to the issues, thx.
+
+> [!TIP]
+> For ComfyUI users, the SD Prompt Reader is now available as a ComfyUI node. 
+> The [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a subproject 
+> of this project, and it is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
 
 ## Download
 ### For Windows users
 Download executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
 ### For macOS users
 Download executable from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
 #### Install via Homebrew Cask
@@ -155,15 +171,18 @@
 ### Remove prompt from image
 - Click "Clear" will generate a new image file with suffix "_data_removed" alongside the original image file.
 - To save to another location, click the expand arrow and click "select directory".
 - To overwrite the original image file, click the expand arrow and click "overwrite the original image".  
 ![remove](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/remove.png)
 
 ### Edit image
-***Please note that the edited image will be written in A1111 format, it meaning that image in any format will become A1111 format after editing.***
+> [!NOTE]
+> The edited image will be written in A1111 format, meaning that image in any format 
+> will become A1111 format after editing.
+
 - Click "Edit" to enter edit mode.
 - Edit the prompt directly in the textbox or import a metadata file in txt format.
 - Click "Save" will generate a edited image file with suffix "_edited" alongside the original image file.
 - To save to another location, click the expand arrow and click "select directory".
 - To overwrite the original image file, click the expand arrow and click "overwrite the original image".  
 ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/save.png)
 
@@ -185,24 +204,37 @@
 | Face restoration        | --restore_faces      |
 
 - Click the expand arrow and click "single line prompt".
 - Paste it into the textbox below the webui script "Prompts from file or textbox".  
 ![single line prompt](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/single_line_prompt.png)
 
 ### ComfyUI SDXL workflow
-***The SDXL workflow does not support editing. 
-If necessary, please remove prompts from image before edit.***  
+> [!NOTE]
+> The SDXL workflow does not support editing. 
+> If necessary, please remove prompts from image before edit. 
+
 If the image's workflow includes multiple sets of SDXL prompts, 
 namely Clip G(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt display mode as shown in the image below. 
 There are two interface options available for the multi-set prompt display mode, and you can switch between them using buttons.  
 ![comfyui_sdxl.png](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png)
 
 ## CLI
 A CLI tool for reading, modifying, and clearing metadata is provided. 
-In order to use the CLI tool, please [install SD Prompt Reader via pip](#for-linux-users-not-regularly-tested).
+### Platforms
+#### For Windows users
+`SD Prompt Reader CLI.exe` will be placed in the zip package as a separate executable.   
+Examples:
+`"SD Prompt Reader CLI.exe" -i example.png`  
+#### For macOS users
+The executable is located at `SD Prompt Reader.app/Contents/MacOS/SD Prompt Reader`.  
+Examples:
+`/Applications/SD\ Prompt\ Reader.app/Contents/MacOS/SD\ Prompt\ Reader -i example.png`  
+#### For pip users
+Examples:
+`sd-prompt-reader-cli -i example.png`
 ### Modes and Options
 #### Modes
 - Read Mode: Activated by `-r` or `--read` flag.
 - Write Mode: Activated by `-w` or `--write` flag.
 - Clear Mode: Activated by `-c` or `--clear` flag.
 #### General Options
 - `-i`, `--input-path`: Path to the input image file or directory containing image files, required parameter.
@@ -259,40 +291,45 @@
 ```
 
 ## Format Limitations
 ### TXT
 1. Importing txt file is only allowed in edit mode.
 2. Only A1111 format txt files are supported. You can use txt files generated by the A1111 webui or use the SD prompt reader to export txt from A1111 images
 ### StableSwarmUI
-StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
+> [!IMPORTANT]
+> StableSwarmUI is still in the Alpha testing phase, and its format may change in the future. I will keep track of upcoming updates of StableSwarmUI.
 ### ComfyUI
-1. When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
-This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
-It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
-2. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
-3. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
+> [!IMPORTANT]
+> When custom nodes are used or when the workflow becomes overly complex, there is a high probability that metadata may not be correctly read. 
+> This is because ComfyUI does not store metadata but only the complete workflow. SD Prompt Reader can only handle basic workflows.
+> It is recommended to embed the [Prompt Saver node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum compatibility.
+
+1. If there are multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means that there are multiple KSampler nodes in the flowchart.
+2. Due to the nature of ComfyUI, all nodes and flowcharts in the workflow are stored in the image, including those that are not being used. Also, a flowchart can have multiple branches, inputs and outputs.
 (e.g. output hires. fixed image and original image simultaneously in a single flowchart)
 SD Prompt Reader will traverse all flowcharts and branches and display the longest branch with complete input and output.  
-4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
+3. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow)
 ### Easy Diffusion
 By default, Easy Diffusion does not write metadata to images. Please change the _Metadata format_ in settings to _embed_ to write the metadata to images
 ### Fooocus-MRE
 Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus) does not support writing metadata to image files, 
 SD Prompt Reader only supports images generated by [Fooocus MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE).
 
 ## FAQ
 ### Malware Alert
-The false positive reported by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a common issue for _pyinstaller_ users. 
-I spent a lot of time trying to fix the Windows Defender false positive before, but I couldn't do it for every antivirus software. 
-So, you can either trust Windows Defender or use the instruction for Linux users to use this app.
+> [!WARNING]
+> The false positive reported by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a common issue for _pyinstaller_ users. 
+> I spent a lot of time trying to fix the Windows Defender false positive before, but I couldn't do it for every antivirus software. 
+> So, you can either trust Windows Defender or use the instruction for Linux users to use this app.
 ### "SD Prompt Reader.app" is damaged and can't be opened. You should move it to the Trash
-This is a very common macOS issue when you run unsigned non-appstore apps, 
-and developers must pay $99 per year to Apple to eliminate this issue. 
-You can choose to **Allow Apps from Anywhere** in **security & privacy** settings which can be dangerous. 
-The way I prefer is to remove the quarantine attributes. 
+> [!IMPORTANT]
+> This is a very common macOS issue when you run unsigned non-appstore apps, 
+> and developers must pay $99 per year to Apple to eliminate this issue. 
+> You can choose to **Allow Apps from Anywhere** in **security & privacy** settings which can be dangerous. 
+> The way I prefer is to remove the quarantine attributes. 
 1. Open Terminal from the Applications folder. 
 2. Type in the following command and hit Enter. 
 
     `xattr -r -d com.apple.quarantine /path/to/app.app`
 
     In my case it's
```

#### html2text {}

```diff
@@ -1,70 +1,78 @@
-Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.5b1.dev1 Summary: A
-simple standalone viewer for reading prompt from Stable Diffusion generated
-image outside the webui. Home-page: https://github.com/receyuki/stable-
-diffusion-prompt-reader License: MIT Author: receyuki Author-email:
-receyuki@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Project-URL: Bug Tracker,
-https://github.com/receyuki/stable-diffusion-prompt-reader/issues Project-URL:
+Metadata-Version: 2.1 Name: sd-prompt-reader Version: 1.3.5b2 Summary: A simple
+standalone viewer for reading prompt from Stable Diffusion generated image
+outside the webui. Home-page: https://github.com/receyuki/stable-diffusion-
+prompt-reader License: MIT Author: receyuki Author-email: receyuki@gmail.com
+Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Dist: click (>=8.1.7,<8.2.0) Requires-Dist: ctktooltip
+(>=0.8,<1.0) Requires-Dist: customtkinter (>=5.2.2,<5.3.0) Requires-Dist:
+pefile (>=2023.2.7,<2023.3.0) Requires-Dist: piexif (>=1.1.3,<1.2.0) Requires-
+Dist: pillow (==10.3.0) Requires-Dist: pyobjc-framework-cocoa (==10.2) ;
+sys_platform == "darwin" Requires-Dist: pyobjus (>=1.2.3,<1.3.0) ; sys_platform
+== "darwin" Requires-Dist: pyperclip (>=1.8.2,<1.9.0) Requires-Dist: requests
+(>=2.31.0,<2.32.0) Requires-Dist: tkinterdnd2-universal (>=1.7.3,<1.8.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) Project-URL: Bug Tracker, https://
+github.com/receyuki/stable-diffusion-prompt-reader/issues Project-URL:
 Documentation, https://github.com/receyuki/stable-diffusion-prompt-reader
 Project-URL: Repository, https://github.com/receyuki/stable-diffusion-prompt-
 reader Description-Content-Type: text/markdown
                                     [icon]
                  ************ SSttaabbllee DDiiffffuussiioonn PPrroommpptt RReeaaddeerr ************
  _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_s_]_[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:
                                _b_l_a_c_k_][platform]
 
 [ç®ä½ä¸­æ](https://github.com/receyuki/stable-diffusion-prompt-reader/blob/
    master/README.zh-Hans.md) | [English](https://github.com/receyuki/stable-
  diffusion-prompt-reader/blob/master/README.md) A simple standalone viewer for
     reading prompt from Stable Diffusion generated image outside the webui.
-_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_o_m_f_y_U_I_ _N_o_d_e â¢ _C_L_I
+_F_e_a_t_u_r_e_s â¢ _S_u_p_p_o_r_t_e_d_ _F_o_r_m_a_t_s â¢ _D_o_w_n_l_o_a_d â¢ _U_s_a_g_e â¢ _C_L_I â¢ _C_o_m_f_y_U_I_ _N_o_d_e
                           â¢ _A_P_I â¢ _F_A_Q â¢ _C_r_e_d_i_t_s
 [https://github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
                              screenshot_v134.png]
->The SD Prompt Reader is now available as a ComfyUI node. Check out >the
-[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
-node) for more information. ## Features - Support macOS, Windows and Linux. -
-Simple drag and drop interaction. - Copy prompt to clipboard. - Remove prompt
-from image. - Export prompt to text file. - Edit or import prompt to images -
-Vertical orientation display and sorting by alphabet - Detect generation tool.
-- Multiple formats support. - Dark and light mode support. ## Supported Formats
-| | PNG | JPEG | WEBP | TXT* | |-----------------------------------------------
------------------------------------------|:---:|:----:|:----:|:----:| |
-[A1111's webUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | â
-| â | â | â | | [Easy Diffusion](https://github.com/easydiffusion/
-easydiffusion) | â | â | â | | | [StableSwarmUI](https://github.com/
-Stability-AI/StableSwarmUI)* | â | â | | | | [StableSwarmUI (prior to
-0.5.8-alpha)](https://github.com/Stability-AI/StableSwarmUI)* | â | â | | |
-| [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)* | â | â | | |
-| [InvokeAI](https://github.com/invoke-ai/InvokeAI) | â | | | | | [InvokeAI
-(prior to 2.3.5-post.2)](https://github.com/invoke-ai/InvokeAI) | â | | | | |
-[InvokeAI (prior to 1.15)](https://github.com/invoke-ai/InvokeAI) | â | | | |
-| [ComfyUI](https://github.com/comfyanonymous/ComfyUI)* | â | | | | | [Draw
-Things](https://drawthings.ai/) | â | | | | | [NovelAI (stealth pnginfo)]
-(https://novelai.net/) | â | | | | | [NovelAI (legacy)](https://novelai.net/
+> [!TIP] > The SD Prompt Reader is now available as a ComfyUI node. Check out >
+the [ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-
+reader-node) for more information. ## Features - Support macOS, Windows and
+Linux. - Provides both GUI and CLI - Simple drag and drop interaction. - Copy
+prompt to clipboard. - Remove prompt from image. - Export prompt to text file.
+- Edit or import prompt to images - Vertical orientation display and sorting by
+alphabet - Detect generation tool. - Multiple formats support. - Dark and light
+mode support. ## Supported Formats | | PNG | JPEG | WEBP | TXT* | |------------
+----------------------------------------------------------------------------|:-
+--:|:----:|:----:|:----:| | [A1111's webUI](https://github.com/AUTOMATIC1111/
+stable-diffusion-webui) | â | â | â | â | | [Easy Diffusion](https://
+github.com/easydiffusion/easydiffusion) | â | â | â | | | [StableSwarmUI]
+(https://github.com/Stability-AI/StableSwarmUI)* | â | â | | | |
+[StableSwarmUI (prior to 0.5.8-alpha)](https://github.com/Stability-AI/
+StableSwarmUI)* | â | â | | | | [Fooocus-MRE](https://github.com/
+MoonRide303/Fooocus-MRE)* | â | â | | | | [NovelAI (stealth pnginfo)]
+(https://novelai.net/) | â | | â | | | [NovelAI (legacy)](https://
+novelai.net/) | â | | | | | [InvokeAI](https://github.com/invoke-ai/InvokeAI)
+| â | | | | | [InvokeAI (prior to 2.3.5-post.2)](https://github.com/invoke-
+ai/InvokeAI) | â | | | | | [InvokeAI (prior to 1.15)](https://github.com/
+invoke-ai/InvokeAI) | â | | | | | [ComfyUI](https://github.com/
+comfyanonymous/ComfyUI)* | â | | | | | [Draw Things](https://drawthings.ai/
 ) | â | | | | | Naifu(4chan) | â | | | | \* Limitations apply. See [format
-limitations](#TXT). If you are using a tool or format that is not on this list,
-please help me to support your format by uploading the original file generated
-by your tool to the issues, thx. For ComfyUI users, the SD Prompt Reader is now
-available as a ComfyUI node. The [ComfyUI Prompt Reader Node](https://
-github.com/receyuki/comfyui-prompt-reader-node) is a subproject of this
-project, and it is recommended to embed the [Prompt Saver node](https://
-github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
-generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
-receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
-compatibility. ## Download ### For Windows users Download executable from
-[GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/
-releases/latest) ### For macOS users Download executable from [GitHub Releases]
-(https://github.com/receyuki/stable-diffusion-prompt-reader/releases/latest)
-#### Install via Homebrew Cask You may also install SD Prompt Reader via
-[Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
+limitations](#TXT). > [!NOTE] > If you are using a tool or format that is not
+on this list, please help me to support your format > by uploading the original
+file generated by your tool to the issues, thx. > [!TIP] > For ComfyUI users,
+the SD Prompt Reader is now available as a ComfyUI node. > The [ComfyUI Prompt
+Reader Node](https://github.com/receyuki/comfyui-prompt-reader-node) is a
+subproject > of this project, and it is recommended to embed the [Prompt Saver
+node](https://github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node-
+-parameter-generator-node) in the [ComfyUI Prompt Reader Node](https://
+github.com/receyuki/comfyui-prompt-reader-node) within your workflow to ensure
+maximum compatibility. ## Download ### For Windows users Download executable
+from [GitHub Releases](https://github.com/receyuki/stable-diffusion-prompt-
+reader/releases/latest) ### For macOS users Download executable from [GitHub
+Releases](https://github.com/receyuki/stable-diffusion-prompt-reader/releases/
+latest) #### Install via Homebrew Cask You may also install SD Prompt Reader
+via [Homebrew](http://brew.sh/) cask. ```bash brew install --no-quarantine
 receyuki/sd-prompt-reader/sd-prompt-reader ``` The parameter `--no-quarantine`
 is used since the SD Prompt Reader is currently unsigned as I mentioned [here]
 (https://github.com/receyuki/stable-diffusion-prompt-reader#sd-prompt-
 readerapp-is-damaged-and-cant-be-opened-you-should-move-it-to-the-trash) ###
 For Linux users (not regularly tested) ~~I'm pretty sure linux users can figure
 things out without an executable.~~ - The minimum version of Python required is
 3.10 - Make sure you have the tkinter package installed in your Python. If not,
@@ -85,64 +93,68 @@
 arrow and click "select directory". ![export](https://github.com/receyuki/
 stable-diffusion-prompt-reader/raw/master/images/export.png) ### Remove prompt
 from image - Click "Clear" will generate a new image file with suffix
 "_data_removed" alongside the original image file. - To save to another
 location, click the expand arrow and click "select directory". - To overwrite
 the original image file, click the expand arrow and click "overwrite the
 original image". ![remove](https://github.com/receyuki/stable-diffusion-prompt-
-reader/raw/master/images/remove.png) ### Edit image ***Please note that the
-edited image will be written in A1111 format, it meaning that image in any
-format will become A1111 format after editing.*** - Click "Edit" to enter edit
-mode. - Edit the prompt directly in the textbox or import a metadata file in
-txt format. - Click "Save" will generate a edited image file with suffix
-"_edited" alongside the original image file. - To save to another location,
-click the expand arrow and click "select directory". - To overwrite the
-original image file, click the expand arrow and click "overwrite the original
-image". ![save](https://github.com/receyuki/stable-diffusion-prompt-reader/raw/
-master/images/save.png) ### Copy as single line prompt Copy image prompt and
-setting in a format that can be read by [Prompts from file or textbox](https://
-github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Features#prompts-from-
-file-or-textbox) The following parameters are supported: | Setting | Parameter
-| |-------------------------|----------------------| | Seed | --seed | |
-Variation seed strength | --subseed_strength | | Seed resize from | --
-seed_resize_from_h | | Seed resize from | --seed_resize_from_w | | Sampler | --
-sampler_name | | Steps | --steps | | CFG scale | --cfg_scale | | Size | --width
-| | Size | --height | | Face restoration | --restore_faces | - Click the expand
-arrow and click "single line prompt". - Paste it into the textbox below the
-webui script "Prompts from file or textbox". ![single line prompt](https://
-github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/
-single_line_prompt.png) ### ComfyUI SDXL workflow ***The SDXL workflow does not
-support editing. If necessary, please remove prompts from image before edit.***
-If the image's workflow includes multiple sets of SDXL prompts, namely Clip G
-(text_g), Clip L(text_l), and Refiner, the SD Prompt Reader will switch to the
-multi-set prompt display mode as shown in the image below. There are two
-interface options available for the multi-set prompt display mode, and you can
-switch between them using buttons. ![comfyui_sdxl.png](https://github.com/
-receyuki/stable-diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ##
-CLI A CLI tool for reading, modifying, and clearing metadata is provided. In
-order to use the CLI tool, please [install SD Prompt Reader via pip](#for-
-linux-users-not-regularly-tested). ### Modes and Options #### Modes - Read
-Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated by `-w` or `-
--write` flag. - Clear Mode: Activated by `-c` or `--clear` flag. #### General
-Options - `-i`, `--input-path`: Path to the input image file or directory
-containing image files, required parameter. - `-o`, `--output-path`: Path to
-the output file or directory where the processed files will be saved. - `-l`,
-`--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN, ERROR).
-#### Read Options - `-f`, `--format-type`: Specifies the output metadata
-format, choices are "TXT" or "JSON". Default format is "TXT" #### Write Options
-- `-m`, `--metadata`: Provides a metadata file for writing. - `-p`, `--
-positive`: Provides a positive prompt string for writing. - `-n`, `--negative`:
-Provides a negative prompt string for writing. - `-s`, `--setting`: Provides a
-setting string for writing. ### Basic Usage - If no output path is specified,
-the modified image will be saved in the current directory with a suffix added
-to the original filename. - To overwrite the source file, set the output path
-equal to the input path. - The write mode only supports modifications to a
-single image. #### Read Mode - Read metadata from an image. - Usage: `sd-
-prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-prompt-
-reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
+reader/raw/master/images/remove.png) ### Edit image > [!NOTE] > The edited
+image will be written in A1111 format, meaning that image in any format > will
+become A1111 format after editing. - Click "Edit" to enter edit mode. - Edit
+the prompt directly in the textbox or import a metadata file in txt format. -
+Click "Save" will generate a edited image file with suffix "_edited" alongside
+the original image file. - To save to another location, click the expand arrow
+and click "select directory". - To overwrite the original image file, click the
+expand arrow and click "overwrite the original image". ![save](https://
+github.com/receyuki/stable-diffusion-prompt-reader/raw/master/images/save.png)
+### Copy as single line prompt Copy image prompt and setting in a format that
+can be read by [Prompts from file or textbox](https://github.com/AUTOMATIC1111/
+stable-diffusion-webui/wiki/Features#prompts-from-file-or-textbox) The
+following parameters are supported: | Setting | Parameter | |------------------
+-------|----------------------| | Seed | --seed | | Variation seed strength | -
+-subseed_strength | | Seed resize from | --seed_resize_from_h | | Seed resize
+from | --seed_resize_from_w | | Sampler | --sampler_name | | Steps | --steps |
+| CFG scale | --cfg_scale | | Size | --width | | Size | --height | | Face
+restoration | --restore_faces | - Click the expand arrow and click "single line
+prompt". - Paste it into the textbox below the webui script "Prompts from file
+or textbox". ![single line prompt](https://github.com/receyuki/stable-
+diffusion-prompt-reader/raw/master/images/single_line_prompt.png) ### ComfyUI
+SDXL workflow > [!NOTE] > The SDXL workflow does not support editing. > If
+necessary, please remove prompts from image before edit. If the image's
+workflow includes multiple sets of SDXL prompts, namely Clip G(text_g), Clip L
+(text_l), and Refiner, the SD Prompt Reader will switch to the multi-set prompt
+display mode as shown in the image below. There are two interface options
+available for the multi-set prompt display mode, and you can switch between
+them using buttons. ![comfyui_sdxl.png](https://github.com/receyuki/stable-
+diffusion-prompt-reader/raw/master/images/comfyui_sdxl.png) ## CLI A CLI tool
+for reading, modifying, and clearing metadata is provided. ### Platforms ####
+For Windows users `SD Prompt Reader CLI.exe` will be placed in the zip package
+as a separate executable. Examples: `"SD Prompt Reader CLI.exe" -i example.png`
+#### For macOS users The executable is located at `SD Prompt Reader.app/
+Contents/MacOS/SD Prompt Reader`. Examples: `/Applications/SD\ Prompt\
+Reader.app/Contents/MacOS/SD\ Prompt\ Reader -i example.png` #### For pip users
+Examples: `sd-prompt-reader-cli -i example.png` ### Modes and Options ####
+Modes - Read Mode: Activated by `-r` or `--read` flag. - Write Mode: Activated
+by `-w` or `--write` flag. - Clear Mode: Activated by `-c` or `--clear` flag.
+#### General Options - `-i`, `--input-path`: Path to the input image file or
+directory containing image files, required parameter. - `-o`, `--output-path`:
+Path to the output file or directory where the processed files will be saved. -
+`-l`, `--log-level`: Specify the log verbosity level (e.g.DEBUG, INFO, WARN,
+ERROR). #### Read Options - `-f`, `--format-type`: Specifies the output
+metadata format, choices are "TXT" or "JSON". Default format is "TXT" ####
+Write Options - `-m`, `--metadata`: Provides a metadata file for writing. - `-
+p`, `--positive`: Provides a positive prompt string for writing. - `-n`, `--
+negative`: Provides a negative prompt string for writing. - `-s`, `--setting`:
+Provides a setting string for writing. ### Basic Usage - If no output path is
+specified, the modified image will be saved in the current directory with a
+suffix added to the original filename. - To overwrite the source file, set the
+output path equal to the input path. - The write mode only supports
+modifications to a single image. #### Read Mode - Read metadata from an image.
+- Usage: `sd-prompt-reader-cli [-r] -i [--format-type ] [-o ]` - Examples: `sd-
+prompt-reader-cli -i example.png` `sd-prompt-reader-cli -i example.png -
 o metadata.txt` `sd-prompt-reader-cli -r -i example.png -f TXT -
 o output_folder/` `sd-prompt-reader-cli -r -i input_folder/ -f JSON -
 o output_folder/` #### Write Mode - Write metadata to an image. - Usage: `sd-
 prompt-reader-cli -w -i -m [-o ]` - Examples: `sd-prompt-reader-cli -w -
 i example.png -m new_metadata.txt` `sd-prompt-reader-cli -w -i example.png -
 m new_metadata.txt -o output.png` `sd-prompt-reader-cli -w -i example.png -
 m new_metadata.json -o output_folder/` #### Clear Mode - Remove all metadata
@@ -151,51 +163,52 @@
 o output.png` `sd-prompt-reader-cli -c -i example.png -o output_folder/` `sd-
 prompt-reader-cli -c -i input_folder/ -o output_folder/` ## API ```Python from
 sd_prompt_reader.image_data_reader import ImageDataReader with open(image_path,
 "rb+") as f: image_metadata = ImageDataReader(f) # WIP ``` ## Format
 Limitations ### TXT 1. Importing txt file is only allowed in edit mode. 2. Only
 A1111 format txt files are supported. You can use txt files generated by the
 A1111 webui or use the SD prompt reader to export txt from A1111 images ###
-StableSwarmUI StableSwarmUI is still in the Alpha testing phase, and its format
-may change in the future. I will keep track of upcoming updates of
-StableSwarmUI. ### ComfyUI 1. When custom nodes are used or when the workflow
-becomes overly complex, there is a high probability that metadata may not be
-correctly read. This is because ComfyUI does not store metadata but only the
-complete workflow. SD Prompt Reader can only handle basic workflows. It is
-recommended to embed the [Prompt Saver node](https://github.com/receyuki/
-comfyui-prompt-reader-node#prompt-saver-node--parameter-generator-node) in the
-[ComfyUI Prompt Reader Node](https://github.com/receyuki/comfyui-prompt-reader-
-node) within your workflow to ensure maximum compatibility. 2. If there are
-multiple sets of data (seed, steps, CFG, etc.) in the setting box, this means
-that there are multiple KSampler nodes in the flowchart. 3. Due to the nature
-of ComfyUI, all nodes and flowcharts in the workflow are stored in the image,
-including those that are not being used. Also, a flowchart can have multiple
-branches, inputs and outputs. (e.g. output hires. fixed image and original
-image simultaneously in a single flowchart) SD Prompt Reader will traverse all
-flowcharts and branches and display the longest branch with complete input and
-output. 4. [ComfyUI SDXL workflow](https://github.com/receyuki/stable-
-diffusion-prompt-reader#comfyui-sdxl-workflow) ### Easy Diffusion By default,
-Easy Diffusion does not write metadata to images. Please change the _Metadata
-format_ in settings to _embed_ to write the metadata to images ### Fooocus-MRE
-Since the original version of [Fooocus](https://github.com/lllyasviel/Fooocus)
-does not support writing metadata to image files, SD Prompt Reader only
-supports images generated by [Fooocus MoonRide Edition](https://github.com/
-MoonRide303/Fooocus-MRE). ## FAQ ### Malware Alert The false positive reported
-by some anti-malwares is caused by the packaging tool _pyinstaller_ which is a
-common issue for _pyinstaller_ users. I spent a lot of time trying to fix the
-Windows Defender false positive before, but I couldn't do it for every
-antivirus software. So, you can either trust Windows Defender or use the
-instruction for Linux users to use this app. ### "SD Prompt Reader.app" is
-damaged and can't be opened. You should move it to the Trash This is a very
-common macOS issue when you run unsigned non-appstore apps, and developers must
-pay $99 per year to Apple to eliminate this issue. You can choose to **Allow
-Apps from Anywhere** in **security & privacy** settings which can be dangerous.
-The way I prefer is to remove the quarantine attributes. 1. Open Terminal from
-the Applications folder. 2. Type in the following command and hit Enter. `xattr
--r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
+StableSwarmUI > [!IMPORTANT] > StableSwarmUI is still in the Alpha testing
+phase, and its format may change in the future. I will keep track of upcoming
+updates of StableSwarmUI. ### ComfyUI > [!IMPORTANT] > When custom nodes are
+used or when the workflow becomes overly complex, there is a high probability
+that metadata may not be correctly read. > This is because ComfyUI does not
+store metadata but only the complete workflow. SD Prompt Reader can only handle
+basic workflows. > It is recommended to embed the [Prompt Saver node](https://
+github.com/receyuki/comfyui-prompt-reader-node#prompt-saver-node--parameter-
+generator-node) in the [ComfyUI Prompt Reader Node](https://github.com/
+receyuki/comfyui-prompt-reader-node) within your workflow to ensure maximum
+compatibility. 1. If there are multiple sets of data (seed, steps, CFG, etc.)
+in the setting box, this means that there are multiple KSampler nodes in the
+flowchart. 2. Due to the nature of ComfyUI, all nodes and flowcharts in the
+workflow are stored in the image, including those that are not being used.
+Also, a flowchart can have multiple branches, inputs and outputs. (e.g. output
+hires. fixed image and original image simultaneously in a single flowchart) SD
+Prompt Reader will traverse all flowcharts and branches and display the longest
+branch with complete input and output. 3. [ComfyUI SDXL workflow](https://
+github.com/receyuki/stable-diffusion-prompt-reader#comfyui-sdxl-workflow) ###
+Easy Diffusion By default, Easy Diffusion does not write metadata to images.
+Please change the _Metadata format_ in settings to _embed_ to write the
+metadata to images ### Fooocus-MRE Since the original version of [Fooocus]
+(https://github.com/lllyasviel/Fooocus) does not support writing metadata to
+image files, SD Prompt Reader only supports images generated by [Fooocus
+MoonRide Edition](https://github.com/MoonRide303/Fooocus-MRE). ## FAQ ###
+Malware Alert > [!WARNING] > The false positive reported by some anti-malwares
+is caused by the packaging tool _pyinstaller_ which is a common issue for
+_pyinstaller_ users. > I spent a lot of time trying to fix the Windows Defender
+false positive before, but I couldn't do it for every antivirus software. > So,
+you can either trust Windows Defender or use the instruction for Linux users to
+use this app. ### "SD Prompt Reader.app" is damaged and can't be opened. You
+should move it to the Trash > [!IMPORTANT] > This is a very common macOS issue
+when you run unsigned non-appstore apps, > and developers must pay $99 per year
+to Apple to eliminate this issue. > You can choose to **Allow Apps from
+Anywhere** in **security & privacy** settings which can be dangerous. > The way
+I prefer is to remove the quarantine attributes. 1. Open Terminal from the
+Applications folder. 2. Type in the following command and hit Enter. `xattr -
+r -d com.apple.quarantine /path/to/app.app` In my case it's `xattr -r -
 d com.apple.quarantine /Applications/SD\ Prompt\ Reader.app` If you are still
 concerned about the security of the app you can use the instruction for Linux
 users to use this app. ## TODO - Batch image processing tool - Gallery/Folder
 view - User preference ## Credits - Inspired by [Stable Diffusion web UI]
 (https://github.com/AUTOMATIC1111/stable-diffusion-webui/) - App icon generated
 using Stable Diffusion with [IconsMI](https://huggingface.co/jvkape/IconsMI-
 AppIconsModelforSD) - Special thanks to [Azusachan](https://github.com/
```

