# Comparing `tmp/mrsegmentator-1.0.3.tar.gz` & `tmp/mrsegmentator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsegmentator-1.0.3.tar", last modified: Sun May 12 15:10:21 2024, max compression
+gzip compressed data, was "mrsegmentator-1.0.4.tar", last modified: Sun May 12 16:11:37 2024, max compression
```

## Comparing `mrsegmentator-1.0.3.tar` & `mrsegmentator-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:21.020377 mrsegmentator-1.0.3/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 15:10:21.016679 mrsegmentator-1.0.3/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4531 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/README.md
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.3/pyproject.toml
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1660 2024-05-12 15:10:21.026015 mrsegmentator-1.0.3/setup.cfg
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:20.875536 mrsegmentator-1.0.3/src/
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:20.950079 mrsegmentator-1.0.3/src/mrsegmentator/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.3/src/mrsegmentator/__init__.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4088 2024-05-12 15:08:12.000000 mrsegmentator-1.0.3/src/mrsegmentator/config.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4749 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/inference.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1427 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/main.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3378 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/parser.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3236 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/simpleitk_reader_writer.py
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2516 2024-05-12 14:10:02.000000 mrsegmentator-1.0.3/src/mrsegmentator/utils.py
-drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 15:10:21.007866 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5561 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/PKG-INFO
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      497 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/SOURCES.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/dependency_links.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/entry_points.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       25 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/requires.txt
--rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-05-12 15:10:20.000000 mrsegmentator-1.0.3/src/mrsegmentator.egg-info/top_level.txt
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 16:11:37.405111 mrsegmentator-1.0.4/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5589 2024-05-12 16:11:37.401195 mrsegmentator-1.0.4/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4531 2024-05-12 14:10:02.000000 mrsegmentator-1.0.4/README.md
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       86 2024-02-27 08:52:29.000000 mrsegmentator-1.0.4/pyproject.toml
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1676 2024-05-12 16:11:37.411038 mrsegmentator-1.0.4/setup.cfg
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 16:11:37.251636 mrsegmentator-1.0.4/src/
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 16:11:37.333172 mrsegmentator-1.0.4/src/mrsegmentator/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        0 2024-02-27 08:52:29.000000 mrsegmentator-1.0.4/src/mrsegmentator/__init__.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     4088 2024-05-12 15:08:12.000000 mrsegmentator-1.0.4/src/mrsegmentator/config.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5003 2024-05-12 16:08:45.000000 mrsegmentator-1.0.4/src/mrsegmentator/inference.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     1427 2024-05-12 14:10:02.000000 mrsegmentator-1.0.4/src/mrsegmentator/main.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3378 2024-05-12 14:10:02.000000 mrsegmentator-1.0.4/src/mrsegmentator/parser.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2174 2024-05-12 16:08:34.000000 mrsegmentator-1.0.4/src/mrsegmentator/postprocessing.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     3236 2024-05-12 14:10:02.000000 mrsegmentator-1.0.4/src/mrsegmentator/simpleitk_reader_writer.py
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     2516 2024-05-12 14:10:02.000000 mrsegmentator-1.0.4/src/mrsegmentator/utils.py
+drwxr-xr-x   0 haha16   (167466) posix-nogroup (100100)        0 2024-05-12 16:11:37.392019 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)     5589 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/PKG-INFO
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)      533 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/SOURCES.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)        1 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/dependency_links.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       58 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/entry_points.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       38 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/requires.txt
+-rw-r--r--   0 haha16   (167466) posix-nogroup (100100)       14 2024-05-12 16:11:37.000000 mrsegmentator-1.0.4/src/mrsegmentator.egg-info/top_level.txt
```

### Comparing `mrsegmentator-1.0.3/PKG-INFO` & `mrsegmentator-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsegmentator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 Home-page: https://github.com/hhaentze/mrsegmentator
 Author: Hartmut Häntze
 Author-email: hartmut.haentze@charite.de
 Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
 Project-URL: repository, https://github.com/hhaentze/mrsegmentator
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: nnunetv2==2.2.1
 Requires-Dist: argparse
+Requires-Dist: monai==1.3.0
 
 <h2 align="center"> MRSegmentator: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences </h2>
 
 ***
 
 <div align="center">
 <a href="https://github.com/hhaentze/MRSegmentator/actions"><img alt="Continuous Integration" src="https://github.com/hhaentze/MRSegmentator/actions/workflows/ci.yml/badge.svg"></a>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.3 Summary: Robust Multi-
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.4 Summary: Robust Multi-
 Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
 github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
 hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
 hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
 hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
 :: Healthcare Industry Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
 Recognition Classifier: Topic :: Scientific/Engineering :: Medical Science
 Apps. Requires-Python: >=3.11 Description-Content-Type: text/markdown Requires-
-Dist: nnunetv2==2.2.1 Requires-Dist: argparse
+Dist: nnunetv2==2.2.1 Requires-Dist: argparse Requires-Dist: monai==1.3.0
  ********** MMRRSSeeggmmeennttaattoorr:: RRoobbuusstt MMuullttii--MMooddaalliittyy SSeeggmmeennttaattiioonn ooff 4400 CCllaasssseess iinn MMRRII
                             aanndd CCTT SSeeqquueenncceess **********
 ***
       _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 > Detect and segment 40 classes in MRI scans of the abdominal / pelvic / thorax
 region Contrary to CT scans, where tools for automatic multi-structure
 segmentation are quite mature, segmentation tasks in MRI scans are often either
```

### Comparing `mrsegmentator-1.0.3/README.md` & `mrsegmentator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/setup.cfg` & `mrsegmentator-1.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mrsegmentator
-version = 1.0.3
+version = 1.0.4
 author = Hartmut Häntze
 author_email = hartmut.haentze@charite.de
 description = Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/hhaentze/mrsegmentator
 project_urls = 
@@ -25,14 +25,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11
 install_requires = 
 	nnunetv2 == 2.2.1
 	argparse
+	monai == 1.3.0
 
 [options.packages.find]
 where = src
 exclude = 
 	bundles*
 	data*
 	logs*
```

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/config.py` & `mrsegmentator-1.0.4/src/mrsegmentator/config.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/inference.py` & `mrsegmentator-1.0.4/src/mrsegmentator/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import ntpath
 from pathlib import Path
 from typing import List, NoReturn, Tuple, Union
 
 import torch
 
-from mrsegmentator import config, utils
+from mrsegmentator import config, postprocessing, utils
 from mrsegmentator.simpleitk_reader_writer import SimpleITKIO
 
 config.disable_nnunet_path_warnings()
 from batchgenerators.utilities.file_and_folder_operations import join  # noqa: E402
 from nnunetv2.inference.predict_from_raw_data import nnUNetPredictor  # noqa: E402
 
 
@@ -92,14 +92,17 @@
                 props,
                 None,
                 num_processes=nproc,
                 save_probabilities=False,
                 num_processes_segmentation_export=nproc_export,
             )
 
+            # postprocessing
+            segmentations = [postprocessing.remap_wrapper(seg) for seg in segmentations]
+
             # paths to output images
             image_names = [ntpath.basename(f) for f in img_chunk]
             out_names = [utils.add_postfix(name, postfix) for name in image_names]
 
             # save images
             for seg, p, out in zip(segmentations, props, out_names):
                 SimpleITKIO().write_seg(seg, join(outdir, out), p, verbose=True)
@@ -126,12 +129,15 @@
             # stitch segmentations back together
             for _ in range(split_level):
                 segmentations = [
                     utils.stitch_segmentations(segmentations[_i], segmentations[_i + 1])
                     for _i in range(0, len(segmentations), 2)
                 ]
 
+            # postprocessing
+            segmentations = [postprocessing.remap_wrapper(seg) for seg in segmentations]
+
             # paths to output image
             out_name = utils.add_postfix(ntpath.basename(img), postfix)
 
             # save image
             SimpleITKIO().write_seg(segmentations[0], join(outdir, out_name), prop, verbose=True)
```

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/main.py` & `mrsegmentator-1.0.4/src/mrsegmentator/main.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/parser.py` & `mrsegmentator-1.0.4/src/mrsegmentator/parser.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/simpleitk_reader_writer.py` & `mrsegmentator-1.0.4/src/mrsegmentator/simpleitk_reader_writer.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator/utils.py` & `mrsegmentator-1.0.4/src/mrsegmentator/utils.py`

 * *Files identical despite different names*

### Comparing `mrsegmentator-1.0.3/src/mrsegmentator.egg-info/PKG-INFO` & `mrsegmentator-1.0.4/src/mrsegmentator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrsegmentator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences
 Home-page: https://github.com/hhaentze/mrsegmentator
 Author: Hartmut Häntze
 Author-email: hartmut.haentze@charite.de
 Project-URL: Bug Tracker, https://github.com/hhaentze/mrsegmentator/issues
 Project-URL: repository, https://github.com/hhaentze/mrsegmentator
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: nnunetv2==2.2.1
 Requires-Dist: argparse
+Requires-Dist: monai==1.3.0
 
 <h2 align="center"> MRSegmentator: Robust Multi-Modality Segmentation of 40 Classes in MRI and CT Sequences </h2>
 
 ***
 
 <div align="center">
 <a href="https://github.com/hhaentze/MRSegmentator/actions"><img alt="Continuous Integration" src="https://github.com/hhaentze/MRSegmentator/actions/workflows/ci.yml/badge.svg"></a>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.3 Summary: Robust Multi-
+Metadata-Version: 2.1 Name: mrsegmentator Version: 1.0.4 Summary: Robust Multi-
 Modality Segmentation of 40 Classes in MRI and CT Sequences Home-page: https://
 github.com/hhaentze/mrsegmentator Author: Hartmut HÃ¤ntze Author-email:
 hartmut.haentze@charite.de Project-URL: Bug Tracker, https://github.com/
 hhaentze/mrsegmentator/issues Project-URL: repository, https://github.com/
 hhaentze/mrsegmentator Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: POSIX :: Linux Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
 :: Healthcare Industry Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
 Recognition Classifier: Topic :: Scientific/Engineering :: Medical Science
 Apps. Requires-Python: >=3.11 Description-Content-Type: text/markdown Requires-
-Dist: nnunetv2==2.2.1 Requires-Dist: argparse
+Dist: nnunetv2==2.2.1 Requires-Dist: argparse Requires-Dist: monai==1.3.0
  ********** MMRRSSeeggmmeennttaattoorr:: RRoobbuusstt MMuullttii--MMooddaalliittyy SSeeggmmeennttaattiioonn ooff 4400 CCllaasssseess iinn MMRRII
                             aanndd CCTT SSeeqquueenncceess **********
 ***
       _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 > Detect and segment 40 classes in MRI scans of the abdominal / pelvic / thorax
 region Contrary to CT scans, where tools for automatic multi-structure
 segmentation are quite mature, segmentation tasks in MRI scans are often either
```

