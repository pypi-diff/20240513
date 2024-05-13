# Comparing `tmp/qtdraw-1.1.8.tar.gz` & `tmp/qtdraw-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.8.tar", last modified: Mon Jul 31 11:56:17 2023, max compression
+gzip compressed data, was "qtdraw-1.1.9.tar", last modified: Sat Aug 12 05:51:22 2023, max compression
```

## Comparing `qtdraw-1.1.8.tar` & `qtdraw-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670512 qtdraw-1.1.8/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.8/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.8/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 11:56:17.670595 qtdraw-1.1.8/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.8/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.662486 qtdraw-1.1.8/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-31 11:33:10.000000 qtdraw-1.1.8/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.668797 qtdraw-1.1.8/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.8/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.8/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.8/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.669552 qtdraw-1.1.8/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.8/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.8/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/multipie/setting.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670066 qtdraw-1.1.8/qtdraw/parser/
--rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.8/qtdraw/parser/element.py
--rw-r--r--   0 hiro       (501) staff       (20)     6330 2023-07-31 11:45:17.000000 qtdraw-1.1.8/qtdraw/parser/read_cif_vesta.py
--rw-------   0 hiro       (501) staff       (20)     2983 2023-07-31 11:45:03.000000 qtdraw-1.1.8/qtdraw/parser/vesta.py
--rw-r--r--   0 hiro       (501) staff       (20)    92584 2023-07-31 11:36:18.000000 qtdraw-1.1.8/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670283 qtdraw-1.1.8/qtdraw/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.8/qtdraw/scripts/qtdraw.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.663480 qtdraw-1.1.8/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1082 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      127 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      753 2023-07-31 11:56:17.670845 qtdraw-1.1.8/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.8/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.193445 qtdraw-1.1.9/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.9/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.9/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-08-12 05:51:22.193528 qtdraw-1.1.9/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.9/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.185718 qtdraw-1.1.9/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-08-12 05:24:35.000000 qtdraw-1.1.9/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.191623 qtdraw-1.1.9/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.9/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2397 2023-08-12 05:36:48.000000 qtdraw-1.1.9/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.9/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.9/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.9/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.192407 qtdraw-1.1.9/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    48611 2023-08-12 05:43:14.000000 qtdraw-1.1.9/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.9/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/multipie/setting.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.192957 qtdraw-1.1.9/qtdraw/parser/
+-rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.9/qtdraw/parser/element.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6330 2023-07-31 11:57:20.000000 qtdraw-1.1.9/qtdraw/parser/read_cif_vesta.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2983 2023-07-31 11:57:20.000000 qtdraw-1.1.9/qtdraw/parser/vesta.py
+-rw-r--r--   0 hiro       (501) staff       (20)    92584 2023-07-31 11:57:20.000000 qtdraw-1.1.9/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.9/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.193206 qtdraw-1.1.9/qtdraw/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.9/qtdraw/scripts/qtdraw.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-08-12 05:51:22.186648 qtdraw-1.1.9/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1082 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       53 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      127 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-08-12 05:51:22.000000 qtdraw-1.1.9/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      753 2023-08-12 05:51:22.193789 qtdraw-1.1.9/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.9/setup.py
```

### Comparing `qtdraw-1.1.8/LICENSE` & `qtdraw-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/PKG-INFO` & `qtdraw-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.8
+Version: 1.1.9
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.9
```

### Comparing `qtdraw-1.1.8/README.md` & `qtdraw-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/basic_object.py` & `qtdraw-1.1.9/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/color_dialog.py` & `qtdraw-1.1.9/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/color_palette.py` & `qtdraw-1.1.9/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/default_panel.ui` & `qtdraw-1.1.9/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/dialog_about.py` & `qtdraw-1.1.9/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.9/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/editable_widget.py` & `qtdraw-1.1.9/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/group_model.py` & `qtdraw-1.1.9/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/group_panel.ui` & `qtdraw-1.1.9/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/group_tab.py` & `qtdraw-1.1.9/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/group_view.py` & `qtdraw-1.1.9/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/line_edit.py` & `qtdraw-1.1.9/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.9/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/qt_logging.py` & `qtdraw-1.1.9/qtdraw/core/qt_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 
 # create a global instance of our class to register the hook
 # qt_exception_hook = UncaughtHook()
 
 
 # ==================================================
 def dprint(s):
-    QMessageBox(None, "dprint", str(s))
+    QMessageBox.information(None, "dprint", str(s))
```

### Comparing `qtdraw-1.1.8/qtdraw/core/qtdraw.png` & `qtdraw-1.1.9/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.9/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/setting.py` & `qtdraw-1.1.9/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/table_dialog.py` & `qtdraw-1.1.9/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/tree_item.py` & `qtdraw-1.1.9/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.9/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/util.py` & `qtdraw-1.1.9/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/core/validator.py` & `qtdraw-1.1.9/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.9/qtdraw/multipie/dialog_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,15 +741,15 @@
             self.tab2_site_proj_c_samb, self.tab2_site_proj_site, self.tab2_site_proj_z_samb = combined_info
 
             site_cluster_samb_select()
 
         def site_cluster_samb_select():
             self.tab2_site_proj_comb_select = self.tab2_site_proj_z_samb["Q"]
             site_proj_irrep1.clear()
-            comb = [self._combined_format(i) for i in self.tab2_site_proj_comb_select]
+            comb = [i[0] for i in self.tab2_site_proj_comb_select]
             site_proj_irrep1.addItems(comb)
             site_proj_irrep1.setCurrentIndex(0)
 
         def plot_site_cluster_samb():
             irrep = site_proj_irrep1.currentIndex()
             try:
                 eq = self.tab2_site_proj_comb_select[irrep][1]
@@ -815,15 +815,15 @@
             self.tab2_bond_proj_c_samb, self.tab2_bond_proj_site, self.tab2_bond_proj_z_samb = combined_info
 
             bond_cluster_samb_select()
 
         def bond_cluster_samb_select():
             self.tab2_bond_proj_comb_select = self.tab2_bond_proj_z_samb["Q"] + self.tab2_bond_proj_z_samb["T"]
             bond_proj_irrep1.clear()
-            comb = [self._combined_format(i) for i in self.tab2_bond_proj_comb_select]
+            comb = [i[0] for i in self.tab2_bond_proj_comb_select]
             bond_proj_irrep1.addItems(comb)
             bond_proj_irrep1.setCurrentIndex(0)
 
         def plot_bond_cluster_samb():
             irrep = bond_proj_irrep1.currentIndex()
             head = bond_proj_irrep1.currentText()[0]
             try:
```

### Comparing `qtdraw-1.1.8/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.9/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/multipie/setting.py` & `qtdraw-1.1.9/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/parser/element.py` & `qtdraw-1.1.9/qtdraw/parser/element.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/parser/read_cif_vesta.py` & `qtdraw-1.1.9/qtdraw/parser/read_cif_vesta.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/parser/vesta.py` & `qtdraw-1.1.9/qtdraw/parser/vesta.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/qt_draw.py` & `qtdraw-1.1.9/qtdraw/qt_draw.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw/qt_draw_base.py` & `qtdraw-1.1.9/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.9/qtdraw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.8
+Version: 1.1.9
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.9
```

### Comparing `qtdraw-1.1.8/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.9/qtdraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.8/setup.cfg` & `qtdraw-1.1.9/setup.cfg`

 * *Files identical despite different names*

