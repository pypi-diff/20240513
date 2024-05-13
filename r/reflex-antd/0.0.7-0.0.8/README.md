# Comparing `tmp/reflex_antd-0.0.7.tar.gz` & `tmp/reflex_antd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.7.tar", last modified: Fri May 10 13:51:16 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.8.tar", last modified: Mon May 13 02:45:24 2024, max compression
```

## Comparing `reflex_antd-0.0.7.tar` & `reflex_antd-0.0.8.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/
--rw-r--r--   0 see       (1000) see       (1000)    11558 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/LICENSE
--rw-r--r--   0 see       (1000) see       (1000)      977 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/PKG-INFO
--rw-r--r--   0 see       (1000) see       (1000)      362 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/README.md
-drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.953543 reflex_antd-0.0.7/custom_components/
-drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.953543 reflex_antd-0.0.7/custom_components/reflex_antd/
--rw-r--r--   0 see       (1000) see       (1000)        0 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/__init__.py
-drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/custom_components/reflex_antd/antd/
--rw-r--r--   0 see       (1000) see       (1000)        0 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/__init__.py
--rw-r--r--   0 see       (1000) see       (1000)      709 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.py
--rw-r--r--   0 see       (1000) see       (1000)     3101 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1015 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.py
--rw-r--r--   0 see       (1000) see       (1000)     5909 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1063 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.py
--rw-r--r--   0 see       (1000) see       (1000)     3655 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1595 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.py
--rw-r--r--   0 see       (1000) see       (1000)     4382 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1065 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.py
--rw-r--r--   0 see       (1000) see       (1000)     5934 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.pyi
--rw-r--r--   0 see       (1000) see       (1000)      856 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.py
--rw-r--r--   0 see       (1000) see       (1000)     6130 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.pyi
--rw-r--r--   0 see       (1000) see       (1000)     3811 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/base.py
--rw-r--r--   0 see       (1000) see       (1000)      769 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.py
--rw-r--r--   0 see       (1000) see       (1000)     5451 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.pyi
--rw-r--r--   0 see       (1000) see       (1000)      957 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.py
--rw-r--r--   0 see       (1000) see       (1000)     3644 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1364 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.py
--rw-r--r--   0 see       (1000) see       (1000)     3605 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1418 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.py
--rw-r--r--   0 see       (1000) see       (1000)     8612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.pyi
--rw-r--r--   0 see       (1000) see       (1000)      844 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.py
--rw-r--r--   0 see       (1000) see       (1000)     3386 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2342 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.py
--rw-r--r--   0 see       (1000) see       (1000)     5957 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1316 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.py
--rw-r--r--   0 see       (1000) see       (1000)     6026 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.pyi
--rw-r--r--   0 see       (1000) see       (1000)      966 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.py
--rw-r--r--   0 see       (1000) see       (1000)     3580 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1483 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.py
--rw-r--r--   0 see       (1000) see       (1000)     4599 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.pyi
--rw-r--r--   0 see       (1000) see       (1000)     5135 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.py
--rw-r--r--   0 see       (1000) see       (1000)    17831 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.pyi
--rw-r--r--   0 see       (1000) see       (1000)      733 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.py
--rw-r--r--   0 see       (1000) see       (1000)     3597 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.pyi
--rw-r--r--   0 see       (1000) see       (1000)      509 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.py
--rw-r--r--   0 see       (1000) see       (1000)     3200 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1442 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.py
--rw-r--r--   0 see       (1000) see       (1000)     4497 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1572 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.py
--rw-r--r--   0 see       (1000) see       (1000)     7254 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.pyi
--rw-r--r--   0 see       (1000) see       (1000)      356 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.py
--rw-r--r--   0 see       (1000) see       (1000)     2839 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.pyi
--rw-r--r--   0 see       (1000) see       (1000)      499 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.py
--rw-r--r--   0 see       (1000) see       (1000)     3049 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1624 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.py
--rw-r--r--   0 see       (1000) see       (1000)     9924 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.pyi
--rw-r--r--   0 see       (1000) see       (1000)     6100 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.py
--rw-r--r--   0 see       (1000) see       (1000)    14023 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.pyi
--rw-r--r--   0 see       (1000) see       (1000)      945 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.py
--rw-r--r--   0 see       (1000) see       (1000)     5943 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.pyi
--rw-r--r--   0 see       (1000) see       (1000)      491 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/helper.py
--rw-r--r--   0 see       (1000) see       (1000)     2315 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.py
--rw-r--r--   0 see       (1000) see       (1000)     4456 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1011 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.py
--rw-r--r--   0 see       (1000) see       (1000)     5829 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2006 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.py
--rw-r--r--   0 see       (1000) see       (1000)    16141 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.py
--rw-r--r--   0 see       (1000) see       (1000)     4745 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1696 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.py
--rw-r--r--   0 see       (1000) see       (1000)    18024 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1158 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.py
--rw-r--r--   0 see       (1000) see       (1000)     8602 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1422 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.py
--rw-r--r--   0 see       (1000) see       (1000)     4545 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2050 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.py
--rw-r--r--   0 see       (1000) see       (1000)     4675 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.pyi
--rw-r--r--   0 see       (1000) see       (1000)     4741 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.py
--rw-r--r--   0 see       (1000) see       (1000)     3176 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.pyi
--rw-r--r--   0 see       (1000) see       (1000)     4559 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.py
--rw-r--r--   0 see       (1000) see       (1000)     4678 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2077 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/notification.py
--rw-r--r--   0 see       (1000) see       (1000)     1208 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.py
--rw-r--r--   0 see       (1000) see       (1000)     3794 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1005 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.py
--rw-r--r--   0 see       (1000) see       (1000)     3709 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.pyi
--rw-r--r--   0 see       (1000) see       (1000)      493 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.py
--rw-r--r--   0 see       (1000) see       (1000)     4413 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1074 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.py
--rw-r--r--   0 see       (1000) see       (1000)     4279 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.pyi
--rw-r--r--   0 see       (1000) see       (1000)      975 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.py
--rw-r--r--   0 see       (1000) see       (1000)     3635 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1267 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.py
--rw-r--r--   0 see       (1000) see       (1000)     8759 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1010 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.py
--rw-r--r--   0 see       (1000) see       (1000)     3600 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.pyi
--rw-r--r--   0 see       (1000) see       (1000)      568 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.py
--rw-r--r--   0 see       (1000) see       (1000)     3263 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.pyi
--rw-r--r--   0 see       (1000) see       (1000)      880 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.py
--rw-r--r--   0 see       (1000) see       (1000)     3432 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2935 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.py
--rw-r--r--   0 see       (1000) see       (1000)     6924 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.pyi
--rw-r--r--   0 see       (1000) see       (1000)      598 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.py
--rw-r--r--   0 see       (1000) see       (1000)     3161 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1314 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.py
--rw-r--r--   0 see       (1000) see       (1000)     4053 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.pyi
--rw-r--r--   0 see       (1000) see       (1000)      787 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.py
--rw-r--r--   0 see       (1000) see       (1000)     6085 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.pyi
--rw-r--r--   0 see       (1000) see       (1000)      612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.py
--rw-r--r--   0 see       (1000) see       (1000)     3247 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1258 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.py
--rw-r--r--   0 see       (1000) see       (1000)     9147 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1074 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.py
--rw-r--r--   0 see       (1000) see       (1000)     3976 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1075 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.py
--rw-r--r--   0 see       (1000) see       (1000)     3595 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2753 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.py
--rw-r--r--   0 see       (1000) see       (1000)     5782 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2169 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.py
--rw-r--r--   0 see       (1000) see       (1000)     5235 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1105 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.py
--rw-r--r--   0 see       (1000) see       (1000)     5717 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.pyi
--rw-r--r--   0 see       (1000) see       (1000)      588 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.py
--rw-r--r--   0 see       (1000) see       (1000)     3170 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1394 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.py
--rw-r--r--   0 see       (1000) see       (1000)     4395 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1277 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.py
--rw-r--r--   0 see       (1000) see       (1000)     4192 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2053 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.py
--rw-r--r--   0 see       (1000) see       (1000)     3910 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2679 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.py
--rw-r--r--   0 see       (1000) see       (1000)     6180 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.pyi
--rw-r--r--   0 see       (1000) see       (1000)     2941 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.py
--rw-r--r--   0 see       (1000) see       (1000)     6424 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1824 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.py
--rw-r--r--   0 see       (1000) see       (1000)    15437 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1631 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.py
--rw-r--r--   0 see       (1000) see       (1000)     4500 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.pyi
--rw-r--r--   0 see       (1000) see       (1000)      766 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.py
--rw-r--r--   0 see       (1000) see       (1000)     3397 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.pyi
--rw-r--r--   0 see       (1000) see       (1000)    26524 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/base.py
--rw-r--r--   0 see       (1000) see       (1000)    11261 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/base.pyi
--rw-r--r--   0 see       (1000) see       (1000)     1967 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/constant.py
--rw-r--r--   0 see       (1000) see       (1000)     1018 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/display.py
--rw-r--r--   0 see       (1000) see       (1000)      918 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/entry.py
--rw-r--r--   0 see       (1000) see       (1000)      526 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/feedback.py
--rw-r--r--   0 see       (1000) see       (1000)      295 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/general.py
--rw-r--r--   0 see       (1000) see       (1000)      153 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/helper.py
--rw-r--r--   0 see       (1000) see       (1000)      248 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/layout.py
--rw-r--r--   0 see       (1000) see       (1000)      295 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/navigation.py
--rw-r--r--   0 see       (1000) see       (1000)     1715 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/util.py
-drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/
--rw-r--r--   0 see       (1000) see       (1000)      977 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/PKG-INFO
--rw-r--r--   0 see       (1000) see       (1000)     6900 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/SOURCES.txt
--rw-r--r--   0 see       (1000) see       (1000)        1 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/dependency_links.txt
--rw-r--r--   0 see       (1000) see       (1000)       33 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/requires.txt
--rw-r--r--   0 see       (1000) see       (1000)       12 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/top_level.txt
--rw-r--r--   0 see       (1000) see       (1000)      833 2024-05-10 13:40:49.000000 reflex_antd-0.0.7/pyproject.toml
--rw-r--r--   0 see       (1000) see       (1000)       38 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.815598 reflex_antd-0.0.8/
+-rw-rw-rw-   0        0        0    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1095 2024-05-13 02:45:24.814599 reflex_antd-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-05-13 02:39:21.000000 reflex_antd-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.589887 reflex_antd-0.0.8/custom_components/
+drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.610886 reflex_antd-0.0.8/custom_components/reflex_antd/
+-rw-rw-rw-   0        0        0        0 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.811597 reflex_antd-0.0.8/custom_components/reflex_antd/antd/
+-rw-rw-rw-   0        0        0        0 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/__init__.py
+-rw-rw-rw-   0        0        0      679 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.py
+-rw-rw-rw-   0        0        0     3027 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.pyi
+-rw-rw-rw-   0        0        0      977 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.py
+-rw-rw-rw-   0        0        0     5761 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.pyi
+-rw-rw-rw-   0        0        0     1028 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.py
+-rw-rw-rw-   0        0        0     3581 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.pyi
+-rw-rw-rw-   0        0        0     1549 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.py
+-rw-rw-rw-   0        0        0     4343 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.pyi
+-rw-rw-rw-   0        0        0     1025 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.py
+-rw-rw-rw-   0        0        0     5821 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.pyi
+-rw-rw-rw-   0        0        0      825 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.py
+-rw-rw-rw-   0        0        0     5982 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.pyi
+-rw-rw-rw-   0        0        0     3683 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.py
+-rw-rw-rw-   0        0        0     6431 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.pyi
+-rw-rw-rw-   0        0        0      760 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.py
+-rw-rw-rw-   0        0        0     5336 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rw-rw-rw-   0        0        0      922 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.py
+-rw-rw-rw-   0        0        0     3570 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.pyi
+-rw-rw-rw-   0        0        0     1318 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.py
+-rw-rw-rw-   0        0        0     3531 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.pyi
+-rw-rw-rw-   0        0        0     1366 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.py
+-rw-rw-rw-   0        0        0     8569 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.pyi
+-rw-rw-rw-   0        0        0      814 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.py
+-rw-rw-rw-   0        0        0     3312 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.pyi
+-rw-rw-rw-   0        0        0     2282 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.py
+-rw-rw-rw-   0        0        0     6036 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.pyi
+-rw-rw-rw-   0        0        0     1269 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.py
+-rw-rw-rw-   0        0        0     5878 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.pyi
+-rw-rw-rw-   0        0        0      935 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.py
+-rw-rw-rw-   0        0        0     3541 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.pyi
+-rw-rw-rw-   0        0        0     1439 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.py
+-rw-rw-rw-   0        0        0     4525 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.pyi
+-rw-rw-rw-   0        0        0     4993 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.py
+-rw-rw-rw-   0        0        0    18220 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.pyi
+-rw-rw-rw-   0        0        0      709 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.py
+-rw-rw-rw-   0        0        0     3523 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.pyi
+-rw-rw-rw-   0        0        0      488 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.pyi
+-rw-rw-rw-   0        0        0     1398 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.py
+-rw-rw-rw-   0        0        0     4423 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.pyi
+-rw-rw-rw-   0        0        0     1518 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.py
+-rw-rw-rw-   0        0        0     7141 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.pyi
+-rw-rw-rw-   0        0        0      340 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.py
+-rw-rw-rw-   0        0        0     2824 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.pyi
+-rw-rw-rw-   0        0        0      476 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.py
+-rw-rw-rw-   0        0        0     2957 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.pyi
+-rw-rw-rw-   0        0        0     1568 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.py
+-rw-rw-rw-   0        0        0     9702 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.pyi
+-rw-rw-rw-   0        0        0     5933 2024-05-13 02:02:38.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.py
+-rw-rw-rw-   0        0        0    13522 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.pyi
+-rw-rw-rw-   0        0        0      907 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.py
+-rw-rw-rw-   0        0        0     5795 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.pyi
+-rw-rw-rw-   0        0        0      472 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/helper.py
+-rw-rw-rw-   0        0        0     2234 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.py
+-rw-rw-rw-   0        0        0     4382 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.pyi
+-rw-rw-rw-   0        0        0      973 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.py
+-rw-rw-rw-   0        0        0     5740 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.pyi
+-rw-rw-rw-   0        0        0     1934 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.py
+-rw-rw-rw-   0        0        0    16264 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.pyi
+-rw-rw-rw-   0        0        0     1565 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.py
+-rw-rw-rw-   0        0        0     4754 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.pyi
+-rw-rw-rw-   0        0        0     1783 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.py
+-rw-rw-rw-   0        0        0    17500 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.pyi
+-rw-rw-rw-   0        0        0     1114 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.py
+-rw-rw-rw-   0        0        0     8452 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.pyi
+-rw-rw-rw-   0        0        0     1383 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.py
+-rw-rw-rw-   0        0        0     4506 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.pyi
+-rw-rw-rw-   0        0        0     1981 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.py
+-rw-rw-rw-   0        0        0     4629 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.pyi
+-rw-rw-rw-   0        0        0     4765 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.py
+-rw-rw-rw-   0        0        0     3207 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.pyi
+-rw-rw-rw-   0        0        0     4427 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.py
+-rw-rw-rw-   0        0        0     5273 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.pyi
+-rw-rw-rw-   0        0        0     2011 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/notification.py
+-rw-rw-rw-   0        0        0     1169 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.py
+-rw-rw-rw-   0        0        0     3720 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.pyi
+-rw-rw-rw-   0        0        0      972 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.py
+-rw-rw-rw-   0        0        0     3683 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.pyi
+-rw-rw-rw-   0        0        0      473 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.py
+-rw-rw-rw-   0        0        0     4339 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.pyi
+-rw-rw-rw-   0        0        0     1039 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.py
+-rw-rw-rw-   0        0        0     4205 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.pyi
+-rw-rw-rw-   0        0        0      941 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.py
+-rw-rw-rw-   0        0        0     3561 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.pyi
+-rw-rw-rw-   0        0        0     1221 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.py
+-rw-rw-rw-   0        0        0     8537 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.pyi
+-rw-rw-rw-   0        0        0      977 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.py
+-rw-rw-rw-   0        0        0     3526 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.pyi
+-rw-rw-rw-   0        0        0      545 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.py
+-rw-rw-rw-   0        0        0     3296 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.pyi
+-rw-rw-rw-   0        0        0      850 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.py
+-rw-rw-rw-   0        0        0     3358 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.pyi
+-rw-rw-rw-   0        0        0     2862 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.py
+-rw-rw-rw-   0        0        0     6991 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.pyi
+-rw-rw-rw-   0        0        0      575 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.py
+-rw-rw-rw-   0        0        0     3087 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.pyi
+-rw-rw-rw-   0        0        0     1272 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.py
+-rw-rw-rw-   0        0        0     3979 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.pyi
+-rw-rw-rw-   0        0        0      755 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.py
+-rw-rw-rw-   0        0        0     5937 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.pyi
+-rw-rw-rw-   0        0        0      588 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.py
+-rw-rw-rw-   0        0        0     3232 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.pyi
+-rw-rw-rw-   0        0        0     1213 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.py
+-rw-rw-rw-   0        0        0     8925 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.pyi
+-rw-rw-rw-   0        0        0     1036 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.py
+-rw-rw-rw-   0        0        0     3902 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.pyi
+-rw-rw-rw-   0        0        0     1042 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.py
+-rw-rw-rw-   0        0        0     3580 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.pyi
+-rw-rw-rw-   0        0        0     2690 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.py
+-rw-rw-rw-   0        0        0     5708 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.pyi
+-rw-rw-rw-   0        0        0     2108 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.py
+-rw-rw-rw-   0        0        0     5255 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.pyi
+-rw-rw-rw-   0        0        0     1063 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.py
+-rw-rw-rw-   0        0        0     5614 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.pyi
+-rw-rw-rw-   0        0        0      566 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.py
+-rw-rw-rw-   0        0        0     3155 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.pyi
+-rw-rw-rw-   0        0        0     1352 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.py
+-rw-rw-rw-   0        0        0     4321 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.pyi
+-rw-rw-rw-   0        0        0     1237 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.py
+-rw-rw-rw-   0        0        0     4153 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.pyi
+-rw-rw-rw-   0        0        0     1997 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.py
+-rw-rw-rw-   0        0        0     3945 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.pyi
+-rw-rw-rw-   0        0        0     2609 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.py
+-rw-rw-rw-   0        0        0     6106 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.pyi
+-rw-rw-rw-   0        0        0     2869 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.py
+-rw-rw-rw-   0        0        0     6439 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.pyi
+-rw-rw-rw-   0        0        0     1763 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.py
+-rw-rw-rw-   0        0        0    15141 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.pyi
+-rw-rw-rw-   0        0        0     1584 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.py
+-rw-rw-rw-   0        0        0     4426 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.pyi
+-rw-rw-rw-   0        0        0      738 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.py
+-rw-rw-rw-   0        0        0     3323 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.pyi
+-rw-rw-rw-   0        0        0    26581 2024-05-13 02:00:08.000000 reflex_antd-0.0.8/custom_components/reflex_antd/base.py
+-rw-rw-rw-   0        0        0    15233 2024-05-13 02:45:09.000000 reflex_antd-0.0.8/custom_components/reflex_antd/base.pyi
+-rw-rw-rw-   0        0        0     1919 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/constant.py
+-rw-rw-rw-   0        0        0      996 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/display.py
+-rw-rw-rw-   0        0        0      899 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/entry.py
+-rw-rw-rw-   0        0        0      515 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/feedback.py
+-rw-rw-rw-   0        0        0      289 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/general.py
+-rw-rw-rw-   0        0        0      163 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/helper.py
+-rw-rw-rw-   0        0        0      243 2024-05-11 09:33:47.000000 reflex_antd-0.0.8/custom_components/reflex_antd/layout.py
+-rw-rw-rw-   0        0        0      288 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/navigation.py
+-rw-rw-rw-   0        0        0     1654 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/util.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.812598 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/
+-rw-rw-rw-   0        0        0     1095 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6944 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      822 2024-05-13 02:39:38.000000 reflex_antd-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:45:24.815598 reflex_antd-0.0.8/setup.cfg
```

### Comparing `reflex_antd-0.0.7/LICENSE` & `reflex_antd-0.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
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
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `reflex_antd-0.0.7/PKG-INFO` & `reflex_antd-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1
-Name: reflex-antd
-Version: 0.0.7
-Summary: Reflex custom component antd
-Author-email: seewind <seewindcn@gmail.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: source, https://github.com/seewindcn/reflex-antd
-Keywords: reflex,reflex-custom-components
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.2
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# reflex-antd
-
-A Reflex custom component wrap [ant.design](https://ant.design/).
-
-## Installation
-
-```bash
-pip install reflex-antd
-```
-
-## antd-demo
-
-[antd-demo](https://antd-demo.reflex.run)
-
-
-### screen
-- table
-![table](docs/img/table1.png)
-- menu
-![menu1](docs/img/menu1.png)
-- transfer
-![transfer1](docs/img/transfer1.png)
-- ...
-
-
-
+Metadata-Version: 2.1
+Name: reflex-antd
+Version: 0.0.8
+Summary: Reflex custom component antd
+Author-email: seewind <seewindcn@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: source, https://github.com/seewindcn/reflex-antd
+Keywords: reflex,reflex-custom-components,ant-design,antd
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: reflex>=0.4.2
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# reflex-antd
+
+A Reflex custom component wrap [ant.design](https://ant.design/).
+pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
+
+## Installation
+
+```bash
+pip install reflex-antd
+```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import OrientationType, DirectionType
-
-
-class Affix(AntdComponent):
-    tag = 'Affix'
-
-    offset_bottom: Optional[Var[int]]
-    offset_top: Optional[Var[int]]
-    target: Optional[Var[JsValue]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda affixed: [affixed],
-        })
-        return _triggers
-
-
-affix = Affix.create
-
-
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import OrientationType, DirectionType
+
+
+class Affix(AntdComponent):
+    tag = 'Affix'
+
+    offset_bottom: Optional[Var[int]]
+    offset_top: Optional[Var[int]]
+    target: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda affixed: [affixed],
+        })
+        return _triggers
+
+
+affix = Affix.create
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 affix = Affix.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType
-
-
-class Alert(AntdComponent):
-    tag = 'Alert'
-
-    action: Optional[Var[ReactNode]]
-    banner: Optional[Var[bool]]
-    closable: Optional[Var[Union[bool, dict]]]
-    description: Optional[ReactNode]
-    icon: Optional[ReactNode]
-    message: Optional[ReactNode]
-    show_icon: Optional[bool]
-    type: Optional[StatusType]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_close": lambda event: [],
-            "after_close": lambda: [],
-        })
-        return _triggers
-
-
-class AlertErrorBoundary(AntdComponent):
-    tag = 'Alert.ErrorBoundary'
-
-    description: Optional[ReactNode]
-    message: Optional[ReactNode]
-
-
-alert = Alert.create
-alert_error_boundary = AlertErrorBoundary.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType
+
+
+class Alert(AntdComponent):
+    tag = 'Alert'
+
+    action: Optional[Var[ReactNode]]
+    banner: Optional[Var[bool]]
+    closable: Optional[Var[Union[bool, dict]]]
+    description: Optional[ReactNode]
+    icon: Optional[ReactNode]
+    message: Optional[ReactNode]
+    show_icon: Optional[bool]
+    type: Optional[StatusType]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_close": lambda event: [],
+            "after_close": lambda: [],
+        })
+        return _triggers
+
+
+class AlertErrorBoundary(AntdComponent):
+    tag = 'Alert.ErrorBoundary'
+
+    description: Optional[ReactNode]
+    message: Optional[ReactNode]
+
+
+alert = Alert.create
+alert_error_boundary = AlertErrorBoundary.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AlertErrorBoundary(AntdComponent):
 
     @overload
     @classmethod
@@ -50,14 +47,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 alert = Alert.create
 alert_error_boundary = AlertErrorBoundary.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,47 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsNode
-from ..constant import OrientationType, DirectionType
-
-
-class Anchor(AntdComponent):
-    tag = 'Anchor'
-
-    affix: Optional[Var[bool]]
-    bounds: Optional[Var[int]]
-    get_container: Optional[Var[JsNode]]
-    get_current_anchor: Optional[Var[JsNode]]
-    offset_top: Optional[Var[int]]
-    show_ink_in_fixed: Optional[Var[bool]]
-    target_offset: Optional[Var[int]]
-    items: Optional[Var[Union[List, ContainVar]]]
-    direction: Optional[Var[DirectionType]]
-    replace: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda link: [link],
-            EventTriggers.ON_CLICK: lambda ev, link: [ev, link],
-        })
-        return _triggers
-
-
-anchor = Anchor.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar
+from ..constant import StatusType, SizeType
+
+
+class Checkbox(AntdComponent):
+    tag = "Checkbox"
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    default_checked: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    indeterminate: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+        })
+        return _triggers
+
+
+class CheckboxGroup(AntdComponent):
+    tag = 'Checkbox.Group'
+
+    default_value: Optional[Var[List[Union[int, str]]]]
+    disabled: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    options: Optional[Var[List[Union[str, int, Dict]]]]
+    value: Optional[Var[List[Union[int, str, bool]]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked_value: [checked_value],
+        })
+        return _triggers
+
+
+checkbox = Checkbox.create
+checkbox_group = CheckboxGroup.create
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 anchor = Anchor.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import VariantType, SizeType
-
-
-class AutoComplete(AntdComponent):
-    tag = "AutoComplete"
-
-    allow_clear: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    backfill: Optional[Var[bool]]
-    default_active_first_option: Optional[Var[bool]]
-    default_open: Optional[Var[bool]]
-    default_value: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    dropdown_match_select_width: Optional[Var[Union[bool, int]]]
-    filter_option: Optional[Var[bool]]
-    not_found_content: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    options: Optional[Var[list]]
-    placeholder: Optional[Var[str]]
-    status: Optional[Var[str]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_BLUR: lambda: [],
-            "on_dropdown_visible_change": lambda open: [open],
-            EventTriggers.ON_FOCUS: lambda: [],
-            "on_search": lambda value: [value],
-            EventTriggers.ON_SELECT: lambda value, option: [value, option],
-            "on_clear": lambda: [],
-        })
-        return _triggers
-
-
-auto_complete = AutoComplete.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import VariantType, SizeType
+
+
+class AutoComplete(AntdComponent):
+    tag = "AutoComplete"
+
+    allow_clear: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    backfill: Optional[Var[bool]]
+    default_active_first_option: Optional[Var[bool]]
+    default_open: Optional[Var[bool]]
+    default_value: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    dropdown_match_select_width: Optional[Var[Union[bool, int]]]
+    filter_option: Optional[Var[bool]]
+    not_found_content: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    options: Optional[Var[list]]
+    placeholder: Optional[Var[str]]
+    status: Optional[Var[str]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_BLUR: lambda: [],
+            "on_dropdown_visible_change": lambda open: [open],
+            EventTriggers.ON_FOCUS: lambda: [],
+            "on_search": lambda value: [value],
+            EventTriggers.ON_SELECT: lambda value, option: [value, option],
+            "on_clear": lambda: [],
+        })
+        return _triggers
+
+
+auto_complete = AutoComplete.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,38 +2,35 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import VariantType, SizeType
 
 class AutoComplete(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, backfill: Optional[Union[Var[bool], bool]]=None, default_active_first_option: Optional[Union[Var[bool], bool]]=None, default_open: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, dropdown_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, filter_option: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, options: Optional[Union[Var[list], list]]=None, placeholder: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_clear: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AutoComplete':
+    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, backfill: Optional[Union[Var[bool], bool]]=None, default_active_first_option: Optional[Union[Var[bool], bool]]=None, default_open: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, dropdown_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, filter_option: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, options: Optional[Union[Var[list], list]]=None, placeholder: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_clear: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AutoComplete':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 auto_complete = AutoComplete.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Avatar(AntdComponent):
-    tag = 'Avatar'
-
-    alt: Optional[Var[str]]
-    gap: Optional[Var[int]]
-    icon: Optional[Var[ReactNode]]
-    shape: Optional[Var[str]]
-    size: Optional[Var[Union[str, int, Dict]]]
-    src: Optional[Var[ReactNode]]
-    src_set: Optional[Var[str]]
-    draggable: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_error": lambda: [],
-        })
-        return _triggers
-
-
-class AvatarGroup(AntdComponent):
-    tag = 'Avatar.Group'
-
-    max_count: Optional[Var[int]]
-    max_popover_placement: Optional[Var[str]]
-    max_popover_trigger: Optional[Var[str]]
-    max_style: Optional[Var[Dict]]
-    size: Optional[Var[Union[str, int, Dict]]]
-    shape: Optional[Var[str]]
-
-
-avatar = Avatar.create
-avatar_group = AvatarGroup.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Avatar(AntdComponent):
+    tag = 'Avatar'
+
+    alt: Optional[Var[str]]
+    gap: Optional[Var[int]]
+    icon: Optional[Var[ReactNode]]
+    shape: Optional[Var[str]]
+    size: Optional[Var[Union[str, int, Dict]]]
+    src: Optional[Var[ReactNode]]
+    src_set: Optional[Var[str]]
+    draggable: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_error": lambda: [],
+        })
+        return _triggers
+
+
+class AvatarGroup(AntdComponent):
+    tag = 'Avatar.Group'
+
+    max_count: Optional[Var[int]]
+    max_popover_placement: Optional[Var[str]]
+    max_popover_trigger: Optional[Var[str]]
+    max_style: Optional[Var[Dict]]
+    size: Optional[Var[Union[str, int, Dict]]]
+    shape: Optional[Var[str]]
+
+
+avatar = Avatar.create
+avatar_group = AvatarGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
 from reflex import Component, Var
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 class Avatar(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, gap: Optional[Union[Var[int], int]]=None, icon: Optional[Union[Var[Component], Component]]=None, shape: Optional[Union[Var[str], str]]=None, size: Optional[Union[Var[Union[str, int, Dict]], Union[str, int, Dict]]]=None, src: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, src_set: Optional[Union[Var[str], str]]=None, draggable: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Avatar':
+    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, gap: Optional[Union[Var[int], int]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, shape: Optional[Union[Var[str], str]]=None, size: Optional[Union[Var[Union[str, int, Dict]], Union[str, int, Dict]]]=None, src: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, src_set: Optional[Union[Var[str], str]]=None, draggable: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Avatar':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class AvatarGroup(AntdComponent):
 
     @overload
     @classmethod
@@ -49,14 +46,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 avatar = Avatar.create
 avatar_group = AvatarGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,44 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var,Component
-
-from ..base import AntdComponent, NodeVar, VarDataMixin
-from ..constant import PlacementType, SizeType, BadgeStatusType
-
-
-class Badge(AntdComponent):
-    tag = "Badge"
-
-    color: Optional[Var[str]]
-    count: Optional[Var[Union[int, NodeVar]]]
-    dot: Optional[Var[bool]]
-    offset: Optional[Var[NodeVar]]
-    overflow_count: Optional[Var[int]]
-    show_zero: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[BadgeStatusType]]
-    text: Optional[Var[Union[str, Component]]]
-
-
-class BadgeRibbon(AntdComponent):
-    tag = 'Badge.Ribbon'
-
-    color: Optional[Var[str]]
-    placement: Optional[Var[PlacementType]]
-    text: Optional[Var[Union[str, NodeVar]]]
-
-
-badge = Badge.create
-badge_ribbon = BadgeRibbon.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import OrientationType, SizeType
+
+
+class Drawer(AntdComponent):
+    tag = 'Drawer'
+
+    auto_focus: Optional[Var[bool]]
+    class_name: Optional[Var[str]]
+    class_names: Optional[Var[ContainVar]]
+    close_icon: Optional[Var[Union[ReactNode, bool]]]
+    destroy_on_close: Optional[Var[bool]]
+    extra: Optional[Var[ReactNode]]
+    footer: Optional[Var[ReactNode]]
+    force_render: Optional[Var[bool]]
+    get_container: Optional[Var[Union[ContainVar, bool]]]
+    height: Optional[Var[Union[str, int]]]
+    keyboard: Optional[Var[bool]]
+    mask: Optional[Var[bool]]
+    mask_closable: Optional[Var[bool]]
+    placement: Optional[Var[OrientationType]]
+    push: Optional[Var[Union[bool, dict]]]
+    root_style: Optional[Var[dict]]
+    size: Optional[Var[SizeType]]
+    styles: Optional[Var[ContainVar]]
+    title: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    width: Optional[Var[Union[str, int]]]
+    z_index: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "after_open_change": lambda open: [open],
+            "on_close": lambda e: [e],
+        })
+        return _triggers
+
+
+drawer = Drawer.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,29 @@
 from ..base import AntdComponent, NodeVar, VarDataMixin
 from ..constant import PlacementType, SizeType, BadgeStatusType
 
 class Badge(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, color: Optional[Union[Var[str], str]]=None, count: Optional[Union[Var[Union[int, NodeVar]], Union[int, NodeVar]]]=None, dot: Optional[Union[Var[bool], bool]]=None, offset: Optional[Union[Var[NodeVar], NodeVar]]=None, overflow_count: Optional[Union[Var[int], int]]=None, show_zero: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['success', 'processing', 'default', 'error', 'warning']], Literal['success', 'processing', 'default', 'error', 'warning']]]=None, text: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Badge':
+    def create(cls, *children, color: Optional[Union[Var[str], str]]=None, count: Optional[Union[Var[Union[int, NodeVar]], Union[int, NodeVar]]]=None, dot: Optional[Union[Var[bool], bool]]=None, offset: Optional[Union[Var[NodeVar], NodeVar]]=None, overflow_count: Optional[Union[Var[int], int]]=None, show_zero: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['success', 'processing', 'default', 'error', 'warning']], Literal['success', 'processing', 'default', 'error', 'warning']]]=None, text: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Badge':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class BadgeRibbon(AntdComponent):
 
     @overload
     @classmethod
@@ -47,14 +44,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 badge = Badge.create
 badge_ribbon = BadgeRibbon.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/base.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from typing import Optional, Union, Dict
-from types import SimpleNamespace
-from functools import lru_cache
-
-import reflex as rx
-from reflex import Var, Component
-from reflex.vars import BaseVar, VarData
-from reflex.utils import imports
-
-
-from .. import base
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
-
-
-next_theme_var_data = VarData(  # type: ignore
-    imports={
-        f"next-themes": {imports.ImportVar(tag="useTheme")},
-        "react": {imports.ImportVar(tag="useContext")},
-        "antd": {imports.ImportVar(tag="theme", alias="AntdTheme")}
-    },
-    hooks={
-        f"const nextTheme = useTheme()": None,
-    },
-)
-next_theme_var = BaseVar(
-    _var_name='nextTheme.theme',
-    _var_type="str",
-    _var_data=next_theme_var_data,
-)
-light_theme_var = BaseVar(
-    _var_name='AntdTheme.defaultAlgorithm',
-)
-dark_theme_var = BaseVar(
-    _var_name='AntdTheme.darkAlgorithm',
-)
-
-
-def theme(**kwargs):
-    if 'algorithm' not in kwargs:
-        kwargs['algorithm'] = rx.cond(next_theme_var == 'dark', dark_theme_var, light_theme_var)
-    return ContainVar.create(**kwargs)
-
-
-class Locale(JsValue):
-
-    @property
-    def lang(self) -> str:
-        return self.value.replace("_", "")
-
-    def serialize(self) -> str:
-        return self.lang
-
-    def get_imports(self) -> imports.ImportDict:
-        return {
-            f'antd/locale/{self.value}': [imports.ImportVar(tag=self.lang, install=False, is_default=True)],
-        }
-
-
-class ConfigProvider(AntdComponent):
-    """Top level antd provider must be included in any app using antd components."""
-
-    tag = "ConfigProvider"
-    alias = "AntdConfigProvider"
-
-    auto_insert_space_in_button: Optional[Var[bool]]
-    component_disabled: Optional[Var[bool]]
-    component_size: Optional[Var[SizeType]]
-    csp: Optional[Var[ContainVar]]
-    direction: Optional[Var[str]]
-    get_popup_container: Optional[Var[JsValue]]
-    get_target_container: Optional[Var[JsValue]]
-    icon_prefix_cls: Optional[Var[str]]
-    locale: Optional[Var[Locale]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    popup_overflow: Optional[Var[str]]
-    prefix_cls: Optional[Var[str]]
-    render_empty: Optional[Var[JsValue]]
-    theme: Optional[Var[Union[Dict, ContainVar]]]
-    virtual: Optional[Var[bool]]
-    warning: Optional[Var[Dict]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        """Create a new ConfigProvider component.
-
-        Returns:
-            A new ConfigProvider component.
-        """
-        if 'theme' not in props:
-            theme = Var.create('theme.styles.global.body.antd', _var_is_local=False)
-            props['theme'] = theme
-
-        return super().create(
-            *children,
-            **props
-        )
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("/utils/theme.js", []).append(
-            imports.ImportVar(tag="theme", is_default=True),
-        )
-        _imports.setdefault("@ant-design/cssinjs", []).append(
-            imports.ImportVar(tag="Theme", alias='antdTheme'),
-        )
-        return _imports
-
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
-        """ support app router """
-        if base.APP_ROUTER:
-            return {
-                (170, "AntdRegistryProvider"): antd_registry_provider(),
-            }
-        else:
-            return {}
-
-
-class AntdRegistryProvider(Component):
-    library = "@ant-design/nextjs-registry"
-    tag = "AntdRegistry"
-
-
-config_provider = ConfigProvider.create
-antd_registry_provider = AntdRegistryProvider.create
-
+from typing import Optional, Union, Dict
+from types import SimpleNamespace
+from functools import lru_cache
+
+import reflex as rx
+from reflex import Var, Component
+from reflex.vars import BaseVar, VarData
+from reflex.utils import imports
+
+
+from .. import base
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType
+
+
+next_theme_var_data = VarData(  # type: ignore
+    imports={
+        f"next-themes": {imports.ImportVar(tag="useTheme")},
+        "react": {imports.ImportVar(tag="useContext")},
+        "antd": {imports.ImportVar(tag="theme", alias="AntdTheme")}
+    },
+    hooks={
+        f"const nextTheme = useTheme()": None,
+    },
+)
+next_theme_var = BaseVar(
+    _var_name='nextTheme.theme',
+    _var_type="str",
+    _var_data=next_theme_var_data,
+)
+light_theme_var = BaseVar(
+    _var_name='AntdTheme.defaultAlgorithm',
+)
+dark_theme_var = BaseVar(
+    _var_name='AntdTheme.darkAlgorithm',
+)
+
+
+def theme(**kwargs):
+    if 'algorithm' not in kwargs:
+        kwargs['algorithm'] = rx.cond(next_theme_var == 'dark', dark_theme_var, light_theme_var)
+    return ContainVar.create(**kwargs)
+
+
+class Locale(JsValue):
+
+    @property
+    def lang(self) -> str:
+        return self.value.replace("_", "")
+
+    def serialize(self) -> str:
+        return self.lang
+
+    def get_imports(self) -> imports.ImportDict:
+        return {
+            f'antd/locale/{self.value}': [imports.ImportVar(tag=self.lang, install=False, is_default=True)],
+        }
+
+
+class ConfigProvider(AntdComponent):
+    """Top level antd provider must be included in any app using antd components."""
+
+    tag = "ConfigProvider"
+    alias = "AntdConfigProvider"
+
+    auto_insert_space_in_button: Optional[Var[bool]]
+    component_disabled: Optional[Var[bool]]
+    component_size: Optional[Var[SizeType]]
+    csp: Optional[Var[ContainVar]]
+    direction: Optional[Var[str]]
+    get_popup_container: Optional[Var[JsValue]]
+    get_target_container: Optional[Var[JsValue]]
+    icon_prefix_cls: Optional[Var[str]]
+    locale: Optional[Var[Locale]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    popup_overflow: Optional[Var[str]]
+    prefix_cls: Optional[Var[str]]
+    render_empty: Optional[Var[JsValue]]
+    theme: Optional[Var[Union[Dict, ContainVar]]]
+    virtual: Optional[Var[bool]]
+    warning: Optional[Var[Dict]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        """Create a new ConfigProvider component.
+
+        Returns:
+            A new ConfigProvider component.
+        """
+        if 'theme' not in props:
+            theme = Var.create('theme.styles.global.body.antd', _var_is_local=False)
+            props['theme'] = theme
+
+        return super().create(
+            *children,
+            **props
+        )
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _imports.setdefault("/utils/theme.js", []).append(
+            imports.ImportVar(tag="theme", is_default=True),
+        )
+        _imports.setdefault("@ant-design/cssinjs", []).append(
+            imports.ImportVar(tag="Theme", alias='antdTheme'),
+        )
+        return _imports
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
+        """ support app router """
+        if base.APP_ROUTER:
+            return {
+                (170, "AntdRegistryProvider"): antd_registry_provider(),
+            }
+        else:
+            return {}
+
+
+class AntdRegistryProvider(Component):
+    library = "@ant-design/nextjs-registry"
+    tag = "AntdRegistry"
+
+
+config_provider = ConfigProvider.create
+antd_registry_provider = AntdRegistryProvider.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var
-
-from ..base import AntdComponent, ContainVar, ReactNode
-
-
-class Breadcrumb(AntdComponent):
-    tag = "Breadcrumb"
-
-    params: Optional[Var[dict]]
-    items: Optional[Var[Union[ContainVar, list]]]
-    separator: Optional[Var[ReactNode]]
-
-
-class RouteItemType(AntdComponent):
-    tag = "RouteItemType"
-
-    class_name: Optional[Var[str]]
-    href: Optional[Var[str]]
-    path: Optional[Var[str]]
-    title: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_click': lambda e: [e],
-        })
-        return _triggers
-
-
-breadcrumb = Breadcrumb.create
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+
+from ..base import AntdComponent, ContainVar, ReactNode
+
+
+class Breadcrumb(AntdComponent):
+    tag = "Breadcrumb"
+
+    params: Optional[Var[dict]]
+    items: Optional[Var[Union[ContainVar, list, Component]]]
+    separator: Optional[Var[ReactNode]]
+
+
+class RouteItemType(AntdComponent):
+    tag = "RouteItemType"
+
+    class_name: Optional[Var[str]]
+    href: Optional[Var[str]]
+    path: Optional[Var[str]]
+    title: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_click': lambda e: [e],
+        })
+        return _triggers
+
+
+breadcrumb = Breadcrumb.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
-from reflex import Var
+from reflex import Var, Component
 from ..base import AntdComponent, ContainVar, ReactNode
 
 class Breadcrumb(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, params: Optional[Union[Var[dict], dict]]=None, items: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, separator: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Breadcrumb':
+    def create(cls, *children, params: Optional[Union[Var[dict], dict]]=None, items: Optional[Union[Var[Union[ContainVar, list, Component]], Union[ContainVar, list, Component]]]=None, separator: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Breadcrumb':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class RouteItemType(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
@@ -49,13 +46,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 breadcrumb = Breadcrumb.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, ReactNode
-from ..constant import TypeType, ButtonShape, SizeType
-
-
-class Button(AntdComponent):
-    tag = "Button"
-
-    block: Optional[Var[bool]]
-    danger: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    ghost: Optional[Var[bool]]
-    href: Optional[Var[str]]
-    target: Optional[Var[str]]
-    html_type: Optional[Var[str]]
-    icon: Optional[Var[ReactNode]]
-    loading: Optional[Var[bool]]
-    shape: Optional[Var[ButtonShape]]
-    size: Optional[Var[SizeType]]
-    type: Optional[Var[TypeType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-button = Button.create
+from typing import Optional, List, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent
+
+
+class Pagination(AntdComponent):
+    tag = 'Pagination'
+
+    current: Optional[Var[int]]
+    default_current: Optional[Var[int]]
+    default_page_size: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    hide_on_single_page: Optional[Var[bool]]
+    page_size: Optional[Var[int]]
+    page_size_options: Optional[Var[List[int]]]
+    responsive: Optional[Var[bool]]
+    show_less_items: Optional[Var[bool]]
+    show_quick_jumper: Optional[Var[bool]]
+    show_size_changer: Optional[Var[bool]]
+    show_title: Optional[Var[bool]]
+    # showTotal
+    simple: Optional[Var[bool]]
+    size: Optional[Var[int]]
+    total: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda page, page_size: [page, page_size],
+            "show_total": lambda total,range: [total,range],
+        })
+        return _triggers
+
+
+pagination = Pagination.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any
+from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, ReactNode
-from ..constant import TypeType, ButtonShape, SizeType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
 
-class Button(AntdComponent):
+class Switch(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, danger: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, ghost: Optional[Union[Var[bool], bool]]=None, href: Optional[Union[Var[str], str]]=None, target: Optional[Union[Var[str], str]]=None, html_type: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, loading: Optional[Union[Var[bool], bool]]=None, shape: Optional[Union[Var[Literal['default', 'circle', 'round']], Literal['default', 'circle', 'round']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Button':
+    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, checked_children: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, loading: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, un_checked_children: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, value: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Switch':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-button = Button.create
+switch = Switch.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue
-from reflex.constants import EventTriggers
-from .base import Locale
-from reflex.utils import imports
-
-
-class DayJS(JsValue):
-    def serialize(self) -> str:
-        return f"dayjs('{self.value}')"
-
-
-class Calendar(AntdComponent):
-    tag = 'Calendar'
-
-    cell_render: Optional[Var[JsValue]]
-    full_cell_render: Optional[Var[JsValue]]
-    default_value: Optional[Var[JsValue]]
-    disabled_date: Optional[Var[JsValue]]
-    fullscreen: Optional[Var[bool]]
-    header_render: Optional[Var[JsValue]]
-    locale: Optional[Var[Locale]]
-    mode: Optional[Var[str]]
-    value: Optional[Var[JsValue]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_select': lambda value, mode: [value, mode],
-            'on_panel_change': lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("dayjs", []).append(
-            imports.ImportVar(tag="dayjs", is_default=True, install=False),
-        )
-        return _imports
-
-
-dayjs = DayJS
-calendar = Calendar.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue
+from reflex.constants import EventTriggers
+from .base import Locale
+from reflex.utils import imports
+
+
+class DayJS(JsValue):
+    def serialize(self) -> str:
+        return f"dayjs('{self.value}')"
+
+
+class Calendar(AntdComponent):
+    tag = 'Calendar'
+
+    cell_render: Optional[Var[JsValue]]
+    full_cell_render: Optional[Var[JsValue]]
+    default_value: Optional[Var[JsValue]]
+    disabled_date: Optional[Var[JsValue]]
+    fullscreen: Optional[Var[bool]]
+    header_render: Optional[Var[JsValue]]
+    locale: Optional[Var[Locale]]
+    mode: Optional[Var[str]]
+    value: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_select': lambda value, mode: [value, mode],
+            'on_panel_change': lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _imports.setdefault("dayjs", []).append(
+            imports.ImportVar(tag="dayjs", is_default=True, install=False),
+        )
+        return _imports
+
+
+dayjs = DayJS
+calendar = Calendar.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 dayjs = DayJS
 calendar = Calendar.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,44 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Card(AntdComponent):
-    tag = 'Card'
-
-    actions: Optional[Var[ContainVar]]
-    active_tab_key: Optional[Var[str]]
-    bordered: Optional[Var[bool]]
-    cover: Optional[Var[ReactNode]]
-    default_active_tab_key: Optional[Var[str]]
-    extra: Optional[Var[ReactNode]]
-    hoverable: Optional[Var[bool]]
-    loading: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    tab_bar_extra_content: Optional[Var[ReactNode]]
-    tab_list: Optional[Var[list[ContainVar]]]
-    title: Optional[Var[ReactNode]]
-    type: Optional[Var[str]]
-    tab_props: Optional[Var[Union[ContainVar, dict]]]
-    class_names: Optional[Var[dict]]
-    styles: Optional[Var[dict]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_tab_change': lambda key: [key],
-        })
-        return _triggers
-
-
-class CardGrid(AntdComponent):
-    tag = 'Card.Grid'
-
-    hoverable: Optional[Var[bool]]
-
-
-class CardMeta(AntdComponent):
-    tag = 'Card.Meta'
-
-    avatar: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    title: Optional[Var[ReactNode]]
-
-
-card = Card.create
-card_grid = CardGrid.create
-card_meta = CardMeta.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType
+
+
+class AList(AntdComponent):
+    tag = 'List'
+
+    bordered: Optional[Var[bool]]
+    data_source: Optional[Var[Any]]
+    footer: Optional[Var[ReactNode]]
+    grid: Optional[Var[dict]]
+    header: Optional[Var[ReactNode]]
+    item_layout: Optional[Var[str]]
+    loading: Optional[Var[Union[bool, dict]]]
+    load_more: Optional[Var[ReactNode]]
+    locale: Optional[Var[dict]]
+    pagination: Optional[Var[Union[bool, dict]]]
+    render_item: Optional[Var[JsValue]]
+    size: Optional[Var[SizeType]]
+    split: Optional[Var[bool]]
+
+
+class ListItem(AntdComponent):
+    tag = 'List.Item'
+
+    actions: Optional[Var[list[ContainVar]]]
+    extra: Optional[Var[ReactNode]]
+
+
+class ListItemMeta(AntdComponent):
+    tag = 'List.Item.Meta'
+
+    avatar: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
+
+
+alist = AList.create
+list_item = ListItem.create
+list_item_meta = ListItemMeta.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,88 +1,81 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
-from reflex import Component, Var
+from reflex import Var, Component
+from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, RadioStyleType, RadioType
 
-class Card(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Radio(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, actions: Optional[Union[Var[ContainVar], ContainVar]]=None, active_tab_key: Optional[Union[Var[str], str]]=None, bordered: Optional[Union[Var[bool], bool]]=None, cover: Optional[Union[Var[Component], Component]]=None, default_active_tab_key: Optional[Union[Var[str], str]]=None, extra: Optional[Union[Var[Component], Component]]=None, hoverable: Optional[Union[Var[bool], bool]]=None, loading: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, tab_bar_extra_content: Optional[Union[Var[Component], Component]]=None, tab_list: Optional[Union[Var[list[ContainVar]], list[ContainVar]]]=None, title: Optional[Union[Var[Component], Component]]=None, type: Optional[Union[Var[str], str]]=None, tab_props: Optional[Union[Var[Union[ContainVar, dict]], Union[ContainVar, dict]]]=None, class_names: Optional[Union[Var[dict], dict]]=None, styles: Optional[Union[Var[dict], dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Card':
+    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Radio':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CardGrid(AntdComponent):
+class RadioButton(Radio):
 
     @overload
     @classmethod
-    def create(cls, *children, hoverable: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CardGrid':
+    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RadioButton':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CardMeta(AntdComponent):
+class RadioGroup(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, avatar: Optional[Union[Var[Component], Component]]=None, description: Optional[Union[Var[Component], Component]]=None, title: Optional[Union[Var[Component], Component]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CardMeta':
+    def create(cls, *children, button_style: Optional[Union[Var[Literal['outline', 'solid']], Literal['outline', 'solid']]]=None, default_value: Optional[Union[Var[Any], Any]]=None, disabled: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[Union[List[Union[str, int]], ContainVar]], Union[List[Union[str, int]], ContainVar]]]=None, optionType: Optional[Union[Var[Literal['default', 'button']], Literal['default', 'button']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RadioGroup':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-card = Card.create
-card_grid = CardGrid.create
-card_meta = CardMeta.create
+radio = Radio.create
+radio_button = RadioButton.create
+radio_group = RadioGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue
-
-
-class Carousel(AntdComponent):
-    tag = 'Carousel'
-
-    autoplay: Optional[Var[bool]]
-    autoplay_speed: Optional[Var[int]]
-    dot_position: Optional[Var[str]]
-    dots: Optional[Var[Union[bool, dict]]]
-    fade: Optional[Var[bool]]
-    infinite: Optional[Var[bool]]
-    speed: Optional[Var[int]]
-    easing: Optional[Var[str]]
-    wait_for_animate: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'after_change': lambda current: [],
-            'before_change': lambda current, next: [],
-        })
-        return _triggers
-
-
-carousel = Carousel.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TypeType
+
+class Popconfirm(AntdComponent):
+    tag = 'Popconfirm'
+
+    cancel_button_orops: Optional[Var[dict]]
+    cancel_text: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    icon: Optional[Var[ReactNode]]
+    ok_button_props: Optional[Var[dict]]
+    ok_text: Optional[Var[str]]
+    ok_type: Optional[Var[TypeType]]
+    open: Optional[Var[bool]]
+    show_cancel: Optional[Var[bool]]
+    title: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_cancel": lambda e: [e],
+            "on_confirm": lambda e: [e],
+            "on_popup_click": lambda e: [e],
+        })
+        return _triggers
+
+
+popconfirm = Popconfirm.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 carousel = Carousel.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,73 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
-
-
-class Cascader(AntdComponent):
-    tag = 'Cascader'
-
-    allow_clear: Optional[Var[bool]]
-    auto_clear_search_value: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    change_on_select: Optional[Var[bool]]
-    default_value: Optional[Var[Union[List[int], List[str]]]]
-    disabled: Optional[Var[bool]]
-    display_render: Optional[Var[JsValue]]
-    tag_render: Optional[Var[JsValue]]
-    popup_class_name: Optional[Var[str]]
-    dropdown_render: Optional[Var[JsValue]]
-    expand_icon: Optional[Var[ReactNode]]
-    expand_trigger: Optional[Var[TriggerType]]
-    field_names: Optional[Var[ContainVar]]
-    get_popup_container: Optional[Var[JsValue]]
-    load_data: Optional[Var[JsValue]]
-    max_tag_count: Optional[Var[int]]
-    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
-    max_tag_text_length: Optional[Var[int]]
-    not_found_content: Optional[Var[str]]
-    open: Optional[Var[bool]]
-    options: Optional[Var[Union[ContainVar, list]]]
-    placeholder: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    show_search: Optional[Var[Union[bool, ContainVar]]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    value: Optional[Var[Union[List[str], List[int]]]]
-    variant: Optional[Var[VariantType]]
-    multiple: Optional[Var[bool]]
-    remove_icon: Optional[Var[ReactNode]]
-    show_checked_strategy: Optional[Var[str]]
-    search_value: Optional[Var[str]]
-    dropdown_menu_column_style: Optional[Var[ContainVar]]
-    loading_icon: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, options: [value, options],
-            "on_dropdown_visible_change": lambda value: [value],
-            "on_search": lambda search: [search]
-        })
-        return _triggers
-
-
-cascader = Cascader.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+
+
+class Select(AntdComponent):
+    tag = 'Select'
+
+    allow_clear: Optional[Var[bool]]
+    auto_clear_search_value: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    default_active_first_option: Optional[Var[bool]]
+    default_open: Optional[Var[bool]]
+    default_value: Optional[Var[Union[int, str, List[str], List[int], ContainVar]]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    dropdown_render: Optional[Var[JsValue]]
+    dropdown_style: Optional[Var[Dict]]
+    field_names: Optional[Var[Dict]]
+    filter_option: Optional[Var[Union[bool, JsValue]]]
+    filter_sort: Optional[Var[JsValue]]
+    get_popup_container: Optional[Var[JsValue]]
+    label_in_value: Optional[Var[bool]]
+    list_height: Optional[Var[int]]
+    loading: Optional[Var[bool]]
+    max_count: Optional[Var[int]]
+    max_tag_count: Optional[Var[Union[int, str]]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
+    max_tag_text_length: Optional[Var[int]]
+    menu_item_selected_icon: Optional[Var[ReactNode]]
+    mode: Optional[Var[SelectModeType]]
+    not_found_content: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    option_filter_prop: Optional[Var[str]]
+    option_label_prop: Optional[Var[str]]
+    options: Optional[Var[Union[list, ContainVar]]]
+    option_render: Optional[Var[JsValue]]
+    placeholder: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    remove_icon: Optional[Var[ReactNode]]
+    search_value: Optional[Var[str]]
+    show_search: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    tag_render: Optional[Var[JsValue]]
+    label_render: Optional[Var[JsValue]]
+    token_separators: Optional[Var[List[str]]]
+    value: Optional[Var[Union[str, int, List[str], List[int], ContainVar]]]
+    variant: Optional[Var[VariantType]]
+    virtual: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda v, option: [v, option],
+            "on_clear": lambda: [],
+            "on_deselect": lambda v: [v],
+            "on_dropdown_visible_change": lambda open: [open],
+            "on_input_key_down": lambda: [],
+            "on_popup_scroll": lambda: [],
+            "on_search": lambda v: [v],
+            "on_select": lambda v, option: [v, option],
+        })
+        return _triggers
+
+
+select = Select.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Component, Var
+from typing import Optional, Union, Dict, Any, List, Tuple
+from dataclasses import dataclass
+from reflex import Component, Var, Base
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType, PlacementType, TabsType
 
-class Cascader(AntdComponent):
+@dataclass(frozen=True)
+class TabItem:
+    close_icon: Optional[Var[ReactNode]]
+    destroy_inactive_tab_pane: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    force_render: Optional[Var[bool]]
+    key: Optional[Union[str, Var[str]]]
+    label: Optional[Union[ReactNode, Var[ReactNode]]]
+    icon: Optional[Var[ReactNode]]
+    children: Optional[Union[ReactNode, Var[ReactNode]]]
+    closable: Optional[Var[bool]]
+
+class Tabs(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, change_on_select: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[List[int], List[str]]], Union[List[int], List[str]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, display_render: Optional[Union[Var[JsValue], JsValue]]=None, tag_render: Optional[Union[Var[JsValue], JsValue]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, dropdown_render: Optional[Union[Var[JsValue], JsValue]]=None, expand_icon: Optional[Union[Var[Component], Component]]=None, expand_trigger: Optional[Union[Var[Literal['click', 'hover', 'focus', 'contextMenu']], Literal['click', 'hover', 'focus', 'contextMenu']]]=None, field_names: Optional[Union[Var[ContainVar], ContainVar]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, load_data: Optional[Union[Var[JsValue], JsValue]]=None, max_tag_count: Optional[Union[Var[int], int]]=None, max_tag_placeholder: Optional[Union[Var[Union[Component, JsValue]], Union[Component, JsValue]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, not_found_content: Optional[Union[Var[str], str]]=None, open: Optional[Union[Var[bool], bool]]=None, options: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, placeholder: Optional[Union[Var[str], str]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, show_search: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, value: Optional[Union[Var[Union[List[int], List[str]]], Union[List[int], List[str]]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, multiple: Optional[Union[Var[bool], bool]]=None, remove_icon: Optional[Union[Var[Component], Component]]=None, show_checked_strategy: Optional[Union[Var[str], str]]=None, search_value: Optional[Union[Var[str], str]]=None, dropdown_menu_column_style: Optional[Union[Var[ContainVar], ContainVar]]=None, loading_icon: Optional[Union[Var[Component], Component]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Cascader':
+    def create(cls, *children, active_key: Optional[Union[Var[str], str]]=None, add_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, animated: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, centered: Optional[Union[Var[bool], bool]]=None, default_active_key: Optional[Union[Var[str], str]]=None, hide_add: Optional[Union[Var[bool], bool]]=None, indicator: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, items: Optional[Union[Var[Union[ContainVar, List]], Union[ContainVar, List]]]=None, more_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, remove_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, render_tab_bar: Optional[Union[Var[JsValue], JsValue]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, tab_bar_extra_content: Optional[Union[Var[Union[str, Component, ContainVar]], Union[str, Component, ContainVar]]]=None, tab_bar_gutter: Optional[Union[Var[int], int]]=None, tab_bar_style: Optional[Union[Var[Dict], Dict]]=None, tab_position: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, destroy_inactive_tab_pane: Optional[Union[Var[bool], bool]]=None, type: Optional[Union[Var[Literal['line', 'card', 'editable-card']], Literal['line', 'card', 'editable-card']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_edit: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tabs':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-cascader = Cascader.create
+tabs = Tabs.create
+tab_item = TabItem
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,55 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var
-from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar
-from ..constant import StatusType, SizeType
+from typing import Optional, Union, Dict
+from reflex import Component, Var
+from reflex.utils import imports
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import AlignType, DirectionType, SizeType
 
-class Checkbox(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Space(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, indeterminate: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Checkbox':
+    def create(cls, *children, align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, class_names: Optional[Union[Var[Dict], Dict]]=None, direction: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, split: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, styles: Optional[Union[Var[Dict], Dict]]=None, wrap: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Space':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CheckboxGroup(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class SpaceCompact(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, default_value: Optional[Union[Var[List[Union[str, int]]], List[Union[str, int]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[List[Union[str, int, Dict]]], List[Union[str, int, Dict]]]]=None, value: Optional[Union[Var[List[Union[int, str, bool]]], List[Union[int, str, bool]]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckboxGroup':
+    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, direction: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'SpaceCompact':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-checkbox = Checkbox.create
-checkbox_group = CheckboxGroup.create
+space = Space.create
+space_compact = SpaceCompact.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Collapse(AntdComponent):
-    tag = 'Collapse'
-
-    accordion: Optional[Var[bool]]
-    active_key: Optional[Var[Union[list[str], str, list[int], int]]]
-    bordered: Optional[Var[bool]]
-    default_active_key: Optional[Var[Union[list[str], str, list[int], int]]]
-    destroy_inactive_panel: Optional[Var[bool]]
-    expand_icon: Optional[Var[ReactNode]]
-    collapsible: Optional[Var[str]]
-    expand_icon_position: Optional[Var[str]]
-    ghost: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    items: Optional[Var[Union[ContainVar, list]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_change': lambda: [],
-        })
-        return _triggers
-
-
-collapse = Collapse.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+
+
+class Slider(AntdComponent):
+    tag = 'Slider'
+
+    auto_adjust_overflow: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    default_value: Optional[Var[Union[int, List[int]]]]
+    disabled: Optional[Var[bool]]
+    keyboard: Optional[Var[bool]]
+    dots: Optional[Var[bool]]
+    included: Optional[Var[bool]]
+    marks: Optional[Var[Union[Dict, ContainVar]]]
+    max: Optional[Var[int]]
+    min: Optional[Var[int]]
+    range: Optional[Var[bool]]
+    reverse: Optional[Var[bool]]
+    step: Optional[Var[int]]
+    tooltip: Optional[Var[Union[Dict, ContainVar]]]
+    value: Optional[Var[Union[int, List[int]]]]
+    vertical: Optional[Var[bool]]
+    # range
+    draggable_track: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_change_complete": lambda v: [v],
+            EventTriggers.ON_CHANGE: lambda v: [v],
+        })
+        return _triggers
+
+
+slider = Slider.create
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Component, Var
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 class Collapse(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, accordion: Optional[Union[Var[bool], bool]]=None, active_key: Optional[Union[Var[Union[list[str], str, list[int], int]], Union[list[str], str, list[int], int]]]=None, bordered: Optional[Union[Var[bool], bool]]=None, default_active_key: Optional[Union[Var[Union[list[str], str, list[int], int]], Union[list[str], str, list[int], int]]]=None, destroy_inactive_panel: Optional[Union[Var[bool], bool]]=None, expand_icon: Optional[Union[Var[Component], Component]]=None, collapsible: Optional[Union[Var[str], str]]=None, expand_icon_position: Optional[Union[Var[str], str]]=None, ghost: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, items: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Collapse':
+    def create(cls, *children, accordion: Optional[Union[Var[bool], bool]]=None, active_key: Optional[Union[Var[Union[list[str], str, list[int], int]], Union[list[str], str, list[int], int]]]=None, bordered: Optional[Union[Var[bool], bool]]=None, default_active_key: Optional[Union[Var[Union[list[str], str, list[int], int]], Union[list[str], str, list[int], int]]]=None, destroy_inactive_panel: Optional[Union[Var[bool], bool]]=None, expand_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, collapsible: Optional[Union[Var[str], str]]=None, expand_icon_position: Optional[Union[Var[str], str]]=None, ghost: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, items: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Collapse':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 collapse = Collapse.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue,ReactNode
-from ..constant import ColorFormatType, SizeType, PlacementType, TriggerType
-
-
-class ColorPicker(AntdComponent):
-    tag = 'ColorPicker'
-
-    allow_clear: Optional[Var[bool]]
-    arrow: Optional[Var[bool]]
-    default_value: Optional[Var[str]]
-    default_format: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    disabled_alpha: Optional[Var[bool]]
-    destroy_tooltip_on_hide: Optional[Var[bool]]
-    format: Optional[Var[ColorFormatType]]
-    open: Optional[Var[bool]]
-    presets: Optional[Var[ContainVar]]
-    placement: Optional[Var[PlacementType]]
-    panel_render: Optional[Var[JsValue]]
-    show_text: Optional[Var[Union[bool, JsValue]]]
-    size: Optional[Var[SizeType]]
-    trigger: Optional[Var[TriggerType]]
-    value: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, hex: [value, hex],
-            'on_change_complete': lambda value: [value],
-            'on_format_change': lambda format: [format],
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-            'on_clear': lambda: [],
-        })
-        return _triggers
-
-
-color_picker = ColorPicker.create
-
-
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType, PlacementType
+
+
+class Mention(AntdComponent):
+    tag = 'Mention'
+
+    allow_clear: Optional[Var[Union[bool, ContainVar]]]
+    auto_focus: Optional[Var[bool]]
+    auto_size: Optional[Var[Union[bool, Dict]]]
+    default_value: Optional[Var[str]]
+    filter_option: Optional[Var[Union[bool, JsValue]]]
+    get_popup_container: Optional[Var[JsValue]]
+    not_found_content: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    prefix: Optional[Var[Union[str, List[str]]]]
+    split: Optional[Var[str]]
+    status: Optional[Var[StatusType]]
+    validate_search: Optional[Var[JsValue]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+    options: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda text: [text],
+            "on_resize": lambda ev: [ev],
+            'on_search': lambda text, prefix: [text, prefix],
+            "on_select": lambda option, prefix: [option, prefix],
+        })
+        return _triggers
+
+
+mention = Mention.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,13 +26,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 color_picker = ColorPicker.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
-
-from .base import Locale
-
-
-class DayJS(JsValue):
-    def serialize(self) -> str:
-        return f"dayjs('{self.value}')"
-
-
-class BaseDatePicker(AntdComponent):
-
-    allow_clear: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    date_render: Optional[Var[JsValue]]
-    cell_render: Optional[Var[JsValue]]
-    components: Optional[Var[Union[ReactNode, list, dict, ContainVar]]]
-    disabled: Optional[Var[bool]]
-    disabled_date: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    order: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    preserve_invalidOn_blur: Optional[Var[bool]]
-    getPopup_container: Optional[Var[JsValue]]
-    input_readOnly: Optional[Var[bool]]
-    locale: Optional[Var[Locale]]
-    min_date: Optional[Var[JsValue]]
-    max_date: Optional[Var[JsValue]]
-    mode: Optional[Var[DatePickerModeType]]
-    need_confirm: Optional[Var[bool]]
-    next_icon: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    panel_render: Optional[Var[JsValue]]
-    picker: Optional[Var[DatePickerType]]
-    placeholder: Optional[Var[Union[str, List[str]]]]
-    placement: Optional[Var[PlacementType]]
-    popup_style: Optional[Var[ContainVar]]
-    presets: Optional[Var[ContainVar]]
-    prev_icon: Optional[Var[ReactNode]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    super_next_icon: Optional[Var[ReactNode]]
-    super_prev_icon: Optional[Var[ReactNode]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-            'on_panel_change': lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("dayjs", []).append(
-            imports.ImportVar(tag="dayjs", is_default=True, install=False),
-        )
-        return _imports
-
-
-class DatePicker(BaseDatePicker):
-    tag = 'DatePicker'
-
-    default_picker_value: Optional[Var[JsValue]]
-    default_value: Optional[Var[ContainVar]]
-    disabled_time: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    multiple: Optional[Var[bool]]
-    picker_value: Optional[Var[ContainVar]]
-    render_extra_footer: Optional[Var[JsValue]]
-    show_now: Optional[Var[bool]]
-    show_time: Optional[Var[Union[bool, ContainVar]]]
-    # showTime.defaultValue
-    show_week: Optional[Var[bool]]
-    value: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda date, sdate: [date, sdate],
-            "on_ok": lambda: [],
-            "on_panel_change": lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-
-class RangePicker(BaseDatePicker):
-    tag = 'RangePicker'
-
-    allow_empty: Optional[Var[Tuple[bool, bool]]]
-    cell_render: Optional[Var[JsValue]]
-    date_render: Optional[Var[JsValue]]
-    default_picker_value: Optional[Var[ContainVar]]
-    default_value: Optional[Var[ContainVar]]
-    disabled: Optional[Var[Tuple[bool, bool]]]
-    disabled_time: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    id: Optional[Var[Dict[str, str]]]
-    picker_value: Optional[Var[ContainVar]]
-    presets: Optional[Var[ContainVar]]
-    render_extra_footer: Optional[Var[JsValue]]
-    separator: Optional[Var[ReactNode]]
-    show_time: Optional[Var[Union[bool, ContainVar]]]
-    # showTime.defaultValue
-    value: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_calendar_change": lambda dates, sdates, info: [dates, sdates, info],
-            EventTriggers.ON_CHANGE: lambda dates, sdates: [dates, sdates],
-            EventTriggers.ON_FOCUS: lambda ev, range: [ev, range],
-            EventTriggers.ON_BLUR: lambda ev, range: [ev, range],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _vars: List = [v for v in _imports[self.library] if v.tag != "RangePicker"]
-        _vars.append(
-            imports.ImportVar(tag="DatePicker"),
-        )
-        _imports[self.library] = _vars
-
-        return _imports
-
-    def _get_hooks(self) -> str | None:
-        return "const { RangePicker } = DatePicker;"
-
-
-dayjs = DayJS
-date_picker = DatePicker.create
-range_picker = RangePicker.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
+
+from .base import Locale
+
+
+class DayJS(JsValue):
+    def serialize(self) -> str:
+        return f"dayjs('{self.value}')"
+
+
+class BaseDatePicker(AntdComponent):
+
+    allow_clear: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    date_render: Optional[Var[JsValue]]
+    cell_render: Optional[Var[JsValue]]
+    components: Optional[Var[Union[ReactNode, list, dict, ContainVar]]]
+    disabled: Optional[Var[bool]]
+    disabled_date: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    order: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    preserve_invalidOn_blur: Optional[Var[bool]]
+    getPopup_container: Optional[Var[JsValue]]
+    input_readOnly: Optional[Var[bool]]
+    locale: Optional[Var[Locale]]
+    min_date: Optional[Var[JsValue]]
+    max_date: Optional[Var[JsValue]]
+    mode: Optional[Var[DatePickerModeType]]
+    need_confirm: Optional[Var[bool]]
+    next_icon: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    panel_render: Optional[Var[JsValue]]
+    picker: Optional[Var[DatePickerType]]
+    placeholder: Optional[Var[Union[str, List[str]]]]
+    placement: Optional[Var[PlacementType]]
+    popup_style: Optional[Var[ContainVar]]
+    presets: Optional[Var[ContainVar]]
+    prev_icon: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    super_next_icon: Optional[Var[ReactNode]]
+    super_prev_icon: Optional[Var[ReactNode]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+            'on_panel_change': lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _imports.setdefault("dayjs", []).append(
+            imports.ImportVar(tag="dayjs", is_default=True, install=False),
+        )
+        return _imports
+
+
+class DatePicker(BaseDatePicker):
+    tag = 'DatePicker'
+
+    default_picker_value: Optional[Var[JsValue]]
+    default_value: Optional[Var[ContainVar]]
+    disabled_time: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    multiple: Optional[Var[bool]]
+    picker_value: Optional[Var[ContainVar]]
+    render_extra_footer: Optional[Var[JsValue]]
+    show_now: Optional[Var[bool]]
+    show_time: Optional[Var[Union[bool, ContainVar]]]
+    # showTime.defaultValue
+    show_week: Optional[Var[bool]]
+    value: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda date, sdate: [date, sdate],
+            "on_ok": lambda: [],
+            "on_panel_change": lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+
+class RangePicker(BaseDatePicker):
+    tag = 'RangePicker'
+
+    allow_empty: Optional[Var[Tuple[bool, bool]]]
+    cell_render: Optional[Var[JsValue]]
+    date_render: Optional[Var[JsValue]]
+    default_picker_value: Optional[Var[ContainVar]]
+    default_value: Optional[Var[ContainVar]]
+    disabled: Optional[Var[Tuple[bool, bool]]]
+    disabled_time: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    id: Optional[Var[Dict[str, str]]]
+    picker_value: Optional[Var[ContainVar]]
+    presets: Optional[Var[ContainVar]]
+    render_extra_footer: Optional[Var[JsValue]]
+    separator: Optional[Var[ReactNode]]
+    show_time: Optional[Var[Union[bool, ContainVar]]]
+    # showTime.defaultValue
+    value: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_calendar_change": lambda dates, sdates, info: [dates, sdates, info],
+            EventTriggers.ON_CHANGE: lambda dates, sdates: [dates, sdates],
+            EventTriggers.ON_FOCUS: lambda ev, range: [ev, range],
+            EventTriggers.ON_BLUR: lambda ev, range: [ev, range],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _vars: List = [v for v in _imports[self.library] if v.tag != "RangePicker"]
+        _vars.append(
+            imports.ImportVar(tag="DatePicker"),
+        )
+        _imports[self.library] = _vars
+
+        return _imports
+
+    def _get_hooks(self) -> str | None:
+        return "const { RangePicker } = DatePicker;"
+
+
+dayjs = DayJS
+date_picker = DatePicker.create
+range_picker = RangePicker.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
 from .base import Locale
 
 class DayJS(JsValue):
 
     def serialize(self) -> str:
         ...
@@ -18,43 +18,40 @@
 class BaseDatePicker(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, components: Optional[Union[Var[Component], Component]]=None, disabled: Optional[Union[Var[bool], bool]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, super_next_icon: Optional[Union[Var[Component], Component]]=None, super_prev_icon: Optional[Union[Var[Component], Component]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'BaseDatePicker':
+    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, components: Optional[Union[Var[Union[str, Component, list, dict, ContainVar]], Union[str, Component, list, dict, ContainVar]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'BaseDatePicker':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DatePicker(BaseDatePicker):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, default_picker_value: Optional[Union[Var[JsValue], JsValue]]=None, default_value: Optional[Union[Var[ContainVar], ContainVar]]=None, disabled_time: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, multiple: Optional[Union[Var[bool], bool]]=None, picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, render_extra_footer: Optional[Union[Var[JsValue], JsValue]]=None, show_now: Optional[Union[Var[bool], bool]]=None, show_time: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, show_week: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[ContainVar], ContainVar]]=None, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, components: Optional[Union[Var[Component], Component]]=None, disabled: Optional[Union[Var[bool], bool]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, super_next_icon: Optional[Union[Var[Component], Component]]=None, super_prev_icon: Optional[Union[Var[Component], Component]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_ok: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'DatePicker':
+    def create(cls, *children, default_picker_value: Optional[Union[Var[JsValue], JsValue]]=None, default_value: Optional[Union[Var[ContainVar], ContainVar]]=None, disabled_time: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, multiple: Optional[Union[Var[bool], bool]]=None, picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, render_extra_footer: Optional[Union[Var[JsValue], JsValue]]=None, show_now: Optional[Union[Var[bool], bool]]=None, show_time: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, show_week: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[ContainVar], ContainVar]]=None, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, components: Optional[Union[Var[Union[str, Component, list, dict, ContainVar]], Union[str, Component, list, dict, ContainVar]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_ok: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'DatePicker':
         """Create the component.
 
         Args:
             *children: The children of the component.
             show_week: showTime.defaultValue
             style: The style of the component.
             key: A unique key for the component.
@@ -62,28 +59,25 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class RangePicker(BaseDatePicker):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_empty: Optional[Union[Var[Tuple[bool, bool]], Tuple[bool, bool]]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, default_picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, default_value: Optional[Union[Var[ContainVar], ContainVar]]=None, disabled: Optional[Union[Var[Tuple[bool, bool]], Tuple[bool, bool]]]=None, disabled_time: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, id: Optional[Union[Var[Dict[str, str]], Dict[str, str]]]=None, picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, render_extra_footer: Optional[Union[Var[JsValue], JsValue]]=None, separator: Optional[Union[Var[Component], Component]]=None, show_time: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, value: Optional[Union[Var[ContainVar], ContainVar]]=None, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, components: Optional[Union[Var[Component], Component]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, super_next_icon: Optional[Union[Var[Component], Component]]=None, super_prev_icon: Optional[Union[Var[Component], Component]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_calendar_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RangePicker':
+    def create(cls, *children, allow_empty: Optional[Union[Var[Tuple[bool, bool]], Tuple[bool, bool]]]=None, cell_render: Optional[Union[Var[JsValue], JsValue]]=None, date_render: Optional[Union[Var[JsValue], JsValue]]=None, default_picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, default_value: Optional[Union[Var[ContainVar], ContainVar]]=None, disabled: Optional[Union[Var[Tuple[bool, bool]], Tuple[bool, bool]]]=None, disabled_time: Optional[Union[Var[JsValue], JsValue]]=None, format: Optional[Union[Var[ContainVar], ContainVar]]=None, id: Optional[Union[Var[Dict[str, str]], Dict[str, str]]]=None, picker_value: Optional[Union[Var[ContainVar], ContainVar]]=None, presets: Optional[Union[Var[ContainVar], ContainVar]]=None, render_extra_footer: Optional[Union[Var[JsValue], JsValue]]=None, separator: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, show_time: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, value: Optional[Union[Var[ContainVar], ContainVar]]=None, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, components: Optional[Union[Var[Union[str, Component, list, dict, ContainVar]], Union[str, Component, list, dict, ContainVar]]]=None, disabled_date: Optional[Union[Var[JsValue], JsValue]]=None, order: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, preserve_invalidOn_blur: Optional[Union[Var[bool], bool]]=None, getPopup_container: Optional[Union[Var[JsValue], JsValue]]=None, input_readOnly: Optional[Union[Var[bool], bool]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, min_date: Optional[Union[Var[JsValue], JsValue]]=None, max_date: Optional[Union[Var[JsValue], JsValue]]=None, mode: Optional[Union[Var[Literal['time', 'date', 'month', 'year', 'decade']], Literal['time', 'date', 'month', 'year', 'decade']]]=None, need_confirm: Optional[Union[Var[bool], bool]]=None, next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, panel_render: Optional[Union[Var[JsValue], JsValue]]=None, picker: Optional[Union[Var[Literal['date', 'week', 'month', 'quarter', 'year']], Literal['date', 'week', 'month', 'quarter', 'year']]]=None, placeholder: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, popup_style: Optional[Union[Var[ContainVar], ContainVar]]=None, prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_next_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, super_prev_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_calendar_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_panel_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RangePicker':
         """Create the component.
 
         Args:
             *children: The children of the component.
             value: showTime.defaultValue
             style: The style of the component.
             key: A unique key for the component.
@@ -91,15 +85,12 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 dayjs = DayJS
 date_picker = DatePicker.create
 range_picker = RangePicker.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue,ReactNode
-from ..constant import VariantType, SizeType,DirectionType
-
-
-class Descriptions(AntdComponent):
-    tag = 'Descriptions'
-
-    bordered: Optional[Var[bool]]
-    colon: Optional[Var[bool]]
-    column: Optional[Var[Union[int,dict]]]
-    content_style: Optional[Var[Union[dict,ContainVar]]]
-    extra: Optional[Var[ReactNode]]
-    items: Optional[Var[Union[ContainVar,list]]]
-    label_style: Optional[Var[dict]]
-    layout: Optional[Var[DirectionType]]
-    size: Optional[Var[SizeType]]
-    title: Optional[Var[ReactNode]]
-
-
-descriptions = Descriptions.create
+from typing import Optional, Union, Dict
+
+from reflex import Component, Var
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import AlignType, DirectionType, SizeType
+
+
+class Space(AntdComponent):
+    tag = 'Space'
+
+    align: Optional[Var[AlignType]]
+    class_names: Optional[Var[Dict]]
+    direction: Optional[Var[DirectionType]]
+    size: Optional[Var[SizeType]]
+    split: Optional[Var[ReactNode]]
+    styles: Optional[Var[Dict]]
+    wrap: Optional[Var[bool]]
+
+
+class SpaceCompact(AntdComponent):
+    tag = 'Space.Compact'
+
+    block: Optional[Var[bool]]
+    direction: Optional[Var[DirectionType]]
+    size: Optional[Var[SizeType]]
+
+
+space = Space.create
+space_compact = SpaceCompact.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 descriptions = Descriptions.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union
-from reflex import Component, Var
-from reflex.utils import imports
-from ..base import AntdComponent, AntdSubComponent, ReactNode
-from ..constant import OrientationType, DirectionType
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import TypeType, ButtonShape, SizeType
 
-class Divider(AntdComponent):
+class Button(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, dashed: Optional[Union[Var[bool], bool]]=None, orientation: Optional[Union[Var[Literal['left', 'right', 'top', 'bottom', 'center']], Literal['left', 'right', 'top', 'bottom', 'center']]]=None, orientation_margin: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, plain: Optional[Union[Var[bool], bool]]=None, type: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Divider':
+    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, danger: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, ghost: Optional[Union[Var[bool], bool]]=None, href: Optional[Union[Var[str], str]]=None, target: Optional[Union[Var[str], str]]=None, html_type: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, loading: Optional[Union[Var[bool], bool]]=None, shape: Optional[Union[Var[Literal['default', 'circle', 'round']], Literal['default', 'circle', 'round']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Button':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-divider = Divider.create
+button = Button.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import OrientationType, SizeType
-
-
-class Drawer(AntdComponent):
-    tag = 'Drawer'
-
-    auto_focus: Optional[Var[bool]]
-    class_name: Optional[Var[str]]
-    class_names: Optional[Var[ContainVar]]
-    close_icon: Optional[Var[Union[ReactNode, bool]]]
-    destroy_on_close: Optional[Var[bool]]
-    extra: Optional[Var[ReactNode]]
-    footer: Optional[Var[ReactNode]]
-    force_render: Optional[Var[bool]]
-    get_container: Optional[Var[Union[ContainVar, bool]]]
-    height: Optional[Var[Union[str, int]]]
-    keyboard: Optional[Var[bool]]
-    mask: Optional[Var[bool]]
-    mask_closable: Optional[Var[bool]]
-    placement: Optional[Var[OrientationType]]
-    push: Optional[Var[Union[bool, dict]]]
-    root_style: Optional[Var[dict]]
-    size: Optional[Var[SizeType]]
-    styles: Optional[Var[ContainVar]]
-    title: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    width: Optional[Var[Union[str, int]]]
-    z_index: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "after_open_change": lambda open: [open],
-            "on_close": lambda e: [e],
-        })
-        return _triggers
-
-
-drawer = Drawer.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, PlacementType, TypeType
+
+
+class Tour(AntdComponent):
+    tag = 'Tour'
+
+    arrow: Optional[Var[bool]]
+    close_icon: Optional[Var[ReactNode]]
+    disabled_interaction: Optional[Var[bool]]
+    placement: Optional[Var[PlacementType]]
+    mask: Optional[Var[Union[bool, Dict]]]
+    type: Optional[Var[TypeType]]
+    open: Optional[Var[bool]]
+    current: Optional[Var[int]]
+    scroll_into_view_options: Optional[Var[Union[bool, Dict]]]
+    steps: Optional[Var[ContainVar]]
+    indicators_render: Optional[Var[JsValue]]
+    z_index: Optional[Var[int]]
+    get_popup_container: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_close': lambda: [],
+            'on_finish': lambda: [],
+            EventTriggers.ON_CHANGE: lambda current: [current],
+            'steps.*.on_close': lambda: [],
+        })
+        return _triggers
+
+
+tour = Tour.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 drawer = Drawer.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import PlacementType, DirectionType
-
-
-class Dropdown(AntdComponent):
-    tag = 'Dropdown'
-
-    arrow: Optional[Var[bool]]
-    auto_adjust_overflow: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    destroy_popup_on_hide: Optional[Var[bool]]
-    dropdown_render: Optional[Var[JsValue]]
-    menu: Optional[Var[Union[ContainVar, list]]]
-    placement: Optional[Var[PlacementType]]
-    trigger: Optional[Var[ContainVar]]
-    open: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open, info: [open, info],
-        })
-        return _triggers
-
-
-class DropdownButton(Dropdown):
-    tag = 'Dropdown.Button'
-
-    buttons_render: Optional[Var[JsValue]]
-    loading: Optional[Var[bool]]
-    danger: Optional[Var[bool]]
-    icon: Optional[Var[ReactNode]]
-    size: Optional[Var[str]]
-    type: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-dropdown = Dropdown.create
-dropdown_button = DropdownButton.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import PlacementType, DirectionType
+
+
+class Dropdown(AntdComponent):
+    tag = 'Dropdown'
+
+    arrow: Optional[Var[bool]]
+    auto_adjust_overflow: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    destroy_popup_on_hide: Optional[Var[bool]]
+    dropdown_render: Optional[Var[JsValue]]
+    menu: Optional[Var[Union[ContainVar, list]]]
+    placement: Optional[Var[PlacementType]]
+    trigger: Optional[Var[ContainVar]]
+    open: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open, info: [open, info],
+        })
+        return _triggers
+
+
+class DropdownButton(Dropdown):
+    tag = 'Dropdown.Button'
+
+    buttons_render: Optional[Var[JsValue]]
+    loading: Optional[Var[bool]]
+    danger: Optional[Var[bool]]
+    icon: Optional[Var[ReactNode]]
+    size: Optional[Var[str]]
+    type: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+dropdown = Dropdown.create
+dropdown_button = DropdownButton.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import PlacementType, DirectionType
 
 class Dropdown(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
@@ -27,42 +27,36 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class DropdownButton(Dropdown):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, buttons_render: Optional[Union[Var[JsValue], JsValue]]=None, loading: Optional[Union[Var[bool], bool]]=None, danger: Optional[Union[Var[bool], bool]]=None, icon: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[str], str]]=None, type: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[bool], bool]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, destroy_popup_on_hide: Optional[Union[Var[bool], bool]]=None, dropdown_render: Optional[Union[Var[JsValue], JsValue]]=None, menu: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[ContainVar], ContainVar]]=None, open: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'DropdownButton':
+    def create(cls, *children, buttons_render: Optional[Union[Var[JsValue], JsValue]]=None, loading: Optional[Union[Var[bool], bool]]=None, danger: Optional[Union[Var[bool], bool]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[str], str]]=None, type: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[bool], bool]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, destroy_popup_on_hide: Optional[Union[Var[bool], bool]]=None, dropdown_render: Optional[Union[Var[JsValue], JsValue]]=None, menu: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[ContainVar], ContainVar]]=None, open: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'DropdownButton':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 dropdown = Dropdown.create
 dropdown_button = DropdownButton.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Component, Var
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 class Empty(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, description: Optional[Union[Var[Component], Component]]=None, image: Optional[Union[Var[Component], Component]]=None, image_style: Optional[Union[Var[dict], dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Empty':
+    def create(cls, *children, description: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, image: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, image_style: Optional[Union[Var[dict], dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Empty':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 empty = Empty.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union
 from reflex import Component, Var
 from reflex.utils import imports
-from ..base import AntdComponent, AntdSubComponent
+from ..base import AntdComponent, ReactNode
 from ..constant import OrientationType, DirectionType
 
-class Flex(AntdComponent):
+class Divider(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, vertical: Optional[Union[Var[bool], bool]]=None, wrap: Optional[Union[Var[str], str]]=None, justify: Optional[Union[Var[str], str]]=None, align: Optional[Union[Var[str], str]]=None, flex: Optional[Union[Var[str], str]]=None, gap: Optional[Union[Var[str], str]]=None, component: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Flex':
+    def create(cls, *children, dashed: Optional[Union[Var[bool], bool]]=None, orientation: Optional[Union[Var[Literal['left', 'right', 'top', 'bottom', 'center']], Literal['left', 'right', 'top', 'bottom', 'center']]]=None, orientation_margin: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, plain: Optional[Union[Var[bool], bool]]=None, type: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Divider':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-flex = Flex.create
+divider = Divider.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, ReactNode, JsValue
-from ..constant import TypeType, TriggerType, FloatGroupShapeType
-
-from .badge import Badge
-
-
-class FloatButton(AntdComponent):
-    tag = "FloatButton"
-
-    icon: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    tooltip: Optional[Var[Union[ReactNode, JsValue]]]
-    type: Optional[Var[TypeType]]
-    shape: Optional[Var[FloatGroupShapeType]]
-    href: Optional[Var[str]]
-    target: Optional[Var[str]]
-    badge: Optional[Var[Union[Dict]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-class FloatGroup(FloatButton):
-    tag = "FloatButton.Group"
-
-    open: Optional[Var[bool]]
-    trigger: Optional[Var[TriggerType]]
-    close_icon: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-        })
-        return _triggers
-
-
-class FloatBackTop(FloatButton):
-    tag = "FloatButton.BackTop"
-
-    duration: Optional[Var[int]]
-    target: Optional[Var[Union[ReactNode, JsValue]]]
-    visibility_height: Optional[Var[int]]
-
-
-float_button = FloatButton.create
-float_group = FloatGroup.create
-float_back_top = FloatBackTop.create
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode, JsValue
+from ..constant import TypeType, TriggerType, FloatGroupShapeType
+
+from .badge import Badge
+
+
+class FloatButton(AntdComponent):
+    tag = "FloatButton"
+
+    icon: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    tooltip: Optional[Var[Union[ReactNode, JsValue]]]
+    type: Optional[Var[TypeType]]
+    shape: Optional[Var[FloatGroupShapeType]]
+    href: Optional[Var[str]]
+    target: Optional[Var[str]]
+    badge: Optional[Var[Union[Dict]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+class FloatGroup(FloatButton):
+    tag = "FloatButton.Group"
+
+    open: Optional[Var[bool]]
+    trigger: Optional[Var[TriggerType]]
+    close_icon: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+        })
+        return _triggers
+
+
+class FloatBackTop(FloatButton):
+    tag = "FloatButton.BackTop"
+
+    duration: Optional[Var[int]]
+    target: Optional[Var[Union[ReactNode, JsValue]]]
+    visibility_height: Optional[Var[int]]
+
+
+float_button = FloatButton.create
+float_group = FloatGroup.create
+float_back_top = FloatBackTop.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FloatGroup(FloatButton):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
@@ -55,17 +52,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FloatBackTop(FloatButton):
 
     @overload
     @classmethod
@@ -80,15 +74,12 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 float_button = FloatButton.create
 float_group = FloatGroup.create
 float_back_top = FloatBackTop.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,168 @@
-import uuid
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers, MemoizationMode, MemoizationDisposition
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, js_value
-from ..constant import AlignType, DirectionType, SizeType, VariantType
-
-
-class Form(AntdComponent):
-    tag = 'Form'
-
-    colon: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    fields: Optional[Var[ContainVar]]
-    form: Optional[Var[str]]
-    initial_values: Optional[Var[Dict]]
-    label_align: Optional[Var[AlignType]]
-    label_wrap: Optional[Var[bool]]
-    label_col: Optional[Var[Dict]]
-    layout: Optional[Var[DirectionType]]
-    name: Optional[Var[str]]
-    preserve: Optional[Var[bool]]
-    required_mark: Optional[Var[Union[bool, JsValue]]]
-    scrollTo_first_error: Optional[Var[Union[bool, Dict]]]
-    size: Optional[Var[SizeType]]
-    validate_messages: Optional[Var[Dict]]
-    validate_trigger: Optional[Var[Union[str, List[str]]]]
-    variant: Optional[Var[VariantType]]
-    wrapper_col: Optional[Var[Dict]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        if 'form' in props and isinstance(props['form'], str):
-            props['form'] = Var.create_safe(f'{props["form"]}', _var_is_local=False)
-        rs = super().create(*children, **props)
-        # form and form.item can not split, if split some components like select don't work;
-        rs._memoization_mode = MemoizationMode()
-        rs._memoization_mode.disposition = MemoizationDisposition.NEVER
-        rs._memoization_mode.recursive = False
-        return rs
-
-    def _get_hooks(self) -> str | None:
-        if hasattr(self, 'form') and self.form is not None:
-            return f"const [{str(self.form).strip('{}')}] = Form.useForm();"
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_fields_change": lambda changed, all: [changed],
-            'on_finish': lambda values: [values],
-            "on_finish_failed": lambda ev: [ev.values, ev.errorFields, ev.outOfDate],
-            "on_values_change": lambda changed, all: [changed, all],
-        })
-        return _triggers
-
-
-class FormItem(AntdComponent):
-    tag = 'Form.Item'
-
-    colon: Optional[Var[bool]]
-    dependencies: Optional[Var[List[Union[str, int, List[Union[str, int]]]]]]
-    extra: Optional[Var[ReactNode]]
-    getValue_from_event: Optional[Var[JsValue]]
-    get_value_props: Optional[Var[JsValue]]
-    has_feedback: Optional[Var[Union[bool, ContainVar]]]
-    help: Optional[Var[ReactNode]]
-    hidden: Optional[Var[bool]]
-    html_for: Optional[Var[str]]
-    initial_value: Optional[Var[str]]
-    label: Optional[Var[str]]
-    label_align: Optional[Var[AlignType]]
-    label_col: Optional[Var[Dict]]
-    message_variables: Optional[Var[JsValue]]
-    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
-    normalize: Optional[Var[JsValue]]
-    no_style: Optional[Var[bool]]
-    preserve: Optional[Var[bool]]
-    required: Optional[Var[bool]]
-    rules: Optional[Var[Union[List[Dict], ContainVar]]]
-    should_update: Optional[Var[bool]]
-    tooltip: Optional[Var[Union[Component, ContainVar]]]
-    trigger: Optional[Var[str]]
-    validate_debounce: Optional[Var[float]]
-    validate_first: Optional[Var[Union[bool, str]]]
-    validate_status: Optional[Var[str]]
-    validate_trigger: Optional[Var[Union[str, List[str]]]]
-    value_prop_name: Optional[Var[str]]
-    wrapper_col: Optional[Var[Dict]]
-
-    rules: Optional[Var[List[Dict]]]
-
-
-class FormList(AntdComponent):
-    tag = 'Form.List'
-
-    # children: Optional[Var[JsValue]]
-    initial_value: Optional[Var[List]]
-    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
-    rules: Optional[Var[ContainVar]]
-
-
-class FormProvider(AntdComponent):
-    tag = 'Form.Provider'
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_form_change": lambda form_name, info: [form_name, info],
-            'on_form_finish': lambda form_name, info: [form_name, info],
-        })
-        return _triggers
-
-
-form = Form.create
-form_item = FormItem.create
-form_list = FormList.create
-form_provider = FormProvider.create
-
-
-def _modal_form(modal_type: str, *children, modal_config=None, form_id: str = None, **props) -> JsValue | Component:
-    from . import modal
-    if form_id is None:
-        form_id = f'form_{uuid.uuid4().hex}'
-    props.update(
-        form=form_id,
-        preserve=False,
-    )
-    f = form(*children, **props)
-
-    modal_config = modal_config or {}
-    modal_config.update(destroy_on_close=True)
-    modal_config['on_ok'] = js_value(f"""() => {{
-        return new Promise((resolve, reject) => {{
-    {form_id}
-      .validateFields({{
-        validateOnly: false,
-      }})
-      .then(() => {{
-        {form_id}.submit();
-      resolve()}})
-      .catch(() => {{
-      reject()}});
-      }});//if catch, modal will close the form //.catch(() => console.log('Oops errors!'));
-      }}
-    """)
-    op = getattr(modal, modal_type)
-    if modal_type == 'confirm':
-        modal_config['content'] = f
-        return op(config=modal_config)
-    else:
-        modal_config['after_open_change'] = js_value(f"""(open) => {{{form_id}.resetFields()}}""")
-        modal = op(
-            f,
-            # on_open=JsValue(f'{form_id}.resetFields()'),
-            **modal_config)
-        return modal
-
-
-def modal_form(*children, modal_config=None, form_id: str = None, **props) -> Component:
-    return _modal_form('modal',
-                       *children, modal_config=modal_config, form_id=form_id, **props)
-
-
-def confirm_form(*children, confirm_config=None, form_id: str = None, **props) -> JsValue:
-    return _modal_form('confirm',
-                       *children, modal_config=confirm_config, form_id=form_id, **props)
+import uuid
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+
+from ..base import (AntdComponent, ContainVar, JsValue, ReactNode, js_value,
+                    memo_never_no_recursive, memo_always_no_recursive)
+from ..constant import AlignType, DirectionType, SizeType, VariantType
+
+
+class Form(AntdComponent):
+    tag = 'Form'
+
+    colon: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    fields: Optional[Var[ContainVar]]
+    form: Optional[Var[str]]
+    initial_values: Optional[Var[Dict]]
+    label_align: Optional[Var[AlignType]]
+    label_wrap: Optional[Var[bool]]
+    label_col: Optional[Var[Dict]]
+    layout: Optional[Var[DirectionType]]
+    name: Optional[Var[str]]
+    preserve: Optional[Var[bool]]
+    required_mark: Optional[Var[Union[bool, JsValue]]]
+    scrollTo_first_error: Optional[Var[Union[bool, Dict]]]
+    size: Optional[Var[SizeType]]
+    validate_messages: Optional[Var[Dict]]
+    validate_trigger: Optional[Var[Union[str, List[str]]]]
+    variant: Optional[Var[VariantType]]
+    wrapper_col: Optional[Var[Dict]]
+
+    # form and form.item can not split, if split some components like select don't work;
+    _memoization_mode = memo_never_no_recursive
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        if 'form' in props and isinstance(props['form'], str):
+            props['form'] = Var.create_safe(f'{props["form"]}', _var_is_local=False)
+        comp = super().create(*children, **props)
+        if comp._get_all_hooks() or comp._get_all_hooks_internal():
+            comp._memoization_mode = memo_always_no_recursive
+        return comp
+
+    def _get_hooks(self) -> str | None:
+        if hasattr(self, 'form') and self.form is not None:
+            return f"const [{str(self.form).strip('{}')}] = Form.useForm();"
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_fields_change": lambda changed, all: [changed],
+            'on_finish': lambda values: [values],
+            "on_finish_failed": lambda ev: [ev.values, ev.errorFields, ev.outOfDate],
+            "on_values_change": lambda changed, all: [changed, all],
+        })
+        return _triggers
+
+
+class FormItem(AntdComponent):
+    tag = 'Form.Item'
+
+    colon: Optional[Var[bool]]
+    dependencies: Optional[Var[List[Union[str, int, List[Union[str, int]]]]]]
+    extra: Optional[Var[ReactNode]]
+    getValue_from_event: Optional[Var[JsValue]]
+    get_value_props: Optional[Var[JsValue]]
+    has_feedback: Optional[Var[Union[bool, ContainVar]]]
+    help: Optional[Var[ReactNode]]
+    hidden: Optional[Var[bool]]
+    html_for: Optional[Var[str]]
+    initial_value: Optional[Var[str]]
+    label: Optional[Var[str]]
+    label_align: Optional[Var[AlignType]]
+    label_col: Optional[Var[Dict]]
+    message_variables: Optional[Var[JsValue]]
+    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
+    normalize: Optional[Var[JsValue]]
+    no_style: Optional[Var[bool]]
+    preserve: Optional[Var[bool]]
+    required: Optional[Var[bool]]
+    rules: Optional[Var[Union[List[Dict], ContainVar]]]
+    should_update: Optional[Var[bool]]
+    tooltip: Optional[Var[Union[Component, ContainVar]]]
+    trigger: Optional[Var[str]]
+    validate_debounce: Optional[Var[float]]
+    validate_first: Optional[Var[Union[bool, str]]]
+    validate_status: Optional[Var[str]]
+    validate_trigger: Optional[Var[Union[str, List[str]]]]
+    value_prop_name: Optional[Var[str]]
+    wrapper_col: Optional[Var[Dict]]
+
+    rules: Optional[Var[List[Dict]]]
+
+
+class FormList(AntdComponent):
+    tag = 'Form.List'
+
+    # children: Optional[Var[JsValue]]
+    initial_value: Optional[Var[List]]
+    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
+    rules: Optional[Var[ContainVar]]
+
+
+class FormProvider(AntdComponent):
+    tag = 'Form.Provider'
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_form_change": lambda form_name, info: [form_name, info],
+            'on_form_finish': lambda form_name, info: [form_name, info],
+        })
+        return _triggers
+
+
+form = Form.create
+form_item = FormItem.create
+form_list = FormList.create
+form_provider = FormProvider.create
+
+
+def _modal_form(modal_type: str, *children, modal_config=None, form_id: str = None, **props) -> JsValue | Component:
+    from . import modal
+    if form_id is None:
+        form_id = f'form_{uuid.uuid4().hex}'
+    props.update(
+        form=form_id,
+        preserve=False,
+    )
+    f = form(*children, **props)
+
+    modal_config = modal_config or {}
+    modal_config.update(destroy_on_close=True)
+    modal_config['on_ok'] = js_value(f"""() => {{
+        return new Promise((resolve, reject) => {{
+    {form_id}
+      .validateFields({{
+        validateOnly: false,
+      }})
+      .then(() => {{
+        {form_id}.submit();
+      resolve()}})
+      .catch(() => {{
+      reject()}});
+      }});//if catch, modal will close the form //.catch(() => console.log('Oops errors!'));
+      }}
+    """)
+    op = getattr(modal, modal_type)
+    if modal_type == 'confirm':
+        modal_config['content'] = f
+        return op(config=modal_config)
+    else:
+        modal_config['after_open_change'] = js_value(f"""(open) => {{{form_id}.resetFields()}}""")
+        modal = op(
+            f,
+            # on_open=JsValue(f'{form_id}.resetFields()'),
+            **modal_config)
+        return modal
+
+
+def modal_form(*children, modal_config=None, form_id: str = None, **props) -> Component:
+    return _modal_form('modal',
+                       *children, modal_config=modal_config, form_id=form_id, **props)
+
+
+def confirm_form(*children, confirm_config=None, form_id: str = None, **props) -> JsValue:
+    return _modal_form('confirm',
+                       *children, modal_config=confirm_config, form_id=form_id, **props)
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,47 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
+import uuid
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
-from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, js_value, memo_never_no_recursive, memo_always_no_recursive
 from ..constant import AlignType, DirectionType, SizeType, VariantType
 
 class Form(AntdComponent):
 
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
-
     @overload
     @classmethod
-    def create(cls, *children, colon: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, fields: Optional[Union[Var[ContainVar], ContainVar]]=None, initial_values: Optional[Union[Var[Dict], Dict]]=None, label_align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, label_wrap: Optional[Union[Var[bool], bool]]=None, label_col: Optional[Union[Var[Dict], Dict]]=None, layout: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, name: Optional[Union[Var[str], str]]=None, preserve: Optional[Union[Var[bool], bool]]=None, required_mark: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, scrollTo_first_error: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, validate_messages: Optional[Union[Var[Dict], Dict]]=None, validate_trigger: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, wrapper_col: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_fields_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_finish: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_finish_failed: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_values_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Form':
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
+    def create(cls, *children, colon: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, fields: Optional[Union[Var[ContainVar], ContainVar]]=None, form: Optional[Union[Var[str], str]]=None, initial_values: Optional[Union[Var[Dict], Dict]]=None, label_align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, label_wrap: Optional[Union[Var[bool], bool]]=None, label_col: Optional[Union[Var[Dict], Dict]]=None, layout: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, name: Optional[Union[Var[str], str]]=None, preserve: Optional[Union[Var[bool], bool]]=None, required_mark: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, scrollTo_first_error: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, validate_messages: Optional[Union[Var[Dict], Dict]]=None, validate_trigger: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, wrapper_col: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_fields_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_finish: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_finish_failed: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_values_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Form':
+        """"""
+        ...
 
-        Raises:
-            TypeError: If an invalid child is passed.
-        """
+    def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
 class FormItem(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, colon: Optional[Union[Var[bool], bool]]=None, dependencies: Optional[Union[Var[List[Union[str, int, List[Union[str, int]]]]], List[Union[str, int, List[Union[str, int]]]]]]=None, extra: Optional[Union[Var[Component], Component]]=None, getValue_from_event: Optional[Union[Var[JsValue], JsValue]]=None, get_value_props: Optional[Union[Var[JsValue], JsValue]]=None, has_feedback: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, help: Optional[Union[Var[Component], Component]]=None, hidden: Optional[Union[Var[bool], bool]]=None, html_for: Optional[Union[Var[str], str]]=None, initial_value: Optional[Union[Var[str], str]]=None, label: Optional[Union[Var[str], str]]=None, label_align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, label_col: Optional[Union[Var[Dict], Dict]]=None, message_variables: Optional[Union[Var[JsValue], JsValue]]=None, name: Optional[Union[Var[Union[str, int, List[Union[str, int]]]], Union[str, int, List[Union[str, int]]]]]=None, normalize: Optional[Union[Var[JsValue], JsValue]]=None, no_style: Optional[Union[Var[bool], bool]]=None, preserve: Optional[Union[Var[bool], bool]]=None, required: Optional[Union[Var[bool], bool]]=None, rules: Optional[Union[Var[List[Dict]], List[Dict]]]=None, should_update: Optional[Union[Var[bool], bool]]=None, tooltip: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, trigger: Optional[Union[Var[str], str]]=None, validate_debounce: Optional[Union[Var[float], float]]=None, validate_first: Optional[Union[Var[Union[bool, str]], Union[bool, str]]]=None, validate_status: Optional[Union[Var[str], str]]=None, validate_trigger: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, value_prop_name: Optional[Union[Var[str], str]]=None, wrapper_col: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'FormItem':
+    def create(cls, *children, colon: Optional[Union[Var[bool], bool]]=None, dependencies: Optional[Union[Var[List[Union[str, int, List[Union[str, int]]]]], List[Union[str, int, List[Union[str, int]]]]]]=None, extra: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, getValue_from_event: Optional[Union[Var[JsValue], JsValue]]=None, get_value_props: Optional[Union[Var[JsValue], JsValue]]=None, has_feedback: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, help: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, hidden: Optional[Union[Var[bool], bool]]=None, html_for: Optional[Union[Var[str], str]]=None, initial_value: Optional[Union[Var[str], str]]=None, label: Optional[Union[Var[str], str]]=None, label_align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, label_col: Optional[Union[Var[Dict], Dict]]=None, message_variables: Optional[Union[Var[JsValue], JsValue]]=None, name: Optional[Union[Var[Union[str, int, List[Union[str, int]]]], Union[str, int, List[Union[str, int]]]]]=None, normalize: Optional[Union[Var[JsValue], JsValue]]=None, no_style: Optional[Union[Var[bool], bool]]=None, preserve: Optional[Union[Var[bool], bool]]=None, required: Optional[Union[Var[bool], bool]]=None, rules: Optional[Union[Var[List[Dict]], List[Dict]]]=None, should_update: Optional[Union[Var[bool], bool]]=None, tooltip: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, trigger: Optional[Union[Var[str], str]]=None, validate_debounce: Optional[Union[Var[float], float]]=None, validate_first: Optional[Union[Var[Union[bool, str]], Union[bool, str]]]=None, validate_status: Optional[Union[Var[str], str]]=None, validate_trigger: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, value_prop_name: Optional[Union[Var[str], str]]=None, wrapper_col: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'FormItem':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormList(AntdComponent):
 
     @overload
     @classmethod
@@ -77,17 +57,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class FormProvider(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
@@ -105,16 +82,19 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 form = Form.create
 form_item = FormItem.create
 form_list = FormList.create
-form_provider = FormProvider.create
+form_provider = FormProvider.create
+
+def modal_form(*children, modal_config=None, form_id: str=None, **props) -> Component:
+    ...
+
+def confirm_form(*children, confirm_config=None, form_id: str=None, **props) -> JsValue:
+    ...
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict
-
-from reflex import Component, Var
-from reflex.utils import imports
-
-from ..base import AntdComponent, ContainVar
-from ..constant import OrientationType, DirectionType
-
-
-class Row(AntdComponent):
-    tag = 'Row'
-
-    align: Optional[Var[str]]
-    gutter: Optional[Var[Union[int, ContainVar]]]
-    justify: Optional[Var[str]]
-    wrap: Optional[Var[str]]
-
-
-class Col(AntdComponent):
-    tag = 'Col'
-
-    flex: Optional[Var[Union[str, int]]]
-    offset: Optional[Var[int]]
-    order: Optional[Var[int]]
-    pull: Optional[Var[int]]
-    push: Optional[Var[int]]
-    span: Optional[Var[int]]
-
-    xs: Optional[Var[Union[int, Dict]]]
-    sm: Optional[Var[Union[int, Dict]]]
-    md: Optional[Var[Union[int, Dict]]]
-    lg: Optional[Var[Union[int, Dict]]]
-    xl: Optional[Var[Union[int, Dict]]]
-    xxl: Optional[Var[Union[int, Dict]]]
-
-
-row = Row.create
-col = Col.create
+from typing import Optional, Union, Dict
+
+from reflex import Component, Var
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar
+from ..constant import OrientationType, DirectionType
+
+
+class Row(AntdComponent):
+    tag = 'Row'
+
+    align: Optional[Var[str]]
+    gutter: Optional[Var[Union[int, ContainVar]]]
+    justify: Optional[Var[str]]
+    wrap: Optional[Var[str]]
+
+
+class Col(AntdComponent):
+    tag = 'Col'
+
+    flex: Optional[Var[Union[str, int]]]
+    offset: Optional[Var[int]]
+    order: Optional[Var[int]]
+    pull: Optional[Var[int]]
+    push: Optional[Var[int]]
+    span: Optional[Var[int]]
+
+    xs: Optional[Var[Union[int, Dict]]]
+    sm: Optional[Var[Union[int, Dict]]]
+    md: Optional[Var[Union[int, Dict]]]
+    lg: Optional[Var[Union[int, Dict]]]
+    xl: Optional[Var[Union[int, Dict]]]
+    xxl: Optional[Var[Union[int, Dict]]]
+
+
+row = Row.create
+col = Col.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict
+from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
-from ..base import AntdComponent, ContainVar
-from ..constant import OrientationType, DirectionType
+from reflex.constants import EventTriggers
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TimelineModeType
 
-class Row(AntdComponent):
+class Tag(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, align: Optional[Union[Var[str], str]]=None, gutter: Optional[Union[Var[Union[int, ContainVar]], Union[int, ContainVar]]]=None, justify: Optional[Union[Var[str], str]]=None, wrap: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Row':
+    def create(cls, *children, close_icon: Optional[Union[Var[Union[bool, str, Component]], Union[bool, str, Component]]]=None, color: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, bordered: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tag':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class Col(AntdComponent):
+class CheckableTag(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, flex: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, offset: Optional[Union[Var[int], int]]=None, order: Optional[Union[Var[int], int]]=None, pull: Optional[Union[Var[int], int]]=None, push: Optional[Union[Var[int], int]]=None, span: Optional[Union[Var[int], int]]=None, xs: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, sm: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, md: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, lg: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, xl: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, xxl: Optional[Union[Var[Union[int, Dict]], Union[int, Dict]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Col':
+    def create(cls, *children, checked: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckableTag':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-row = Row.create
-col = Col.create
+tag = Tag.create
+checkable_tag = CheckableTag.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from typing import Optional
-
-from reflex import Component, Var
-from reflex.utils import format
-
-from ..base import VarDataMixin
-
-
-class BaseIconComponent(Component):
-    library = "@ant-design/icons"
-
-
-class IconComponent(BaseIconComponent):
-    tag = "None"
-
-    rotate: Optional[Var[int]]
-    spin: Optional[Var[bool]]
-    two_tone_color: Optional[Var[str]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        """Initialize the Icon component.
-        """
-        if children:
-            if len(children) == 1 and type(children[0]) == str:
-                props["tag"] = children[0]
-                children = []
-            else:
-                raise AttributeError(
-                    f"Passing multiple children to Icon component is not allowed: remove positional arguments {children[1:]} to fix"
-                )
-        if "tag" not in props.keys():
-            raise AttributeError("Missing 'tag' keyword-argument for Icon")
-
-        # if (
-        #     type(props["tag"]) != str
-        #     or format.to_snake_case(props["tag"]) not in LUCIDE_ICON_LIST
-        # ):
-        #     raise ValueError(
-        #         f"Invalid icon tag: {props['tag']}. Please use one of the following: {', '.join(LUCIDE_ICON_LIST[0:25])}, ..."
-        #         "\nSee full list at https://lucide.dev/icons."
-        #     )
-
-        # props["tag"] = format.to_title_case(format.to_snake_case(props["tag"]))
-        # props["alias"] = f"antd{props['tag']}"
-        return super().create(*children, **props)
-
-
-icon = IconComponent.create
-
-
-# class CustomerServiceOutlined(BaseIconComponent):
-#     tag = 'CustomerServiceOutlined'
-#
-#
-# class CommentOutlined(BaseIconComponent):
-#     tag = 'CommentOutlined'
-#
-#
-# class QuestionCircleOutlined(BaseIconComponent):
-#     tag = 'QuestionCircleOutlined'
-#
-#
-# class LaptopOutlined(BaseIconComponent):
-#     tag = 'LaptopOutlined'
-#
-#
-# class NotificationOutlined(BaseIconComponent):
-#     tag = 'NotificationOutlined'
-#
-#
-# class CloseCircleOutlined(BaseIconComponent):
-#     tag = 'CloseCircleOutlined'
-#
-#
-# class CloseSquareOutlined(BaseIconComponent):
-#     tag = 'CloseSquareOutlined'
-#
-#
-# class UserOutlined(BaseIconComponent):
-#     tag = 'UserOutlined'
+from typing import Optional
+
+from reflex import Component, Var
+from reflex.utils import format
+
+from ..base import VarDataMixin
+
+
+class BaseIconComponent(Component):
+    library = "@ant-design/icons"
+
+
+class IconComponent(BaseIconComponent):
+    tag = "None"
+
+    rotate: Optional[Var[int]]
+    spin: Optional[Var[bool]]
+    two_tone_color: Optional[Var[str]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        """Initialize the Icon component.
+        """
+        if children:
+            if len(children) == 1 and type(children[0]) == str:
+                props["tag"] = children[0]
+                children = []
+            else:
+                raise AttributeError(
+                    f"Passing multiple children to Icon component is not allowed: remove positional arguments {children[1:]} to fix"
+                )
+        if "tag" not in props.keys():
+            raise AttributeError("Missing 'tag' keyword-argument for Icon")
+
+        # if (
+        #     type(props["tag"]) != str
+        #     or format.to_snake_case(props["tag"]) not in LUCIDE_ICON_LIST
+        # ):
+        #     raise ValueError(
+        #         f"Invalid icon tag: {props['tag']}. Please use one of the following: {', '.join(LUCIDE_ICON_LIST[0:25])}, ..."
+        #         "\nSee full list at https://lucide.dev/icons."
+        #     )
+
+        # props["tag"] = format.to_title_case(format.to_snake_case(props["tag"]))
+        # props["alias"] = f"antd{props['tag']}"
+        return super().create(*children, **props)
+
+
+icon = IconComponent.create
+
+
+# class CustomerServiceOutlined(BaseIconComponent):
+#     tag = 'CustomerServiceOutlined'
+#
+#
+# class CommentOutlined(BaseIconComponent):
+#     tag = 'CommentOutlined'
+#
+#
+# class QuestionCircleOutlined(BaseIconComponent):
+#     tag = 'QuestionCircleOutlined'
+#
+#
+# class LaptopOutlined(BaseIconComponent):
+#     tag = 'LaptopOutlined'
+#
+#
+# class NotificationOutlined(BaseIconComponent):
+#     tag = 'NotificationOutlined'
+#
+#
+# class CloseCircleOutlined(BaseIconComponent):
+#     tag = 'CloseCircleOutlined'
+#
+#
+# class CloseSquareOutlined(BaseIconComponent):
+#     tag = 'CloseSquareOutlined'
+#
+#
+# class UserOutlined(BaseIconComponent):
+#     tag = 'UserOutlined'
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class IconComponent(BaseIconComponent):
 
     @overload
     @classmethod
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Image(AntdComponent):
-    tag = 'Image'
-
-    alt: Optional[Var[str]]
-    fallback: Optional[Var[str]]
-    height: Optional[Var[Union[str, int]]]
-    placeholder: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    preview: Optional[Var[Union[bool, dict]]]
-    src: Optional[Var[str]]
-    width: Optional[Var[Union[str, int]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            "on_error": lambda event: [],
-        })
-        return _triggers
-
-
-class ImagePreviewGroup(AntdComponent):
-    tag = 'Image.PreviewGroup'
-
-    preview: Optional[Var[Union[bool, Component]]]
-    items: Optional[Var[list]]
-    fallback: Optional[Var[str]]
-
-
-image = Image.create
-image_preview_group = ImagePreviewGroup.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Image(AntdComponent):
+    tag = 'Image'
+
+    alt: Optional[Var[str]]
+    fallback: Optional[Var[str]]
+    height: Optional[Var[Union[str, int]]]
+    placeholder: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    preview: Optional[Var[Union[bool, dict]]]
+    src: Optional[Var[str]]
+    width: Optional[Var[Union[str, int]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            "on_error": lambda event: [],
+        })
+        return _triggers
+
+
+class ImagePreviewGroup(AntdComponent):
+    tag = 'Image.PreviewGroup'
+
+    preview: Optional[Var[Union[bool, Component]]]
+    items: Optional[Var[list]]
+    fallback: Optional[Var[str]]
+
+
+image = Image.create
+image_preview_group = ImagePreviewGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Component, Var
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 class Image(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, fallback: Optional[Union[Var[str], str]]=None, height: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, placeholder: Optional[Union[Var[Component], Component]]=None, description: Optional[Union[Var[Component], Component]]=None, preview: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, src: Optional[Union[Var[str], str]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Image':
+    def create(cls, *children, alt: Optional[Union[Var[str], str]]=None, fallback: Optional[Union[Var[str], str]]=None, height: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, placeholder: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, description: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, preview: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, src: Optional[Union[Var[str], str]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_error: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Image':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ImagePreviewGroup(AntdComponent):
 
     @overload
     @classmethod
@@ -49,14 +46,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 image = Image.create
 image_preview_group = ImagePreviewGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType
-
-
-class Input(AntdComponent):
-    tag = "Input"
-
-    addon_after: Optional[Var[ReactNode]]
-    addon_before: Optional[Var[ReactNode]]
-    allow_clear: Optional[Var[Union[bool, ContainVar]]]
-    count: Optional[Var[Union[Dict, ContainVar]]]
-    default_value: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    id: Optional[Var[str]]
-    max_length: Optional[Var[int]]
-    prefix: Optional[Var[ReactNode]]
-    show_count: Optional[Var[Union[bool, JsValue]]]
-    status: Optional[Var[StatusType]]
-    size: Optional[Var[SizeType]]
-    suffix: Optional[Var[ReactNode]]
-    type: Optional[Var[str]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-    placeholder: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-            'on_press_enter': lambda e: [e],
-        })
-        return _triggers
-
-
-class TextArea(Input):
-    tag = "Input.TextArea"
-
-    auto_size: Optional[Var[Union[bool, Dict]]]
-
-
-class Search(Input):
-    tag = 'Input.Search'
-
-    enter_button: Optional[Var[ReactNode]]
-    loading: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_search': lambda value, event, info: [value],
-        })
-        return _triggers
-
-
-class Password(Input):
-    tag = 'Input.Password'
-
-    icon_render: Optional[Var[JsValue]]
-    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
-
-
-input = Input.create  # noqa
-text_area = TextArea.create
-search = Search.create
-password = Password.create
-
-
-
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
+
+
+class Input(AntdComponent):
+    tag = "Input"
+
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    allow_clear: Optional[Var[Union[bool, ContainVar]]]
+    count: Optional[Var[Union[Dict, ContainVar]]]
+    default_value: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    id: Optional[Var[str]]
+    max_length: Optional[Var[int]]
+    prefix: Optional[Var[ReactNode]]
+    show_count: Optional[Var[Union[bool, JsValue]]]
+    status: Optional[Var[StatusType]]
+    size: Optional[Var[SizeType]]
+    suffix: Optional[Var[ReactNode]]
+    type: Optional[Var[str]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+    placeholder: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+            'on_press_enter': lambda e: [e],
+        })
+        return _triggers
+
+
+class TextArea(Input):
+    tag = "Input.TextArea"
+
+    auto_size: Optional[Var[Union[bool, Dict]]]
+
+
+class Search(Input):
+    tag = 'Input.Search'
+
+    enter_button: Optional[Var[ReactNode]]
+    loading: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_search': lambda value, event, info: [value],
+        })
+        return _triggers
+
+
+class Password(Input):
+    tag = 'Input.Password'
+
+    icon_render: Optional[Var[JsValue]]
+    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
+
+
+input = Input.create  # noqa
+text_area = TextArea.create
+search = Search.create
+password = Password.create
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,119 +1,107 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, VariantType
 
 class Input(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, addon_after: Optional[Union[Var[Component], Component]]=None, addon_before: Optional[Union[Var[Component], Component]]=None, allow_clear: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Component], Component]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Component], Component]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Input':
+    def create(cls, *children, addon_after: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, addon_before: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, allow_clear: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Input':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TextArea(Input):
 
     @overload
     @classmethod
-    def create(cls, *children, auto_size: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, addon_after: Optional[Union[Var[Component], Component]]=None, addon_before: Optional[Union[Var[Component], Component]]=None, allow_clear: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Component], Component]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Component], Component]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TextArea':
+    def create(cls, *children, auto_size: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, addon_after: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, addon_before: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, allow_clear: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TextArea':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Search(Input):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, enter_button: Optional[Union[Var[Component], Component]]=None, loading: Optional[Union[Var[bool], bool]]=None, addon_after: Optional[Union[Var[Component], Component]]=None, addon_before: Optional[Union[Var[Component], Component]]=None, allow_clear: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Component], Component]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Component], Component]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Search':
+    def create(cls, *children, enter_button: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, loading: Optional[Union[Var[bool], bool]]=None, addon_after: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, addon_before: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, allow_clear: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Search':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Password(Input):
 
     @overload
     @classmethod
-    def create(cls, *children, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, visibility_toggle: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, addon_after: Optional[Union[Var[Component], Component]]=None, addon_before: Optional[Union[Var[Component], Component]]=None, allow_clear: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Component], Component]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Component], Component]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Password':
+    def create(cls, *children, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, visibility_toggle: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, addon_after: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, addon_before: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, allow_clear: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, count: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, default_value: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, id: Optional[Union[Var[str], str]]=None, max_length: Optional[Union[Var[int], int]]=None, prefix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, show_count: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, suffix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, type: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, placeholder: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Password':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 input = Input.create
 text_area = TextArea.create
 search = Search.create
 password = Password.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,60 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType
-
-
-class InputNumber(AntdComponent):
-    tag = "InputNumber"
-
-    addon_after: Optional[Var[ReactNode]]
-    addon_before: Optional[Var[ReactNode]]
-    auto_focus: Optional[Var[bool]]
-    change_on_blur: Optional[Var[bool]]
-    change_on_wheel: Optional[Var[bool]]
-    controls: Optional[Var[Union[bool, ContainVar]]]
-    decimal_separator: Optional[Var[str]]
-    placeholder: Optional[Var[str]]
-    default_value: Optional[Var[int]]
-    disabled: Optional[Var[bool]]
-    formatter: Optional[Var[JsValue]]
-    keyboard: Optional[Var[bool]]
-    max: Optional[Var[int]]
-    min: Optional[Var[int]]
-    parser: Optional[Var[JsValue]]
-    precision: Optional[Var[int]]
-    read_only: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    prefix: Optional[Var[ReactNode]]
-    size: Optional[Var[SizeType]]
-    step: Optional[Var[Union[int, str]]]
-    string_mode: Optional[Var[bool]]
-    value: Optional[Var[int]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value: [value],
-            'on_press_enter': lambda e: [e],
-            "on_step": lambda value, info: [value, info],
-        })
-        return _triggers
-
-
-input_number = InputNumber.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
+
+
+class Cascader(AntdComponent):
+    tag = 'Cascader'
+
+    allow_clear: Optional[Var[bool]]
+    auto_clear_search_value: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    change_on_select: Optional[Var[bool]]
+    default_value: Optional[Var[Union[List[int], List[str]]]]
+    disabled: Optional[Var[bool]]
+    display_render: Optional[Var[JsValue]]
+    tag_render: Optional[Var[JsValue]]
+    popup_class_name: Optional[Var[str]]
+    dropdown_render: Optional[Var[JsValue]]
+    expand_icon: Optional[Var[ReactNode]]
+    expand_trigger: Optional[Var[TriggerType]]
+    field_names: Optional[Var[ContainVar]]
+    get_popup_container: Optional[Var[JsValue]]
+    load_data: Optional[Var[JsValue]]
+    max_tag_count: Optional[Var[int]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
+    max_tag_text_length: Optional[Var[int]]
+    not_found_content: Optional[Var[str]]
+    open: Optional[Var[bool]]
+    options: Optional[Var[Union[ContainVar, list]]]
+    placeholder: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    show_search: Optional[Var[Union[bool, ContainVar]]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    value: Optional[Var[Union[List[str], List[int]]]]
+    variant: Optional[Var[VariantType]]
+    multiple: Optional[Var[bool]]
+    remove_icon: Optional[Var[ReactNode]]
+    show_checked_strategy: Optional[Var[str]]
+    search_value: Optional[Var[str]]
+    dropdown_menu_column_style: Optional[Var[ContainVar]]
+    loading_icon: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, options: [value, options],
+            "on_dropdown_visible_change": lambda value: [value],
+            "on_search": lambda search: [search]
+        })
+        return _triggers
+
+
+cascader = Cascader.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any
+from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, VariantType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType, PlacementType
 
-class InputNumber(AntdComponent):
+class Mention(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, addon_after: Optional[Union[Var[Component], Component]]=None, addon_before: Optional[Union[Var[Component], Component]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, change_on_blur: Optional[Union[Var[bool], bool]]=None, change_on_wheel: Optional[Union[Var[bool], bool]]=None, controls: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, decimal_separator: Optional[Union[Var[str], str]]=None, placeholder: Optional[Union[Var[str], str]]=None, default_value: Optional[Union[Var[int], int]]=None, disabled: Optional[Union[Var[bool], bool]]=None, formatter: Optional[Union[Var[JsValue], JsValue]]=None, keyboard: Optional[Union[Var[bool], bool]]=None, max: Optional[Union[Var[int], int]]=None, min: Optional[Union[Var[int], int]]=None, parser: Optional[Union[Var[JsValue], JsValue]]=None, precision: Optional[Union[Var[int], int]]=None, read_only: Optional[Union[Var[bool], bool]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, prefix: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, step: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, string_mode: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[int], int]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_step: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'InputNumber':
+    def create(cls, *children, allow_clear: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, auto_size: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, default_value: Optional[Union[Var[str], str]]=None, filter_option: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, not_found_content: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, prefix: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, split: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, validate_search: Optional[Union[Var[JsValue], JsValue]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, options: Optional[Union[Var[ContainVar], ContainVar]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_resize: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Mention':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-input_number = InputNumber.create
+mention = Mention.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,56 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ReactNode, ContainVar
-from ..constant import BreakpointType, ThemeType
-
-
-class LayoutBase(AntdComponent):
-    pass
-
-
-class Layout(LayoutBase):
-    tag = 'Layout'
-
-    has_sider: Optional[Var[bool]]
-
-    # def _get_custom_code(self) -> str | None:
-    #     return """
-    #     const { Header, Content, Footer, Sider } = Layout;
-    #     """
-
-
-class SubLayout(AntdComponent):
-    width: Optional[Var[Union[int, str]]]
-
-
-class Header(SubLayout):
-    tag = 'Layout.Header'
-
-
-class Content(SubLayout):
-    tag = 'Layout.Content'
-
-
-class Footer(SubLayout):
-    tag = 'Layout.Footer'
-
-
-class Sider(SubLayout):
-    tag = 'Layout.Sider'
-
-    breakpoint: Optional[Var[Union[BreakpointType, Dict]]]
-    collapsed: Optional[Var[bool]]
-    collapsed_width: Optional[Var[int]]
-    collapsible: Optional[Var[bool]]
-    default_collapsed: Optional[Var[bool]]
-    reverse_arrow: Optional[Var[bool]]
-    theme: Optional[Var[ThemeType]]
-    trigger: Optional[Var[ReactNode]]
-    zero_width_trigger_style: Optional[Var[Union[Dict, ContainVar]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_breakpoint': lambda broken: [broken],
-            'on_collapse': lambda collapsed, type: [collapsed, type],
-        })
-        return _triggers
-
-
-layout = Layout.create
-header = Header.create
-content = Content.create
-footer = Footer.create
-sider = Sider.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, js_value, ReactNode
+from ..constant import StatusType
+
+
+class Transfer(AntdComponent):
+    tag = 'Transfer'
+    _rename_props: Dict[str, str] = {"itemRender": "render"}
+
+    data_source: Optional[Var[List]]
+    disabled: Optional[Var[bool]]
+    selections_icon: Optional[Var[ReactNode]]
+    filter_option: Optional[Var[JsValue]]
+    footer: Optional[Var[JsValue]]
+    list_style: Optional[Var[Union[Dict, JsValue]]]
+    locale: Optional[Var[Union[Dict, ContainVar]]]
+    one_way: Optional[Var[bool]]
+    operations: Optional[Var[List[str]]]
+    operation_style: Optional[Var[Dict]]
+    pagination: Optional[Var[Union[bool, ContainVar]]]
+    item_render: Optional[Var[Union[JsValue, ContainVar]]]
+    row_key: Optional[Var[JsValue]]
+    select_all_labels: Optional[Var[JsValue]]
+    selected_keys: Optional[Var[List[str]]]
+    show_search: Optional[Var[bool]]
+    showSelect_all: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    target_keys: Optional[Var[List[str]]]
+    titles: Optional[Var[ContainVar]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        if 'item_render' not in props:
+            props['item_render'] = js_value(lambda record: 'return record.title;')
+        com = super().create(*children, **props)
+        return com
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda target_keys, direction, move_keys: [target_keys, direction, move_keys],
+            EventTriggers.ON_SCROLL: lambda direction, ev: [direction, ev],
+            "on_search": lambda direction, value: [direction, value],
+            "on_select_change": lambda s_keys, t_keys: [s_keys, t_keys],
+        })
+        return _triggers
+
+
+transfer = Transfer.create
+
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, AntdSubComponent, ReactNode, ContainVar
+from ..base import AntdComponent, ReactNode, ContainVar, memo_never
 from ..constant import BreakpointType, ThemeType
 
 class LayoutBase(AntdComponent):
     pass
 
     @overload
     @classmethod
@@ -25,17 +25,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Layout(LayoutBase):
 
     @overload
     @classmethod
@@ -50,17 +47,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class SubLayout(AntdComponent):
 
     @overload
     @classmethod
@@ -75,17 +69,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Header(SubLayout):
 
     @overload
     @classmethod
@@ -100,17 +91,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Content(SubLayout):
 
     @overload
     @classmethod
@@ -125,17 +113,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Footer(SubLayout):
 
     @overload
     @classmethod
@@ -150,45 +135,39 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Sider(SubLayout):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, breakpoint: Optional[Union[Var[Union[Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl'], Dict]], Union[Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl'], Dict]]]=None, collapsed: Optional[Union[Var[bool], bool]]=None, collapsed_width: Optional[Union[Var[int], int]]=None, collapsible: Optional[Union[Var[bool], bool]]=None, default_collapsed: Optional[Union[Var[bool], bool]]=None, reverse_arrow: Optional[Union[Var[bool], bool]]=None, theme: Optional[Union[Var[Literal['light', 'dark']], Literal['light', 'dark']]]=None, trigger: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, zero_width_trigger_style: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, width: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_breakpoint: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_collapse: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Sider':
+    def create(cls, *children, breakpoint: Optional[Union[Var[Union[Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl'], Dict]], Union[Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl'], Dict]]]=None, collapsed: Optional[Union[Var[bool], bool]]=None, collapsed_width: Optional[Union[Var[int], int]]=None, collapsible: Optional[Union[Var[bool], bool]]=None, default_collapsed: Optional[Union[Var[bool], bool]]=None, reverse_arrow: Optional[Union[Var[bool], bool]]=None, theme: Optional[Union[Var[Literal['light', 'dark']], Literal['light', 'dark']]]=None, trigger: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, zero_width_trigger_style: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, width: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_breakpoint: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_collapse: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Sider':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 layout = Layout.create
 header = Header.create
 content = Content.create
 footer = Footer.create
 sider = Sider.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,33 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import SizeType
-
-
-class AList(AntdComponent):
-    tag = 'List'
-
-    bordered: Optional[Var[bool]]
-    data_source: Optional[Var[Any]]
-    footer: Optional[Var[ReactNode]]
-    grid: Optional[Var[dict]]
-    header: Optional[Var[ReactNode]]
-    item_layout: Optional[Var[str]]
-    loading: Optional[Var[Union[bool, dict]]]
-    load_more: Optional[Var[ReactNode]]
-    locale: Optional[Var[dict]]
-    pagination: Optional[Var[Union[bool, dict]]]
-    render_item: Optional[Var[JsValue]]
-    size: Optional[Var[SizeType]]
-    split: Optional[Var[bool]]
-
-
-class ListItem(AntdComponent):
-    tag = 'List.Item'
-
-    actions: Optional[Var[list[ContainVar]]]
-    extra: Optional[Var[ReactNode]]
-
-
-class ListItemMeta(AntdComponent):
-    tag = 'List.Item.Meta'
-
-    avatar: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    title: Optional[Var[ReactNode]]
-
-
-alist = AList.create
-list_item = ListItem.create
-list_item_meta = ListItemMeta.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, RadioStyleType, RadioType
+
+
+class Rate(AntdComponent):
+    tag = 'Rate'
+
+    allow_clear: Optional[Var[bool]]
+    allow_half: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    character: Optional[Var[Union[Component, JsValue]]]
+    count: Optional[Var[int]]
+    default_value: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    tooltips: Optional[Var[List[str]]]
+    value: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda v: [v],
+            "on_hover_change": lambda v: [v],
+            EventTriggers.ON_KEY_DOWN: lambda e: [e],
+        })
+        return _triggers
+
+
+rate = Rate.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,80 +7,71 @@
 from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import SizeType
 
 class AList(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, bordered: Optional[Union[Var[bool], bool]]=None, data_source: Optional[Union[Var[Any], Any]]=None, footer: Optional[Union[Var[Component], Component]]=None, grid: Optional[Union[Var[dict], dict]]=None, header: Optional[Union[Var[Component], Component]]=None, item_layout: Optional[Union[Var[str], str]]=None, loading: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, load_more: Optional[Union[Var[Component], Component]]=None, locale: Optional[Union[Var[dict], dict]]=None, pagination: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, render_item: Optional[Union[Var[JsValue], JsValue]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, split: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AList':
+    def create(cls, *children, bordered: Optional[Union[Var[bool], bool]]=None, data_source: Optional[Union[Var[Any], Any]]=None, footer: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, grid: Optional[Union[Var[dict], dict]]=None, header: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, item_layout: Optional[Union[Var[str], str]]=None, loading: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, load_more: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, locale: Optional[Union[Var[dict], dict]]=None, pagination: Optional[Union[Var[Union[bool, dict]], Union[bool, dict]]]=None, render_item: Optional[Union[Var[JsValue], JsValue]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, split: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AList':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ListItem(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, actions: Optional[Union[Var[list[ContainVar]], list[ContainVar]]]=None, extra: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ListItem':
+    def create(cls, *children, actions: Optional[Union[Var[list[ContainVar]], list[ContainVar]]]=None, extra: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ListItem':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class ListItemMeta(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, avatar: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, description: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, title: Optional[Union[Var[Union[Component, str]], Union[Component, str]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ListItemMeta':
+    def create(cls, *children, avatar: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, description: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ListItemMeta':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 alist = AList.create
 list_item = ListItem.create
 list_item_meta = ListItemMeta.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType, PlacementType
-
-
-class Mention(AntdComponent):
-    tag = 'Mention'
-
-    allow_clear: Optional[Var[Union[bool, ContainVar]]]
-    auto_focus: Optional[Var[bool]]
-    auto_size: Optional[Var[Union[bool, Dict]]]
-    default_value: Optional[Var[str]]
-    filter_option: Optional[Var[Union[bool, JsValue]]]
-    get_popup_container: Optional[Var[JsValue]]
-    not_found_content: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    prefix: Optional[Var[Union[str, List[str]]]]
-    split: Optional[Var[str]]
-    status: Optional[Var[StatusType]]
-    validate_search: Optional[Var[JsValue]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-    options: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda text: [text],
-            "on_resize": lambda ev: [ev],
-            'on_search': lambda text, prefix: [text, prefix],
-            "on_select": lambda option, prefix: [option, prefix],
-        })
-        return _triggers
-
-
-mention = Mention.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue,ReactNode
+from ..constant import ColorFormatType, SizeType, PlacementType, TriggerType
+
+
+class ColorPicker(AntdComponent):
+    tag = 'ColorPicker'
+
+    allow_clear: Optional[Var[bool]]
+    arrow: Optional[Var[bool]]
+    default_value: Optional[Var[str]]
+    default_format: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    disabled_alpha: Optional[Var[bool]]
+    destroy_tooltip_on_hide: Optional[Var[bool]]
+    format: Optional[Var[ColorFormatType]]
+    open: Optional[Var[bool]]
+    presets: Optional[Var[ContainVar]]
+    placement: Optional[Var[PlacementType]]
+    panel_render: Optional[Var[JsValue]]
+    show_text: Optional[Var[Union[bool, JsValue]]]
+    size: Optional[Var[SizeType]]
+    trigger: Optional[Var[TriggerType]]
+    value: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, hex: [value, hex],
+            'on_change_complete': lambda value: [value],
+            'on_format_change': lambda format: [format],
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+            'on_clear': lambda: [],
+        })
+        return _triggers
+
+
+color_picker = ColorPicker.create
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
+from typing import Optional, Union, Dict, Any, List, Tuple
+from reflex import Component, Var
+from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, VariantType, PlacementType
+from ..constant import SizeType
+from .tooltip import Tooltip
 
-class Mention(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Popover(Tooltip):
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, auto_size: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, default_value: Optional[Union[Var[str], str]]=None, filter_option: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, prefix: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, split: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, validate_search: Optional[Union[Var[JsValue], JsValue]]=None, value: Optional[Union[Var[str], str]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, options: Optional[Union[Var[ContainVar], ContainVar]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_resize: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Mention':
+    def create(cls, *children, content: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, title: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, align: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, color: Optional[Union[Var[str], str]]=None, default_open: Optional[Union[Var[bool], bool]]=None, destroy_tooltip_on_hide: Optional[Union[Var[bool], bool]]=None, fresh: Optional[Union[Var[bool], bool]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, mouse_enter_delay: Optional[Union[Var[int], int]]=None, mouse_leave_delay: Optional[Union[Var[int], int]]=None, overlay_class_name: Optional[Union[Var[str], str]]=None, overlay_style: Optional[Union[Var[Dict], Dict]]=None, overlay_inner_style: Optional[Union[Var[Dict], Dict]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]], Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]]]=None, open: Optional[Union[Var[bool], bool]]=None, z_index: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Popover':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-mention = Mention.create
+popover = Popover.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from typing import Optional, Union, Type, Dict, List, Any, Iterator
-from reflex import Component, Var, EventChain, Base
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, ReactNode, pydantic
-from ..constant import ThemeType, DirectionType, TriggerType
-
-
-class MenuItem(pydantic.BaseModel):
-    key: str
-    label: str
-    icon: Component
-    children: Optional[List["MenuItem"]] = None
-
-
-# class MenuItems(ContainVar):
-#     pass
-
-class OnSelectEvent(Base):
-    item: Any
-    key: Any
-    keyPath: Any
-    selectedKeys: List[str]
-
-
-class Menu(AntdComponent):
-    tag = 'Menu'
-
-    default_open_keys: Optional[Var[List[str]]]
-    default_selected_keys: Optional[Var[List[str]]]
-    expand_icon: Optional[Var[ReactNode]]
-    force_sub_menu_render: Optional[Var[bool]]
-    inline_collapsed: Optional[Var[bool]]
-    inline_indent: Optional[Var[bool]]
-
-    items: Var[Union[ContainVar, list]]
-    mode: Optional[Var[DirectionType]]
-    multiple: Optional[Var[bool]]
-    open_keys: Optional[Var[List[str]]]
-    overflowed_indicator: Optional[Var[ReactNode]]
-    selectable: Optional[Var[bool]]
-    selected_keys: Optional[Var[List[str]]]
-    sub_menu_close_delay: Optional[Var[float]]
-    sub_menu_open_delay: Optional[Var[float]]
-
-    theme: Optional[Var[ThemeType]]
-    trigger_sub_menu_action: Optional[Var[TriggerType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        def _on_select(ev: OnSelectEvent):
-            return [ev.selectedKeys]
-
-        def _on_click(ev: OnSelectEvent):
-            return [ev.key, ev.keyPath]
-
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open_keys: [open_keys],
-            EventTriggers.ON_SELECT: _on_select,
-            EventTriggers.ON_CLICK: _on_click,
-            'on_deselect': _on_click,
-        })
-        return _triggers
-
-
-menu = Menu.create
-# menu_items = ContainVar.create
+from typing import Optional, Union, Type, Dict, List, Any, Iterator
+from reflex import Component, Var, EventChain, Base
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode, pydantic
+from ..constant import ThemeType, DirectionType, TriggerType
+
+
+class MenuItem(pydantic.BaseModel):
+    key: str
+    label: str
+    icon: Component
+    children: Optional[List["MenuItem"]] = None
+
+
+# class MenuItems(ContainVar):
+#     pass
+
+class OnSelectEvent(Base):
+    item: Any
+    key: Any
+    keyPath: Any
+    selectedKeys: List[str]
+
+
+class Menu(AntdComponent):
+    tag = 'Menu'
+
+    default_open_keys: Optional[Var[List[str]]]
+    default_selected_keys: Optional[Var[List[str]]]
+    expand_icon: Optional[Var[ReactNode]]
+    force_sub_menu_render: Optional[Var[bool]]
+    inline_collapsed: Optional[Var[bool]]
+    inline_indent: Optional[Var[bool]]
+
+    items: Var[Union[ContainVar, list]]
+    mode: Optional[Var[DirectionType]]
+    multiple: Optional[Var[bool]]
+    open_keys: Optional[Var[List[str]]]
+    overflowed_indicator: Optional[Var[ReactNode]]
+    selectable: Optional[Var[bool]]
+    selected_keys: Optional[Var[List[str]]]
+    sub_menu_close_delay: Optional[Var[float]]
+    sub_menu_open_delay: Optional[Var[float]]
+
+    theme: Optional[Var[ThemeType]]
+    trigger_sub_menu_action: Optional[Var[TriggerType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        def _on_select(ev: OnSelectEvent):
+            return [ev.selectedKeys]
+
+        def _on_click(ev: OnSelectEvent):
+            return [ev.key, ev.keyPath]
+
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open_keys: [open_keys],
+            EventTriggers.ON_SELECT: _on_select,
+            EventTriggers.ON_CLICK: _on_click,
+            'on_deselect': _on_click,
+        })
+        return _triggers
+
+
+menu = Menu.create
+# menu_items = ContainVar.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Type, Dict, List, Any, Iterator
-from pydantic import BaseModel
 from reflex import Component, Var, EventChain, Base
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, AntdSubComponent, ContainVar
+from ..base import AntdComponent, ContainVar, ReactNode, pydantic
 from ..constant import ThemeType, DirectionType, TriggerType
 
-class MenuItem(BaseModel):
+class MenuItem(pydantic.BaseModel):
     key: str
     label: str
     icon: Component
     children: Optional[List['MenuItem']]
 
 class OnSelectEvent(Base):
     item: Any
@@ -25,28 +24,25 @@
 class Menu(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, default_open_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, expand_icon: Optional[Union[Var[Component], Component]]=None, force_sub_menu_render: Optional[Union[Var[bool], bool]]=None, inline_collapsed: Optional[Union[Var[bool], bool]]=None, inline_indent: Optional[Union[Var[bool], bool]]=None, items: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, mode: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, multiple: Optional[Union[Var[bool], bool]]=None, open_keys: Optional[Union[Var[List[str]], List[str]]]=None, overflowed_indicator: Optional[Union[Var[Component], Component]]=None, selectable: Optional[Union[Var[bool], bool]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, sub_menu_close_delay: Optional[Union[Var[float], float]]=None, sub_menu_open_delay: Optional[Union[Var[float], float]]=None, theme: Optional[Union[Var[Literal['light', 'dark']], Literal['light', 'dark']]]=None, trigger_sub_menu_action: Optional[Union[Var[Literal['click', 'hover', 'focus', 'contextMenu']], Literal['click', 'hover', 'focus', 'contextMenu']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_deselect: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Menu':
+    def create(cls, *children, default_open_keys: Optional[Union[Var[List[str]], List[str]]]=None, default_selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, expand_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, force_sub_menu_render: Optional[Union[Var[bool], bool]]=None, inline_collapsed: Optional[Union[Var[bool], bool]]=None, inline_indent: Optional[Union[Var[bool], bool]]=None, items: Optional[Union[Var[Union[ContainVar, list]], Union[ContainVar, list]]]=None, mode: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, multiple: Optional[Union[Var[bool], bool]]=None, open_keys: Optional[Union[Var[List[str]], List[str]]]=None, overflowed_indicator: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, selectable: Optional[Union[Var[bool], bool]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, sub_menu_close_delay: Optional[Union[Var[float], float]]=None, sub_menu_open_delay: Optional[Union[Var[float], float]]=None, theme: Optional[Union[Var[Literal['light', 'dark']], Literal['light', 'dark']]]=None, trigger_sub_menu_action: Optional[Union[Var[Literal['click', 'hover', 'focus', 'contextMenu']], Literal['click', 'hover', 'focus', 'contextMenu']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_deselect: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Menu':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 menu = Menu.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,157 @@
-from typing import Optional, Union, Dict, Any, List, Set, Iterator
-import uuid
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.components.base.bare import Bare
-from reflex.vars import BaseVar
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
-from ..constant import MessageType
-from . import helper
-
-
-class Message(JsValue):
-    is_global: bool = True
-    class_name: Optional[Var[str]]
-    content: Optional[Var[ReactNode]]
-    duration: Optional[Var[Union[int, float]]]
-    icon: Optional[Var[ReactNode]]
-    key: Optional[Var[Union[str, int]]]
-    style: Optional[Var[dict]]
-    type: Optional[MessageType] = 'info'
-    config: Optional[Var[dict]]
-
-    top: Optional[Var[int]]
-    rtl: Optional[Var[bool]]
-    prefix_cls: Optional[Var[str]]
-    max_count: Optional[Var[int]]
-
-    @property
-    def config_item(self) -> Optional[ExStateItem]:
-        if not hasattr(self, 'config') or self.config is None:
-            return None
-        try:
-            return self._config_item
-        except AttributeError:
-            self._config_item = ExStateItem(self.config, self)
-            return self._config_item
-
-    @property
-    def uid(self) -> str:
-        try:
-            return self._uid
-        except AttributeError:
-            self._uid = uuid.uuid4().hex
-            return self._uid
-
-    def get_open_message(self) -> str:
-        return f'openMessage_{self.uid}'
-
-    def get_imports(self) -> imports.ImportDict:
-        _imports = {
-            "antd": [imports.ImportVar(tag='message')],
-            "react": [imports.ImportVar(tag="useEffect")],
-        }
-        return _imports
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if self.config_item is not None:
-            open_func = """const %(name)s = () => {
-                           %(mn)s.open(%(cfg)s);
-                       };""" % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                cfg=self.config_item.serialize(),
-            )
-        else:
-            key_s = f'{self.key},' if hasattr(self, 'key') else ''
-            duration_s = f'duration: {self.duration},' if hasattr(self, 'duration') else ''
-            top_s = f'top: {self.top},' if hasattr(self, 'top') else ''
-
-            open_func = """
-            const %(name)s = () => {
-                %(mn)s.open({
-                  %(key)s
-                  type: '%(type)s',
-                  content: '%(content)s',
-                  %(duration)s %(top)s
-                });
-            };
-            """ % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                key=key_s, type=self.type, content=self.content,
-                duration=duration_s,
-                top=top_s,
-            )
-        others = []
-        if self.config_item:
-            state = self.config_item.serialize()
-            others.extend([
-                *self.config_item.get_hooks(),
-                helper.hook_state(
-                    state_field=state,
-                    on_update='%(name)s(%(state)s)' % dict(name=self.get_open_message(), state=state),
-                    on_null='messageApi.destroy()',
-                ),
-            ])
-
-        _hooks = []
-        if self.is_global:
-            _hooks.extend([
-                open_func
-            ])
-        else:
-            _hooks.extend([
-                """const [messageApi, contextHolder] = message.useMessage();""",
-                open_func,
-                *others,
-            ])
-        if version <= '000.004.006':
-            return set(_hooks)
-        return dict((h, None) for h in _hooks)
-
-    def serialize(self) -> str:
-        # if self.config_item is not None:
-        #     return '{contextHolder}'
-        return self.get_open_message()
-
-
-class MessageHolder(Bare):
-    msg: Optional[Message]
-
-    @classmethod
-    def create(cls, msg: Message) -> Component:
-        cs = ['<>']
-        if not msg.is_global:
-            cs.append('{contextHolder}')
-        cs.append('</>')
-        return cls(
-            msg=msg,
-            contents='\n'.join(cs),
-        )
-
-    def _get_vars(self, include_children: bool = False) -> Iterator[Var]:
-        yield self.contents
-        yield BaseVar(
-            _var_name='',
-            _var_is_local=True,
-            _var_data=self.msg.get_var_data(),
-        )
-
-
-message = Message
-message_holder = MessageHolder.create
-
-# def message_holder():
-#     return Var.create_safe('{contextHolder}')
+from typing import Optional, Union, Dict, Any, List, Set, Iterator
+import uuid
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.components.base.bare import Bare
+from reflex.vars import BaseVar
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
+from ..constant import MessageType
+from . import helper
+
+
+class Message(JsValue):
+    is_global: bool = True
+    class_name: Optional[Var[str]]
+    content: Optional[Var[ReactNode]]
+    duration: Optional[Var[Union[int, float]]]
+    icon: Optional[Var[ReactNode]]
+    key: Optional[Var[Union[str, int]]]
+    style: Optional[Var[dict]]
+    type: Optional[MessageType] = 'info'
+    config: Optional[Var[dict]]
+
+    top: Optional[Var[int]]
+    rtl: Optional[Var[bool]]
+    prefix_cls: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+
+    @property
+    def config_item(self) -> Optional[ExStateItem]:
+        if not hasattr(self, 'config') or self.config is None:
+            return None
+        try:
+            return self._config_item
+        except AttributeError:
+            self._config_item = ExStateItem(self.config, self)
+            return self._config_item
+
+    @property
+    def uid(self) -> str:
+        try:
+            return self._uid
+        except AttributeError:
+            self._uid = uuid.uuid4().hex
+            return self._uid
+
+    def get_open_message(self) -> str:
+        return f'openMessage_{self.uid}'
+
+    def get_imports(self) -> imports.ImportDict:
+        _imports = {
+            "antd": [imports.ImportVar(tag='message')],
+            "react": [imports.ImportVar(tag="useEffect")],
+        }
+        return _imports
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if self.config_item is not None:
+            open_func = """const %(name)s = () => {
+                           %(mn)s.open(%(cfg)s);
+                       };""" % dict(
+                name=self.get_open_message(),
+                mn='messageApi' if not self.is_global else 'message',
+                cfg=self.config_item.serialize(),
+            )
+        else:
+            key_s = f'{self.key},' if hasattr(self, 'key') else ''
+            duration_s = f'duration: {self.duration},' if hasattr(self, 'duration') else ''
+            top_s = f'top: {self.top},' if hasattr(self, 'top') else ''
+
+            open_func = """
+            const %(name)s = () => {
+                %(mn)s.open({
+                  %(key)s
+                  type: '%(type)s',
+                  content: '%(content)s',
+                  %(duration)s %(top)s
+                });
+            };
+            """ % dict(
+                name=self.get_open_message(),
+                mn='messageApi' if not self.is_global else 'message',
+                key=key_s, type=self.type, content=self.content,
+                duration=duration_s,
+                top=top_s,
+            )
+        others = []
+        if self.config_item:
+            state = self.config_item.serialize()
+            others.extend([
+                *self.config_item.get_hooks(),
+                helper.hook_state(
+                    state_field=state,
+                    on_update='%(name)s(%(state)s)' % dict(name=self.get_open_message(), state=state),
+                    on_null='messageApi.destroy()',
+                ),
+            ])
+
+        _hooks = []
+        if self.is_global:
+            _hooks.extend([
+                open_func
+            ])
+        else:
+            _hooks.extend([
+                """const [messageApi, contextHolder] = message.useMessage();""",
+                open_func,
+                *others,
+            ])
+        if version <= '000.004.006':
+            return set(_hooks)
+        return dict((h, None) for h in _hooks)
+
+    def serialize(self) -> str:
+        # if self.config_item is not None:
+        #     return '{contextHolder}'
+        return self.get_open_message()
+
+
+class MessageHolder(Bare):
+    """
+    Message.hook:
+        const [messageApi, contextHolder] = message.useMessage();
+
+    MessageHolder:
+        <>
+            {contextHolder}
+        </>
+     """
+    msg: Optional[Message]
+
+    @classmethod
+    def create(cls, msg: Message) -> Component:
+        cs = ['<>']
+        if not msg.is_global:
+            cs.append('{contextHolder}')
+        cs.append('</>')
+        return cls(
+            msg=msg,
+            contents='\n'.join(cs),
+        )
+
+    def _get_vars(self, include_children: bool = False) -> Iterator[Var]:
+        yield self.contents
+        yield BaseVar(
+            _var_name='',
+            _var_is_local=True,
+            _var_data=self.msg.get_var_data(),
+        )
+
+
+message = Message
+message_holder = MessageHolder.create
+
+# def message_holder():
+#     return Var.create_safe('{contextHolder}')
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Set, Iterator
 import uuid
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.components.base.bare import Bare
 from reflex.vars import BaseVar
-from ..base import AntdComponent, AntdSubComponent, ContainVar, JsValue, ReactNode, ExStateItem
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
 from ..constant import MessageType
+from . import helper
 
 class Message(JsValue):
     is_global: bool
     class_name: Optional[Var[str]]
     content: Optional[Var[ReactNode]]
     duration: Optional[Var[Union[int, float]]]
     icon: Optional[Var[ReactNode]]
@@ -36,15 +37,15 @@
 
     def get_open_message(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def serialize(self) -> str:
         ...
 
 class MessageHolder(Bare):
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,64 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
+from typing import Optional, Union, Dict, Any, List, Set
+import uuid
 from reflex import Component, Var
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from reflex.utils import imports
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, FakeComponentMixin
 from ..constant import TypeType
+from . import helper
 
 class Modal(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, class_names: Optional[Union[Var[ContainVar], ContainVar]]=None, styles: Optional[Union[Var[ContainVar], ContainVar]]=None, cancel_button_props: Optional[Union[Var[ContainVar], ContainVar]]=None, cancel_text: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, centered: Optional[Union[Var[bool], bool]]=None, close_icon: Optional[Union[Var[Union[str, Component, bool]], Union[str, Component, bool]]]=None, confirm_loading: Optional[Union[Var[bool], bool]]=None, destroy_on_close: Optional[Union[Var[bool], bool]]=None, focus_trigger_after_close: Optional[Union[Var[bool], bool]]=None, footer: Optional[Union[Var[ContainVar], ContainVar]]=None, force_render: Optional[Union[Var[bool], bool]]=None, get_container: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, keyboard: Optional[Union[Var[bool], bool]]=None, mask: Optional[Union[Var[bool], bool]]=None, mask_closable: Optional[Union[Var[bool], bool]]=None, modal_render: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_button_props: Optional[Union[Var[ContainVar], ContainVar]]=None, ok_text: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, title: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, wrapClassName: Optional[Union[Var[str], str]]=None, zIndex: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, after_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, after_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_cancel: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_ok: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Modal':
+    def create(cls, *children, class_names: Optional[Union[Var[ContainVar], ContainVar]]=None, styles: Optional[Union[Var[ContainVar], ContainVar]]=None, cancel_button_props: Optional[Union[Var[ContainVar], ContainVar]]=None, cancel_text: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, centered: Optional[Union[Var[bool], bool]]=None, close_icon: Optional[Union[Var[Union[str, Component, bool]], Union[str, Component, bool]]]=None, confirm_loading: Optional[Union[Var[bool], bool]]=None, destroy_on_close: Optional[Union[Var[bool], bool]]=None, focus_trigger_after_close: Optional[Union[Var[bool], bool]]=None, footer: Optional[Union[Var[ContainVar], ContainVar]]=None, force_render: Optional[Union[Var[bool], bool]]=None, get_container: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, keyboard: Optional[Union[Var[bool], bool]]=None, mask: Optional[Union[Var[bool], bool]]=None, mask_closable: Optional[Union[Var[bool], bool]]=None, modal_render: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_button_props: Optional[Union[Var[ContainVar], ContainVar]]=None, ok_text: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, width: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, wrapClassName: Optional[Union[Var[str], str]]=None, zIndex: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, after_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, after_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_cancel: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_ok: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Modal':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-modal = Modal.create
+
+class Confirm(FakeComponentMixin, JsValue):
+    config: Optional[Var[dict]]
+
+    @property
+    def config_item(self) -> Optional[ExStateItem]:
+        ...
+
+    @property
+    def uid(self) -> str:
+        ...
+
+    def get_name(self) -> str:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        ...
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        ...
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
+
+    def serialize(self) -> str:
+        ...
+modal = Modal.create
+confirm = Confirm
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/notification.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from typing import Optional, Union, Dict, Any, List, Set
-
-from reflex import Component, Var
-from reflex.utils import imports
-import uuid
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, version
-from ..constant import PlacementType, RoleType
-
-
-class Notification(JsValue):
-    btn: Optional[Var[ReactNode]]
-    class_name: Optional[Var[str]]
-    close_icon: Optional[Var[ReactNode]]
-    description: Optional[Var[str]]
-    duration: Optional[Var[int]]
-    icon: Optional[Var[ReactNode]]
-    key: Optional[Var[str]]
-    message: Optional[Var[str]]
-    placement: Optional[Var[PlacementType]]
-    role: Optional[Var[RoleType]]
-    props: Optional[Var[Union[dict, ContainVar]]]
-
-    def get_imports(self) -> imports.ImportDict:
-        _imports = {
-            "antd": [imports.ImportVar(tag='notification')],
-        }
-        return _imports
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        open_func = """
-        const %(name)s = () => {
-          notification.open({
-            message: '%(message)s',
-            description:'%(description)s',
-            placement:'%(placement)s',
-            duration:'%(duration)s',
-          });
-        };
-        """ % dict(name=self.get_open_notification(), message=self.message, description=self.description,
-                   placement=self.placement, duration=self.duration)
-
-        _hooks = []
-        _hooks.extend([
-            """const [api, contextHolder] = notification.useNotification();""",
-            open_func,
-        ])
-        if version <= '000.004.006':
-            return set(_hooks)
-        return dict((h, None) for h in _hooks)
-
-    @property
-    def uid(self) -> str:
-        try:
-            return self._uid
-        except AttributeError:
-            self._uid = uuid.uuid4().hex
-            return self._uid
-
-    def get_open_notification(self) -> str:
-        return f'openNotification_{self.uid}'
-
-    def serialize(self) -> str:
-        return self.get_open_notification()
-
-
-notification = Notification
+from typing import Optional, Union, Dict, Any, List, Set
+
+from reflex import Component, Var
+from reflex.utils import imports
+import uuid
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, version
+from ..constant import PlacementType, RoleType
+
+
+class Notification(JsValue):
+    btn: Optional[Var[ReactNode]]
+    class_name: Optional[Var[str]]
+    close_icon: Optional[Var[ReactNode]]
+    description: Optional[Var[str]]
+    duration: Optional[Var[int]]
+    icon: Optional[Var[ReactNode]]
+    key: Optional[Var[str]]
+    message: Optional[Var[str]]
+    placement: Optional[Var[PlacementType]]
+    role: Optional[Var[RoleType]]
+    props: Optional[Var[Union[dict, ContainVar]]]
+
+    def get_imports(self) -> imports.ImportDict:
+        _imports = {
+            "antd": [imports.ImportVar(tag='notification')],
+        }
+        return _imports
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        open_func = """
+        const %(name)s = () => {
+          notification.open({
+            message: '%(message)s',
+            description:'%(description)s',
+            placement:'%(placement)s',
+            duration:'%(duration)s',
+          });
+        };
+        """ % dict(name=self.get_open_notification(), message=self.message, description=self.description,
+                   placement=self.placement, duration=self.duration)
+
+        _hooks = []
+        _hooks.extend([
+            """const [api, contextHolder] = notification.useNotification();""",
+            open_func,
+        ])
+        if version <= '000.004.006':
+            return set(_hooks)
+        return dict((h, None) for h in _hooks)
+
+    @property
+    def uid(self) -> str:
+        try:
+            return self._uid
+        except AttributeError:
+            self._uid = uuid.uuid4().hex
+            return self._uid
+
+    def get_open_notification(self) -> str:
+        return f'openNotification_{self.uid}'
+
+    def serialize(self) -> str:
+        return self.get_open_notification()
+
+
+notification = Notification
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 pagination = Pagination.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TypeType
-
-class Popconfirm(AntdComponent):
-    tag = 'Popconfirm'
-
-    cancel_button_orops: Optional[Var[dict]]
-    cancel_text: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    icon: Optional[Var[ReactNode]]
-    ok_button_props: Optional[Var[dict]]
-    ok_text: Optional[Var[str]]
-    ok_type: Optional[Var[TypeType]]
-    open: Optional[Var[bool]]
-    show_cancel: Optional[Var[bool]]
-    title: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_cancel": lambda e: [e],
-            "on_confirm": lambda e: [e],
-            "on_popup_click": lambda e: [e],
-        })
-        return _triggers
-
-
-popconfirm = Popconfirm.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, RadioStyleType, RadioType
+
+
+class Radio(AntdComponent):
+    tag = 'Radio'
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    default_checked: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    value: Optional[Var[Any]]
+
+
+class RadioButton(Radio):
+    tag = 'Radio.Button'
+
+
+class RadioGroup(AntdComponent):
+    tag = 'Radio.Group'
+
+    button_style: Optional[Var[RadioStyleType]]
+    default_value: Optional[Var[Any]]
+    disabled: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    options: Optional[Var[Union[List[Union[str, int]], ContainVar]]]
+    optionType: Optional[Var[RadioType]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[Any]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+        })
+        return _triggers
+
+
+radio = Radio.create
+radio_button = RadioButton.create
+radio_group = RadioGroup.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,25 @@
 class Popconfirm(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, cancel_button_orops: Optional[Union[Var[dict], dict]]=None, cancel_text: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_button_props: Optional[Union[Var[dict], dict]]=None, ok_text: Optional[Union[Var[str], str]]=None, ok_type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, open: Optional[Union[Var[bool], bool]]=None, show_cancel: Optional[Union[Var[bool], bool]]=None, title: Optional[Union[Var[Component], Component]]=None, description: Optional[Union[Var[Component], Component]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_cancel: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_confirm: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_popup_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Popconfirm':
+    def create(cls, *children, cancel_button_orops: Optional[Union[Var[dict], dict]]=None, cancel_text: Optional[Union[Var[str], str]]=None, disabled: Optional[Union[Var[bool], bool]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, ok_button_props: Optional[Union[Var[dict], dict]]=None, ok_text: Optional[Union[Var[str], str]]=None, ok_type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, open: Optional[Union[Var[bool], bool]]=None, show_cancel: Optional[Union[Var[bool], bool]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, description: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_cancel: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_confirm: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_popup_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Popconfirm':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 popconfirm = Popconfirm.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List, Tuple
-from reflex import Component, Var
-from reflex.utils import imports
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
-from .tooltip import Tooltip
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
 
-class Popover(Tooltip):
+class InputNumber(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, content: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, title: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, align: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, color: Optional[Union[Var[str], str]]=None, default_open: Optional[Union[Var[bool], bool]]=None, destroy_tooltip_on_hide: Optional[Union[Var[bool], bool]]=None, fresh: Optional[Union[Var[bool], bool]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, mouse_enter_delay: Optional[Union[Var[int], int]]=None, mouse_leave_delay: Optional[Union[Var[int], int]]=None, overlay_class_name: Optional[Union[Var[str], str]]=None, overlay_style: Optional[Union[Var[Dict], Dict]]=None, overlay_inner_style: Optional[Union[Var[Dict], Dict]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]], Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]]]=None, open: Optional[Union[Var[bool], bool]]=None, z_index: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Popover':
+    def create(cls, *children, addon_after: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, addon_before: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, change_on_blur: Optional[Union[Var[bool], bool]]=None, change_on_wheel: Optional[Union[Var[bool], bool]]=None, controls: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, decimal_separator: Optional[Union[Var[str], str]]=None, placeholder: Optional[Union[Var[str], str]]=None, default_value: Optional[Union[Var[int], int]]=None, disabled: Optional[Union[Var[bool], bool]]=None, formatter: Optional[Union[Var[JsValue], JsValue]]=None, keyboard: Optional[Union[Var[bool], bool]]=None, max: Optional[Union[Var[int], int]]=None, min: Optional[Union[Var[int], int]]=None, parser: Optional[Union[Var[JsValue], JsValue]]=None, precision: Optional[Union[Var[int], int]]=None, read_only: Optional[Union[Var[bool], bool]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, prefix: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, step: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, string_mode: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[int], int]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_press_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_step: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'InputNumber':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-popover = Popover.create
+input_number = InputNumber.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, ProgressType, SizeType, OrientationType
-
-
-class Progress(AntdComponent):
-    tag = 'Progress'
-
-    format: Optional[Var[JsValue]]
-    percent: Optional[Var[int]]
-    show_info: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    stroke_color: Optional[Var[str]]
-    stroke_linecap: Optional[Var[str]]
-    success: Optional[Var[Dict]]
-    trail_color: Optional[Var[str]]
-    type: Optional[Var[ProgressType]]
-    size: Optional[Var[Union[int, SizeType, List[Union[int, SizeType]]]]]
-    # type=...
-    steps: Optional[Var[Union[int, Dict]]]
-    stroke_color: Optional[Var[Union[str, List[str], Dict]]]
-    stroke_width: Optional[Var[int]]
-    # dashboard
-    gap_degree: Optional[Var[int]]
-    gap_position: Optional[Var[OrientationType]]
-
-
-progress = Progress.create
-
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, ProgressType, SizeType, OrientationType
+
+
+class Progress(AntdComponent):
+    tag = 'Progress'
+
+    format: Optional[Var[JsValue]]
+    percent: Optional[Var[int]]
+    show_info: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    stroke_color: Optional[Var[str]]
+    stroke_linecap: Optional[Var[str]]
+    success: Optional[Var[Dict]]
+    trail_color: Optional[Var[str]]
+    type: Optional[Var[ProgressType]]
+    size: Optional[Var[Union[int, SizeType, List[Union[int, SizeType]]]]]
+    # type=...
+    steps: Optional[Var[Union[int, Dict]]]
+    stroke_color: Optional[Var[Union[str, List[str], Dict]]]
+    stroke_width: Optional[Var[int]]
+    # dashboard
+    gap_degree: Optional[Var[int]]
+    gap_position: Optional[Var[OrientationType]]
+
+
+progress = Progress.create
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 progress = Progress.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType, QRCodeType, QRCodeErrorLevelType, QRCodeStatusType
-
-
-class QRCode(AntdComponent):
-    tag = 'QRCode'
-
-    value: Optional[Var[str]]
-    type: Optional[Var[QRCodeType]]
-    icon: Optional[Var[str]]
-    size: Optional[Var[int]]
-    icon_size: Optional[Var[int]]
-    color: Optional[Var[str]]
-    bg_color: Optional[Var[str]]
-    bordered: Optional[Var[bool]]
-    error_level: Optional[Var[QRCodeErrorLevelType]]
-    status: Optional[Var[QRCodeStatusType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_refresh": lambda: [],
-        })
-        return _triggers
-
-
-qrcode = QRCode.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType, QRCodeType, QRCodeErrorLevelType, QRCodeStatusType
+
+
+class QRCode(AntdComponent):
+    tag = 'QRCode'
+
+    value: Optional[Var[str]]
+    type: Optional[Var[QRCodeType]]
+    icon: Optional[Var[str]]
+    size: Optional[Var[int]]
+    icon_size: Optional[Var[int]]
+    color: Optional[Var[str]]
+    bg_color: Optional[Var[str]]
+    bordered: Optional[Var[bool]]
+    error_level: Optional[Var[QRCodeErrorLevelType]]
+    status: Optional[Var[QRCodeStatusType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_refresh": lambda: [],
+        })
+        return _triggers
+
+
+qrcode = QRCode.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 qrcode = QRCode.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,33 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, RadioStyleType, RadioType
-
-
-class Radio(AntdComponent):
-    tag = 'Radio'
-
-    auto_focus: Optional[Var[bool]]
-    checked: Optional[Var[bool]]
-    default_checked: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    value: Optional[Var[Any]]
-
-
-class RadioButton(Radio):
-    tag = 'Radio.Button'
-
-
-class RadioGroup(AntdComponent):
-    tag = 'Radio.Group'
-
-    button_style: Optional[Var[RadioStyleType]]
-    default_value: Optional[Var[Any]]
-    disabled: Optional[Var[bool]]
-    name: Optional[Var[str]]
-    options: Optional[Var[Union[List[Union[str, int]], ContainVar]]]
-    optionType: Optional[Var[RadioType]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[Any]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-        })
-        return _triggers
-
-
-radio = Radio.create
-radio_button = RadioButton.create
-radio_group = RadioGroup.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+
+
+class Switch(AntdComponent):
+    tag = 'Switch'
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    checked_children: Optional[Var[ReactNode]]
+    default_checked: Optional[Var[bool]]
+    default_value: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    loading: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    un_checked_children: Optional[Var[ReactNode]]
+    value: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked, e: [checked, e],
+            EventTriggers.ON_CLICK: lambda checked, e: [checked, e],
+        })
+        return _triggers
+
+
+switch = Switch.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,79 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, RadioStyleType, RadioType
+from reflex import Component, Var
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
-class Radio(AntdComponent):
+class Card(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Radio':
+    def create(cls, *children, actions: Optional[Union[Var[ContainVar], ContainVar]]=None, active_tab_key: Optional[Union[Var[str], str]]=None, bordered: Optional[Union[Var[bool], bool]]=None, cover: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, default_active_tab_key: Optional[Union[Var[str], str]]=None, extra: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, hoverable: Optional[Union[Var[bool], bool]]=None, loading: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, tab_bar_extra_content: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, tab_list: Optional[Union[Var[list[ContainVar]], list[ContainVar]]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, type: Optional[Union[Var[str], str]]=None, tab_props: Optional[Union[Var[Union[ContainVar, dict]], Union[ContainVar, dict]]]=None, class_names: Optional[Union[Var[dict], dict]]=None, styles: Optional[Union[Var[dict], dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Card':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class RadioButton(Radio):
+class CardGrid(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RadioButton':
+    def create(cls, *children, hoverable: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CardGrid':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class RadioGroup(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class CardMeta(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, button_style: Optional[Union[Var[Literal['outline', 'solid']], Literal['outline', 'solid']]]=None, default_value: Optional[Union[Var[Any], Any]]=None, disabled: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[Union[List[Union[str, int]], ContainVar]], Union[List[Union[str, int]], ContainVar]]]=None, optionType: Optional[Union[Var[Literal['default', 'button']], Literal['default', 'button']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[Any], Any]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'RadioGroup':
+    def create(cls, *children, avatar: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, description: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CardMeta':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-radio = Radio.create
-radio_button = RadioButton.create
-radio_group = RadioGroup.create
+card = Card.create
+card_grid = CardGrid.create
+card_meta = CardMeta.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, RadioStyleType, RadioType
-
-
-class Rate(AntdComponent):
-    tag = 'Rate'
-
-    allow_clear: Optional[Var[bool]]
-    allow_half: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    character: Optional[Var[Union[Component, JsValue]]]
-    count: Optional[Var[int]]
-    default_value: Optional[Var[int]]
-    disabled: Optional[Var[bool]]
-    tooltips: Optional[Var[List[str]]]
-    value: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda v: [v],
-            "on_hover_change": lambda v: [v],
-            EventTriggers.ON_KEY_DOWN: lambda e: [e],
-        })
-        return _triggers
-
-
-rate = Rate.create
-
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsNode
+from ..constant import OrientationType, DirectionType
+
+
+class Anchor(AntdComponent):
+    tag = 'Anchor'
+
+    affix: Optional[Var[bool]]
+    bounds: Optional[Var[int]]
+    get_container: Optional[Var[JsNode]]
+    get_current_anchor: Optional[Var[JsNode]]
+    offset_top: Optional[Var[int]]
+    show_ink_in_fixed: Optional[Var[bool]]
+    target_offset: Optional[Var[int]]
+    items: Optional[Var[Union[List, ContainVar]]]
+    direction: Optional[Var[DirectionType]]
+    replace: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda link: [link],
+            EventTriggers.ON_CLICK: lambda ev, link: [ev, link],
+        })
+        return _triggers
+
+
+anchor = Anchor.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,13 +26,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 rate = Rate.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType
-
-
-class Result(AntdComponent):
-    tag = 'Result'
-
-    extra: Optional[Var[ReactNode]]
-    icon: Optional[Var[ReactNode]]
-    status: Optional[Var[Union[StatusType, str]]]
-    sub_title: Optional[Var[ReactNode]]
-    title: Optional[Var[ReactNode]]
-
-
-result = Result.create
-
-
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue
+
+
+class Carousel(AntdComponent):
+    tag = 'Carousel'
+
+    autoplay: Optional[Var[bool]]
+    autoplay_speed: Optional[Var[int]]
+    dot_position: Optional[Var[str]]
+    dots: Optional[Var[Union[bool, dict]]]
+    fade: Optional[Var[bool]]
+    infinite: Optional[Var[bool]]
+    speed: Optional[Var[int]]
+    easing: Optional[Var[str]]
+    wait_for_animate: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'after_change': lambda current: [],
+            'before_change': lambda current, next: [],
+        })
+        return _triggers
+
+
+carousel = Carousel.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TimelineModeType
 
-class Result(AntdComponent):
+class Timeline(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, extra: Optional[Union[Var[Component], Component]]=None, icon: Optional[Union[Var[Component], Component]]=None, status: Optional[Union[Var[Union[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active'], str]], Union[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active'], str]]]=None, sub_title: Optional[Union[Var[Component], Component]]=None, title: Optional[Union[Var[Component], Component]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Result':
+    def create(cls, *children, mode: Optional[Union[Var[Literal['left', 'alternate', 'right']], Literal['left', 'alternate', 'right']]]=None, pending: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, pending_dot: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, reverse: Optional[Union[Var[bool], bool]]=None, items: Optional[Union[Var[Union[List, ContainVar]], Union[List, ContainVar]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Timeline':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-result = Result.create
+timeline = Timeline.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType, PlacementType, TabsType
-
-
-class Segmented(AntdComponent):
-    tag = 'Segmented'
-
-    block: Optional[Var[bool]]
-    default_value: Optional[Var[Union[str, int]]]
-    disabled: Optional[Var[bool]]
-    options: Optional[Union[List[str], List[int], List[Dict]]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[Union[str, int]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value: [value],
-        })
-        return _triggers
-
-
-segmented = Segmented.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType, PlacementType, TabsType
+
+
+class Segmented(AntdComponent):
+    tag = 'Segmented'
+
+    block: Optional[Var[bool]]
+    default_value: Optional[Var[Union[str, int]]]
+    disabled: Optional[Var[bool]]
+    options: Optional[Union[List[str], List[int], List[Dict]]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[Union[str, int]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value: [value],
+        })
+        return _triggers
+
+
+segmented = Segmented.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,38 +2,32 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType, PlacementType, TabsType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType
 
-class Segmented(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Spin(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, options: Optional[Union[List[str], List[int], List[Dict]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Segmented':
+    def create(cls, *children, delay: Optional[Union[Var[int], int]]=None, indicator: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, spinning: Optional[Union[Var[bool], bool]]=None, tip: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, wrapper_class_name: Optional[Union[Var[str], str]]=None, fullscreen: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Spin':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-segmented = Segmented.create
+spin = Spin.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
-
-
-class Select(AntdComponent):
-    tag = 'Select'
-
-    allow_clear: Optional[Var[bool]]
-    auto_clear_search_value: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    default_active_first_option: Optional[Var[bool]]
-    default_open: Optional[Var[bool]]
-    default_value: Optional[Var[Union[int, str, List[str], List[int], ContainVar]]]
-    disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    dropdown_render: Optional[Var[JsValue]]
-    dropdown_style: Optional[Var[Dict]]
-    field_names: Optional[Var[Dict]]
-    filter_option: Optional[Var[Union[bool, JsValue]]]
-    filter_sort: Optional[Var[JsValue]]
-    get_popup_container: Optional[Var[JsValue]]
-    label_in_value: Optional[Var[bool]]
-    list_height: Optional[Var[int]]
-    loading: Optional[Var[bool]]
-    max_count: Optional[Var[int]]
-    max_tag_count: Optional[Var[Union[int, str]]]
-    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
-    max_tag_text_length: Optional[Var[int]]
-    menu_item_selected_icon: Optional[Var[ReactNode]]
-    mode: Optional[Var[SelectModeType]]
-    not_found_content: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    option_filter_prop: Optional[Var[str]]
-    option_label_prop: Optional[Var[str]]
-    options: Optional[Var[Union[list, ContainVar]]]
-    option_render: Optional[Var[JsValue]]
-    placeholder: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    remove_icon: Optional[Var[ReactNode]]
-    search_value: Optional[Var[str]]
-    show_search: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    tag_render: Optional[Var[JsValue]]
-    label_render: Optional[Var[JsValue]]
-    token_separators: Optional[Var[List[str]]]
-    value: Optional[Var[Union[str, int, List[str], List[int], ContainVar]]]
-    variant: Optional[Var[VariantType]]
-    virtual: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda v, option: [v, option],
-            "on_clear": lambda: [],
-            "on_deselect": lambda v: [v],
-            "on_dropdown_visible_change": lambda open: [open],
-            "on_input_key_down": lambda: [],
-            "on_popup_scroll": lambda: [],
-            "on_search": lambda v: [v],
-            "on_select": lambda v, option: [v, option],
-        })
-        return _triggers
-
-
-select = Select.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsNode, ReactNode
+
+
+class TreeSelect(AntdComponent):
+    tag = 'TreeSelect'
+
+    allow_clear: Optional[Var[Union[bool, ReactNode]]]
+    auto_clear_search_value: Optional[Var[bool]]
+    default_value: Optional[Var[Union[str, List[str]]]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    dropdown_render: Optional[Var[JsNode]]
+    dropdown_style: Optional[Var[Dict]]
+    field_names: Optional[Var[Dict]]
+    filter_tree_node: Optional[Var[Union[bool, JsNode]]]
+    get_popup_container: Optional[Var[JsNode]]
+    label_in_value: Optional[Var[bool]]
+    list_height: Optional[Var[int]]
+    load_data: Optional[Var[JsNode]]
+    max_tag_count: Optional[Var[int]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsNode]]]
+    max_tag_text_length: Optional[Var[int]]
+    multiple: Optional[Var[bool]]
+    not_found_content: Optional[Var[ReactNode]]
+    placeholder: Optional[Var[str]]
+    placement: Optional[Var[str]]
+    search_value: Optional[Var[str]]
+    show_checked_strategy: Optional[Var[str]]
+    show_search: Optional[Var[bool]]
+    size: Optional[Var[str]]
+    status: Optional[Var[str]]
+    suffix_icon: Optional[Var[ReactNode]]
+    switcher_icon: Optional[Var[Union[ReactNode, ContainVar]]]
+    tag_render: Optional[Var[JsNode]]
+    tree_checkable: Optional[Var[bool]]
+    tree_check_strictly: Optional[Var[bool]]
+    tree_data: Optional[Var[List[Dict]]]
+    tree_data_simple_mode: Optional[Var[Union[bool, Dict]]]
+    tree_default_expand_all: Optional[Var[bool]]
+    tree_default_expanded_keys: Optional[Var[List]]
+    tree_expand_action: Optional[Var[Union[str, bool]]]
+    tree_expanded_keys: Optional[Var[List[str]]]
+    tree_icon: Optional[Var[bool]]
+    tree_line: Optional[Var[Union[bool, Dict]]]
+    tree_loaded_keys: Optional[Var[List[str]]]
+    tree_node_filter_prop: Optional[Var[str]]
+    tree_node_label_prop: Optional[Var[str]]
+    value: Optional[Var[Union[str, List[str]]]]
+    variant: Optional[Var[str]]
+    virtual: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, label, extra: [value, label, extra],
+            EventTriggers.ON_SELECT: lambda value, node, extra: [value, node, extra],
+            "on_dropdown_visible_change": lambda open: [open],
+            "on_search": lambda value: [value],
+            "on_tree_expand": lambda keys: [keys],
+
+            "filter_tree_node": lambda node: [node],
+            "load_data": lambda node: [node],
+        })
+        return _triggers
+
+
+tree_select = TreeSelect.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
 
 class Select(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, default_active_first_option: Optional[Union[Var[bool], bool]]=None, default_open: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[int, str, List[str], List[int], ContainVar]], Union[int, str, List[str], List[int], ContainVar]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[JsValue], JsValue]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_option: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, filter_sort: Optional[Union[Var[JsValue], JsValue]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, loading: Optional[Union[Var[bool], bool]]=None, max_count: Optional[Union[Var[int], int]]=None, max_tag_count: Optional[Union[Var[Union[int, str]], Union[int, str]]]=None, max_tag_placeholder: Optional[Union[Var[Union[Component, JsValue]], Union[Component, JsValue]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, menu_item_selected_icon: Optional[Union[Var[Component], Component]]=None, mode: Optional[Union[Var[Literal['multiple', 'tags']], Literal['multiple', 'tags']]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, open: Optional[Union[Var[bool], bool]]=None, option_filter_prop: Optional[Union[Var[str], str]]=None, option_label_prop: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[Union[list, ContainVar]], Union[list, ContainVar]]]=None, option_render: Optional[Union[Var[JsValue], JsValue]]=None, placeholder: Optional[Union[Var[Component], Component]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, remove_icon: Optional[Union[Var[Component], Component]]=None, search_value: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, tag_render: Optional[Union[Var[JsValue], JsValue]]=None, label_render: Optional[Union[Var[JsValue], JsValue]]=None, token_separators: Optional[Union[Var[List[str]], List[str]]]=None, value: Optional[Union[Var[Union[int, str, List[str], List[int], ContainVar]], Union[int, str, List[str], List[int], ContainVar]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, virtual: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_clear: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_deselect: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_input_key_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_popup_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Select':
+    def create(cls, *children, allow_clear: Optional[Union[Var[bool], bool]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, auto_focus: Optional[Union[Var[bool], bool]]=None, default_active_first_option: Optional[Union[Var[bool], bool]]=None, default_open: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[int, str, List[str], List[int], ContainVar]], Union[int, str, List[str], List[int], ContainVar]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[JsValue], JsValue]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_option: Optional[Union[Var[Union[bool, JsValue]], Union[bool, JsValue]]]=None, filter_sort: Optional[Union[Var[JsValue], JsValue]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, loading: Optional[Union[Var[bool], bool]]=None, max_count: Optional[Union[Var[int], int]]=None, max_tag_count: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, max_tag_placeholder: Optional[Union[Var[Union[str, Component, JsValue]], Union[str, Component, JsValue]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, menu_item_selected_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, mode: Optional[Union[Var[Literal['multiple', 'tags']], Literal['multiple', 'tags']]]=None, not_found_content: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, open: Optional[Union[Var[bool], bool]]=None, option_filter_prop: Optional[Union[Var[str], str]]=None, option_label_prop: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[Union[list, ContainVar]], Union[list, ContainVar]]]=None, option_render: Optional[Union[Var[JsValue], JsValue]]=None, placeholder: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, remove_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, search_value: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, suffix_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, tag_render: Optional[Union[Var[JsValue], JsValue]]=None, label_render: Optional[Union[Var[JsValue], JsValue]]=None, token_separators: Optional[Union[Var[List[str]], List[str]]]=None, value: Optional[Union[Var[Union[int, str, List[str], List[int], ContainVar]], Union[int, str, List[str], List[int], ContainVar]]]=None, variant: Optional[Union[Var[Literal['outlined', 'borderless', 'filled']], Literal['outlined', 'borderless', 'filled']]]=None, virtual: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_clear: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_deselect: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_input_key_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_popup_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Select':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 select = Select.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
-
-
-class Skeleton(AntdComponent):
-    tag = 'Skeleton'
-
-    active: Optional[Var[bool]]
-    avatar: Optional[Var[Union[bool, Dict]]]
-    loading: Optional[Var[bool]]
-    paragraph: Optional[Var[Union[bool, Dict]]]
-    round: Optional[Var[bool]]
-    title: Optional[Var[Union[bool, Dict]]]
-
-
-skeleton = Skeleton.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType
+
+
+class Spin(AntdComponent):
+    tag = 'Spin'
+
+    delay: Optional[Var[int]]
+    indicator: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    spinning: Optional[Var[bool]]
+    tip: Optional[Var[ReactNode]]
+    wrapper_class_name: Optional[Var[str]]
+    fullscreen: Optional[Var[bool]]
+
+
+spin = Spin.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
+from ..constant import SizeType, PlacementType, TabsType
 
-class Skeleton(AntdComponent):
+class Segmented(AntdComponent):
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
 
     @overload
     @classmethod
-    def create(cls, *children, active: Optional[Union[Var[bool], bool]]=None, avatar: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, loading: Optional[Union[Var[bool], bool]]=None, paragraph: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, round: Optional[Union[Var[bool], bool]]=None, title: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Skeleton':
+    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, options: Optional[Union[List[str], List[int], List[Dict]]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, value: Optional[Union[Var[Union[str, int]], Union[str, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Segmented':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-skeleton = Skeleton.create
+segmented = Segmented.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
-
-
-class Slider(AntdComponent):
-    tag = 'Slider'
-
-    auto_adjust_overflow: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    default_value: Optional[Var[Union[int, List[int]]]]
-    disabled: Optional[Var[bool]]
-    keyboard: Optional[Var[bool]]
-    dots: Optional[Var[bool]]
-    included: Optional[Var[bool]]
-    marks: Optional[Var[Union[Dict, ContainVar]]]
-    max: Optional[Var[int]]
-    min: Optional[Var[int]]
-    range: Optional[Var[bool]]
-    reverse: Optional[Var[bool]]
-    step: Optional[Var[int]]
-    tooltip: Optional[Var[Union[Dict, ContainVar]]]
-    value: Optional[Var[Union[int, List[int]]]]
-    vertical: Optional[Var[bool]]
-    # range
-    draggable_track: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_change_complete": lambda v: [v],
-            EventTriggers.ON_CHANGE: lambda v: [v],
-        })
-        return _triggers
-
-
-slider = Slider.create
-
-
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
+
+
+class InputNumber(AntdComponent):
+    tag = "InputNumber"
+
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    auto_focus: Optional[Var[bool]]
+    change_on_blur: Optional[Var[bool]]
+    change_on_wheel: Optional[Var[bool]]
+    controls: Optional[Var[Union[bool, ContainVar]]]
+    decimal_separator: Optional[Var[str]]
+    placeholder: Optional[Var[str]]
+    default_value: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    formatter: Optional[Var[JsValue]]
+    keyboard: Optional[Var[bool]]
+    max: Optional[Var[int]]
+    min: Optional[Var[int]]
+    parser: Optional[Var[JsValue]]
+    precision: Optional[Var[int]]
+    read_only: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    prefix: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    step: Optional[Var[Union[int, str]]]
+    string_mode: Optional[Var[bool]]
+    value: Optional[Var[int]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value: [value],
+            'on_press_enter': lambda e: [e],
+            "on_step": lambda value, info: [value, info],
+        })
+        return _triggers
+
+
+input_number = InputNumber.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 slider = Slider.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict
-from reflex import Component, Var
+from types import SimpleNamespace
+from functools import lru_cache
+import reflex as rx
+from reflex import Var, Component
+from reflex.vars import BaseVar, VarData
 from reflex.utils import imports
-from ..base import AntdComponent, ContainVar, ReactNode
-from ..constant import AlignType, DirectionType, SizeType
+from .. import base
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType
+next_theme_var_data = VarData(imports={f'next-themes': {imports.ImportVar(tag='useTheme')}, 'react': {imports.ImportVar(tag='useContext')}, 'antd': {imports.ImportVar(tag='theme', alias='AntdTheme')}}, hooks={f'const nextTheme = useTheme()': None})
+next_theme_var = BaseVar(_var_name='nextTheme.theme', _var_type='str', _var_data=next_theme_var_data)
+light_theme_var = BaseVar(_var_name='AntdTheme.defaultAlgorithm')
+dark_theme_var = BaseVar(_var_name='AntdTheme.darkAlgorithm')
 
-class Space(AntdComponent):
+def theme(**kwargs):
+    ...
+
+class Locale(JsValue):
+
+    @property
+    def lang(self) -> str:
+        ...
+
+    def serialize(self) -> str:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        ...
+
+class ConfigProvider(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, align: Optional[Union[Var[Literal['start', 'end', 'center', 'baseline', 'left', 'right']], Literal['start', 'end', 'center', 'baseline', 'left', 'right']]]=None, class_names: Optional[Union[Var[Dict], Dict]]=None, direction: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, split: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, styles: Optional[Union[Var[Dict], Dict]]=None, wrap: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Space':
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
+    def create(cls, *children, auto_insert_space_in_button: Optional[Union[Var[bool], bool]]=None, component_disabled: Optional[Union[Var[bool], bool]]=None, component_size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, csp: Optional[Union[Var[ContainVar], ContainVar]]=None, direction: Optional[Union[Var[str], str]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, get_target_container: Optional[Union[Var[JsValue], JsValue]]=None, icon_prefix_cls: Optional[Union[Var[str], str]]=None, locale: Optional[Union[Var[Locale], Locale]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, popup_overflow: Optional[Union[Var[str], str]]=None, prefix_cls: Optional[Union[Var[str], str]]=None, render_empty: Optional[Union[Var[JsValue], JsValue]]=None, theme: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, virtual: Optional[Union[Var[bool], bool]]=None, warning: Optional[Union[Var[Dict], Dict]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'ConfigProvider':
+        """Create a new ConfigProvider component.
 
         Returns:
-            The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
+            A new ConfigProvider component.
         """
         ...
 
-class SpaceCompact(AntdComponent):
+class AntdRegistryProvider(Component):
 
     @overload
     @classmethod
-    def create(cls, *children, block: Optional[Union[Var[bool], bool]]=None, direction: Optional[Union[Var[Literal['vertical', 'horizontal', 'inline']], Literal['vertical', 'horizontal', 'inline']]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'SpaceCompact':
+    def create(cls, *children, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdRegistryProvider':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-space = Space.create
-space_compact = SpaceCompact.create
+config_provider = ConfigProvider.create
+antd_registry_provider = AntdRegistryProvider.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType
 
-class Spin(AntdComponent):
+class Result(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, delay: Optional[Union[Var[int], int]]=None, indicator: Optional[Union[Var[Component], Component]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, spinning: Optional[Union[Var[bool], bool]]=None, tip: Optional[Union[Var[Component], Component]]=None, wrapper_class_name: Optional[Union[Var[str], str]]=None, fullscreen: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Spin':
+    def create(cls, *children, extra: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, status: Optional[Union[Var[Union[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active'], str]], Union[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active'], str]]]=None, sub_title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, title: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Result':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-spin = Spin.create
+result = Result.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import SizeType, PlacementType, TabsType
-
-
-class StatisticBase(AntdComponent):
-    prefix: Optional[Var[ReactNode]]
-    suffix: Optional[Var[ReactNode]]
-    title: Optional[Var[ReactNode]]
-    value: Optional[Var[Union[str, int]]]
-    value_style: Optional[Var[Dict]]
-
-
-class Statistic(StatisticBase):
-    tag = 'Statistic'
-
-    decimal_separator: Optional[Var[str]]
-    formatter: Optional[Var[JsValue]]
-    group_separator: Optional[Var[str]]
-    loading: Optional[Var[bool]]
-    precision: Optional[Var[int]]
-
-
-class StatisticCountdown(StatisticBase):
-    tag = 'Statistic.Countdown'
-
-    format: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_finish": lambda: [],
-            EventTriggers.ON_CHANGE: lambda value: [value],
-        })
-        return _triggers
-
-
-statistic = Statistic.create
-statistic_countdown = StatisticCountdown.create
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import TypeType, ButtonShape, SizeType
+
+
+class Button(AntdComponent):
+    tag = "Button"
+
+    block: Optional[Var[bool]]
+    danger: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    ghost: Optional[Var[bool]]
+    href: Optional[Var[str]]
+    target: Optional[Var[str]]
+    html_type: Optional[Var[str]]
+    icon: Optional[Var[ReactNode]]
+    loading: Optional[Var[bool]]
+    shape: Optional[Var[ButtonShape]]
+    size: Optional[Var[SizeType]]
+    type: Optional[Var[TypeType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+button = Button.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class Statistic(StatisticBase):
 
     @overload
     @classmethod
@@ -49,17 +46,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class StatisticCountdown(StatisticBase):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
@@ -77,14 +71,11 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 statistic = Statistic.create
 statistic_countdown = StatisticCountdown.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import PlacementType, DirectionType, SizeType, StepsStatusType, StepsType
-
-
-class Steps(AntdComponent):
-    tag = 'Steps'
-
-    current: Optional[Var[int]]
-    direction: Optional[Var[DirectionType]]
-    initial: Optional[Var[int]]
-    label_placement: Optional[Var[DirectionType]]
-    percent: Optional[Var[int]]
-    progress_dot: Optional[Var[Union[bool, JsValue]]]
-    responsive: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StepsStatusType]]
-    type: Optional[Var[StepsType]]
-
-    items: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda current: [current],
-        })
-        return _triggers
-
-
-steps = Steps.create
-
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import PlacementType, DirectionType, SizeType, StepsStatusType, StepsType
+
+
+class Steps(AntdComponent):
+    tag = 'Steps'
+
+    current: Optional[Var[int]]
+    direction: Optional[Var[DirectionType]]
+    initial: Optional[Var[int]]
+    label_placement: Optional[Var[DirectionType]]
+    percent: Optional[Var[int]]
+    progress_dot: Optional[Var[Union[bool, JsValue]]]
+    responsive: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StepsStatusType]]
+    type: Optional[Var[StepsType]]
+
+    items: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda current: [current],
+        })
+        return _triggers
+
+
+steps = Steps.create
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 steps = Steps.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
+from typing import Optional, Union, Dict, Any, List, Tuple
+from reflex import Component, Var
+from reflex.utils import imports
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, PlacementType, TypeType
 
-class Switch(AntdComponent):
+class Tour(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, checked_children: Optional[Union[Var[Component], Component]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, loading: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, un_checked_children: Optional[Union[Var[Component], Component]]=None, value: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Switch':
+    def create(cls, *children, arrow: Optional[Union[Var[bool], bool]]=None, close_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, disabled_interaction: Optional[Union[Var[bool], bool]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, mask: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, type: Optional[Union[Var[Literal['default', 'primary']], Literal['default', 'primary']]]=None, open: Optional[Union[Var[bool], bool]]=None, current: Optional[Union[Var[int], int]]=None, scroll_into_view_options: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, steps: Optional[Union[Var[ContainVar], ContainVar]]=None, indicators_render: Optional[Union[Var[JsValue], JsValue]]=None, z_index: Optional[Union[Var[int], int]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_finish: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, steps.*.on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tour':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-switch = Switch.create
+tour = Tour.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-from reflex.utils import imports
-
-from ..base import AntdComponent, ContainVar, JsValue, JsEvent
-from ..constant import StatusType, SizeType
-
-
-class Table(AntdComponent):
-    tag = 'Table'
-
-    bordered: Optional[Var[bool]]
-    columns: Optional[Var[Union[ContainVar, list]]]
-    data_source: Optional[Var[List[Dict[str, Any]]]]
-    expandable: Optional[Var[ContainVar]]
-    footer: Optional[Var[JsValue]]
-    get_popup_container: Optional[Var[JsValue]]
-    loading: Optional[Var[bool]]
-    locale: Optional[Var[ContainVar]]
-    pagination: Optional[Var[Union[bool, ContainVar]]]
-    row_key: Optional[Var[Union[str, JsValue]]]
-    row_selection: Optional[Var[ContainVar]]
-    scroll: Optional[Var[Union[ContainVar, Dict]]]
-    show_header: Optional[Var[bool]]
-    show_sorter_tooltip: Optional[Var[Union[bool, ContainVar]]]
-    size: Optional[Var[SizeType]] = 'middle'
-    sort_directions: Optional[Var[ContainVar]]
-    sticky: Optional[Var[Union[bool, JsValue]]]
-    summary: Optional[Var[JsValue]]
-    table_layout: Optional[Var[str]]
-    title: Optional[Var[JsValue]]
-    virtual: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda pagination, filters, sorter: [pagination, filters, sorter],
-            'on_header_row': lambda columns, index: [columns, index],
-            'on_row': lambda record, index: [record, index],
-            'on_scroll': lambda ev: [ev],
-
-            'columns.*.on_header_cell': lambda column: [column],
-            'columns.*.on_cell': lambda record, row_index: [record, row_index],
-            'columns.*.on_filter': lambda: [],
-            'columns.*.on_filter_dropdown_open_change': lambda visible: [visible],
-
-            'pagination.on_change': lambda page, size: [page, size],
-            'pagination.on_show_size_change': lambda current, size: [current, size],
-
-            'expandable.on_expand': lambda record, event: [record, event],
-            'expandable.on_expanded_rows_change': lambda rows: [rows],
-
-            'row_selection.on_cell': lambda record, index: [record, index],
-            'row_selection.on_change': lambda keys, rows, info: [keys, info],
-            'row_selection.on_select': lambda record, selected, selected_rows: [record, selected, selected_rows],
-            'row_selection.on_select_all':
-                lambda selected, selected_rows, change_rows: [selected, selected_rows, change_rows],
-        })
-        return _triggers
-
-
-table = Table.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar, JsValue, JsEvent
+from ..constant import StatusType, SizeType
+
+
+class Table(AntdComponent):
+    tag = 'Table'
+
+    bordered: Optional[Var[bool]]
+    columns: Optional[Var[Union[ContainVar, list]]]
+    data_source: Optional[Var[List[Dict[str, Any]]]]
+    expandable: Optional[Var[ContainVar]]
+    footer: Optional[Var[JsValue]]
+    get_popup_container: Optional[Var[JsValue]]
+    loading: Optional[Var[bool]]
+    locale: Optional[Var[ContainVar]]
+    pagination: Optional[Var[Union[bool, ContainVar]]]
+    row_key: Optional[Var[Union[str, JsValue]]]
+    row_selection: Optional[Var[ContainVar]]
+    scroll: Optional[Var[Union[ContainVar, Dict]]]
+    show_header: Optional[Var[bool]]
+    show_sorter_tooltip: Optional[Var[Union[bool, ContainVar]]]
+    size: Optional[Var[SizeType]] = 'middle'
+    sort_directions: Optional[Var[ContainVar]]
+    sticky: Optional[Var[Union[bool, JsValue]]]
+    summary: Optional[Var[JsValue]]
+    table_layout: Optional[Var[str]]
+    title: Optional[Var[JsValue]]
+    virtual: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda pagination, filters, sorter: [pagination, filters, sorter],
+            'on_header_row': lambda columns, index: [columns, index],
+            'on_row': lambda record, index: [record, index],
+            'on_scroll': lambda ev: [ev],
+
+            'columns.*.on_header_cell': lambda column: [column],
+            'columns.*.on_cell': lambda record, row_index: [record, row_index],
+            'columns.*.on_filter': lambda: [],
+            'columns.*.on_filter_dropdown_open_change': lambda visible: [visible],
+
+            'pagination.on_change': lambda page, size: [page, size],
+            'pagination.on_show_size_change': lambda current, size: [current, size],
+
+            'expandable.on_expand': lambda record, event: [record, event],
+            'expandable.on_expanded_rows_change': lambda rows: [rows],
+
+            'row_selection.on_cell': lambda record, index: [record, index],
+            'row_selection.on_change': lambda keys, rows, info: [keys, info],
+            'row_selection.on_select': lambda record, selected, selected_rows: [record, selected, selected_rows],
+            'row_selection.on_select_all':
+                lambda selected, selected_rows, change_rows: [selected, selected_rows, change_rows],
+        })
+        return _triggers
+
+
+table = Table.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,13 +27,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 table = Table.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-from dataclasses import dataclass
-
-from reflex import Component, Var, Base
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import SizeType, PlacementType, TabsType
-
-
-@dataclass(frozen=True)
-class TabItem:
-    close_icon: Optional[Var[ReactNode]] = None
-    destroy_inactive_tab_pane: Optional[Var[bool]] = None
-    disabled: Optional[Var[bool]] = None
-    force_render: Optional[Var[bool]] = None
-    key: Optional[Union[str, Var[str]]] = None
-    label: Optional[Union[ReactNode, Var[ReactNode]]] = None
-    icon: Optional[Var[ReactNode]] = None
-    children: Optional[Union[ReactNode, Var[ReactNode]]] = None
-    closable: Optional[Var[bool]] = None
-
-
-class Tabs(AntdComponent):
-    tag = 'Tabs'
-
-    active_key: Optional[Var[str]]
-    add_icon: Optional[Var[ReactNode]]
-    animated: Optional[Var[Union[bool, Dict]]]
-    centered: Optional[Var[bool]]
-    default_active_key: Optional[Var[str]]
-    hide_add: Optional[Var[bool]]
-    indicator: Optional[Var[Union[Dict, ContainVar]]]
-    items: Optional[Var[Union[ContainVar, List]]]
-    more_icon: Optional[Var[ReactNode]]
-    remove_icon: Optional[Var[ReactNode]]
-    popup_class_name: Optional[Var[str]]
-    render_tab_bar: Optional[Var[JsValue]]
-    size: Optional[Var[SizeType]]
-    tab_bar_extra_content: Optional[Var[Union[ReactNode, ContainVar]]]
-    tab_bar_gutter: Optional[Var[int]]
-    tab_bar_style: Optional[Var[Dict]]
-    tab_position: Optional[Var[PlacementType]]
-    destroy_inactive_tab_pane: Optional[Var[bool]]
-    type: Optional[Var[TabsType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda key: [key],
-            EventTriggers.ON_EDIT: lambda e0, e1: [e0, e1],
-            "on_tab_click": lambda key, ev: [key, ev],
-            "on_tab_scroll": lambda ev: [ev],
-        })
-        return _triggers
-
-
-tabs = Tabs.create
-tab_item = TabItem
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+from dataclasses import dataclass
+
+from reflex import Component, Var, Base
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType, PlacementType, TabsType
+
+
+@dataclass(frozen=True)
+class TabItem:
+    close_icon: Optional[Var[ReactNode]] = None
+    destroy_inactive_tab_pane: Optional[Var[bool]] = None
+    disabled: Optional[Var[bool]] = None
+    force_render: Optional[Var[bool]] = None
+    key: Optional[Union[str, Var[str]]] = None
+    label: Optional[Union[ReactNode, Var[ReactNode]]] = None
+    icon: Optional[Var[ReactNode]] = None
+    children: Optional[Union[ReactNode, Var[ReactNode]]] = None
+    closable: Optional[Var[bool]] = None
+
+
+class Tabs(AntdComponent):
+    tag = 'Tabs'
+
+    active_key: Optional[Var[str]]
+    add_icon: Optional[Var[ReactNode]]
+    animated: Optional[Var[Union[bool, Dict]]]
+    centered: Optional[Var[bool]]
+    default_active_key: Optional[Var[str]]
+    hide_add: Optional[Var[bool]]
+    indicator: Optional[Var[Union[Dict, ContainVar]]]
+    items: Optional[Var[Union[ContainVar, List]]]
+    more_icon: Optional[Var[ReactNode]]
+    remove_icon: Optional[Var[ReactNode]]
+    popup_class_name: Optional[Var[str]]
+    render_tab_bar: Optional[Var[JsValue]]
+    size: Optional[Var[SizeType]]
+    tab_bar_extra_content: Optional[Var[Union[ReactNode, ContainVar]]]
+    tab_bar_gutter: Optional[Var[int]]
+    tab_bar_style: Optional[Var[Dict]]
+    tab_position: Optional[Var[PlacementType]]
+    destroy_inactive_tab_pane: Optional[Var[bool]]
+    type: Optional[Var[TabsType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda key: [key],
+            EventTriggers.ON_EDIT: lambda e0, e1: [e0, e1],
+            "on_tab_click": lambda key, ev: [key, ev],
+            "on_tab_scroll": lambda ev: [ev],
+        })
+        return _triggers
+
+
+tabs = Tabs.create
+tab_item = TabItem
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
-from dataclasses import dataclass
-from reflex import Component, Var, Base
+from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType, PlacementType, TabsType
+from ..constant import StatusType, PlacementType, TriggerType
 
-@dataclass(frozen=True)
-class TabItem:
-    close_icon: Optional[Var[Component]]
-    destroy_inactive_tab_pane: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    force_render: Optional[Var[bool]]
-    key: Optional[Union[str, Var[str]]]
-    label: Optional[Union[str, Component, Var]]
-    icon: Optional[Var[Component]]
-    children: Optional[Union[str, Component, Var[Component]]]
-    closable: Optional[Var[bool]]
-
-class Tabs(AntdComponent):
+class Tooltip(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, active_key: Optional[Union[Var[str], str]]=None, add_icon: Optional[Union[Var[Component], Component]]=None, animated: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, centered: Optional[Union[Var[bool], bool]]=None, default_active_key: Optional[Union[Var[str], str]]=None, hide_add: Optional[Union[Var[bool], bool]]=None, indicator: Optional[Union[Var[Union[ContainVar, Dict]], Union[ContainVar, Dict]]]=None, items: Optional[Union[Var[Union[ContainVar, List]], Union[ContainVar, List]]]=None, more_icon: Optional[Union[Var[Component], Component]]=None, remove_icon: Optional[Union[Var[Component], Component]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, render_tab_bar: Optional[Union[Var[JsValue], JsValue]]=None, size: Optional[Union[Var[Literal['default', 'small', 'medium', 'middle', 'large']], Literal['default', 'small', 'medium', 'middle', 'large']]]=None, tab_bar_extra_content: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, tab_bar_gutter: Optional[Union[Var[int], int]]=None, tab_bar_style: Optional[Union[Var[Dict], Dict]]=None, tab_position: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, destroy_inactive_tab_pane: Optional[Union[Var[bool], bool]]=None, type: Optional[Union[Var[Literal['line', 'card', 'editable-card']], Literal['line', 'card', 'editable-card']]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_edit: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tab_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tabs':
+    def create(cls, *children, title: Optional[Union[Var[Union[str, Component, JsValue]], Union[str, Component, JsValue]]]=None, align: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, color: Optional[Union[Var[str], str]]=None, default_open: Optional[Union[Var[bool], bool]]=None, destroy_tooltip_on_hide: Optional[Union[Var[bool], bool]]=None, fresh: Optional[Union[Var[bool], bool]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, mouse_enter_delay: Optional[Union[Var[int], int]]=None, mouse_leave_delay: Optional[Union[Var[int], int]]=None, overlay_class_name: Optional[Union[Var[str], str]]=None, overlay_style: Optional[Union[Var[Dict], Dict]]=None, overlay_inner_style: Optional[Union[Var[Dict], Dict]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]], Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]]]=None, open: Optional[Union[Var[bool], bool]]=None, z_index: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tooltip':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-tabs = Tabs.create
-tab_item = TabItem
+tooltip = Tooltip.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TimelineModeType
-
-
-class Tag(AntdComponent):
-    tag = 'Tag'
-
-    close_icon: Optional[Var[Union[bool, ReactNode]]]
-    color: Optional[Var[str]]
-    icon: Optional[Var[ReactNode]]
-    bordered: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_close': lambda e: [e],
-        })
-        return _triggers
-
-
-class CheckableTag(AntdComponent):
-    tag = 'Tag.CheckableTag'
-
-    checked: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda checked: [checked],
-        })
-        return _triggers
-
-
-tag = Tag.create
-checkable_tag = CheckableTag.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TimelineModeType
+
+
+class Tag(AntdComponent):
+    tag = 'Tag'
+
+    close_icon: Optional[Var[Union[bool, ReactNode]]]
+    color: Optional[Var[str]]
+    icon: Optional[Var[ReactNode]]
+    bordered: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_close': lambda e: [e],
+        })
+        return _triggers
+
+
+class CheckableTag(AntdComponent):
+    tag = 'Tag.CheckableTag'
+
+    checked: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked: [checked],
+        })
+        return _triggers
+
+
+tag = Tag.create
+checkable_tag = CheckableTag.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List, Tuple
-from reflex import Component, Var
-from reflex.utils import imports
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TimelineModeType
+from ..base import AntdComponent, ContainVar
+from ..constant import StatusType, SizeType
 
-class Tag(AntdComponent):
+class Checkbox(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, close_icon: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, color: Optional[Union[Var[str], str]]=None, icon: Optional[Union[Var[Component], Component]]=None, bordered: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_close: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tag':
+    def create(cls, *children, auto_focus: Optional[Union[Var[bool], bool]]=None, checked: Optional[Union[Var[bool], bool]]=None, default_checked: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, indeterminate: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Checkbox':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class CheckableTag(AntdComponent):
+class CheckboxGroup(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, checked: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckableTag':
+    def create(cls, *children, default_value: Optional[Union[Var[List[Union[str, int]]], List[Union[str, int]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, options: Optional[Union[Var[List[Union[str, int, Dict]]], List[Union[str, int, Dict]]]]=None, value: Optional[Union[Var[List[Union[int, str, bool]]], List[Union[int, str, bool]]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'CheckboxGroup':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-tag = Tag.create
-checkable_tag = CheckableTag.create
+checkbox = Checkbox.create
+checkbox_group = CheckboxGroup.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List, Tuple
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TimelineModeType
+from ..constant import OrientationType, DirectionType
 
-class Timeline(AntdComponent):
+class Watermark(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, mode: Optional[Union[Var[Literal['left', 'alternate', 'right']], Literal['left', 'alternate', 'right']]]=None, pending: Optional[Union[Var[Component], Component]]=None, pending_dot: Optional[Union[Var[Component], Component]]=None, reverse: Optional[Union[Var[bool], bool]]=None, items: Optional[Union[Var[Union[List, ContainVar]], Union[List, ContainVar]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Timeline':
+    def create(cls, *children, width: Optional[Union[Var[int], int]]=None, height: Optional[Union[Var[int], int]]=None, inherit: Optional[Union[Var[bool], bool]]=None, rotate: Optional[Union[Var[int], int]]=None, z_index: Optional[Union[Var[int], int]]=None, image: Optional[Union[Var[str], str]]=None, content: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, font: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, gap: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, offset: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Watermark':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-timeline = Timeline.create
+watermark = Watermark.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, PlacementType, TriggerType
-
-
-class Tooltip(AntdComponent):
-    tag = "Tooltip"
-
-    title: Optional[Var[Union[str, Component, JsValue]]]
-    align: Optional[Var[str]]
-    arrow: Optional[Var[Union[bool, Dict]]]
-    auto_adjust_overflow: Optional[Var[bool]]
-    color: Optional[Var[str]]
-    default_open: Optional[Var[bool]]
-    destroy_tooltip_on_hide: Optional[Var[bool]]
-    fresh: Optional[Var[bool]]
-    get_popup_container: Optional[Var[JsValue]]
-    mouse_enter_delay: Optional[Var[int]]
-    mouse_leave_delay: Optional[Var[int]]
-    overlay_class_name: Optional[Var[str]]
-    overlay_style: Optional[Var[Dict]]
-    overlay_inner_style: Optional[Var[Dict]]
-    placement: Optional[Var[PlacementType]]
-    trigger: Optional[Var[Union[TriggerType, List[TriggerType]]]]
-    open: Optional[Var[bool]]
-    z_index: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-        })
-        return _triggers
-
-
-tooltip = Tooltip.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, PlacementType, TriggerType
+
+
+class Tooltip(AntdComponent):
+    tag = "Tooltip"
+
+    title: Optional[Var[Union[str, Component, JsValue]]]
+    align: Optional[Var[str]]
+    arrow: Optional[Var[Union[bool, Dict]]]
+    auto_adjust_overflow: Optional[Var[bool]]
+    color: Optional[Var[str]]
+    default_open: Optional[Var[bool]]
+    destroy_tooltip_on_hide: Optional[Var[bool]]
+    fresh: Optional[Var[bool]]
+    get_popup_container: Optional[Var[JsValue]]
+    mouse_enter_delay: Optional[Var[int]]
+    mouse_leave_delay: Optional[Var[int]]
+    overlay_class_name: Optional[Var[str]]
+    overlay_style: Optional[Var[Dict]]
+    overlay_inner_style: Optional[Var[Dict]]
+    placement: Optional[Var[PlacementType]]
+    trigger: Optional[Var[Union[TriggerType, List[TriggerType]]]]
+    open: Optional[Var[bool]]
+    z_index: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+        })
+        return _triggers
+
+
+tooltip = Tooltip.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List, Tuple
-from reflex import Component, Var
-from reflex.utils import imports
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, PlacementType, TriggerType
 
-class Tooltip(AntdComponent):
+class Upload(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, title: Optional[Union[Var[Union[str, Component, JsValue]], Union[str, Component, JsValue]]]=None, align: Optional[Union[Var[str], str]]=None, arrow: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, auto_adjust_overflow: Optional[Union[Var[bool], bool]]=None, color: Optional[Union[Var[str], str]]=None, default_open: Optional[Union[Var[bool], bool]]=None, destroy_tooltip_on_hide: Optional[Union[Var[bool], bool]]=None, fresh: Optional[Union[Var[bool], bool]]=None, get_popup_container: Optional[Union[Var[JsValue], JsValue]]=None, mouse_enter_delay: Optional[Union[Var[int], int]]=None, mouse_leave_delay: Optional[Union[Var[int], int]]=None, overlay_class_name: Optional[Union[Var[str], str]]=None, overlay_style: Optional[Union[Var[Dict], Dict]]=None, overlay_inner_style: Optional[Union[Var[Dict], Dict]]=None, placement: Optional[Union[Var[Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']], Literal['start', 'end', 'bottom', 'bottomLeft', 'bottomRight', 'top', 'topLeft', 'topRight']]]=None, trigger: Optional[Union[Var[Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]], Union[Literal['click', 'hover', 'focus', 'contextMenu'], List[Literal['click', 'hover', 'focus', 'contextMenu']]]]]=None, open: Optional[Union[Var[bool], bool]]=None, z_index: Optional[Union[Var[int], int]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_open_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Tooltip':
+    def create(cls, *children, accept: Optional[Union[Var[str], str]]=None, action: Optional[Union[Var[Union[str, JsValue]], Union[str, JsValue]]]=None, before_upload: Optional[Union[Var[JsValue], JsValue]]=None, custom_request: Optional[Union[Var[JsValue], JsValue]]=None, data: Optional[Union[Var[Union[ContainVar, JsValue]], Union[ContainVar, JsValue]]]=None, default_file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, directory: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, headers: Optional[Union[Var[Dict], Dict]]=None, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, is_image_url: Optional[Union[Var[JsValue], JsValue]]=None, list_type: Optional[Union[Var[str], str]]=None, max_count: Optional[Union[Var[int], int]]=None, method: Optional[Union[Var[str], str]]=None, multiple: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, open_file_dialog_on_click: Optional[Union[Var[bool], bool]]=None, preview_file: Optional[Union[Var[JsValue], JsValue]]=None, progress: Optional[Union[Var[Dict], Dict]]=None, show_upload_list: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, with_credentials: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_download: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_preview: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_remove: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Upload':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-tooltip = Tooltip.create
+upload = Upload.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,47 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, js_value, ReactNode
-from ..constant import StatusType
-
-
-class Transfer(AntdComponent):
-    tag = 'Transfer'
-    _rename_props: Dict[str, str] = {"itemRender": "render"}
-
-    data_source: Optional[Var[List]]
-    disabled: Optional[Var[bool]]
-    selections_icon: Optional[Var[ReactNode]]
-    filter_option: Optional[Var[JsValue]]
-    footer: Optional[Var[JsValue]]
-    list_style: Optional[Var[Union[Dict, JsValue]]]
-    locale: Optional[Var[Union[Dict, ContainVar]]]
-    one_way: Optional[Var[bool]]
-    operations: Optional[Var[List[str]]]
-    operation_style: Optional[Var[Dict]]
-    pagination: Optional[Var[Union[bool, ContainVar]]]
-    item_render: Optional[Var[Union[JsValue, ContainVar]]]
-    row_key: Optional[Var[JsValue]]
-    select_all_labels: Optional[Var[JsValue]]
-    selected_keys: Optional[Var[List[str]]]
-    show_search: Optional[Var[bool]]
-    showSelect_all: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    target_keys: Optional[Var[List[str]]]
-    titles: Optional[Var[ContainVar]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        if 'item_render' not in props:
-            props['item_render'] = js_value(lambda record: 'return record.title;')
-        com = super().create(*children, **props)
-        return com
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda target_keys, direction, move_keys: [target_keys, direction, move_keys],
-            EventTriggers.ON_SCROLL: lambda direction, ev: [direction, ev],
-            "on_search": lambda direction, value: [direction, value],
-            "on_select_change": lambda s_keys, t_keys: [s_keys, t_keys],
-        })
-        return _triggers
-
-
-transfer = Transfer.create
-
-
-
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+
+
+class Upload(AntdComponent):
+    tag = 'Upload'
+
+    accept: Optional[Var[str]]
+    action: Optional[Var[Union[str, JsValue]]]
+    before_upload: Optional[Var[JsValue]]
+    custom_request: Optional[Var[JsValue]]
+    data: Optional[Var[Union[ContainVar, JsValue]]]
+    default_file_list: Optional[Var[List[ContainVar]]]
+    directory: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    file_list: Optional[Var[List[ContainVar]]]
+    headers: Optional[Var[Dict]]
+    icon_render: Optional[Var[JsValue]]
+    is_image_url: Optional[Var[JsValue]]
+    list_type: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+    method: Optional[Var[str]]
+    multiple: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    open_file_dialog_on_click: Optional[Var[bool]]
+    preview_file: Optional[Var[JsValue]]
+    progress: Optional[Var[Dict]]
+    show_upload_list: Optional[Var[Union[bool, Dict]]]
+    with_credentials: Optional[Var[Union[bool]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda file, file_list: [file, file_list],
+            "on_drop": lambda event: [event],
+            "on_download": lambda file: [file],
+            "on_preview": lambda file: [file],
+            "on_remove": lambda file: [file]
+        })
+        return _triggers
+
+
+upload = Upload.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue, js_value
+from ..base import AntdComponent, ContainVar, JsValue, js_value, ReactNode
 from ..constant import StatusType
 
 class Transfer(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, data_source: Optional[Union[Var[List], List]]=None, disabled: Optional[Union[Var[bool], bool]]=None, selections_icon: Optional[Union[Var[Component], Component]]=None, filter_option: Optional[Union[Var[JsValue], JsValue]]=None, footer: Optional[Union[Var[JsValue], JsValue]]=None, list_style: Optional[Union[Var[Union[Dict, JsValue]], Union[Dict, JsValue]]]=None, locale: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, one_way: Optional[Union[Var[bool], bool]]=None, operations: Optional[Union[Var[List[str]], List[str]]]=None, operation_style: Optional[Union[Var[Dict], Dict]]=None, pagination: Optional[Union[Var[Union[bool, ContainVar]], Union[bool, ContainVar]]]=None, item_render: Optional[Union[Var[Union[JsValue, ContainVar]], Union[JsValue, ContainVar]]]=None, row_key: Optional[Union[Var[JsValue], JsValue]]=None, select_all_labels: Optional[Union[Var[JsValue], JsValue]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, show_search: Optional[Union[Var[bool], bool]]=None, showSelect_all: Optional[Union[Var[bool], bool]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, target_keys: Optional[Union[Var[List[str]], List[str]]]=None, titles: Optional[Union[Var[ContainVar], ContainVar]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Transfer':
+    def create(cls, *children, data_source: Optional[Union[Var[List], List]]=None, disabled: Optional[Union[Var[bool], bool]]=None, selections_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, filter_option: Optional[Union[Var[JsValue], JsValue]]=None, footer: Optional[Union[Var[JsValue], JsValue]]=None, list_style: Optional[Union[Var[Union[Dict, JsValue]], Union[Dict, JsValue]]]=None, locale: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, one_way: Optional[Union[Var[bool], bool]]=None, operations: Optional[Union[Var[List[str]], List[str]]]=None, operation_style: Optional[Union[Var[Dict], Dict]]=None, pagination: Optional[Union[Var[Union[ContainVar, bool]], Union[ContainVar, bool]]]=None, item_render: Optional[Union[Var[Union[JsValue, ContainVar]], Union[JsValue, ContainVar]]]=None, row_key: Optional[Union[Var[JsValue], JsValue]]=None, select_all_labels: Optional[Union[Var[JsValue], JsValue]]=None, selected_keys: Optional[Union[Var[List[str]], List[str]]]=None, show_search: Optional[Union[Var[bool], bool]]=None, showSelect_all: Optional[Union[Var[bool], bool]]=None, status: Optional[Union[Var[Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']], Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']]]=None, target_keys: Optional[Union[Var[List[str]], List[str]]]=None, titles: Optional[Union[Var[ContainVar], ContainVar]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Transfer':
         """"""
         ...
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 transfer = Transfer.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,13 +28,10 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 tree = Tree.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsNode
+from ..base import AntdComponent, ContainVar, JsNode, ReactNode
 
 class TreeSelect(AntdComponent):
 
     def get_event_triggers(self) -> Dict[str, Any]:
         ...
 
     @overload
     @classmethod
-    def create(cls, *children, allow_clear: Optional[Union[Var[Union[bool, Component]], Union[bool, Component]]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[bool, JsValue, JsEvent]], Union[bool, JsValue, JsEvent]]]=None, get_popup_container: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, max_tag_count: Optional[Union[Var[int], int]]=None, max_tag_placeholder: Optional[Union[Var[Union[Component, JsValue, JsEvent]], Union[Component, JsValue, JsEvent]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, multiple: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Component], Component]]=None, placeholder: Optional[Union[Var[str], str]]=None, placement: Optional[Union[Var[str], str]]=None, search_value: Optional[Union[Var[str], str]]=None, show_checked_strategy: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, suffix_icon: Optional[Union[Var[Component], Component]]=None, switcher_icon: Optional[Union[Var[Union[Component, ContainVar]], Union[Component, ContainVar]]]=None, tag_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_checkable: Optional[Union[Var[bool], bool]]=None, tree_check_strictly: Optional[Union[Var[bool], bool]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, tree_data_simple_mode: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_default_expand_all: Optional[Union[Var[bool], bool]]=None, tree_default_expanded_keys: Optional[Union[Var[List], List]]=None, tree_expand_action: Optional[Union[Var[Union[str, bool]], Union[str, bool]]]=None, tree_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_icon: Optional[Union[Var[bool], bool]]=None, tree_line: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_node_filter_prop: Optional[Union[Var[str], str]]=None, tree_node_label_prop: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[str], str]]=None, virtual: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tree_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TreeSelect':
+    def create(cls, *children, allow_clear: Optional[Union[Var[Union[bool, str, Component]], Union[bool, str, Component]]]=None, auto_clear_search_value: Optional[Union[Var[bool], bool]]=None, default_value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, disabled: Optional[Union[Var[bool], bool]]=None, popup_class_name: Optional[Union[Var[str], str]]=None, popup_match_select_width: Optional[Union[Var[Union[bool, int]], Union[bool, int]]]=None, dropdown_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, dropdown_style: Optional[Union[Var[Dict], Dict]]=None, field_names: Optional[Union[Var[Dict], Dict]]=None, filter_tree_node: Optional[Union[Var[Union[bool, JsValue, JsEvent]], Union[bool, JsValue, JsEvent]]]=None, get_popup_container: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, label_in_value: Optional[Union[Var[bool], bool]]=None, list_height: Optional[Union[Var[int], int]]=None, load_data: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, max_tag_count: Optional[Union[Var[int], int]]=None, max_tag_placeholder: Optional[Union[Var[Union[str, Component, JsValue, JsEvent]], Union[str, Component, JsValue, JsEvent]]]=None, max_tag_text_length: Optional[Union[Var[int], int]]=None, multiple: Optional[Union[Var[bool], bool]]=None, not_found_content: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, placeholder: Optional[Union[Var[str], str]]=None, placement: Optional[Union[Var[str], str]]=None, search_value: Optional[Union[Var[str], str]]=None, show_checked_strategy: Optional[Union[Var[str], str]]=None, show_search: Optional[Union[Var[bool], bool]]=None, size: Optional[Union[Var[str], str]]=None, status: Optional[Union[Var[str], str]]=None, suffix_icon: Optional[Union[Var[Union[str, Component]], Union[str, Component]]]=None, switcher_icon: Optional[Union[Var[Union[str, Component, ContainVar]], Union[str, Component, ContainVar]]]=None, tag_render: Optional[Union[Var[Union[JsValue, JsEvent]], Union[JsValue, JsEvent]]]=None, tree_checkable: Optional[Union[Var[bool], bool]]=None, tree_check_strictly: Optional[Union[Var[bool], bool]]=None, tree_data: Optional[Union[Var[List[Dict]], List[Dict]]]=None, tree_data_simple_mode: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_default_expand_all: Optional[Union[Var[bool], bool]]=None, tree_default_expanded_keys: Optional[Union[Var[List], List]]=None, tree_expand_action: Optional[Union[Var[Union[bool, str]], Union[bool, str]]]=None, tree_expanded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_icon: Optional[Union[Var[bool], bool]]=None, tree_line: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, tree_loaded_keys: Optional[Union[Var[List[str]], List[str]]]=None, tree_node_filter_prop: Optional[Union[Var[str], str]]=None, tree_node_label_prop: Optional[Union[Var[str], str]]=None, value: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, variant: Optional[Union[Var[str], str]]=None, virtual: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, filter_tree_node: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, load_data: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_dropdown_visible_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_search: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_select: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_tree_expand: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'TreeSelect':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 tree_select = TreeSelect.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TypographyTextType
-
-
-class TypographyBase(AntdComponent):
-    code: Optional[Var[bool]]
-    copyable: Optional[Var[Union[bool, ContainVar]]]
-    delete: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    editable: Optional[Var[Union[bool, ContainVar]]]
-    ellipsis: Optional[Var[Union[bool, ContainVar]]]
-
-    mark: Optional[Var[bool]]
-    italic: Optional[Var[bool]]
-    type: Optional[Var[TypographyTextType]]
-    underline: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda ev: [ev],
-            'copyable.on_copy': lambda ev: [ev],
-            'editable.on_change': lambda s: [s],
-            'editable.on_cancel': lambda: [],
-            'editable.on_start': lambda: [],
-            'editable.on_end': lambda: [],
-            'ellipsis.on_expand': lambda ev, info: [ev, info],
-            'ellipsis.on_ellipsis': lambda ellipsis: [ellipsis],
-        })
-        return _triggers
-
-
-class TypographyText(TypographyBase):
-    tag = 'Typography.Text'
-
-    keyboard: Optional[Var[bool]]
-    strong: Optional[Var[bool]]
-
-
-class TypographyTitle(TypographyBase):
-    tag = 'Typography.Title'
-
-    level: Optional[Var[int]]
-
-
-class TypographyParagraph(TypographyBase):
-    tag = 'Typography.Paragraph'
-
-    strong: Optional[Var[bool]]
-
-
-typography_text = TypographyText.create
-typography_title = TypographyTitle.create
-typography_paragraph = TypographyParagraph.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import TypographyTextType
+
+
+class TypographyBase(AntdComponent):
+    code: Optional[Var[bool]]
+    copyable: Optional[Var[Union[bool, ContainVar]]]
+    delete: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    editable: Optional[Var[Union[bool, ContainVar]]]
+    ellipsis: Optional[Var[Union[bool, ContainVar]]]
+
+    mark: Optional[Var[bool]]
+    italic: Optional[Var[bool]]
+    type: Optional[Var[TypographyTextType]]
+    underline: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda ev: [ev],
+            'copyable.on_copy': lambda ev: [ev],
+            'editable.on_change': lambda s: [s],
+            'editable.on_cancel': lambda: [],
+            'editable.on_start': lambda: [],
+            'editable.on_end': lambda: [],
+            'ellipsis.on_expand': lambda ev, info: [ev, info],
+            'ellipsis.on_ellipsis': lambda ellipsis: [ellipsis],
+        })
+        return _triggers
+
+
+class TypographyText(TypographyBase):
+    tag = 'Typography.Text'
+
+    keyboard: Optional[Var[bool]]
+    strong: Optional[Var[bool]]
+
+
+class TypographyTitle(TypographyBase):
+    tag = 'Typography.Title'
+
+    level: Optional[Var[int]]
+
+
+class TypographyParagraph(TypographyBase):
+    tag = 'Typography.Paragraph'
+
+    strong: Optional[Var[bool]]
+
+
+typography_text = TypographyText.create
+typography_title = TypographyTitle.create
+typography_paragraph = TypographyParagraph.create
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TypographyText(TypographyBase):
 
     @overload
     @classmethod
@@ -52,17 +49,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TypographyTitle(TypographyBase):
 
     @overload
     @classmethod
@@ -77,17 +71,14 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 class TypographyParagraph(TypographyBase):
 
     @overload
     @classmethod
@@ -102,15 +93,12 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 typography_text = TypographyText.create
 typography_title = TypographyTitle.create
 typography_paragraph = TypographyParagraph.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
+from typing import Optional, Union, Dict, Any, List, Tuple
+from reflex import Component, Var
+from reflex.utils import imports
 from reflex.constants import EventTriggers
 from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType
 
-class Upload(AntdComponent):
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        ...
+class Skeleton(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, accept: Optional[Union[Var[str], str]]=None, action: Optional[Union[Var[Union[str, JsValue]], Union[str, JsValue]]]=None, before_upload: Optional[Union[Var[JsValue], JsValue]]=None, custom_request: Optional[Union[Var[JsValue], JsValue]]=None, data: Optional[Union[Var[Union[ContainVar, JsValue]], Union[ContainVar, JsValue]]]=None, default_file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, directory: Optional[Union[Var[bool], bool]]=None, disabled: Optional[Union[Var[bool], bool]]=None, file_list: Optional[Union[Var[List[ContainVar]], List[ContainVar]]]=None, headers: Optional[Union[Var[Dict], Dict]]=None, icon_render: Optional[Union[Var[JsValue], JsValue]]=None, is_image_url: Optional[Union[Var[JsValue], JsValue]]=None, list_type: Optional[Union[Var[str], str]]=None, max_count: Optional[Union[Var[int], int]]=None, method: Optional[Union[Var[str], str]]=None, multiple: Optional[Union[Var[bool], bool]]=None, name: Optional[Union[Var[str], str]]=None, open_file_dialog_on_click: Optional[Union[Var[bool], bool]]=None, preview_file: Optional[Union[Var[JsValue], JsValue]]=None, progress: Optional[Union[Var[Dict], Dict]]=None, show_upload_list: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, with_credentials: Optional[Union[Var[bool], bool]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_change: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_download: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_drop: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_preview: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_remove: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Upload':
+    def create(cls, *children, active: Optional[Union[Var[bool], bool]]=None, avatar: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, loading: Optional[Union[Var[bool], bool]]=None, paragraph: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, round: Optional[Union[Var[bool], bool]]=None, title: Optional[Union[Var[Union[bool, Dict]], Union[bool, Dict]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Skeleton':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-upload = Upload.create
+skeleton = Skeleton.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import OrientationType, DirectionType
-
-
-class Watermark(AntdComponent):
-    tag = 'Watermark'
-
-    width: Optional[Var[int]]
-    height: Optional[Var[int]]
-    inherit: Optional[Var[bool]]
-    rotate: Optional[Var[int]]
-    z_index: Optional[Var[int]]
-    image: Optional[Var[str]]
-    content: Optional[Var[Union[str, List[str]]]]
-    font: Optional[Var[Union[Dict, ContainVar]]]
-    gap: Optional[Var[Tuple[int, int]]]
-    offset: Optional[Var[Tuple[int, int]]]
-
-
-watermark = Watermark.create
-
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import OrientationType, DirectionType
+
+
+class Watermark(AntdComponent):
+    tag = 'Watermark'
+
+    width: Optional[Var[int]]
+    height: Optional[Var[int]]
+    inherit: Optional[Var[bool]]
+    rotate: Optional[Var[int]]
+    z_index: Optional[Var[int]]
+    image: Optional[Var[str]]
+    content: Optional[Var[Union[str, List[str]]]]
+    font: Optional[Var[Union[Dict, ContainVar]]]
+    gap: Optional[Var[Tuple[int, int]]]
+    offset: Optional[Var[Tuple[int, int]]]
+
+
+watermark = Watermark.create
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Optional, Union, Dict, Any, List, Tuple
+from typing import Optional, Union
 from reflex import Component, Var
 from reflex.utils import imports
-from reflex.constants import EventTriggers
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent
 from ..constant import OrientationType, DirectionType
 
-class Watermark(AntdComponent):
+class Flex(AntdComponent):
 
     @overload
     @classmethod
-    def create(cls, *children, width: Optional[Union[Var[int], int]]=None, height: Optional[Union[Var[int], int]]=None, inherit: Optional[Union[Var[bool], bool]]=None, rotate: Optional[Union[Var[int], int]]=None, z_index: Optional[Union[Var[int], int]]=None, image: Optional[Union[Var[str], str]]=None, content: Optional[Union[Var[Union[str, List[str]]], Union[str, List[str]]]]=None, font: Optional[Union[Var[Union[Dict, ContainVar]], Union[Dict, ContainVar]]]=None, gap: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, offset: Optional[Union[Var[Tuple[int, int]], Tuple[int, int]]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Watermark':
+    def create(cls, *children, vertical: Optional[Union[Var[bool], bool]]=None, wrap: Optional[Union[Var[str], str]]=None, justify: Optional[Union[Var[str], str]]=None, align: Optional[Union[Var[str], str]]=None, flex: Optional[Union[Var[str], str]]=None, gap: Optional[Union[Var[str], str]]=None, component: Optional[Union[Var[str], str]]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'Flex':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
-watermark = Watermark.create
+flex = Flex.create
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.8/custom_components/reflex_antd/base.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional
+from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional, Self
 import sys
 from os import path
 from abc import ABC, abstractmethod
 from functools import lru_cache, wraps
 from hashlib import md5
 import uuid
 import dataclasses
 import inspect
 import re
-from pydantic import PrivateAttr
 import reflex as rx
 from reflex import Component, Var, State, Base
+from reflex.base import pydantic
 from reflex.components.component import BaseComponent, CustomComponent, StatefulComponent
-from reflex.constants import Hooks, Reflex, MemoizationDisposition
+from reflex.components.base.bare import Bare
+from reflex.constants import Hooks, Reflex, MemoizationDisposition, MemoizationMode
 from reflex.utils import imports, format
 from reflex.vars import BaseVar, VarData
 from reflex.event import EventHandler, EventSpec, EventChain
 from .constant import SizeType
 from .util import OrderedSet
 version = '.'.join(map(lambda x: x.zfill(3), Reflex.VERSION.split('.')))
 my_path = path.abspath(path.dirname(__file__))
 template_path = path.join(my_path, '.templates')
 APP_ROUTER = False
 RE_KEY_IDX = re.compile('\\.\\d+\\.')
+memo_never = MemoizationMode().set(disposition=MemoizationDisposition.NEVER)
+memo_never_no_recursive = MemoizationMode().set(disposition=MemoizationDisposition.NEVER, recursive=False)
+memo_always = MemoizationMode().set(disposition=MemoizationDisposition.ALWAYS)
+memo_always_no_recursive = MemoizationMode().set(disposition=MemoizationDisposition.ALWAYS, recursive=False)
 
 def stateful(hd: Callable[..., Component]=None, forced=True) -> Callable:
     ...
 
 def pretty_dumps(value: Any, indent=2) -> str:
     ...
 
+def get_component_all_imports(com: Component) -> imports.ImportDict:
+    ...
+
+def get_component_hooks(com) -> Set[str] | Dict[str, None]:
+    ...
+
+def get_component_custom_code(com: Component) -> Set[str]:
+    ...
+
 class ExItem(ABC):
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
         ...
 
     @abstractmethod
@@ -46,15 +60,15 @@
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
     def get_state(self) -> str:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_interpolations(self) -> List[Tuple[int, int]]:
         ...
 
     def get_var_data(self) -> VarData:
         ...
@@ -74,15 +88,15 @@
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_custom_components(self) -> set[CustomComponent]:
         ...
 
     def get_custom_code(self) -> set[str]:
         ...
@@ -98,20 +112,24 @@
         ...
 
     def serialize(self) -> str:
         ...
 
 class JsEvent:
     hd: EventHandler
+    event_trigger: Callable
 
     def get_state_full_name(self) -> str:
         ...
 
     def get_event_args(self) -> str:
         ...
+
+    def get_ex_item(self, parent, key) -> ExItem:
+        ...
 js_event = JsEvent
 
 class ExEventHandlerItem(ExItem):
     item: JsEvent
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
@@ -120,34 +138,35 @@
     @property
     def hd_item(self) -> 'ExLambdaHandlerItem':
         ...
 
     def serialize(self) -> str:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
 class ExLambdaHandlerItem(ExItem):
     item: Callable
+    event_trigger: Callable
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
         ...
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
 class ExCallableItem(ExItem):
     item: Callable
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
@@ -155,15 +174,15 @@
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
 class ExStateItem(ExItem):
     item: BaseVar
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
@@ -171,33 +190,47 @@
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_state(self) -> str:
         ...
 
+class FakeComponentMixin:
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        ...
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        ...
+
 class JsValue:
-    value: Callable | str
+    value: Callable | str | Component
+
+    def get_ex_item(self, parent, key) -> ExItem:
+        ...
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
     def get_state(self) -> str:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_var_data(self) -> VarData:
         ...
 
     def get_custom_components(self) -> set[CustomComponent]:
         ...
@@ -206,21 +239,21 @@
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_custom_components(self) -> set[CustomComponent]:
         ...
 
-def js_value(value: Union[str, Callable], **kwargs) -> JsValue:
+def js_value(value: Union[str, Callable, Component], **kwargs) -> JsValue:
     ...
 
 class ExJsItem(ExItem):
     item: JsValue
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
@@ -228,33 +261,58 @@
 
     def serialize(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_custom_components(self) -> set[CustomComponent]:
         ...
 
+class ExVarItem(ExItem):
+    item: Var
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        ...
+
+    def serialize(self) -> str:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        ...
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        ...
+
+    def get_state(self) -> str:
+        ...
+
+    def get_interpolations(self) -> List[Tuple[int, int]]:
+        ...
+
 class ExFormatter:
     items: List[Type[ExItem]]
 
+    def get_ex_item(self, key: str) -> ExItem | None:
+        ...
+
     def get_value(self) -> str:
         ...
 
     def get_imports(self) -> imports.ImportDict:
         ...
 
     def get_state(self) -> str:
         ...
 
-    def get_hooks(self) -> Set[str]:
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
         ...
 
     def get_interpolations(self) -> List[Tuple[int, int]]:
         ...
 
     def get_var_data(self) -> VarData:
         ...
@@ -266,39 +324,62 @@
 class NodeVar(ExVar):
     pass
 
 @dataclasses.dataclass(eq=False, **{'slots': True} if sys.version_info >= (3, 10) else {})
 class ContainVar(ExVar):
 
     @classmethod
-    def create(cls, _args_: Any=None, **kwargs) -> Var | None:
+    def create(cls, _args_: Any=None, **kwargs) -> Self:
         ...
 
-    def init(self, parent: Component, name: str):
+    def init(self, parent: Component, name: str) -> Self:
         ...
 
     def get_custom_components(self) -> set[CustomComponent]:
         ...
 
     def get_custom_code(self) -> Set[str]:
         ...
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        ...
 contain = ContainVar.create
 
+def container(data: Union[list, dict], name: str='') -> rx.Component:
+    ...
+
 class VarDataMixin:
     ...
 
-class AntdBaseMixin:
+class AntdBaseComponent(Component):
 
-    def get_custom_components(self, seen: set[str] | None=None) -> Set[CustomComponent]:
-        ...
+    @overload
+    @classmethod
+    def create(cls, *children, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdBaseComponent':
+        """Create the component.
 
-    def get_custom_code(self) -> Set[str]:
+        Args:
+            *children: The children of the component.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
         ...
 
-class AntdComponent(AntdBaseMixin, Component):
+class AntdComponent(AntdBaseComponent):
 
     @overload
     @classmethod
     def create(cls, *children, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdComponent':
         """Create the component.
 
         Args:
@@ -309,42 +390,36 @@
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
-class AntdSubComponent(AntdBaseMixin, Component):
+class AntdSubComponent(AntdBaseComponent, Component):
 
     @overload
     @classmethod
-    def create(cls, *children, base_tag: Optional[str]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdSubComponent':
+    def create(cls, *children, base_tag: Optional[str]=None, _custom_components: Optional[Set[CustomComponent]]=None, style: Optional[Style]=None, key: Optional[Any]=None, id: Optional[Any]=None, class_name: Optional[Any]=None, autofocus: Optional[bool]=None, custom_attrs: Optional[Dict[str, Union[Var, str]]]=None, on_blur: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_context_menu: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_double_click: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_focus: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_down: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_enter: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_leave: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_move: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_out: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_over: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_mouse_up: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_scroll: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, on_unmount: Optional[Union[EventHandler, EventSpec, list, function, BaseVar]]=None, **props) -> 'AntdSubComponent':
         """Create the component.
 
         Args:
             *children: The children of the component.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
-
-        Raises:
-            TypeError: If an invalid child is passed.
         """
         ...
 
 def default_config(provider: Component):
     ...
 
 def patch_all():
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/constant.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Literal
-
-
-ThemeType = Literal["light", "dark"]
-PlacementType = Literal["start", "end", "bottom", "bottomLeft", "bottomRight", "top", "topLeft", "topRight"]
-AlignType = Literal["start", "end", "center", "baseline", "left", "right"]
-OrientationType = Literal["left", "right", "top", "bottom", "center"]
-DirectionType = Literal["vertical", "horizontal", "inline"]
-SizeType = Literal["default", "small", "medium", "middle", "large"]
-StatusType = Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']
-TriggerType = Literal["click", "hover", "focus", 'contextMenu']
-VariantType = Literal['outlined', 'borderless', 'filled']
-TypeType = Literal['default', 'primary']
-RoleType = Literal['alert', 'status']
-BreakpointType = Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl']
-
-ColorFormatType = Literal['rgb', 'hex', 'hsb']
-
-ButtonShape = Literal['default', 'circle', 'round']
-
-TypographyTextType = Literal['secondary', 'success', 'warning', 'danger']
-
-FloatGroupShapeType = Literal["circle", "square"]
-
-BadgeStatusType = Literal["success", 'processing', 'default', 'error', 'warning']
-
-StepsStatusType = Literal['wait', 'process', 'finish', 'error']
-StepsType = Literal['default', 'navigation', 'inline']
-
-DatePickerModeType = Literal['time', 'date', 'month', 'year', 'decade']
-DatePickerType = Literal['date', 'week', 'month', 'quarter', 'year']
-
-RadioStyleType = Literal['outline', 'solid']
-RadioType = Literal['default', 'button']
-
-SelectModeType = Literal['multiple', 'tags']
-
-ProgressType = Literal['line', 'circle', 'dashboard']
-
-TimelineModeType = Literal['left', 'alternate', 'right']
-
-TabsType = Literal['line', 'card', 'editable-card']
-
-QRCodeType = Literal['canvas', 'svg']
-QRCodeErrorLevelType = Literal['L', 'M', 'Q', 'H']
-QRCodeStatusType = Literal['active', 'expired', 'loading', 'scanned']
-
-MessageType = Literal['info', 'success', 'error', 'loading', 'warning']
+from typing import Literal
+
+
+ThemeType = Literal["light", "dark"]
+PlacementType = Literal["start", "end", "bottom", "bottomLeft", "bottomRight", "top", "topLeft", "topRight"]
+AlignType = Literal["start", "end", "center", "baseline", "left", "right"]
+OrientationType = Literal["left", "right", "top", "bottom", "center"]
+DirectionType = Literal["vertical", "horizontal", "inline"]
+SizeType = Literal["default", "small", "medium", "middle", "large"]
+StatusType = Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']
+TriggerType = Literal["click", "hover", "focus", 'contextMenu']
+VariantType = Literal['outlined', 'borderless', 'filled']
+TypeType = Literal['default', 'primary']
+RoleType = Literal['alert', 'status']
+BreakpointType = Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl']
+
+ColorFormatType = Literal['rgb', 'hex', 'hsb']
+
+ButtonShape = Literal['default', 'circle', 'round']
+
+TypographyTextType = Literal['secondary', 'success', 'warning', 'danger']
+
+FloatGroupShapeType = Literal["circle", "square"]
+
+BadgeStatusType = Literal["success", 'processing', 'default', 'error', 'warning']
+
+StepsStatusType = Literal['wait', 'process', 'finish', 'error']
+StepsType = Literal['default', 'navigation', 'inline']
+
+DatePickerModeType = Literal['time', 'date', 'month', 'year', 'decade']
+DatePickerType = Literal['date', 'week', 'month', 'quarter', 'year']
+
+RadioStyleType = Literal['outline', 'solid']
+RadioType = Literal['default', 'button']
+
+SelectModeType = Literal['multiple', 'tags']
+
+ProgressType = Literal['line', 'circle', 'dashboard']
+
+TimelineModeType = Literal['left', 'alternate', 'right']
+
+TabsType = Literal['line', 'card', 'editable-card']
+
+QRCodeType = Literal['canvas', 'svg']
+QRCodeErrorLevelType = Literal['L', 'M', 'Q', 'H']
+QRCodeStatusType = Literal['active', 'expired', 'loading', 'scanned']
+
+MessageType = Literal['info', 'success', 'error', 'loading', 'warning']
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/display.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .antd.badge import badge, badge_ribbon  # noqa
-from .antd.table import table  # noqa
-from .antd.tree import tree  # noqa
-from .antd.avatar import avatar,avatar_group  # noqa
-from .antd.calendar import calendar,dayjs  # noqa
-from .antd.card import card,card_grid,card_meta  # noqa
-from .antd.carousel import carousel  # noqa
-from .antd.collapse import collapse  # noqa
-from .antd.descriptions import descriptions  # noqa
-from .antd.empty import empty  # noqa
-from .antd.image import image,image_preview_group  # noqa
-from .antd.list import alist,list_item,list_item_meta  # noqa
-from .antd.popover import popover  # noqa
-from .antd.qrcode import qrcode  # noqa
-from .antd.segmented import segmented  # noqa
-from .antd.statistic import statistic, statistic_countdown  # noqa
-from .antd.tabs import tabs, tab_item  # noqa
-from .antd.tag import tag, checkable_tag  # noqa
-from .antd.timeline import timeline  # noqa
-from .antd.tooltip import tooltip  # noqa
-from .antd.tour import tour  # noqa
-
+from .antd.badge import badge, badge_ribbon  # noqa
+from .antd.table import table  # noqa
+from .antd.tree import tree  # noqa
+from .antd.avatar import avatar,avatar_group  # noqa
+from .antd.calendar import calendar,dayjs  # noqa
+from .antd.card import card,card_grid,card_meta  # noqa
+from .antd.carousel import carousel  # noqa
+from .antd.collapse import collapse  # noqa
+from .antd.descriptions import descriptions  # noqa
+from .antd.empty import empty  # noqa
+from .antd.image import image,image_preview_group  # noqa
+from .antd.list import alist,list_item,list_item_meta  # noqa
+from .antd.popover import popover  # noqa
+from .antd.qrcode import qrcode  # noqa
+from .antd.segmented import segmented  # noqa
+from .antd.statistic import statistic, statistic_countdown  # noqa
+from .antd.tabs import tabs, tab_item  # noqa
+from .antd.tag import tag, checkable_tag  # noqa
+from .antd.timeline import timeline  # noqa
+from .antd.tooltip import tooltip  # noqa
+from .antd.tour import tour  # noqa
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/entry.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from .antd.auto_complete import auto_complete  # noqa
-from .antd.cascader import cascader  # noqa
-from .antd.checkbox import checkbox_group, checkbox  # noqa
-from .antd.color_picker import color_picker  # noqa
-from .antd.date_picker import dayjs, date_picker, range_picker  # noqa
-from .antd.form import form, form_item, form_list, form_provider, confirm_form, modal_form  # noqa
-from .antd.input import input, text_area, search, password  # noqa
-from .antd.input_number import input_number  # noqa
-from .antd.mentions import mention  # noqa
-from .antd.radio import radio, radio_button, radio_group  # noqa
-from .antd.rate import rate  # noqa
-from .antd.select import select  # noqa
-from .antd.tree_select import tree_select  # noqa
-from .antd.slider import slider  # noqa
-from .antd.switch import switch  # noqa
-from .antd.transfer import transfer  # noqa
-from .antd.upload import upload  # noqa
-
-
+from .antd.auto_complete import auto_complete  # noqa
+from .antd.cascader import cascader  # noqa
+from .antd.checkbox import checkbox_group, checkbox  # noqa
+from .antd.color_picker import color_picker  # noqa
+from .antd.date_picker import dayjs, date_picker, range_picker  # noqa
+from .antd.form import form, form_item, form_list, form_provider, confirm_form, modal_form  # noqa
+from .antd.input import input, text_area, search, password  # noqa
+from .antd.input_number import input_number  # noqa
+from .antd.mentions import mention  # noqa
+from .antd.radio import radio, radio_button, radio_group  # noqa
+from .antd.rate import rate  # noqa
+from .antd.select import select  # noqa
+from .antd.tree_select import tree_select  # noqa
+from .antd.slider import slider  # noqa
+from .antd.switch import switch  # noqa
+from .antd.transfer import transfer  # noqa
+from .antd.upload import upload  # noqa
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd/feedback.py` & `reflex_antd-0.0.8/custom_components/reflex_antd/feedback.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .antd.progress import progress  # noqa
-from .antd.result import result  # noqa
-from .antd.skeleton import skeleton  # noqa
-from .antd.spin import spin  # noqa
-from .antd.watermark import watermark  # noqa
-from .antd.alert import alert, alert_error_boundary  # noqa
-from .antd.drawer import drawer  # noqa
-from .antd.message import message, message_holder  # noqa
-from .antd.notification import notification  # noqa
-from .antd.modal import modal, confirm  # noqa
-from .antd.popconfirm import popconfirm  # noqa
+from .antd.progress import progress  # noqa
+from .antd.result import result  # noqa
+from .antd.skeleton import skeleton  # noqa
+from .antd.spin import spin  # noqa
+from .antd.watermark import watermark  # noqa
+from .antd.alert import alert, alert_error_boundary  # noqa
+from .antd.drawer import drawer  # noqa
+from .antd.message import message, message_holder  # noqa
+from .antd.notification import notification  # noqa
+from .antd.modal import modal, confirm  # noqa
+from .antd.popconfirm import popconfirm  # noqa
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1
-Name: reflex-antd
-Version: 0.0.7
-Summary: Reflex custom component antd
-Author-email: seewind <seewindcn@gmail.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: source, https://github.com/seewindcn/reflex-antd
-Keywords: reflex,reflex-custom-components
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.2
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# reflex-antd
-
-A Reflex custom component wrap [ant.design](https://ant.design/).
-
-## Installation
-
-```bash
-pip install reflex-antd
-```
-
-## antd-demo
-
-[antd-demo](https://antd-demo.reflex.run)
-
-
-### screen
-- table
-![table](docs/img/table1.png)
-- menu
-![menu1](docs/img/menu1.png)
-- transfer
-![transfer1](docs/img/transfer1.png)
-- ...
-
-
-
+Metadata-Version: 2.1
+Name: reflex-antd
+Version: 0.0.8
+Summary: Reflex custom component antd
+Author-email: seewind <seewindcn@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: source, https://github.com/seewindcn/reflex-antd
+Keywords: reflex,reflex-custom-components,ant-design,antd
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: reflex>=0.4.2
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# reflex-antd
+
+A Reflex custom component wrap [ant.design](https://ant.design/).
+pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
+
+## Installation
+
+```bash
+pip install reflex-antd
+```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 custom_components/reflex_antd/antd/auto_complete.py
 custom_components/reflex_antd/antd/auto_complete.pyi
 custom_components/reflex_antd/antd/avatar.py
 custom_components/reflex_antd/antd/avatar.pyi
 custom_components/reflex_antd/antd/badge.py
 custom_components/reflex_antd/antd/badge.pyi
 custom_components/reflex_antd/antd/base.py
+custom_components/reflex_antd/antd/base.pyi
 custom_components/reflex_antd/antd/breadcrumb.py
 custom_components/reflex_antd/antd/breadcrumb.pyi
 custom_components/reflex_antd/antd/button.py
 custom_components/reflex_antd/antd/button.pyi
 custom_components/reflex_antd/antd/calendar.py
 custom_components/reflex_antd/antd/calendar.pyi
 custom_components/reflex_antd/antd/card.py
```

### Comparing `reflex_antd-0.0.7/pyproject.toml` & `reflex_antd-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "reflex-antd"
-version = "0.0.7"
-description = "Reflex custom component antd"
-readme = "README.md"
-license = { text = "Apache-2.0" }
-requires-python = ">=3.8"
-authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
-keywords = [
-    "reflex",
-    "reflex-custom-components"]
-
-dependencies = [
-    "reflex>=0.4.2"
-]
-
-classifiers = [
-  "Development Status :: 4 - Beta",
-]
-
-[project.urls]
-Homepage = "https://github.com/seewindcn/reflex-antd"
-homepage = "https://github.com/seewindcn/reflex-antd"
-source = "https://github.com/seewindcn/reflex-antd"
-
-[project.optional-dependencies]
-dev = ["build", "twine"]
-
-
-
-[tool.setuptools.packages.find]
-where = ["custom_components"]
+[build-system]
+requires = [
+    "setuptools",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "reflex-antd"
+version = "0.0.8"
+description = "Reflex custom component antd"
+readme = "README.md"
+license = { text = "Apache-2.0" }
+requires-python = ">=3.8"
+authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
+keywords = [
+    "reflex",
+    "reflex-custom-components",
+    "ant-design", "antd",
+]
+
+dependencies = [
+    "reflex>=0.4.2"
+]
+
+classifiers = [
+  "Development Status :: 4 - Beta",
+]
+
+[project.urls]
+Homepage = "https://github.com/seewindcn/reflex-antd"
+homepage = "https://github.com/seewindcn/reflex-antd"
+source = "https://github.com/seewindcn/reflex-antd"
+
+[project.optional-dependencies]
+dev = ["build", "twine"]
+
+
+
+[tool.setuptools.packages.find]
+where = ["custom_components"]
```

