# Comparing `tmp/axoden-1.0.0.tar.gz` & `tmp/axoden-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axoden-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "axoden-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axoden-1.0.0.tar` & `axoden-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1691 2024-05-13 18:18:50.691683 axoden-1.0.0/.github/workflows/build_executables.yml
--rw-r--r--   0        0        0      768 2024-05-13 18:18:50.691683 axoden-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      338 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      436 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1195 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      494 2024-05-13 18:18:50.695683 axoden-1.0.0/.gitignore
--rw-r--r--   0        0        0      154 2024-05-13 18:18:50.695683 axoden-1.0.0/.streamlit/config.toml
--rw-r--r--   0        0        0    32422 2024-05-13 18:18:50.695683 axoden-1.0.0/LICENSE
--rw-r--r--   0        0        0    10581 2024-05-13 18:18:50.695683 axoden-1.0.0/README.md
--rw-r--r--   0        0        0      599 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/__init__.py
--rw-r--r--   0        0        0      325 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/__init__.py
--rw-r--r--   0        0        0     9998 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/gui_projections_quantification.py
--rw-r--r--   0        0        0     5314 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/1_📊️_Axoden.py
--rw-r--r--   0        0        0        0 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/__init__.py
--rw-r--r--   0        0        0      526 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/__main__.py
--rw-r--r--   0        0        0     7857 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/app_utils.py
--rw-r--r--   0        0        0     8263 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
--rw-r--r--   0        0        0      570 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
--rw-r--r--   0        0        0     2433 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pdf_utils.py
--rw-r--r--   0        0        0    29140 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/volume_projections.py
--rw-r--r--   0        0        0    85110 2024-05-13 18:18:50.695683 axoden-1.0.0/media/control_plots.jpg
--rw-r--r--   0        0        0    29869 2024-05-13 18:18:50.695683 axoden-1.0.0/media/summary_data.pdf
--rw-r--r--   0        0        0   327888 2024-05-13 18:18:50.699683 axoden-1.0.0/media/summary_data_axis.pdf
--rw-r--r--   0        0        0     1396 2024-05-13 18:18:50.699683 axoden-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-13 18:18:50.823683 axoden-1.0.0/tox.ini
--rw-r--r--   0        0        0    11404 1970-01-01 00:00:00.000000 axoden-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1691 2024-05-13 19:14:56.944570 axoden-1.0.1/.github/workflows/build_executables.yml
+-rw-r--r--   0        0        0      768 2024-05-13 19:14:56.944570 axoden-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      338 2024-05-13 19:14:56.944570 axoden-1.0.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      436 2024-05-13 19:14:56.944570 axoden-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1195 2024-05-13 19:14:56.944570 axoden-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      494 2024-05-13 19:14:56.944570 axoden-1.0.1/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-13 19:14:56.944570 axoden-1.0.1/.streamlit/config.toml
+-rw-r--r--   0        0        0    32422 2024-05-13 19:14:56.944570 axoden-1.0.1/LICENSE
+-rw-r--r--   0        0        0    10581 2024-05-13 19:14:56.944570 axoden-1.0.1/README.md
+-rw-r--r--   0        0        0      599 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/__init__.py
+-rw-r--r--   0        0        0     9998 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/gui_projections_quantification.py
+-rw-r--r--   0        0        0     5314 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/1_📊️_Axoden.py
+-rw-r--r--   0        0        0        0 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/__init__.py
+-rw-r--r--   0        0        0      526 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/__main__.py
+-rw-r--r--   0        0        0     7857 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/app_utils.py
+-rw-r--r--   0        0        0     8408 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
+-rw-r--r--   0        0        0      570 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
+-rw-r--r--   0        0        0     2433 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/gui/streamlit_app/pdf_utils.py
+-rw-r--r--   0        0        0    29140 2024-05-13 19:14:56.944570 axoden-1.0.1/axoden/volume_projections.py
+-rw-r--r--   0        0        0    85110 2024-05-13 19:14:56.944570 axoden-1.0.1/media/control_plots.jpg
+-rw-r--r--   0        0        0    29852 2024-05-13 19:14:56.944570 axoden-1.0.1/media/summary_data.pdf
+-rw-r--r--   0        0        0   327888 2024-05-13 19:14:56.948570 axoden-1.0.1/media/summary_data_axis.pdf
+-rw-r--r--   0        0        0     1396 2024-05-13 19:14:56.948570 axoden-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-13 19:14:57.072570 axoden-1.0.1/tox.ini
+-rw-r--r--   0        0        0    11404 1970-01-01 00:00:00.000000 axoden-1.0.1/PKG-INFO
```

### Comparing `axoden-1.0.0/.github/workflows/build_executables.yml` & `axoden-1.0.1/.github/workflows/build_executables.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/.github/workflows/docs.yml` & `axoden-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/.github/workflows/test.yml` & `axoden-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/LICENSE` & `axoden-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/README.md` & `axoden-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/__init__.py` & `axoden-1.0.1/axoden/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 axoden simplifies the quantification of axonal projections in neuroscience.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from .volume_projections import (  # noqa: F401
     load_table,
     plot_signal_intensity_along_axis,
     plot_summary_data,
     process_folder,
     process_image,
```

### Comparing `axoden-1.0.0/axoden/gui/gui_projections_quantification.py` & `axoden-1.0.1/axoden/gui/gui_projections_quantification.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/1_📊️_Axoden.py` & `axoden-1.0.1/axoden/gui/streamlit_app/1_📊️_Axoden.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/__main__.py` & `axoden-1.0.1/axoden/gui/streamlit_app/__main__.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/app_utils.py` & `axoden-1.0.1/axoden/gui/streamlit_app/app_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py` & `axoden-1.0.1/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,26 @@
         - On the top menu select Image > Adjust > Brightness/Contrast
         - Decrease the “Maximum” value using the sliding bar to increase fluorescence intensity.
         - Increase the “Minimum” value using the sliding bar to decrease background fluorescence.
     7. Save the resulting image following AxoDen naming convention.
 
 > :point_up: :blue[_TIP:_]  
 > _Use the histogram (Analyze > Histogram) to confirm that the background fluorescence in the brain region does not contain zero values._
-
-:warning: TODO: add image of final result in ImageJ/FIJI
 """
     )
 
     st.markdown("""## Part 2: AxoDen analysis""")
 
+    st.markdown(
+        """
+If you want to test AxoDen quickly, you can download the test images from
+[the github repository](https://github.com/raqueladaia/AxoDen/tree/main/test_images)
+"""
+    )
+
     st.markdown("""#### Steps""")
 
     st.markdown(
         """
 1. Give a name to your project.
 2. Change the pixel size to your specification.
 The pixel size will depend on your objective and machine you used to acquire the images.
@@ -102,24 +107,24 @@
 One control plot is created for each image uploaded.
 
 Inspect the control plots to make sure the masking of the image is accurate.
 - The mask appears on the second row of the first column.
 - The mask is shown in white.
 - The mask should cover any part of the image that contains tissue.
 - If the mask present black spots within, that is because the background fluorescence of the tissue is 0.
-- To correct the mask, repeat Part 1, steps 3.5 to h to create a new masked image.
+- To correct the mask, repeat Part 1, steps 3.2 to 3.7 to create a new masked image.
 - If you cannot correct the mask, it means that during acquistion the background fluorescence was too low. **Consider retaking the image.**
 
 Inspect the control plots to make sure the signal does not bleed to surrounding areas.
 - In this case, you want to examine the binarized image.
 - The binarized image appears on the first row of the second column.
 - The signal is shown in white.
 - If the signal extends beyond the axon limits (=bleeding to surrounding areas),
 it means the signal intensity is too high.
-- To correct, repeat Part 1, steps 3.5 to h to create a new masked image.
+- To correct, repeat Part 1, steps 3.2 to 3.7 to create a new masked image.
 - If you cannot correct the bleeding, your image is likely overexposed. **Consider retaking the image.**
 
 You can also download the control plots to check them in detail and keep them as reference for later use.
 Simply click the “Download figure as pdf” button.
 """
     )
```

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py` & `axoden-1.0.1/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/gui/streamlit_app/pdf_utils.py` & `axoden-1.0.1/axoden/gui/streamlit_app/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/axoden/volume_projections.py` & `axoden-1.0.1/axoden/volume_projections.py`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/media/control_plots.jpg` & `axoden-1.0.1/media/control_plots.jpg`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/media/summary_data.pdf` & `axoden-1.0.1/media/summary_data.pdf`

 * *Files 12% similar despite different names*

#### Comparing `axoden-1.0.0/media/summary_data.pdf` & `axoden-1.0.1/media/summary_data.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240513172619+02'00'"
+CreationDate: "D:20240513210309+02'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 Project "AxoDen Analysis"
 Data Summary
 
 30
 
-204
+0.204
 
 30
 
 L
 -C
 TH
 
@@ -67,28 +67,28 @@
 -V
 P
 
 0
 
 L
 
-0
+0.000
 
 M
 
 0
 
 -M
 D
 
 10
 
 L
 
-68
+0.068
 
 -V
 L
 
 10
 
 TH
@@ -96,25 +96,25 @@
 Animals per Brain Region
 
 20
 
 -V
 L
 
-136
+0.136
 
 TH
 
 Pixel value
 
 40
 
 Area (mm²)
 
-272
+0.272
 
 20
 
 Threshold for binarization
 
 50
 
@@ -124,15 +124,15 @@
 -V
 P
 
 Innervation (%)
 
 Area of the brain region
 
-340
+0.340
 
 TH
 -V
 P
 
 Percentage of innervation
```

### Comparing `axoden-1.0.0/media/summary_data_axis.pdf` & `axoden-1.0.1/media/summary_data_axis.pdf`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/pyproject.toml` & `axoden-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `axoden-1.0.0/PKG-INFO` & `axoden-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axoden
-Version: 1.0.0
+Version: 1.0.1
 Summary: axoden simplifies the quantification of axonal projections in neuroscience.
 Author-email: Raquel Adaia Sandoval Ortega <raqueladaia@gmail.com>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: tqdm >= 4.0.0
 Requires-Dist: numpy >= 1.16.0
```

