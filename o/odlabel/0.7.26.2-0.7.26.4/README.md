# Comparing `tmp/odlabel-0.7.26.2.tar.gz` & `tmp/odlabel-0.7.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.2.tar", last modified: Fri May 10 15:39:38 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.4.tar", last modified: Mon May 13 17:35:45 2024, max compression
```

## Comparing `odlabel-0.7.26.2.tar` & `odlabel-0.7.26.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.2/LICENSE
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7054 2024-05-08 19:12:44.000000 odlabel-0.7.26.2/README.md
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-0.7.26.2/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.2/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-09 20:46:40.000000 odlabel-0.7.26.2/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.2/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-09 20:44:28.000000 odlabel-0.7.26.2/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-10 15:31:20.000000 odlabel-0.7.26.2/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.119205 odlabel-0.7.26.2/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.2/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10458 2024-05-02 20:55:30.000000 odlabel-0.7.26.2/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.2/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 15:39:29.000000 odlabel-0.7.26.2/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.2/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7818 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-10 15:39:38.000000 odlabel-0.7.26.2/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-10 15:39:38.123205 odlabel-0.7.26.2/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-10 15:19:59.000000 odlabel-0.7.26.2/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.4/LICENSE
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7825 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7061 2024-05-13 17:34:36.000000 odlabel-0.7.26.4/README.md
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-0.7.26.4/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.4/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-13 17:05:33.000000 odlabel-0.7.26.4/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.4/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.4/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-10 15:31:20.000000 odlabel-0.7.26.4/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.4/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:05:28.000000 odlabel-0.7.26.4/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.4/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.4/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.4/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7825 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-13 17:35:45.359650 odlabel-0.7.26.4/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-13 17:35:34.000000 odlabel-0.7.26.4/setup.py
```

### Comparing `odlabel-0.7.26.2/LICENSE` & `odlabel-0.7.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/PKG-INFO` & `odlabel-0.7.26.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.2
+Version: 0.7.26.4
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/9fb27b28-eab1-4edb-9c1d-0535c4e0e99a)
+![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
 ## Features
 
@@ -97,15 +97,15 @@
 
 4. **Color Space Distribution:** A 3D scatter plot that visualizes the color space distribution of the input images. Each point in the plot represents a unique color space, with its position determined by the mean values of the red, green, and blue channels. The size of the points indicates the frequency of that particular color space in the dataset.
 
 5. **Detected Object Count:** A bar chart displaying the count of detected objects for each class. The first bar represents the total number of input images, while the subsequent bars show the number of instances for each object class detected across the dataset.
 
 6. **Detection Confidence Histogram:** A histogram that illustrates the distribution of detection confidence scores. The x-axis represents the confidence level, and the bars show the frequency of detections within each confidence bin.
 
-7. **Labelism: Bounding Boxes:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
+7. **Spatial Distribution of Objects:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
 
 8. **Heatmap of Detection:** A heatmap visualization that showcases the spatial distribution of detected objects within the image space. The heatmap uses different colors to indicate the density of detections at various locations, with brighter colors representing higher concentrations.
 
 These figures provide valuable insights into the input image data and the object detection results, enabling users to identify potential issues, patterns, and areas for further analysis or improvement. The dashboard serves as a powerful tool for exploring and understanding the data, facilitating informed decision-making and enhancing the overall object detection and labeling workflow.
 
 ## Update
```

### Comparing `odlabel-0.7.26.2/README.md` & `odlabel-0.7.26.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/9fb27b28-eab1-4edb-9c1d-0535c4e0e99a)
+![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
 ## Features
 
@@ -76,15 +76,15 @@
 
 4. **Color Space Distribution:** A 3D scatter plot that visualizes the color space distribution of the input images. Each point in the plot represents a unique color space, with its position determined by the mean values of the red, green, and blue channels. The size of the points indicates the frequency of that particular color space in the dataset.
 
 5. **Detected Object Count:** A bar chart displaying the count of detected objects for each class. The first bar represents the total number of input images, while the subsequent bars show the number of instances for each object class detected across the dataset.
 
 6. **Detection Confidence Histogram:** A histogram that illustrates the distribution of detection confidence scores. The x-axis represents the confidence level, and the bars show the frequency of detections within each confidence bin.
 
-7. **Labelism: Bounding Boxes:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
+7. **Spatial Distribution of Objects:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
 
 8. **Heatmap of Detection:** A heatmap visualization that showcases the spatial distribution of detected objects within the image space. The heatmap uses different colors to indicate the density of detections at various locations, with brighter colors representing higher concentrations.
 
 These figures provide valuable insights into the input image data and the object detection results, enabling users to identify potential issues, patterns, and areas for further analysis or improvement. The dashboard serves as a powerful tool for exploring and understanding the data, facilitating informed decision-making and enhancing the overall object detection and labeling workflow.
 
 ## Update
```

### Comparing `odlabel-0.7.26.2/app/main_window.py` & `odlabel-0.7.26.4/app/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/app/workers/chart_worker.py` & `odlabel-0.7.26.4/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/app/workers/detection_worker.py` & `odlabel-0.7.26.4/app/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.4/app/workers/utils/chart_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,37 +231,37 @@
     ax_conf = fig_conf.add_subplot(1, 1, 1)
     ax_conf.hist(confidences, bins=20, range=(0, 1))
     ax_conf.set_xlim(0, 1)
     ax_conf.set_xlabel("Confidence")
     ax_conf.set_ylabel("Frequency")
     ax_conf.set_title("Detection Confidence Histogram", y=1.05)
 
-    # Labelism: Bounding Box Chart
-    fig_labelism = Figure(figsize=(4, 3), dpi=100)
-    ax_labelism = fig_labelism.add_subplot(1, 1, 1)
+    # Spatial Distribution of Objects
+    fig_labels = Figure(figsize=(4, 3), dpi=100)
+    ax_labels = fig_labels.add_subplot(1, 1, 1)
 
     max_count = max(labelism_counts.values())
     cmap = plt.get_cmap("Reds")
 
     for (x, y, w, h), count in labelism_counts.items():
         rect = Rectangle(
             (x, y),
             w,
             h,
             linewidth=0.7,
             edgecolor=cmap(count / max_count),
             facecolor="none",
         )
-        ax_labelism.add_patch(rect)
+        ax_labels.add_patch(rect)
 
-    ax_labelism.set_xlim(0, 1)
-    ax_labelism.set_ylim(0, 1)
-    ax_labelism.set_title("Labelism: Bounding Boxes", y=1.05)
-    ax_labelism.set_xlabel("X")
-    ax_labelism.set_ylabel("Y")
+    ax_labels.set_xlim(0, 1)
+    ax_labels.set_ylim(0, 1)
+    ax_labels.set_title("Spatial Distribution of Objects", y=1.05)
+    ax_labels.set_xlabel("X")
+    ax_labels.set_ylabel("Y")
 
     # Heatmap of Detection
     fig_heatmap = Figure(figsize=(4, 3), dpi=100)
     ax_heatmap = fig_heatmap.add_subplot(1, 1, 1)
 
     max_count = max(heatmap_coords.values())
     cmap = plt.get_cmap("Blues")
@@ -274,15 +274,15 @@
 
     ax_heatmap.set_xlim(0, 1)
     ax_heatmap.set_ylim(0, 1)
     ax_heatmap.set_title("Heatmap of Detection")
     ax_heatmap.set_xlabel("X")
     ax_heatmap.set_ylabel("Y")
 
-    return fig_count, fig_conf, fig_labelism, fig_heatmap
+    return fig_count, fig_conf, fig_labels, fig_heatmap
 
 
 def display_chart(fig, frame, row, col):
     if isinstance(fig, tuple):
         fig, _ = fig
     else:
         _ = fig.get_axes()[0]
```

### Comparing `odlabel-0.7.26.2/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.4/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/app/workers/utils/draw_utils.py` & `odlabel-0.7.26.4/app/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/app/workers/utils/write_utils.py` & `odlabel-0.7.26.4/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/odlabel.egg-info/PKG-INFO` & `odlabel-0.7.26.4/odlabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.2
+Version: 0.7.26.4
 Summary: A tool for object detection, labeling and visualization
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/9fb27b28-eab1-4edb-9c1d-0535c4e0e99a)
+![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
 ## Features
 
@@ -97,15 +97,15 @@
 
 4. **Color Space Distribution:** A 3D scatter plot that visualizes the color space distribution of the input images. Each point in the plot represents a unique color space, with its position determined by the mean values of the red, green, and blue channels. The size of the points indicates the frequency of that particular color space in the dataset.
 
 5. **Detected Object Count:** A bar chart displaying the count of detected objects for each class. The first bar represents the total number of input images, while the subsequent bars show the number of instances for each object class detected across the dataset.
 
 6. **Detection Confidence Histogram:** A histogram that illustrates the distribution of detection confidence scores. The x-axis represents the confidence level, and the bars show the frequency of detections within each confidence bin.
 
-7. **Labelism: Bounding Boxes:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
+7. **Spatial Distribution of Objects:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
 
 8. **Heatmap of Detection:** A heatmap visualization that showcases the spatial distribution of detected objects within the image space. The heatmap uses different colors to indicate the density of detections at various locations, with brighter colors representing higher concentrations.
 
 These figures provide valuable insights into the input image data and the object detection results, enabling users to identify potential issues, patterns, and areas for further analysis or improvement. The dashboard serves as a powerful tool for exploring and understanding the data, facilitating informed decision-making and enhancing the overall object detection and labeling workflow.
 
 ## Update
```

### Comparing `odlabel-0.7.26.2/odlabel.egg-info/SOURCES.txt` & `odlabel-0.7.26.4/odlabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.2/setup.py` & `odlabel-0.7.26.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26.2",
+    version="0.7.26.4",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
```

