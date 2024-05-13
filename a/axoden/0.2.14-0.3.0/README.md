# Comparing `tmp/axoden-0.2.14.tar.gz` & `tmp/axoden-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axoden-0.2.14.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "axoden-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `axoden-0.2.14.tar` & `axoden-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1829 2024-05-13 10:05:34.570717 axoden-0.2.14/.github/workflows/build_executables.yml
--rw-r--r--   0        0        0      679 2024-05-13 10:05:34.570717 axoden-0.2.14/.github/workflows/docs.yml
--rw-r--r--   0        0        0      364 2024-05-13 10:05:34.570717 axoden-0.2.14/.github/workflows/lint.yml
--rw-r--r--   0        0        0      436 2024-05-13 10:05:34.570717 axoden-0.2.14/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1219 2024-05-13 10:05:34.570717 axoden-0.2.14/.github/workflows/test.yml
--rw-r--r--   0        0        0      494 2024-05-13 10:05:34.570717 axoden-0.2.14/.gitignore
--rw-r--r--   0        0        0      154 2024-05-13 10:05:34.570717 axoden-0.2.14/.streamlit/config.toml
--rw-r--r--   0        0        0    32422 2024-05-13 10:05:34.570717 axoden-0.2.14/LICENSE
--rw-r--r--   0        0        0    12088 2024-05-13 10:05:34.570717 axoden-0.2.14/README.md
--rw-r--r--   0        0        0      650 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/__init__.py
--rw-r--r--   0        0        0      325 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/__init__.py
--rw-r--r--   0        0        0     9998 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/gui_projections_quantification.py
--rw-r--r--   0        0        0     5213 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/1_📊️_Axoden.py
--rw-r--r--   0        0        0        0 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/__init__.py
--rw-r--r--   0        0        0      526 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/__main__.py
--rw-r--r--   0        0        0     7857 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/app_utils.py
--rw-r--r--   0        0        0     3303 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
--rw-r--r--   0        0        0      570 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
--rw-r--r--   0        0        0     2433 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/gui/streamlit_app/pdf_utils.py
--rw-r--r--   0        0        0    29038 2024-05-13 10:05:34.570717 axoden-0.2.14/axoden/volume_projections.py
--rw-r--r--   0        0        0      638 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/Makefile
--rw-r--r--   0        0        0      804 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/make.bat
--rw-r--r--   0        0        0       62 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/source/axoden.rst
--rw-r--r--   0        0        0     1276 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/source/conf.py
--rw-r--r--   0        0        0      486 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/source/gui.rst
--rw-r--r--   0        0        0      454 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/source/index.rst
--rw-r--r--   0        0        0      261 2024-05-13 10:05:34.570717 axoden-0.2.14/docs/source/volume_projections.rst
--rw-r--r--   0        0        0     1281 2024-05-13 10:05:34.574717 axoden-0.2.14/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-13 10:05:34.698718 axoden-0.2.14/tox.ini
--rw-r--r--   0        0        0    12924 1970-01-01 00:00:00.000000 axoden-0.2.14/PKG-INFO
+-rw-r--r--   0        0        0     1691 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/build_executables.yml
+-rw-r--r--   0        0        0      768 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      338 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      436 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1195 2024-05-13 16:04:11.242441 axoden-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      494 2024-05-13 16:04:11.242441 axoden-0.3.0/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-13 16:04:11.242441 axoden-0.3.0/.streamlit/config.toml
+-rw-r--r--   0        0        0    32422 2024-05-13 16:04:11.242441 axoden-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12172 2024-05-13 16:04:11.242441 axoden-0.3.0/README.md
+-rw-r--r--   0        0        0      599 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/__init__.py
+-rw-r--r--   0        0        0     9998 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/gui_projections_quantification.py
+-rw-r--r--   0        0        0     5314 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/1_📊️_Axoden.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/__init__.py
+-rw-r--r--   0        0        0      526 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/__main__.py
+-rw-r--r--   0        0        0     7857 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/app_utils.py
+-rw-r--r--   0        0        0     8263 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py
+-rw-r--r--   0        0        0      570 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py
+-rw-r--r--   0        0        0     2433 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/gui/streamlit_app/pdf_utils.py
+-rw-r--r--   0        0        0    29018 2024-05-13 16:04:11.242441 axoden-0.3.0/axoden/volume_projections.py
+-rw-r--r--   0        0        0      638 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0       62 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/axoden.rst
+-rw-r--r--   0        0        0     1276 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      486 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/gui.rst
+-rw-r--r--   0        0        0      454 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0      261 2024-05-13 16:04:11.242441 axoden-0.3.0/docs/source/volume_projections.rst
+-rw-r--r--   0        0        0     1351 2024-05-13 16:04:11.246441 axoden-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-13 16:04:11.378441 axoden-0.3.0/tox.ini
+-rw-r--r--   0        0        0    12995 1970-01-01 00:00:00.000000 axoden-0.3.0/PKG-INFO
```

### Comparing `axoden-0.2.14/.github/workflows/build_executables.yml` & `axoden-0.3.0/.github/workflows/build_executables.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 name: build executables
 
-on: workflow_dispatch
-  # push:
-  #   tags:
-  #     - 'v*'
+on:
+  push:
+    tags:
+      - 'v*'
 
 env:
   VERSION: ${{ github.ref_name }}
 
 jobs:
   pyinstaller-builds:
     if: startsWith(github.ref, 'refs/tags/')
     runs-on: ${{ matrix.os }}-latest
     permissions:
       contents: write
     strategy:
       matrix:
-        # os: [ubuntu]
         include:
           - os: ubuntu
             file_extension: ""
             options: --onefile
           - os: macos
             file_extension: ".app"
             options: --windowed
@@ -30,15 +29,14 @@
     steps:
       - name: Create Standalone Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: "3.11"
           spec: "axoden/gui/gui_projections_quantification.py"
           requirements: "requirements.txt"
-          # upload_exe_with_name: "Axoden_${{ env.VERSION }}.${{ matrix.file_extension }}"
           options: ${{ matrix.options }} --name "Axoden_${{ env.VERSION }}" --hidden-import="PIL._tkinter_finder"
 
       - name: Echo 1
         run: ls dist
 
       - name: Zip executable ubuntu and macos
         if: ${{ matrix.os == 'ubuntu' || matrix.os == 'macos' }}
```

### Comparing `axoden-0.2.14/.github/workflows/test.yml` & `axoden-0.3.0/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Test
 
-on: workflow_dispatch
-  # push:
-  #   branches: [ "main", "release" ]
-  # pull_request:
-  #   branches: [ "main", "release" ]
+on:
+  push:
+    branches: [ "main", "release" ]
+  pull_request:
+    branches: [ "main", "release" ]
     
 concurrency:
   group: test-${{ github.ref }}
   cancel-in-progress: true
   
 jobs:
   test:
@@ -24,16 +24,16 @@
           - "3.12"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
         os:
           - ubuntu-latest
-          - macos-latest
           - windows-latest
+          # - macos-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v5
         with:
```

### Comparing `axoden-0.2.14/LICENSE` & `axoden-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/README.md` & `axoden-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 - [ ] Raquel to think if I want a question mark with explanation when hoovering over it
 - [x] Raquel to double check that the units are correct, volume_projections.py line 443 seems strange
 - [x] Raquel to include sample images
 
 - [x] Pascal to set up gh action for unit testing
 - [x] Pascal to set up gh action for linting
 - [x] Pascal to set up gh action to build standalone executables
+- [x] Pascal to automatically create release using gh action and attach executables
 - [x] Pascal to add badge for pypi
 - [x] Pascal to create gh action to update pip module from release
-- [ ] Pascal to test pip module publish from gh action once secret is set up
+- [x] Pascal to test pip module publish from gh action once secret is set up
 - [x] Pascal to build documentation using sphinx
 - [ ] Pascal to upload documentation once secret is set up
 
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
```

### Comparing `axoden-0.2.14/axoden/__init__.py` & `axoden-0.3.0/axoden/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
-The `axoden` module provides functionality for performing various operations related to
-quantification of axonal projections.
+axoden simplifies the quantification of axonal projections in neuroscience.
 """
 
-__version__ = "0.2.14"
+__version__ = "0.3.0"
 
 from .volume_projections import (  # noqa: F401
     load_table,
     plot_signal_intensity_along_axis,
     plot_summary_data,
     process_folder,
     process_image,
```

### Comparing `axoden-0.2.14/axoden/gui/gui_projections_quantification.py` & `axoden-0.3.0/axoden/gui/gui_projections_quantification.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/axoden/gui/streamlit_app/1_📊️_Axoden.py` & `axoden-0.3.0/axoden/gui/streamlit_app/1_📊️_Axoden.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         "Pixel Size (um):",
         value=DEFAULT_PIXEL_SIZE,
         format="%f",
         on_change=invalidate_figure_cache,
         key="pixel_size",
     )  # Set the pixel size
     st.text(
-        "Note:\nThe default pixel size is for the 20x Objective of the Keyence BZ-810X series.\n"
+        "Note:\nThe default pixel size is for the 20x Objective of the Keyence BZ-810X "
+        "series.\n"
         "Please change it according to the objective used.\n\n4x Objective: 3.77396\n"
         "20x Objective: 0.75521\n"
     )
 
     raw_files = st.file_uploader(
         "Upload image here. You can add more or remove them later.",
         type=["tif"],
@@ -89,35 +90,39 @@
     ) = process_images(
         raw_files, pixel_size, is_masked, cache=st.session_state.figure_cache
     )
 
     # plot table data results
     if st.session_state.table_data is not None:
         logger.info("Creating data section")
-        st.header("Data")
+        st.header("Summary Data")
 
         fig, fig_stream = cached_plot_summary_data(
             st.session_state.table_data, project_name
         )
 
         st.pyplot(fig)
-        st.download_button("Download figure as pdf", fig_stream, "data.pdf")
+        st.download_button(
+            "Download figure as pdf", fig_stream, "axoden_summary_data.pdf"
+        )
         st.dataframe(st.session_state.table_data)
 
     # plot table data by axis results
     if st.session_state.table_data_axis is not None:
         logger.info("Creating data axis section")
-        st.header("Data Axis")
+        st.header("Summary Data Axis")
 
         fig, fig_stream = cached_plot_signal_intensity_along_axis(
             project_name, st.session_state.table_data_axis, pixel_size
         )
         st.pyplot(fig)
 
-        st.download_button("Download figure as pdf", fig_stream, "data_axis.pdf")
+        st.download_button(
+            "Download figure as pdf", fig_stream, "axoden_summary_data_axis.pdf"
+        )
         st.dataframe(st.session_state.table_data_axis)
 
     logger.info("Creating control plots pdf")
     st.session_state.ctrl_plots_pdf = join_pdfs(st.session_state.figures)
 
     brain_regions = get_brain_regions(raw_files)
     if brain_regions:
```

### Comparing `axoden-0.2.14/axoden/gui/streamlit_app/__main__.py` & `axoden-0.3.0/axoden/gui/streamlit_app/__main__.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/axoden/gui/streamlit_app/app_utils.py` & `axoden-0.3.0/axoden/gui/streamlit_app/app_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py` & `axoden-0.3.0/axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/axoden/gui/streamlit_app/pdf_utils.py` & `axoden-0.3.0/axoden/gui/streamlit_app/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/axoden/volume_projections.py` & `axoden-0.3.0/axoden/volume_projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,17 +434,15 @@
     img, msk = collect_image_mask(file_name, is_masked)
     msk_bool = msk.astype(bool)
     thr = compute_threshold(img[~msk_bool])
     img_bin = binarize_image(img, thr)
 
     [w, b, total] = count_pixels(img_bin[~msk_bool])
     area_w, area_b, area_img = compute_area(img_bin[~msk_bool], pixel_size)
-    area_image_mm = (
-        area_img / 1000
-    )
+    area_image_mm = area_img / 1000
 
     # Append the information to the DataFrame for the image
     data = {
         "animal": animal,
         "brain_area": brain_area,
         "group": group,
         "pixels_signal": w,
@@ -835,15 +833,15 @@
     plt.subplots_adjust(top=0.92, bottom=0.05, hspace=0.5, wspace=0.2)
 
     return fig
 
 
 if __name__ == "__main__":
     pixel_size = (
-        0.75521  # um, based on 20x objective from the Keyence BZ-810X series microscope.
+        0.75521  # um, based on 20x objective from Keyence BZ-810X series microscope.
     )
     input_dir = "sample_images"
     output_dir = "output_data"
     is_masked = True
 
     # Collect the data and save it as a csv file
     quant_projections, quant_along_axis = process_folder(
```

### Comparing `axoden-0.2.14/docs/Makefile` & `axoden-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/docs/make.bat` & `axoden-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/docs/source/conf.py` & `axoden-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `axoden-0.2.14/pyproject.toml` & `axoden-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 pythonpath = [
     '.'
 ]
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
-exclude = ["axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py"]
+exclude = [
+    "axoden/gui/streamlit_app/pages/2_❔️_Tutorial_&_How_To.py",
+    "axoden/gui/streamlit_app/pages/3_📖️_Cite_Axoden.py",
+]
 
 [tool.ruff.lint]
 select = ['E', 'F', 'W', 'A', 'PLC', 'PLE', 'PLW', 'I', 'E501']
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
```

### Comparing `axoden-0.2.14/PKG-INFO` & `axoden-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: axoden
-Version: 0.2.14
-Summary: The `axoden` module provides functionality for performing various operations related to
+Version: 0.3.0
+Summary: axoden simplifies the quantification of axonal projections in neuroscience.
 Author-email: Raquel Adaia Sandoval Ortega <raqueladaia@gmail.com>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: tqdm >= 4.0.0
 Requires-Dist: numpy >= 1.16.0
 Requires-Dist: pandas >= 2.0.0
@@ -45,17 +45,18 @@
 - [ ] Raquel to think if I want a question mark with explanation when hoovering over it
 - [x] Raquel to double check that the units are correct, volume_projections.py line 443 seems strange
 - [x] Raquel to include sample images
 
 - [x] Pascal to set up gh action for unit testing
 - [x] Pascal to set up gh action for linting
 - [x] Pascal to set up gh action to build standalone executables
+- [x] Pascal to automatically create release using gh action and attach executables
 - [x] Pascal to add badge for pypi
 - [x] Pascal to create gh action to update pip module from release
-- [ ] Pascal to test pip module publish from gh action once secret is set up
+- [x] Pascal to test pip module publish from gh action once secret is set up
 - [x] Pascal to build documentation using sphinx
 - [ ] Pascal to upload documentation once secret is set up
 
 ## Table of Contents
 
 - [How to use AxoDen](#how-to-use-axoden)
   - [Streamlit App](#streamlit-app)
```

