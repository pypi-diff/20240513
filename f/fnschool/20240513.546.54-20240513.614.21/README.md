# Comparing `tmp/fnschool-20240513.546.54.tar.gz` & `tmp/fnschool-20240513.614.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240513.546.54.tar", last modified: Sun May 12 21:46:57 2024, max compression
+gzip compressed data, was "fnschool-20240513.614.21.tar", last modified: Sun May 12 22:14:23 2024, max compression
```

## Comparing `fnschool-20240513.546.54.tar` & `fnschool-20240513.614.21.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.964203 fnschool-20240513.546.54/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:46:57.963203 fnschool-20240513.546.54/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 21:46:57.964203 fnschool-20240513.546.54/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.938203 fnschool-20240513.546.54/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.943203 fnschool-20240513.546.54/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.952203 fnschool-20240513.546.54/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.546.54/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6175 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/consume.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.955203 fnschool-20240513.546.54/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.546.54/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.546.54/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.546.54/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.959203 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2332 2024-05-12 21:46:19.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10292 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1893 2024-05-12 21:46:19.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5208 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.546.54/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.546.54/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.959203 fnschool-20240513.546.54/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.546.54/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1241 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.940203 fnschool-20240513.546.54/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.961203 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.940203 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.961203 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.546.54/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.546.54/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.962203 fnschool-20240513.546.54/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.891404 fnschool-20240513.614.21/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 22:14:23.891404 fnschool-20240513.614.21/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.870401 fnschool-20240513.614.21/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.876402 fnschool-20240513.614.21/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 22:14:21.000000 fnschool-20240513.614.21/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.883403 fnschool-20240513.614.21/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.614.21/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6175 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/consume.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.885403 fnschool-20240513.614.21/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.614.21/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.614.21/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.614.21/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.614.21/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.888403 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2332 2024-05-12 21:46:19.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10292 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1893 2024-05-12 21:46:19.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5208 2024-05-12 21:46:20.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.614.21/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.614.21/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.888403 fnschool-20240513.614.21/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.614.21/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.614.21/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1231 2024-05-12 22:13:50.000000 fnschool-20240513.614.21/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.871402 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.889403 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.872402 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 22:14:20.000000 fnschool-20240513.614.21/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.614.21/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.614.21/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.614.21/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 22:14:23.890403 fnschool-20240513.614.21/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 22:14:23.000000 fnschool-20240513.614.21/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240513.546.54/LICENSE` & `fnschool-20240513.614.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/PKG-INFO` & `fnschool-20240513.614.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.546.54
+Version: 20240513.614.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.546.54/README.md` & `fnschool-20240513.614.21/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/pyproject.toml` & `fnschool-20240513.614.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/__init__.py` & `fnschool-20240513.614.21/src/fnschool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.log import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240513.0546.54"
+__version__ = "20240513.0614.21"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/bill.cp.py` & `fnschool-20240513.614.21/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/bill.py` & `fnschool-20240513.614.21/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/canteen.toml` & `fnschool-20240513.614.21/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/config.py` & `fnschool-20240513.614.21/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240513.614.21/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240513.614.21/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240513.614.21/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/food.cp.py` & `fnschool-20240513.614.21/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/food.py` & `fnschool-20240513.614.21/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/food_classes.toml` & `fnschool-20240513.614.21/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/operator.py` & `fnschool-20240513.614.21/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/path.py` & `fnschool-20240513.614.21/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/profile.py` & `fnschool-20240513.614.21/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240513.614.21/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/test.py` & `fnschool-20240513.614.21/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/canteen/workbook.py` & `fnschool-20240513.614.21/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/entry.py` & `fnschool-20240513.614.21/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/external.py` & `fnschool-20240513.614.21/src/fnschool/external.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,20 +43,22 @@
         else ""
     )
 
 
 def open_file(file_path):
     file_path = str(file_path)
     bin_name = "open" if (sys_is_linux() or sys_is_darwin()) else "start"
+    file_path = '"' + file_path + '"'
     if sys_is_win():
-        if file_path.endswith(".toml"):
+        if file_path.endswith('.toml"'):
             bin_name = "notepad"
-        if " " in file_path:
-            file_path = '"' + file_path + '"'
-    else:
-        file_path = "'" + file_path + "'"
+        else:
+            os.startfile(file_path)
 
-    _sh = f"{bin_name} {file_path}"
-    os.system(_sh)
+            return None
+
+    os.system(f"{bin_name} {file_path}")
+
+    return None
 
 
 # The end.
```

### Comparing `fnschool-20240513.546.54/src/fnschool/language.py` & `fnschool-20240513.614.21/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240513.614.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/log.py` & `fnschool-20240513.614.21/src/fnschool/log.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/path.py` & `fnschool-20240513.614.21/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool/test.py` & `fnschool-20240513.614.21/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.546.54/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240513.614.21/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.546.54
+Version: 20240513.614.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.546.54/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240513.614.21/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

