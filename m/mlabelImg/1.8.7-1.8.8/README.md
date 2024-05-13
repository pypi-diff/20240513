# Comparing `tmp/mlabelimg-1.8.7.tar.gz` & `tmp/mlabelimg-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlabelimg-1.8.7.tar", last modified: Fri May 10 04:38:46 2024, max compression
+gzip compressed data, was "mlabelimg-1.8.8.tar", last modified: Mon May 13 08:39:49 2024, max compression
```

## Comparing `mlabelimg-1.8.7.tar` & `mlabelimg-1.8.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 04:38:46.803063 mlabelimg-1.8.7/
--rw-rw-rw-   0        0        0       83 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1659 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/HISTORY.rst
--rw-rw-rw-   0        0        0     1197 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/LICENSE
--rw-rw-rw-   0        0        0      300 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3233 2024-05-10 04:38:46.803063 mlabelimg-1.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     2133 2024-05-10 04:26:51.000000 mlabelimg-1.8.7/README.md
--rw-rw-rw-   0        0        0        0 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:38:46.756669 mlabelimg-1.8.7/data/
--rw-rw-rw-   0        0        0      145 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/data/predefined_classes.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 04:38:46.783594 mlabelimg-1.8.7/libs/
--rw-rw-rw-   0        0        0       76 2024-05-10 04:38:06.000000 mlabelimg-1.8.7/libs/__init__.py
--rw-rw-rw-   0        0        0    27971 2024-05-10 04:09:45.000000 mlabelimg-1.8.7/libs/canvas.py
--rw-rw-rw-   0        0        0     1295 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/colorDialog.py
--rw-rw-rw-   0        0        0      967 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/combobox.py
--rw-rw-rw-   0        0        0      668 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/constants.py
--rw-rw-rw-   0        0        0     3852 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/create_ml_io.py
--rw-rw-rw-   0        0        0      784 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/hashableQListWidgetItem.py
--rw-rw-rw-   0        0        0     3153 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/labelDialog.py
--rw-rw-rw-   0        0        0     6341 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/labelFile.py
--rw-rw-rw-   0        0        0     6324 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/pascal_voc_io.py
--rw-rw-rw-   0        0        0   640841 2024-05-10 04:05:55.000000 mlabelimg-1.8.7/libs/resources.py
--rw-rw-rw-   0        0        0     1238 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/settings.py
--rw-rw-rw-   0        0        0     6604 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/shape.py
--rw-rw-rw-   0        0        0     2506 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/stringBundle.py
--rw-rw-rw-   0        0        0     1192 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/toolBar.py
--rw-rw-rw-   0        0        0      534 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/ustr.py
--rw-rw-rw-   0        0        0     2897 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/utils.py
--rw-rw-rw-   0        0        0     4998 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/yolo_io.py
--rw-rw-rw-   0        0        0      780 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/libs/zoomWidget.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:38:46.803063 mlabelimg-1.8.7/mlabelImg.egg-info/
--rw-rw-rw-   0        0        0     3233 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 04:17:09.000000 mlabelimg-1.8.7/mlabelImg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-10 04:38:46.000000 mlabelimg-1.8.7/mlabelImg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    67987 2024-05-10 03:46:00.000000 mlabelimg-1.8.7/mlabelImg.py
--rw-rw-rw-   0        0        0     2078 2021-10-11 20:15:19.000000 mlabelimg-1.8.7/resources.qrc
--rw-rw-rw-   0        0        0      149 2024-05-10 04:38:46.810076 mlabelimg-1.8.7/setup.cfg
--rw-rw-rw-   0        0        0     3668 2024-05-10 04:35:47.000000 mlabelimg-1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.693939 mlabelimg-1.8.8/
+-rw-rw-rw-   0        0        0       83 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1659 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1197 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/LICENSE
+-rw-rw-rw-   0        0        0      300 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3233 2024-05-13 08:39:49.693939 mlabelimg-1.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2133 2024-05-10 04:26:51.000000 mlabelimg-1.8.8/README.md
+-rw-rw-rw-   0        0        0        0 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.651054 mlabelimg-1.8.8/data/
+-rw-rw-rw-   0        0        0      145 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/data/predefined_classes.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.672995 mlabelimg-1.8.8/libs/
+-rw-rw-rw-   0        0        0       76 2024-05-13 08:37:20.000000 mlabelimg-1.8.8/libs/__init__.py
+-rw-rw-rw-   0        0        0    27971 2024-05-10 04:09:45.000000 mlabelimg-1.8.8/libs/canvas.py
+-rw-rw-rw-   0        0        0     1295 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/colorDialog.py
+-rw-rw-rw-   0        0        0     1151 2024-05-13 08:35:32.000000 mlabelimg-1.8.8/libs/combobox.py
+-rw-rw-rw-   0        0        0      668 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/constants.py
+-rw-rw-rw-   0        0        0     3852 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/create_ml_io.py
+-rw-rw-rw-   0        0        0      784 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/hashableQListWidgetItem.py
+-rw-rw-rw-   0        0        0     3153 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/labelDialog.py
+-rw-rw-rw-   0        0        0     6341 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/labelFile.py
+-rw-rw-rw-   0        0        0     6324 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/pascal_voc_io.py
+-rw-rw-rw-   0        0        0   641015 2024-05-13 07:19:21.000000 mlabelimg-1.8.8/libs/resources.py
+-rw-rw-rw-   0        0        0     1238 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/settings.py
+-rw-rw-rw-   0        0        0     6604 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/shape.py
+-rw-rw-rw-   0        0        0     2506 2024-05-13 04:49:14.000000 mlabelimg-1.8.8/libs/stringBundle.py
+-rw-rw-rw-   0        0        0     1192 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/toolBar.py
+-rw-rw-rw-   0        0        0      534 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/ustr.py
+-rw-rw-rw-   0        0        0     2897 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/utils.py
+-rw-rw-rw-   0        0        0     4998 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/yolo_io.py
+-rw-rw-rw-   0        0        0      780 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/zoomWidget.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.692942 mlabelimg-1.8.8/mlabelImg.egg-info/
+-rw-rw-rw-   0        0        0     3233 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 04:17:09.000000 mlabelimg-1.8.8/mlabelImg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    68154 2024-05-13 08:36:14.000000 mlabelimg-1.8.8/mlabelImg.py
+-rw-rw-rw-   0        0        0     2078 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/resources.qrc
+-rw-rw-rw-   0        0        0      149 2024-05-13 08:39:49.695934 mlabelimg-1.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     3668 2024-05-10 04:35:47.000000 mlabelimg-1.8.8/setup.py
```

### Comparing `mlabelimg-1.8.7/HISTORY.rst` & `mlabelimg-1.8.8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/LICENSE` & `mlabelimg-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/PKG-INFO` & `mlabelimg-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlabelImg
-Version: 1.8.7
+Version: 1.8.8
 Summary: LabelImg is a graphical image annotation tool and label object bounding boxes in images (Modified Version)
 Home-page: https://github.com/PD-Mera/mlabelImg
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 License: MIT license
 Keywords: labelImg labelTool development annotation deeplearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlabelimg-1.8.7/README.md` & `mlabelimg-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/canvas.py` & `mlabelimg-1.8.8/libs/canvas.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/colorDialog.py` & `mlabelimg-1.8.8/libs/colorDialog.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/combobox.py` & `mlabelimg-1.8.8/libs/combobox.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,9 +25,13 @@
 
         layout.addWidget(self.cb)
         self.setLayout(layout)
 
     def update_items(self, items):
         self.items = items
 
+        current_text = "[SHOW ALL]" if self.cb.currentText() == "" else self.cb.currentText()
+        new_index = items.index(current_text)
         self.cb.clear()
         self.cb.addItems(self.items)
+        self.cb.setCurrentIndex(new_index)
+
```

### Comparing `mlabelimg-1.8.7/libs/constants.py` & `mlabelimg-1.8.8/libs/constants.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/create_ml_io.py` & `mlabelimg-1.8.8/libs/create_ml_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/hashableQListWidgetItem.py` & `mlabelimg-1.8.8/libs/hashableQListWidgetItem.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/labelDialog.py` & `mlabelimg-1.8.8/libs/labelDialog.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/labelFile.py` & `mlabelimg-1.8.8/libs/labelFile.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/pascal_voc_io.py` & `mlabelimg-1.8.8/libs/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/resources.py` & `mlabelimg-1.8.8/libs/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -8857,15 +8857,15 @@
 \x6c\xce\x95\xeb\x6b\xfc\xab\x51\xe5\x22\x4a\x73\xae\xcd\x1b\xbf\
 \x78\x8d\xec\xe4\xfb\x2f\x43\xfa\xfa\x15\x00\xf0\x2f\x85\x8b\xb3\
 \x0f\x4d\xfd\xfc\x85\x6f\x4f\xd5\xc7\x77\x23\xe8\xeb\x9a\x98\x6a\
 \x57\x6d\x0a\x5c\xcd\x12\xc5\x82\xa2\xe0\xd4\xd1\xe9\x34\xe8\x7e\
 \xfc\x07\x48\x9e\x04\x74\xcd\x00\x54\x9f\x00\xf8\xcd\xbc\xfd\xff\
 \xbf\x55\xfe\xcb\xed\xdf\x99\xd5\xe1\x33\x6b\x2f\x52\xdc\x00\x00\
 \x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x09\x81\
+\x00\x00\x09\xab\
 \x6f\
 \x70\x65\x6e\x46\x69\x6c\x65\x3d\x4f\x70\x65\x6e\x0a\x6f\x70\x65\
 \x6e\x46\x69\x6c\x65\x44\x65\x74\x61\x69\x6c\x3d\x4f\x70\x65\x6e\
 \x20\x69\x6d\x61\x67\x65\x20\x6f\x72\x20\x6c\x61\x62\x65\x6c\x20\
 \x66\x69\x6c\x65\x0a\x71\x75\x69\x74\x3d\x51\x75\x69\x74\x0a\x71\
 \x75\x69\x74\x41\x70\x70\x3d\x51\x75\x69\x74\x20\x61\x70\x70\x6c\
 \x69\x63\x61\x74\x69\x6f\x6e\x0a\x6f\x70\x65\x6e\x44\x69\x72\x3d\
@@ -9011,15 +9011,17 @@
 \x52\x65\x63\x65\x6e\x74\x3d\x4f\x70\x65\x6e\x20\x26\x52\x65\x63\
 \x65\x6e\x74\x0a\x63\x68\x6f\x6f\x73\x65\x4c\x69\x6e\x65\x43\x6f\
 \x6c\x6f\x72\x3d\x43\x68\x6f\x6f\x73\x65\x20\x4c\x69\x6e\x65\x20\
 \x43\x6f\x6c\x6f\x72\x0a\x63\x68\x6f\x6f\x73\x65\x46\x69\x6c\x6c\
 \x43\x6f\x6c\x6f\x72\x3d\x43\x68\x6f\x6f\x73\x65\x20\x46\x69\x6c\
 \x6c\x20\x43\x6f\x6c\x6f\x72\x0a\x64\x72\x61\x77\x53\x71\x75\x61\
 \x72\x65\x73\x3d\x44\x72\x61\x77\x20\x53\x71\x75\x61\x72\x65\x73\
-\
+\x0a\x6c\x61\x62\x65\x6c\x54\x65\x78\x74\x42\x6f\x78\x3d\x59\x4f\
+\x4c\x4f\x20\x4c\x61\x62\x65\x6c\x73\x0a\x6c\x61\x62\x65\x6c\x54\
+\x65\x78\x74\x3d\x4c\x61\x62\x65\x6c\x73\
 \x00\x00\x10\x3c\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x3c\x00\x00\x00\x3c\x08\x04\x00\x00\x00\x90\xf5\x11\xf9\
 \x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0b\x13\x00\x00\x0b\x13\
 \x01\x00\x9a\x9c\x18\x00\x00\x06\xc1\x69\x54\x58\x74\x58\x4d\x4c\
 \x3a\x63\x6f\x6d\x2e\x61\x64\x6f\x62\x65\x2e\x78\x6d\x70\x00\x00\
@@ -9684,16 +9686,16 @@
 \x00\x00\x01\xd8\x00\x00\x00\x00\x00\x01\x00\x01\xfb\x37\
 \x00\x00\x01\xea\x00\x00\x00\x00\x00\x01\x00\x01\xfc\x8a\
 \x00\x00\x01\xfc\x00\x00\x00\x00\x00\x01\x00\x02\x05\xdb\
 \x00\x00\x02\x14\x00\x00\x00\x00\x00\x01\x00\x02\x0b\x34\
 \x00\x00\x02\x26\x00\x00\x00\x00\x00\x01\x00\x02\x17\x19\
 \x00\x00\x02\x42\x00\x00\x00\x00\x00\x01\x00\x02\x19\xc0\
 \x00\x00\x02\x56\x00\x00\x00\x00\x00\x01\x00\x02\x24\xbf\
-\x00\x00\x02\x6a\x00\x00\x00\x00\x00\x01\x00\x02\x2e\x44\
-\x00\x00\x02\x8e\x00\x00\x00\x00\x00\x01\x00\x02\x3e\x84\
+\x00\x00\x02\x6a\x00\x00\x00\x00\x00\x01\x00\x02\x2e\x6e\
+\x00\x00\x02\x8e\x00\x00\x00\x00\x00\x01\x00\x02\x3e\xae\
 "
 
 qt_resource_struct_v2 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x23\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
@@ -9756,18 +9758,18 @@
 \x00\x00\x02\x14\x00\x00\x00\x00\x00\x01\x00\x02\x0b\x34\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
 \x00\x00\x02\x26\x00\x00\x00\x00\x00\x01\x00\x02\x17\x19\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
 \x00\x00\x02\x42\x00\x00\x00\x00\x00\x01\x00\x02\x19\xc0\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
 \x00\x00\x02\x56\x00\x00\x00\x00\x00\x01\x00\x02\x24\xbf\
+\x00\x00\x01\x8f\x70\x47\xf3\x0e\
+\x00\x00\x02\x6a\x00\x00\x00\x00\x00\x01\x00\x02\x2e\x6e\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
-\x00\x00\x02\x6a\x00\x00\x00\x00\x00\x01\x00\x02\x2e\x44\
-\x00\x00\x01\x7c\x70\xfe\xcb\xd8\
-\x00\x00\x02\x8e\x00\x00\x00\x00\x00\x01\x00\x02\x3e\x84\
+\x00\x00\x02\x8e\x00\x00\x00\x00\x00\x01\x00\x02\x3e\xae\
 \x00\x00\x01\x7c\x70\xfe\xcb\xd8\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
```

### Comparing `mlabelimg-1.8.7/libs/settings.py` & `mlabelimg-1.8.8/libs/settings.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/shape.py` & `mlabelimg-1.8.8/libs/shape.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/stringBundle.py` & `mlabelimg-1.8.8/libs/stringBundle.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/toolBar.py` & `mlabelimg-1.8.8/libs/toolBar.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/ustr.py` & `mlabelimg-1.8.8/libs/ustr.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/utils.py` & `mlabelimg-1.8.8/libs/utils.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/yolo_io.py` & `mlabelimg-1.8.8/libs/yolo_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/libs/zoomWidget.py` & `mlabelimg-1.8.8/libs/zoomWidget.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/mlabelImg.egg-info/PKG-INFO` & `mlabelimg-1.8.8/mlabelImg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlabelImg
-Version: 1.8.7
+Version: 1.8.8
 Summary: LabelImg is a graphical image annotation tool and label object bounding boxes in images (Modified Version)
 Home-page: https://github.com/PD-Mera/mlabelImg
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 License: MIT license
 Keywords: labelImg labelTool development annotation deeplearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlabelimg-1.8.7/mlabelImg.egg-info/SOURCES.txt` & `mlabelimg-1.8.8/mlabelImg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/mlabelImg.py` & `mlabelimg-1.8.8/mlabelImg.py`

 * *Files 0% similar despite different names*

```diff
@@ -837,17 +837,17 @@
 
     def update_combo_box(self):
         # Get the unique labels and add them to the Combobox.
         items_text_list = [str(self.label_list.item(i).text()) for i in range(self.label_list.count())]
 
         unique_text_list = list(set(items_text_list))
         # Add a null row for showing all the labels
-        unique_text_list.append("")
         unique_text_list.sort()
-
+        unique_text_list.insert(0, "[SHOW ALL]")
+        unique_text_list.insert(1, "[HIDE ALL]")
         self.combo_box.update_items(unique_text_list)
 
     def save_labels(self, annotation_file_path):
         annotation_file_path = ustr(annotation_file_path)
         if self.label_file is None:
             self.label_file = LabelFile()
             self.label_file.verified = self.canvas.verified
@@ -891,16 +891,18 @@
         self.add_label(self.canvas.copy_selected_shape())
         # fix copy and delete
         self.shape_selection_changed(True)
 
     def combo_selection_changed(self, index):
         text = self.combo_box.cb.itemText(index)
         for i in range(self.label_list.count()):
-            if text == "":
+            if text == "[SHOW ALL]":
                 self.label_list.item(i).setCheckState(2)
+            elif text == "[HIDE ALL]":
+                self.label_list.item(i).setCheckState(0)
             elif text != self.label_list.item(i).text():
                 self.label_list.item(i).setCheckState(0)
             else:
                 self.label_list.item(i).setCheckState(2)
 
     def label_selection_changed(self):
         item = self.current_item()
```

### Comparing `mlabelimg-1.8.7/resources.qrc` & `mlabelimg-1.8.8/resources.qrc`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.7/setup.py` & `mlabelimg-1.8.8/setup.py`

 * *Files identical despite different names*

