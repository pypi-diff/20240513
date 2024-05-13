# Comparing `tmp/axoden-0.3.0.tar.gz` & `tmp/axoden-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axoden-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "axoden-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axoden-0.3.0.tar` & `axoden-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,26 @@
--rw-r--r--   0        0        0     1691 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/build_executables.yml
--rw-r--r--   0        0        0      768 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      338 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      436 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1195 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      494 2024-05-13 16:04:11.242441 axoden-0.3.0/.gitignore
--rw-r--r--   0        0        0      154 2024-05-13 16:04:11.242441 axoden-0.3.0/.streamlit/config.toml
--rw-r--r--   0        0        0    32422 2024-05-13 16:04:11.242441 axoden-0.3.0/LICENSE
--rw-r--r--   0        0        0    12172 2024-05-13 16:04:11.242441 axoden-0.3.0/README.md
--rw-r--r--   0        0        0      599 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/__init__.py
--rw-r--r--   0        0        0      325 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/__init__.py
--rw-r--r--   0        0        0     9998 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/gui_projections_quantification.py
--rw-r--r--   0        0        0     5314 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/1_📊️_Axoden.py
--rw-r--r--   0        0        0        0 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/__init__.py
--rw-r--r--   0        0        0      526 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/__main__.py
--rw-r--r--   0        0        0     7857 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/app_utils.py
--rw-r--r--   0        0        0     8263 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
--rw-r--r--   0        0        0      570 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
--rw-r--r--   0        0        0     2433 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pdf_utils.py
--rw-r--r--   0        0        0    29018 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/volume_projections.py
--rw-r--r--   0        0        0      638 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      804 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/make.bat
--rw-r--r--   0        0        0       62 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/axoden.rst
--rw-r--r--   0        0        0     1276 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      486 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/gui.rst
--rw-r--r--   0        0        0      454 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0      261 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/volume_projections.rst
--rw-r--r--   0        0        0     1351 2024-05-13 16:04:11.246441 axoden-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-13 16:04:11.378441 axoden-0.3.0/tox.ini
--rw-r--r--   0        0        0    12995 1970-01-01 00:00:00.000000 axoden-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1691 2024-05-13 18:18:50.691683 axoden-1.0.0/.github/workflows/build_executables.yml
+-rw-r--r--   0        0        0      768 2024-05-13 18:18:50.691683 axoden-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      338 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      436 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1195 2024-05-13 18:18:50.695683 axoden-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      494 2024-05-13 18:18:50.695683 axoden-1.0.0/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-13 18:18:50.695683 axoden-1.0.0/.streamlit/config.toml
+-rw-r--r--   0        0        0    32422 2024-05-13 18:18:50.695683 axoden-1.0.0/LICENSE
+-rw-r--r--   0        0        0    10581 2024-05-13 18:18:50.695683 axoden-1.0.0/README.md
+-rw-r--r--   0        0        0      599 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/__init__.py
+-rw-r--r--   0        0        0     9998 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/gui_projections_quantification.py
+-rw-r--r--   0        0        0     5314 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/1_📊️_Axoden.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/__init__.py
+-rw-r--r--   0        0        0      526 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/__main__.py
+-rw-r--r--   0        0        0     7857 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/app_utils.py
+-rw-r--r--   0        0        0     8263 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
+-rw-r--r--   0        0        0      570 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
+-rw-r--r--   0        0        0     2433 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/gui/streamlit_app/pdf_utils.py
+-rw-r--r--   0        0        0    29140 2024-05-13 18:18:50.695683 axoden-1.0.0/axoden/volume_projections.py
+-rw-r--r--   0        0        0    85110 2024-05-13 18:18:50.695683 axoden-1.0.0/media/control_plots.jpg
+-rw-r--r--   0        0        0    29869 2024-05-13 18:18:50.695683 axoden-1.0.0/media/summary_data.pdf
+-rw-r--r--   0        0        0   327888 2024-05-13 18:18:50.699683 axoden-1.0.0/media/summary_data_axis.pdf
+-rw-r--r--   0        0        0     1396 2024-05-13 18:18:50.699683 axoden-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-13 18:18:50.823683 axoden-1.0.0/tox.ini
+-rw-r--r--   0        0        0    11404 1970-01-01 00:00:00.000000 axoden-1.0.0/PKG-INFO
```

### Comparing `axoden-0.3.0/.github/workflows/build_executables.yml` & `axoden-1.0.0/.github/workflows/build_executables.yml`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/.github/workflows/docs.yml` & `axoden-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/.github/workflows/test.yml` & `axoden-1.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/LICENSE` & `axoden-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/README.md` & `axoden-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,35 @@
+Metadata-Version: 2.1
+Name: axoden
+Version: 1.0.0
+Summary: axoden simplifies the quantification of axonal projections in neuroscience.
+Author-email: Raquel Adaia Sandoval Ortega <raqueladaia@gmail.com>
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Dist: tqdm >= 4.0.0
+Requires-Dist: numpy >= 1.16.0
+Requires-Dist: pandas >= 2.0.0
+Requires-Dist: seaborn >= 0.10.0
+Requires-Dist: matplotlib >= 3.0.0
+Requires-Dist: pillow >= 10.0.0
+Requires-Dist: scikit-image >= 0.20.0
+Requires-Dist: streamlit >= 1.30.0 ; extra == "gui"
+Requires-Dist: streamlit-pdf-viewer >= 0.0.10 ; extra == "gui"
+Requires-Dist: pypdf >= 4.0.0 ; extra == "gui"
+Project-URL: Home, https://github.com/raqueladaia/AxoDen
+Provides-Extra: gui
+
 [![Test](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml)
 [![Lint](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml)
 [![PyPI](https://img.shields.io/pypi/v/axoden?label=pypi%20package)](https://pypi.org/project/axoden)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/axoden)
 
 # Axoden
 
-## TODOs
-
-- [ ] add one figure from the paper here that describes what AxoDen does
-- [x] set up github token to make it possible to upload release directly from gh action
-- [x] add `FLIT_PASSWORD` to github secrets to allow publish from gh action
-- [x] Raquel to write quick overview (=intro of 2-3 sentences) here in README.md
-- [ ] Test deployed streamlit app with two concurrent users and 100+ files each
-- [ ] Decide on upload limit for deployed app
-- [ ] Add citation here once publication is submitted
-- [ ] Add citation to streamlit app once publication is submitted
-- [ ] Add link to publication
-- [ ] make repo public once we're ready :muscle:
-
-- [ ] Raquel to write text for initial tutorial --> Add screenshots of steps & more explanation.
-- [x] Raquel to write section about how data is used on streamlit tutorial page. See readme.
-- [x] Raquel to go over main streamlit app and correct/adapt naming
-- [ ] Raquel to think if I want a question mark with explanation when hoovering over it
-- [x] Raquel to double check that the units are correct, volume_projections.py line 443 seems strange
-- [x] Raquel to include sample images
-
-- [x] Pascal to set up gh action for unit testing
-- [x] Pascal to set up gh action for linting
-- [x] Pascal to set up gh action to build standalone executables
-- [x] Pascal to automatically create release using gh action and attach executables
-- [x] Pascal to add badge for pypi
-- [x] Pascal to create gh action to update pip module from release
-- [x] Pascal to test pip module publish from gh action once secret is set up
-- [x] Pascal to build documentation using sphinx
-- [ ] Pascal to upload documentation once secret is set up
-
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
   - [Standalone GUI](#standalone-gui)
 - [Installation](#installation)
   - [With pip](#pip-install)
@@ -213,14 +204,15 @@
 usually at http://localhost:8501.
 
 
 This is the same interface as the [Streamlit Web App](https://axoden.streamlit.app).
 
 # Using axoden in your code
 Below you find a few examples of how to use axoden.
+You can see the full [documentation here](https://raqueladaia.github.io/AxoDen/).
 
 You can process a single image. This will not save any results or plots.
 ```python
 import axoden
 
 img_path = "test_images/745_TH-CL.tif"
 fig, data, data_axis = axoden.process_image(img_path, is_masked=True, pixel_size=0.75521)
@@ -251,7 +243,8 @@
 
 fig_data = axoden.plot_summary_data(df_data, "my_project")
 fig_data_axis = axoden.plot_signal_intensity_along_axis("my_project", df_data_axis, pixel_size=0.75521)
 
 fig_data.show()
 fig_data_axis.show()
 ```
+
```

### Comparing `axoden-0.3.0/axoden/__init__.py` & `axoden-1.0.0/axoden/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 axoden simplifies the quantification of axonal projections in neuroscience.
 """
 
-__version__ = "0.3.0"
+__version__ = "1.0.0"
 
 from .volume_projections import (  # noqa: F401
     load_table,
     plot_signal_intensity_along_axis,
     plot_summary_data,
     process_folder,
     process_image,
```

### Comparing `axoden-0.3.0/axoden/gui/gui_projections_quantification.py` & `axoden-1.0.0/axoden/gui/gui_projections_quantification.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/1_📊️_Axoden.py` & `axoden-1.0.0/axoden/gui/streamlit_app/1_📊️_Axoden.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         st.write("If you use the app for your research, cite it using the following:")
         st.page_link("pages/3_📖️_Cite_Axoden.py", label="Cite AxoDen", icon="📖️")
 
     st.header("Input")
     project_name = st.text_input(label="Project Name", value="AxoDen Analysis")
     pixel_size = st.number_input(
-        "Pixel Size (um):",
+        "Pixel Size (μm):",
         value=DEFAULT_PIXEL_SIZE,
         format="%f",
         on_change=invalidate_figure_cache,
         key="pixel_size",
     )  # Set the pixel size
     st.text(
         "Note:\nThe default pixel size is for the 20x Objective of the Keyence BZ-810X "
@@ -72,15 +72,15 @@
             "You uploaded {len(raw_files)}, remaining images will not be used in the "
             "analysis!"
         )
         raw_files = raw_files[:MAX_IMAGES]
 
     is_masked = st.checkbox(
         "Images are masked (desired brain region are cropped out, "
-        "backround fluorescence has values above 0,\n"
+        "backround fluorescence has values above 0, "
         "areas of the image lacking tissue have value 0)",
         value=True,
         on_change=invalidate_figure_cache,
         key="is_masked",
     )
 
     (
```

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/__main__.py` & `axoden-1.0.0/axoden/gui/streamlit_app/__main__.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/app_utils.py` & `axoden-1.0.0/axoden/gui/streamlit_app/app_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py` & `axoden-1.0.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py` & `axoden-1.0.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/gui/streamlit_app/pdf_utils.py` & `axoden-1.0.0/axoden/gui/streamlit_app/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-0.3.0/axoden/volume_projections.py` & `axoden-1.0.0/axoden/volume_projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
     img, msk = collect_image_mask(file_name, is_masked)
     msk_bool = msk.astype(bool)
     thr = compute_threshold(img[~msk_bool])
     img_bin = binarize_image(img, thr)
 
     [w, b, total] = count_pixels(img_bin[~msk_bool])
     area_w, area_b, area_img = compute_area(img_bin[~msk_bool], pixel_size)
-    area_image_mm = area_img / 1000
+    area_image_mm = area_img / 1000000
 
     # Append the information to the DataFrame for the image
     data = {
         "animal": animal,
         "brain_area": brain_area,
         "group": group,
         "pixels_signal": w,
@@ -654,15 +654,18 @@
     for i_col, col in enumerate(data_cols):
         # Set the column name as the title
         ax[i_col].set_title(sublplot_titles[i_col], weight="bold")
         # Set the xticks and labels for each data column
         ax[i_col].set_xticks(np.arange(0, len(brain_areas)))
         ax[i_col].set_xticklabels(brain_areas, rotation=45)
         # Set the y maximum value
-        yval_max = np.ceil(ax[i_col].get_ylim()[1] / 10) * 10
+        if col == "area_img_mm":
+            yval_max = np.ceil(ax[i_col].get_ylim()[1] * 100) / 100
+        else:
+            yval_max = np.ceil(ax[i_col].get_ylim()[1] / 10) * 10
         ax[i_col].set_yticks(np.linspace(0, yval_max, 6))
         ax[i_col].set_ylim(0, yval_max)
         # Set the y label
         ax[i_col].set_ylabel(ylabel_dict[col])
 
     # Print the number of animals per brain area
     df = pd.DataFrame.from_dict(dict_animals_brain_area, orient="index")
```

### Comparing `axoden-0.3.0/pyproject.toml` & `axoden-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Home = "https://github.com/raqueladaia/AxoDen"
 
 [tool.setuptools.dynamic]
 version = {attr = "axoden.__vesion__"}
 
 [tool.flit.sdist]
 include = ["axoden"]
-exclude = ["tests", "media", "test_images", "requirements*"]
+exclude = ["tests", "media/tkinter_gui.png", "test_images", "requirements*", "how_to_release.md", "docs"]
 
 [project.optional-dependencies]
 gui = [
     "streamlit >= 1.30.0",
     "streamlit-pdf-viewer >= 0.0.10",
     "pypdf >= 4.0.0",
 ]
```

### Comparing `axoden-0.3.0/PKG-INFO` & `axoden-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,14 @@
-Metadata-Version: 2.1
-Name: axoden
-Version: 0.3.0
-Summary: axoden simplifies the quantification of axonal projections in neuroscience.
-Author-email: Raquel Adaia Sandoval Ortega <raqueladaia@gmail.com>
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Dist: tqdm >= 4.0.0
-Requires-Dist: numpy >= 1.16.0
-Requires-Dist: pandas >= 2.0.0
-Requires-Dist: seaborn >= 0.10.0
-Requires-Dist: matplotlib >= 3.0.0
-Requires-Dist: pillow >= 10.0.0
-Requires-Dist: scikit-image >= 0.20.0
-Requires-Dist: streamlit >= 1.30.0 ; extra == "gui"
-Requires-Dist: streamlit-pdf-viewer >= 0.0.10 ; extra == "gui"
-Requires-Dist: pypdf >= 4.0.0 ; extra == "gui"
-Project-URL: Home, https://github.com/raqueladaia/AxoDen
-Provides-Extra: gui
-
 [![Test](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/test.yml)
 [![Lint](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/raqueladaia/AxoDen/actions/workflows/lint.yml)
 [![PyPI](https://img.shields.io/pypi/v/axoden?label=pypi%20package)](https://pypi.org/project/axoden)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/axoden)
 
 # Axoden
 
-## TODOs
-
-- [ ] add one figure from the paper here that describes what AxoDen does
-- [x] set up github token to make it possible to upload release directly from gh action
-- [x] add `FLIT_PASSWORD` to github secrets to allow publish from gh action
-- [x] Raquel to write quick overview (=intro of 2-3 sentences) here in README.md
-- [ ] Test deployed streamlit app with two concurrent users and 100+ files each
-- [ ] Decide on upload limit for deployed app
-- [ ] Add citation here once publication is submitted
-- [ ] Add citation to streamlit app once publication is submitted
-- [ ] Add link to publication
-- [ ] make repo public once we're ready :muscle:
-
-- [ ] Raquel to write text for initial tutorial --> Add screenshots of steps & more explanation.
-- [x] Raquel to write section about how data is used on streamlit tutorial page. See readme.
-- [x] Raquel to go over main streamlit app and correct/adapt naming
-- [ ] Raquel to think if I want a question mark with explanation when hoovering over it
-- [x] Raquel to double check that the units are correct, volume_projections.py line 443 seems strange
-- [x] Raquel to include sample images
-
-- [x] Pascal to set up gh action for unit testing
-- [x] Pascal to set up gh action for linting
-- [x] Pascal to set up gh action to build standalone executables
-- [x] Pascal to automatically create release using gh action and attach executables
-- [x] Pascal to add badge for pypi
-- [x] Pascal to create gh action to update pip module from release
-- [x] Pascal to test pip module publish from gh action once secret is set up
-- [x] Pascal to build documentation using sphinx
-- [ ] Pascal to upload documentation once secret is set up
-
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
   - [Standalone GUI](#standalone-gui)
 - [Installation](#installation)
   - [With pip](#pip-install)
@@ -234,14 +183,15 @@
 usually at http://localhost:8501.
 
 
 This is the same interface as the [Streamlit Web App](https://axoden.streamlit.app).
 
 # Using axoden in your code
 Below you find a few examples of how to use axoden.
+You can see the full [documentation here](https://raqueladaia.github.io/AxoDen/).
 
 You can process a single image. This will not save any results or plots.
 ```python
 import axoden
 
 img_path = "test_images/745_TH-CL.tif"
 fig, data, data_axis = axoden.process_image(img_path, is_masked=True, pixel_size=0.75521)
@@ -272,8 +222,7 @@
 
 fig_data = axoden.plot_summary_data(df_data, "my_project")
 fig_data_axis = axoden.plot_signal_intensity_along_axis("my_project", df_data_axis, pixel_size=0.75521)
 
 fig_data.show()
 fig_data_axis.show()
 ```
-
```

