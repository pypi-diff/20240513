# Comparing `tmp/fnschool-20240513.518.24.tar.gz` & `tmp/fnschool-20240513.546.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240513.518.24.tar", last modified: Sun May 12 21:18:27 2024, max compression
+gzip compressed data, was "fnschool-20240513.546.54.tar", last modified: Sun May 12 21:46:57 2024, max compression
```

## Comparing `fnschool-20240513.518.24.tar` & `fnschool-20240513.546.54.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.017329 fnschool-20240513.518.24/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.021328 fnschool-20240513.518.24/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.026328 fnschool-20240513.518.24/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.518.24/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6174 2024-05-12 20:48:48.000000 fnschool-20240513.518.24/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/consume.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.027328 fnschool-20240513.518.24/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.518.24/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.518.24/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.518.24/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.518.24/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2341 2024-05-12 20:35:40.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10300 2024-05-12 20:57:14.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-12 20:14:52.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5216 2024-05-12 20:17:59.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.518.24/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.518.24/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.518.24/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.518.24/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1166 2024-05-12 19:33:42.000000 fnschool-20240513.518.24/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.030328 fnschool-20240513.518.24/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.018329 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.019328 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.031328 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:18:24.000000 fnschool-20240513.518.24/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.518.24/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.518.24/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.518.24/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:18:27.032328 fnschool-20240513.518.24/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 21:18:27.000000 fnschool-20240513.518.24/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 21:18:26.000000 fnschool-20240513.518.24/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.964203 fnschool-20240513.546.54/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:46:57.963203 fnschool-20240513.546.54/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-12 21:46:57.964203 fnschool-20240513.546.54/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.938203 fnschool-20240513.546.54/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.943203 fnschool-20240513.546.54/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.952203 fnschool-20240513.546.54/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240513.546.54/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13812 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6175 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/consume.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.955203 fnschool-20240513.546.54/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240513.546.54/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240513.546.54/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-11 17:45:02.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240513.546.54/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2484 2024-05-12 19:33:41.000000 fnschool-20240513.546.54/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2804 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.959203 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2332 2024-05-12 21:46:19.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10292 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1823 2024-05-12 19:33:41.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1893 2024-05-12 21:46:19.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5208 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9360 2024-05-12 19:33:42.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7241 2024-05-12 20:48:06.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7013 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8829 2024-05-12 20:01:28.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2290 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3990 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9595 2024-05-12 20:57:04.000000 fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98369 2024-05-12 20:36:18.000000 fnschool-20240513.546.54/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240513.546.54/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.959203 fnschool-20240513.546.54/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240513.546.54/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-12 17:45:50.000000 fnschool-20240513.546.54/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1241 2024-05-12 21:46:20.000000 fnschool-20240513.546.54/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.940203 fnschool-20240513.546.54/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    15614 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.960203 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.939203 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.961203 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.940203 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.961203 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-12 21:46:54.000000 fnschool-20240513.546.54/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-12 17:45:50.000000 fnschool-20240513.546.54/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-12 07:39:38.000000 fnschool-20240513.546.54/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240513.546.54/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-12 21:46:57.962203 fnschool-20240513.546.54/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-12 21:46:57.000000 fnschool-20240513.546.54/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240513.518.24/LICENSE` & `fnschool-20240513.546.54/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/PKG-INFO` & `fnschool-20240513.546.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.518.24
+Version: 20240513.546.54
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.518.24/README.md` & `fnschool-20240513.546.54/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/pyproject.toml` & `fnschool-20240513.546.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/__init__.py` & `fnschool-20240513.546.54/src/fnschool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.log import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240513.0518.24"
+__version__ = "20240513.0546.54"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/bill.cp.py` & `fnschool-20240513.546.54/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/bill.py` & `fnschool-20240513.546.54/src/fnschool/canteen/bill.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 )
             )
 
         return self._time_nodes
 
     @property
     def food_class_names(self):
-        fclass_names = ["蔬菜类"]+ list(self.food_classes.keys())
+        fclass_names = ["蔬菜类"] + list(self.food_classes.keys())
         return fclass_names
 
     @property
     def food_classes(self):
         if not self._food_classes:
             print_info(_("Food classes files:"))
             for f in [
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/canteen.toml` & `fnschool-20240513.546.54/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/config.py` & `fnschool-20240513.546.54/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240513.546.54/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240513.546.54/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240513.546.54/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/food.cp.py` & `fnschool-20240513.546.54/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/food.py` & `fnschool-20240513.546.54/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/food_classes.toml` & `fnschool-20240513.546.54/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/operator.py` & `fnschool-20240513.546.54/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/path.py` & `fnschool-20240513.546.54/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/profile.py` & `fnschool-20240513.546.54/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     @property
     def consuming_day_m1(self):
         dates = []
         for f in self.bfoods:
             dates += [d for d, __ in f.consumptions]
         date = max(dates)
         return date.day
-        
 
     @property
     def bill_foods(self):
         return self.bill.foods
 
     @property
     def bfoods(self):
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                     min_col=2,
                     max_col=7,
                 ):
                     for cell in row:
                         cell.value = ""
 
         self.format()
-        
+
         wb = self.bwb
         wb.active = csheet
         print_info(_("Sheet '%s' was updated.") % self.sheet.title)
 
     def format(self):
         csheet = self.sheet
         merged_ranges = list(csheet.merged_cells.ranges)
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         w_seasoning_total_price = sum(
             [f.count * f.unit_price for f in wfoods if ("调味" in f.fclass)]
         )
         unw_seasoning_total_price = sum(
             [f.count * f.unit_price for f in uwfoods if ("调味" in f.fclass)]
         )
 
-        for row_index in range(3,11):
-            cvsheet.cell(row_index,3,"")
+        for row_index in range(3, 11):
+            cvsheet.cell(row_index, 3, "")
 
         cvsheet.cell(
             8,
             3,
             f"入库：{w_seasoning_total_price:.2f}元；"
             + f"未入库：{unw_seasoning_total_price:.2f}元",
         )
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 'If you save updated data to "{0}", '
                 + "data of food sheets will be saved "
                 + "for every month."
             ).format(self.operator.bill_fpath)
         )
 
         s_input = input(">_ ")
-        
+
         print()
         print_info(_("Saving. . ."))
 
         if len(s_input) > 0 and s_input in "Yy":
             self.bwb.save(self.operator.bill_fpath)
             bill_fpath0 = sefl.operator.bill_fpath
             print_info(
```

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240513.546.54/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/test.py` & `fnschool-20240513.546.54/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/canteen/workbook.py` & `fnschool-20240513.546.54/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/entry.py` & `fnschool-20240513.546.54/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/external.py` & `fnschool-20240513.546.54/src/fnschool/external.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 
 def open_file(file_path):
     file_path = str(file_path)
     bin_name = "open" if (sys_is_linux() or sys_is_darwin()) else "start"
     if sys_is_win():
         if file_path.endswith(".toml"):
             bin_name = "notepad"
+        if " " in file_path:
+            file_path = '"' + file_path + '"'
     else:
         file_path = "'" + file_path + "'"
 
     _sh = f"{bin_name} {file_path}"
     os.system(_sh)
```

### Comparing `fnschool-20240513.518.24/src/fnschool/language.py` & `fnschool-20240513.546.54/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240513.546.54/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/log.py` & `fnschool-20240513.546.54/src/fnschool/log.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/path.py` & `fnschool-20240513.546.54/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool/test.py` & `fnschool-20240513.546.54/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240513.518.24/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240513.546.54/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240513.518.24
+Version: 20240513.546.54
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240513.518.24/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240513.546.54/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

