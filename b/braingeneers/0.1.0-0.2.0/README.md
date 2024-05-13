# Comparing `tmp/braingeneers-0.1.0.tar.gz` & `tmp/braingeneers-0.2.0.tar.gz`

## Comparing `braingeneers-0.1.0.tar` & `braingeneers-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.gitattributes
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 braingeneers-0.1.0/Makefile
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 braingeneers-0.1.0/noxfile.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.devcontainer/post_create.sh
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 braingeneers-0.1.0/braingeneers/data/test_data/maxwell-metadata.expected.json
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 braingeneers-0.1.0/braingeneers/data/test_data/maxwell-metadata.old.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 braingeneers-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 braingeneers-0.1.0/docs/source/index.md
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/py.typed
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/analysis/__init__.py
--rw-r--r--   0        0        0    56578 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/analysis/analysis.py
--rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/analysis/analysis_test.py
--rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/analysis/visualize_maxwell.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/__init__.py
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets.py
--rw-r--r--   0        0        0    69091 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets_electrophysiology.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets_electrophysiology_test.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets_fluidics.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets_imaging.py
--rw-r--r--   0        0        0    20526 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/datasets_neuron.py
--rw-r--r--   0        0        0    35776 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Linux/libcompression.so
--rw-r--r--   0        0        0    34545 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Mac_arm64/libcompression.dylib
--rw-r--r--   0        0        0    17020 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Mac_x86_64/libcompression.dylib
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Windows/compression.dll
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/data/transforms/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/__init__.py
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/gui.py
--rw-r--r--   0        0        0    39712 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/messaging.py
--rw-r--r--   0        0        0    12828 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/messaging_test.py
--rw-r--r--   0        0        0    22618 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/shadows.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/shadows_dev_playground.py
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/iot/simple.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/ml/__init__.py
--rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/ml/ephys_dataloader.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/__init__.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/common_utils.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/configure.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/configure_test.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/memoize_s3.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/memoize_s3_test.py
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/numpy_s3_memmap.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/numpy_s3_memmap_test.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/s3wrangler/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/s3wrangler/s3wrangler_test.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/smart_open_braingeneers/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 braingeneers-0.1.0/src/braingeneers/utils/smart_open_braingeneers/smart_open_braingeneers_test.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 braingeneers-0.1.0/tests/test_package.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 braingeneers-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 braingeneers-0.1.0/LICENSE
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 braingeneers-0.1.0/README.md
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 braingeneers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10511 2020-02-02 00:00:00.000000 braingeneers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 braingeneers-0.2.0/Makefile
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 braingeneers-0.2.0/noxfile.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.devcontainer/post_create.sh
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 braingeneers-0.2.0/braingeneers/data/test_data/maxwell-metadata.expected.json
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 braingeneers-0.2.0/braingeneers/data/test_data/maxwell-metadata.old.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 braingeneers-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 braingeneers-0.2.0/docs/source/index.md
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/py.typed
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/analysis/__init__.py
+-rw-r--r--   0        0        0    56578 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/analysis/analysis.py
+-rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/analysis/analysis_test.py
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/analysis/visualize_maxwell.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/__init__.py
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets.py
+-rw-r--r--   0        0        0    62788 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets_electrophysiology.py
+-rw-r--r--   0        0        0    22241 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets_electrophysiology_test.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets_fluidics.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets_imaging.py
+-rw-r--r--   0        0        0    20526 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/datasets_neuron.py
+-rw-r--r--   0        0        0    35776 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Linux/libcompression.so
+-rw-r--r--   0        0        0    34545 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Mac_arm64/libcompression.dylib
+-rw-r--r--   0        0        0    17020 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Mac_x86_64/libcompression.dylib
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Windows/compression.dll
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/data/transforms/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/__init__.py
+-rw-r--r--   0        0        0    45073 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/device.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/example_device.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/example_device_main.py
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/gui.py
+-rw-r--r--   0        0        0    39659 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/messaging.py
+-rw-r--r--   0        0        0    12829 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/messaging_test.py
+-rw-r--r--   0        0        0    22618 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/shadows.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/shadows_dev_playground.py
+-rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/iot/simple.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/ml/__init__.py
+-rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/ml/ephys_dataloader.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/__init__.py
+-rw-r--r--   0        0        0    15799 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/common_utils.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/common_utils_test.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/configure.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/configure_test.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/memoize_s3.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/memoize_s3_test.py
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/numpy_s3_memmap.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/numpy_s3_memmap_test.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/s3wrangler/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/s3wrangler/s3wrangler_test.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/smart_open_braingeneers/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 braingeneers-0.2.0/src/braingeneers/utils/smart_open_braingeneers/smart_open_braingeneers_test.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 braingeneers-0.2.0/tests/test_package.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 braingeneers-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 braingeneers-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 braingeneers-0.2.0/README.md
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 braingeneers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 braingeneers-0.2.0/PKG-INFO
```

### Comparing `braingeneers-0.1.0/.pre-commit-config.yaml` & `braingeneers-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/noxfile.py` & `braingeneers-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/.github/CONTRIBUTING.md` & `braingeneers-0.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/.github/matchers/pylint.json` & `braingeneers-0.2.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/.github/workflows/cd.yml` & `braingeneers-0.2.0/.github/workflows/cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,42 +27,42 @@
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Build sdist and wheel
         run: pipx run build
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist
 
       - name: Check products
         run: pipx run twine check dist/*
   
   test-built-dist:
     needs: [dist]
     name: Test built distribution
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     steps:
-      - uses: actions/setup-python@v4.7.0
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: '3.10'
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
       - name: List contents of built dist
         run: |
           ls -ltrh
           ls -ltrh dist
       - name: Publish to Test PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.10
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           repository-url: https://test.pypi.org/legacy/
           verbose: true
           skip-existing: true
       - name: Check pypi packages
         run: |
           sleep 3
@@ -88,14 +88,14 @@
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.10
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         if: startsWith(github.ref, 'refs/tags')
```

### Comparing `braingeneers-0.1.0/.github/workflows/ci.yml` & `braingeneers-0.2.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,31 +20,31 @@
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.10", "3.11"]  # add this back later: , "3.12"
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
         experimental: [false, false, true]
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
 
       - name: Install package
-        run: python -m pip install .[test]
+        run: python -m pip install .[dev]
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
+        uses: codecov/codecov-action@v4.3.1
```

### Comparing `braingeneers-0.1.0/braingeneers/data/test_data/maxwell-metadata.expected.json` & `braingeneers-0.2.0/braingeneers/data/test_data/maxwell-metadata.expected.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 00001870: 3230 3233 2d30 382d 3132 2054 3137 3a32  2023-08-12 T17:2
 00001880: 373a 3539 3b22 0a20 2020 2020 2020 2020  7:59;".         
 00001890: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
 000018a0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
 000018b0: 2020 2020 2264 6174 615f 666f 726d 6174      "data_format
 000018c0: 223a 2022 4e65 7572 6f64 6174 6157 6974  ": "NeurodataWit
 000018d0: 686f 7574 426f 7264 6572 7322 0a20 2020  houtBorders".   
-000018e0: 2020 2020 207d 0a20 2020 207d 0a7d            }.    }.}
+000018e0: 2020 2020 207d 0a20 2020 207d 0a7d 0a         }.    }.}.
```

### Comparing `braingeneers-0.1.0/braingeneers/data/test_data/maxwell-metadata.old.json` & `braingeneers-0.2.0/braingeneers/data/test_data/maxwell-metadata.old.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -386,8 +386,8 @@
 00001810: 5f32 3032 3437 2e72 6177 2e68 3522 2c0a  _20247.raw.h5",.
 00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001830: 2020 2020 2274 696d 6573 7461 6d70 223a      "timestamp":
 00001840: 2022 3230 3233 2d30 382d 3132 2054 3137   "2023-08-12 T17
 00001850: 3a32 373a 3539 3b22 0a20 2020 2020 2020  :27:59;".       
 00001860: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
 00001870: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00001880: 207d 0a20 2020 207d 0a7d                  }.    }.}
+00001880: 207d 0a20 2020 207d 0a7d 0a               }.    }.}.
```

### Comparing `braingeneers-0.1.0/docs/source/conf.py` & `braingeneers-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/__init__.py` & `braingeneers-0.2.0/src/braingeneers/__init__.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/analysis/analysis.py` & `braingeneers-0.2.0/src/braingeneers/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/analysis/analysis_test.py` & `braingeneers-0.2.0/src/braingeneers/analysis/analysis_test.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/analysis/visualize_maxwell.py` & `braingeneers-0.2.0/src/braingeneers/analysis/visualize_maxwell.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/__init__.py` & `braingeneers-0.2.0/src/braingeneers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/datasets.py` & `braingeneers-0.2.0/src/braingeneers/data/datasets.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/datasets_electrophysiology.py` & `braingeneers-0.2.0/src/braingeneers/data/datasets_electrophysiology.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import os
+import sys
 import json
 import warnings
 import copy
+import diskcache
 
 import matplotlib.pyplot as plt
 import numpy as np
 import shutil
 import h5py
 import braingeneers.utils.smart_open_braingeneers as smart_open
 from collections import namedtuple
@@ -23,18 +25,14 @@
 import posixpath
 import pandas as pd
 from datetime import datetime
 import requests
 import re
 from types import ModuleType
 import bisect
-try:
-    import neuraltoolkit as ntk  # optional import
-except ImportError:
-    pass
 
 
 VALID_LOAD_DATA_DTYPES = [np.int16, np.float16, np.float32, np.float64]
 load_data_cache = dict()  # minimal cache for avoiding looping lookups of metadata in load_data
 
 
 # todo: david replace this with common utils
@@ -59,37 +57,64 @@
     else:
         # list file locally
         return os.listdir(braingeneers.get_default_endpoint() + '/ephys/')
 
 
 def save_metadata(metadata: dict):
     """
-    Saves a metadata file back to S3. This is not multi-writer safe, you can use a lock as shown in the example:
-
-    from braingeneers.iot.messaging import MessageBroker()
-    import braingeneers.data.datasets_electrophysiology as de
-
-    with MessageBroker().get_lock('a-unique-lock-name-for-your-process'):
-        metadata = de.load_metadata(uuid)
-        metadata = do_something_to(metadata)
-        de.save_metadata(metadata)
+    Saves a metadata file back to S3. This is not multi-writer safe, you can use:
+        braingeneers.utils.common_utils.checkout
+        braingeneers.utils.common_utils.checkin
+    to lock the file while you are writing to it.
 
     :param metadata: the metadata dictionary as obtained from load_metadata(uuid)
     """
     batch_uuid = metadata['uuid']
     save_path = posixpath.join(
         braingeneers.utils.common_utils.get_basepath(),
         'ephys',
         batch_uuid,
         'metadata.json'
     )
     with smart_open.open(save_path, 'w') as f:
         f.write(json.dumps(metadata, indent=2))
 
 
+def cached_load_data(cache_path: str, max_size_gb: int = 10, **kwargs):
+    """
+    Wraps a call to load_data with a diskcache at path `cache_path`.
+    This is multiprocessing/thread safe.
+    All arguments after the cache_path are passed to load_data (see load_data docs)
+    You must specify the load_data argument names to avoid ambiguity with the cached_load_data parameters.
+
+    When reading data from S3 (or even a compressed local file), this can provide a significant speedup by
+    storing the results of load_data in a local (uncompressed) cache.
+
+    Example usage:
+        from braingeneers.data.datasets_electrophysiology import load_metadata, cached_load_data
+
+        metadata = load_metadata('9999-00-00-e-test')
+        data = cached_load_data(cache_path='/tmp/cache-dir', metadata=metadata, experiment=0, offset=0, length=1000)
+
+    Note: this can safely be used with `map2` from `braingeneers.utils.common_utils` to parallelize calls to load_data.
+
+    :param cache_path: str, path to the cache directory.
+    :param max_size_gb: int, maximum size of the cache in GB (10 GB default). If the cache exceeds this size, the oldest items will be removed.
+    :param kwargs: keyword arguments to pass to load_data, see load_data documentation.
+    """
+    cache = diskcache.Cache(cache_path, size_limit=10 ** 9 * max_size_gb)
+    key = json.dumps(kwargs)
+    if key in cache:
+        return cache[key]
+    else:
+        data = load_data(**kwargs)
+        cache[key] = data
+        return data
+
+
 def load_metadata(batch_uuid: str) -> dict:
     """
     Loads the batch UUID metadata.
     Metadata structure documentation:
         https://github.com/braingeneers/wiki/blob/main/shared/organizing-data.md#metadata-json-file
     Example usage:
         metadata_json = load_metadata('2020-03-10-e-128silicon-mouse-p35')
@@ -283,19 +308,19 @@
 
     for i,center in enumerate(window_centers):
         # window is (start, end)
         window = (center - window_sz//2, center + window_sz//2)
 
         # Check if window is out of bounds
         if window[0] < 0 or window[1] > dataset_length:
-            print("Window out of bounds, inserting zeros for window",window)
+            print("Window out of bounds, inserting zeros for window", window)
             try:
                 data_temp = np.zeros((data_temp.shape[0],window_sz),dtype=dtype)
             except Exception as e:
-                print(e)
+                print(e, file=sys.stderr)
                 data_temp = load_window(metadata, exp, window, dtype=dtype, channels=channels)
         else:
             data_temp = load_window(metadata, exp, window, dtype=dtype, channels=channels)
         
         # Check if window is the right size
         if data_temp.shape[1] != window_sz:
             print("Data shape mismatch, inserting zeros for window",window)
@@ -655,34 +680,36 @@
         with smart_open.open(stim_path, 'rb') as f:
             # read the csv into dataframe
             f = io.TextIOWrapper(f, encoding='utf-8')
             df = pd.read_csv(f, header=0)#, index_col=0)
         return df
         
     except FileNotFoundError:
-        print(f'\tThere seems to be no stim log file for this experiment! :(')
+        print(f'\tThere seems to be no stim log file for this experiment! :(', file=sys.stderr)
         return None
     except OSError:
-        print(f'\tThere seems to be no stim log file (on s3) for this experiment! :(')
+        print(f'\tThere seems to be no stim log file (on s3) for this experiment! :(', file=sys.stderr)
         return None
 
    
-def load_gpio_maxwell(dataset_path, fs=20000):
+def load_gpio_maxwell(dataset_path, fs=20000.0):
     """
     Loads the GPIO events for optogenetics stimulation.
     :param dataset_path: a local or a s3 path
     :param fs: sample rate
     :return: an array of opto stimulation pairs as [[start, end]] in seconds
     """
     with smart_open.open(dataset_path, 'rb') as f:
         with h5py.File(f, 'r') as dataset:
-            assert 'bits' in dataset.keys(), 'No GPIO event in the dataset!'
+            if 'bits' not in dataset.keys():
+                print('No GPIO event in the dataset!', file=sys.stderr)
+                return np.array([])
             bits_dataset = list(dataset['bits'])
-            bits_dataframe = [bits_dataset[i][0] for i in range(len(bits_dataset))]  
-            rec_startframe = dataset['raw'][-1, 0] << 16 | dataset['raw'][-2, 0]
+            bits_dataframe = [bits_dataset[i][0] for i in range(len(bits_dataset))]
+            rec_startframe = dataset['sig'][-1, 0] << 16 | dataset['sig'][-2, 0]
     if len(bits_dataframe) % 2 == 0:
         stim_pairs = (np.array(bits_dataframe) - rec_startframe).reshape(len(bits_dataframe) // 2, 2)
         return stim_pairs / fs
     else:
         print("Odd number of GPIO events can't be paired. Here returns all the events.")
         return (np.array(bits_dataframe) - rec_startframe)/fs
 
@@ -840,141 +867,14 @@
 
 
 def _read_hengenlab_ecube_timestamp(filepath: str) -> int:
     with smart_open.open(filepath, 'rb') as f:
         return int(np.frombuffer(f.read(8), dtype=np.uint64))
 
 
-def generate_metadata_hengenlab(batch_uuid: str,
-                                dataset_name: str,
-                                experiment_name: Union[List[str], str] = 'experiment1',
-                                fs: int = 25000,
-                                n_threads: int = 32,
-                                save: bool = False):
-    """
-    Generates a metadata json and experiment1...experimentN section for a hengenlab dataset upload.
-    File locations in S3 for hengenlab neural data files:
-        s3://braingeneers/ephys/YYYY-MM-DD-e-${DATASET_NAME}/original/data/*.bin
-    Contiguous recording periods
-    :param batch_uuid: location on braingeneers storage (S3)
-    :param dataset_name: the dataset_name as defined in `neuraltoolkit`. Metadata will be pulled from `neuraltoolkit`.
-    :param experiment_name: Dataset name as stored in `neuraltoolkit`. For example "CAF26"
-    :param fs: sampling rate, default to 25,000
-    :param n_threads: number of threads to use for reading ecube timestamps (default: 32)
-    :param save: (default False) option to save the metadata.json back to S3
-        (or the current braingeneers.default_endpoint)
-    :return: metadata.json
-    """
-    # hengenlab's (current) source of record for experiment metadata is stored in a repo which can't be imported
-    # due to unacceptable dependencies. Instead, the source code is being downloaded with the relevant static
-    # functions parsed out explicitly. This is a hacky approach, but this data shouldn't be stored
-    # in a repo and is expected to be replaced with a proper database in the future.
-    # All current solutions to this problem are bad, this is the least objectionable solution.
-    crit_utils_src = requests.get('https://raw.githubusercontent.com/hengenlab/sahara_work/master/crit_utils.py').text
-
-    src_get_birthday = re.search(r'(def get_birthday\(animal, returnall=False\):.+?)\ndef ', crit_utils_src, flags=re.S).group(1)
-    src_get_regions = re.search(r'(def get_regions\(animal\):.+?)\ndef ', crit_utils_src, flags=re.S).group(1)
-    src_get_sex = re.search(r'(def get_sex\(animal\):.+?)\ndef ', crit_utils_src, flags=re.S).group(1)
-    src_get_genotype = re.search(r'(def get_genotype\(animal\):.+?)\ndef ', crit_utils_src, flags=re.S).group(1)
-    src_get_hstype = re.search(r'(def get_hstype\(animal\):.+?)\ndef ', crit_utils_src, flags=re.S).group(1)
-
-    module = ModuleType('tempmodule')
-    module.dt = datetime  # the only import necessary to run these static functions
-    exec(compile(src_get_birthday, '', 'exec'), module.__dict__)
-    exec(compile(src_get_regions, '', 'exec'), module.__dict__)
-    exec(compile(src_get_sex, '', 'exec'), module.__dict__)
-    exec(compile(src_get_genotype, '', 'exec'), module.__dict__)
-    exec(compile(src_get_hstype, '', 'exec'), module.__dict__)
-
-    headstage_types = module.get_hstype(dataset_name.lower())
-
-    # list neural data files on S3
-    s3_path = f's3://braingeneers/ephys/{batch_uuid}/original/{experiment_name}/'
-    neural_data_files = common_utils.file_list(s3_path)
-    assert len(neural_data_files) > 0, f'No neural data files found at: {s3_path}'
-
-    args = [s3_path + ndf[0] for ndf in neural_data_files]
-
-    # get ecube times for each file
-    ecube_timestamps = common_utils.map2(
-        _read_hengenlab_ecube_timestamp,
-        args=args,
-        parallelism=n_threads,
-        use_multithreading=True,
-    )
-
-    # sort data files by ecube timestamps
-    neural_data_files = [(*ndf, et) for ndf, et in zip(neural_data_files, ecube_timestamps)]
-    neural_data_files.sort(key=lambda ndf: ndf[3])
-
-    # parse n_channels from file name
-    channels_match = re.search(r'.*Headstages_(\d+)_Channels.*', neural_data_files[0][0])
-    assert channels_match is not None, f'Unable to parse n_channels from filename: {neural_data_files[0][0]}'
-    n_channels = int(channels_match.group(1))
-
-    # parse timestamp from first file name
-    timestamp_match = re.search(r'.*_Channels_int16_(.+)\.bin', neural_data_files[0][0])
-    assert timestamp_match is not None, f'Unable to parse timestamp from filename: {neural_data_files[0][0]}'
-    timestamp = datetime.strptime(timestamp_match.group(1), '%Y-%m-%d_%H-%M-%S')
-
-    channels_per_probe = n_channels // len(headstage_types)
-    channel_map = list(itertools.chain(*[
-        (ntk.find_channel_map(hstype, number_of_channels=channels_per_probe) + i * channels_per_probe).tolist()
-        for i, hstype in enumerate(headstage_types)
-    ]))
-
-    metadata = dict(
-        uuid=batch_uuid,
-        timestamp=timestamp.isoformat(),
-        issue='',
-        channel_map=channel_map,
-        headstage_types=headstage_types,
-        notes=dict(
-            purpose_of_experiment='',
-            comments='',
-            biology=dict(
-                sample_type='mouse',
-                dataset_name=dataset_name,
-                birthday=module.get_birthday(dataset_name.lower()).isoformat(),
-                gender=module.get_sex(dataset_name.lower()),
-                genotype=module.get_genotype(dataset_name.lower()),
-            ),
-        ),
-        ephys_experiments=[dict(
-            name=experiment_name,
-            hardware='Hengenlab',
-            num_channels=n_channels,
-            sample_rate=fs,
-            voltage_scaling_factor=0.19073486328125,
-            timestamp=timestamp.isoformat(),
-            units='\u00b5V',
-            version='1.0.0',
-            blocks=[
-                {
-                    'num_frames': (size - 8) // 2 // n_channels,
-                    'path': f'original/{experiment_name}/{neural_data_file.split("/")[-1]}',
-                    'timestamp': datetime.strptime(
-                        re.search(r'.*_Channels_int16_(.+)\.bin', neural_data_file).group(1),
-                        '%Y-%m-%d_%H-%M-%S',
-                    ).isoformat(),
-                    'ecube_time': ecube_time,
-                }
-                for neural_data_file, last_modified_timestamp, size, ecube_time in neural_data_files
-            ],
-        )],
-    )
-
-    if save is True:
-        save_path = f's3://braingeneers/ephys/{batch_uuid}/metadata.json'
-        with smart_open.open(save_path, 'w') as f:
-            f.write(json.dumps(metadata, indent=2))
-
-    return metadata
-
-
 # --- AXION READER -----------------------------
 def from_uint64(all_values):
     """
     FromUint64: Deserializes an entry record from its native 64
     bit format in AxIS files.
     ----------------64 Bits--------------
     | ID (1 Byte) |   Length (7 Bytes)  |
@@ -1224,15 +1124,15 @@
                     # need electrode layout in rows and columns
                     corrected_idx = ((item.eRow - 1) * electrode_layout_row_col[0]) + (item.eCol - 1)
                     assert corrected_idx is not None and well is not None and isinstance(corrected_idx, int)
                     corrected_map[well][corrected_idx] = idx
 
                 fid.seek(start + int(obj.length.item()), 0)
                 if fid.tell() != start + obj.length:
-                    print('Unexpected Channel array length')
+                    print('Unexpected Channel array length', file=sys.stderr)
 
             elif obj.type == 3:
                 continue
 
             elif obj.type == 4:
                 start = fid.tell()
                 data_start = fid.tell()
@@ -1296,55 +1196,14 @@
         # A3 = (1,3) 128-191
         # B1 = (2,1) 192-255
         # B2 = (2,2) 256-319
         # B3 = (2,3) 320-383
         return final_raw_data_reshaped
 
 
-# class IndexedList(list):
-#     """
-#     A variant of OrderedDict indexable by index (int) or name (str).
-#     This class forces ints to represent index by location, else index by name/object.
-#     Example usages:
-#         metadata['ephys_experiments']['experiment0']    # index by name (must use str type)
-#         metadata['ephys_experiments'][0]                # index by location (must use int type)
-#     """
-#
-#     def __init__(self, original_list: list, key: callable):
-#         self.keys_ordered = [key(v) for v in original_list]
-#         self.dict = {key(v): v for v in original_list}
-#         super().__init__()
-#
-#     def __getitem__(self, key):
-#         print(key)
-#         if isinstance(key, int):
-#             return self.dict[self.keys_ordered[key]]
-#         elif isinstance(key, str):
-#             return self.dict[key]
-#         else:
-#             raise KeyError(f'Key must be type int (index by location) or str (index by name), got type: {type(key)}')
-#
-#     def __iter__(self) -> Iterator:
-#         def g():
-#             for k in self.keys_ordered:
-#                 yield self.dict[k]
-#
-#         return g()
-#
-#     def __hash__(self):
-#         return self.dict.__hash__()
-#
-#     def __eq__(self, other):
-#         return isinstance(other, IndexedList) and self.dict.__eq__(other.dict)
-#
-#     def __add__(self, value):
-#         self.keys_ordered.append(value)
-#         self.dict[value] = value
-
-
 def get_mearec_h5_recordings_file(batch_uuid: str):
     """
     Returns the filepath to the MEArec .h5/.hdf5 recordings file for the given UUID.
 
     Assumes (and enforces) that exactly one data file is stored:
         ${ENDPOINT}/ephys/YYYY-MM-DD-e-[descriptor]/original/experiments/recordings_*.h5 ( or "recordings_*.hdf5")
         (ENDPOINT defaults to s3://braingeneers)
```

### Comparing `braingeneers-0.1.0/src/braingeneers/data/datasets_electrophysiology_test.py` & `braingeneers-0.2.0/src/braingeneers/data/datasets_electrophysiology_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import unittest
+import tempfile
+import shutil
+import diskcache
+import json
+import threading
 import braingeneers
 import braingeneers.data.datasets_electrophysiology as ephys
-import json
 from braingeneers import skip_unittest_if_offline
-# import braingeneers.utils.smart_open_braingeneers as smart_open
-import smart_open
+import braingeneers.utils.smart_open_braingeneers as smart_open
 import boto3
 import numpy as np
-
+from unittest.mock import patch
+from braingeneers.data.datasets_electrophysiology import cached_load_data
 from unittest.mock import patch
 
+
 class MaxwellReaderTests(unittest.TestCase):
 
     @skip_unittest_if_offline
     def test_online_maxwell_stitched_uuid(self):
         uuid = '2023-04-17-e-causal_v1'
         metadata = ephys.load_metadata(uuid)
         data = ephys.load_data(
@@ -120,14 +125,33 @@
 
         with open('test_data/maxwell-metadata.expected.json', 'r') as f:
             expected_metadata = json.load(f)
             expected_metadata['timestamp'] = ''
 
         assert modified_metadata == expected_metadata
 
+    @skip_unittest_if_offline
+    def test_load_gpio_maxwell(self):
+        """ Read gpio event for Maxwell V1 file"""
+        data_1 = "s3://braingeneers/ephys/" \
+                 "2023-04-02-hc328_rec/original/data/" \
+                 "2023_04_02_hc328_0.raw.h5"
+        data_2 = "s3://braingeneers/ephys/" \
+                 "2023-04-04-e-hc328_hckcr1-2_040423_recs/original/data/" \
+                 "hc3.28_hckcr1_chip8787_plated4.4_rec4.4.raw.h5"
+        data_3 = "s3://braingeneers/ephys/" \
+                 "2023-04-04-e-hc328_hckcr1-2_040423_recs/original/data/" \
+                 "2023_04_04_hc328_hckcr1-2_3.raw.h5"
+        gpio_1 = ephys.load_gpio_maxwell(data_1)
+        gpio_2 = ephys.load_gpio_maxwell(data_2)
+        gpio_3 = ephys.load_gpio_maxwell(data_3)
+        self.assertEqual(gpio_1.shape, (1, 2))
+        self.assertEqual(gpio_2.shape, (0,))
+        self.assertEqual(gpio_3.shape, (29,))
+
 
 class MEArecReaderTests(unittest.TestCase):
     """The fake reader test."""
     batch_uuid = '2023-08-29-e-mearec-6cells-tetrode'
 
     @skip_unittest_if_offline
     def test_online_mearec_generate_metadata(self):
@@ -390,51 +414,91 @@
         expected_float32 = np.array(expected_raw, dtype=np.int16) * gain
 
         # this can't be checked with ntk easily because ntk also applies an odd int16 scaling of the data
         self.assertTrue(np.all(expected_float32 == data[1, :]))
         self.assertEqual((192, 4), data.shape)
         self.assertEqual(np.float32, data.dtype)
 
-    @skip_unittest_if_offline
-    def test_online_generate_metadata(self):
-        metadata = ephys.generate_metadata_hengenlab(
-            batch_uuid=self.batch_uuid,
-            dataset_name='CAF26',
-            save=False,
-        )
 
-        # top level items
-        self.assertEqual(metadata['uuid'], '2020-04-12-e-hengenlab-caf26')
-        self.assertEqual(metadata['timestamp'], '2020-08-07T14:00:15')
-        self.assertEqual(metadata['issue'], '')
-        self.assertEqual(metadata['headstage_types'], ['EAB50chmap_00', 'APT_PCB', 'APT_PCB'])
+class TestCachedLoadData(unittest.TestCase):
+
+    def setUp(self):
+        # Create a temporary directory for the cache
+        self.cache_dir = tempfile.mkdtemp(prefix='test_cache_')
+
+    def tearDown(self):
+        # Remove the temporary directory after the test
+        shutil.rmtree(self.cache_dir)
+
+    @patch('braingeneers.data.datasets_electrophysiology.load_data')
+    def test_caching_mechanism(self, mock_load_data):
+        """
+        Test that data is properly cached and retrieved on subsequent calls with the same parameters.
+        """
+        mock_load_data.return_value = 'mock_data'
+        metadata = {'uuid': 'test_uuid'}
+
+        # First call should invoke load_data
+        first_call_data = cached_load_data(self.cache_dir, metadata=metadata, experiment=0)
+        mock_load_data.assert_called_once()
+
+        # Second call should retrieve data from cache and not invoke load_data again
+        second_call_data = cached_load_data(self.cache_dir, metadata=metadata, experiment=0)
+        self.assertEqual(first_call_data, second_call_data)
+        mock_load_data.assert_called_once()  # Still called only once
+
+    @patch('braingeneers.data.datasets_electrophysiology.load_data')
+    def test_cache_eviction_when_full(self, mock_load_data):
+        """
+        Test that the oldest items are evicted from the cache when it exceeds its size limit.
+        """
+        mock_load_data.side_effect = lambda **kwargs: f"data_{kwargs['experiment']}"
+        max_size_gb = 0.000001  # Set a very small cache size to test eviction
+
+        # Populate the cache with enough data to exceed its size limit
+        for i in range(10):
+            cached_load_data(self.cache_dir, max_size_gb=max_size_gb, metadata={'uuid': 'test_uuid'}, experiment=i)
+
+        cache = diskcache.Cache(self.cache_dir)
+        self.assertLess(len(cache), 10)  # Ensure some items were evicted
+
+    @patch('braingeneers.data.datasets_electrophysiology.load_data')
+    def test_arguments_passed_to_load_data(self, mock_load_data):
+        """
+        Test that all arguments after cache_path are correctly passed to the underlying load_data function.
+        """
+        # Mock load_data to return a serializable object, e.g., a numpy array
+        mock_load_data.return_value = np.array([1, 2, 3])
+
+        kwargs = {'metadata': {'uuid': 'test_uuid'}, 'experiment': 0, 'offset': 0, 'length': 1000}
+        cached_load_data(self.cache_dir, **kwargs)
+        mock_load_data.assert_called_with(**kwargs)
+
+    @patch('braingeneers.data.datasets_electrophysiology.load_data')
+    def test_multiprocessing_thread_safety(self, mock_load_data):
+        """
+        Test that the caching mechanism is multiprocessing/thread-safe.
+        """
+        # Mock load_data to return a serializable object, e.g., a numpy array
+        mock_load_data.return_value = np.array([1, 2, 3])
 
-        # notes
-        self.assertEqual(metadata['notes']['biology']['sample_type'], 'mouse')
-        self.assertEqual(metadata['notes']['biology']['dataset_name'], 'CAF26')
-        self.assertEqual(metadata['notes']['biology']['birthday'], '2020-02-20T07:30:00')
-        self.assertEqual(metadata['notes']['biology']['genotype'], 'wt')
-
-        # ephys_experiments
-        self.assertEqual(len(metadata['ephys_experiments']), 1)
-        self.assertTrue(isinstance(metadata['ephys_experiments'], list))
-
-        experiment = metadata['ephys_experiments'][0]
-        self.assertEqual(experiment['name'], 'experiment1')
-        self.assertEqual(experiment['hardware'], 'Hengenlab')
-        self.assertEqual(experiment['num_channels'], 192)
-        self.assertEqual(experiment['sample_rate'], 25000)
-        self.assertEqual(experiment['voltage_scaling_factor'], 0.19073486328125)
-        self.assertEqual(experiment['timestamp'], '2020-08-07T14:00:15')
-        self.assertEqual(experiment['units'], '\u00b5V')
-        self.assertEqual(experiment['version'], '1.0.0')
-        self.assertEqual(len(experiment['blocks']), 324)
-
-        block1 = metadata['ephys_experiments'][0]['blocks'][1]
-        self.assertEqual(block1['num_frames'], 7500000)
-        self.assertEqual(block1['path'], 'original/experiment1/Headstages_192_Channels_int16_2020-08-07_14-05-16.bin')
-        self.assertEqual(block1['timestamp'], '2020-08-07T14:05:16')
-        self.assertEqual(block1['ecube_time'], 301061600050)
+        def thread_function(cache_path, metadata, experiment):
+            # This function uses the mocked load_data indirectly via cached_load_data
+            cached_load_data(cache_path, metadata=metadata, experiment=experiment)
+
+        metadata = {'uuid': 'test_uuid'}
+        threads = []
+        for i in range(10):
+            t = threading.Thread(target=thread_function, args=(self.cache_dir, metadata, i))
+            threads.append(t)
+            t.start()
+
+        for t in threads:
+            t.join()
+
+        # If the cache is thread-safe, this operation should complete without error
+        # This assertion is basic and assumes the test's success implies thread safety
+        self.assertTrue(True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `braingeneers-0.1.0/src/braingeneers/data/datasets_imaging.py` & `braingeneers-0.2.0/src/braingeneers/data/datasets_imaging.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/datasets_neuron.py` & `braingeneers-0.2.0/src/braingeneers/data/datasets_neuron.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Linux/libcompression.so` & `braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Linux/libcompression.so`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Mac_arm64/libcompression.dylib` & `braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Mac_arm64/libcompression.dylib`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Mac_x86_64/libcompression.dylib` & `braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Mac_x86_64/libcompression.dylib`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/data/mxw_h5_plugin/Windows/compression.dll` & `braingeneers-0.2.0/src/braingeneers/data/mxw_h5_plugin/Windows/compression.dll`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/gui.py` & `braingeneers-0.2.0/src/braingeneers/iot/gui.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/messaging.py` & `braingeneers-0.2.0/src/braingeneers/iot/messaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 """ A simplified MQTT client for Braingeneers specific connections """
-
 import redis
-import tempfile
-import functools
-import json
-import inspect
 import logging
 import os
 import re
-import time
 import io
 import configparser
 import threading
 import queue
 import uuid
-from typing import Callable, Tuple, List, Dict, Union
 import random
 import json
 import braingeneers.iot.shadows as sh
-from paho.mqtt import client as mqtt_client
-from deprecated import deprecated
 import pickle
-from tenacity import retry, wait_exponential, after_log
+
+from typing import Callable, Tuple, List, Dict, Union
+from deprecated import deprecated
+from paho.mqtt import client as mqtt_client
+from paho.mqtt.enums import CallbackAPIVersion
 
 
 AWS_REGION = 'us-west-2'
 AWS_PROFILE = 'aws-braingeneers-iot'
 REDIS_HOST = 'redis.braingeneers.gi.ucsc.edu'
 REDIS_PORT = 6379
 
@@ -763,15 +758,15 @@
                 else:
                     self.logger.error("Failed to connect to MQTT, return code %d\n", rc)
 
             def on_log(client, userdata, level, buf):
                 self.logger.debug("MQTT log: %s", buf)
 
             client_id = f'braingeneerspy-{random.randint(0, 1000)}'
-            self._mqtt_connection = mqtt_client.Client(client_id)
+            self._mqtt_connection = mqtt_client.Client(CallbackAPIVersion.VERSION1, client_id)
             self._mqtt_connection.username_pw_set(self._mqtt_profile_id, self._mqtt_profile_key)
             self._mqtt_connection.on_connect = on_connect
             self._mqtt_connection.on_log = on_log
             self._mqtt_connection.reconnect_delay_set(min_delay=1, max_delay=60)
             self._mqtt_connection.connect(host=self._mqtt_endpoint, port=self._mqtt_port, keepalive=15)
             self._mqtt_connection.loop_start()
 
@@ -817,8 +812,7 @@
         else:
             os.environ[self.env] = self.save_original_env_value
 
 
 def _mqtt_topic_regex(topic: str) -> str:
     """ Converts a topic string with wildcards to a regex string """
     return "^" + topic.replace("+", "[^/]+").replace("#", ".*").replace("$", "\\$") + "$"
-
```

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/messaging_test.py` & `braingeneers-0.2.0/src/braingeneers/iot/messaging_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,9 +299,10 @@
 
     def test_acquire_release(self):
         lock = self.mb.get_lock('unittest')
         lock.acquire()
         lock.release()
 
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/shadows.py` & `braingeneers-0.2.0/src/braingeneers/iot/shadows.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/shadows_dev_playground.py` & `braingeneers-0.2.0/src/braingeneers/iot/shadows_dev_playground.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/iot/simple.py` & `braingeneers-0.2.0/src/braingeneers/iot/simple.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/ml/ephys_dataloader.py` & `braingeneers-0.2.0/src/braingeneers/ml/ephys_dataloader.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/__init__.py` & `braingeneers-0.2.0/src/braingeneers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/memoize_s3.py` & `braingeneers-0.2.0/src/braingeneers/utils/memoize_s3.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/memoize_s3_test.py` & `braingeneers-0.2.0/src/braingeneers/utils/memoize_s3_test.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/numpy_s3_memmap.py` & `braingeneers-0.2.0/src/braingeneers/utils/numpy_s3_memmap.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/numpy_s3_memmap_test.py` & `braingeneers-0.2.0/src/braingeneers/utils/numpy_s3_memmap_test.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/src/braingeneers/utils/smart_open_braingeneers/smart_open_braingeneers_test.py` & `braingeneers-0.2.0/src/braingeneers/utils/smart_open_braingeneers/smart_open_braingeneers_test.py`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/.gitignore` & `braingeneers-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/LICENSE` & `braingeneers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `braingeneers-0.1.0/README.md` & `braingeneers-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,51 +17,63 @@
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/braingeneers/braingeneerspy?quickstart=1)
 
 Instruction on how to contribute to this project can be found in the [CONTRIBUTION.md](https://github.com/braingeneers/braingeneerspy/blob/development/.github/CONTRIBUTING.md).
 
 ## Installation
 
-You can install `braingeneerspy` using `pip` with the following commands:
+You can install `braingeneers` using `pip` with the following commands:
 
 ### Install from PyPI (Recommended)
 
 ```bash
-pip install braingeneerspy
+pip install braingeneers
 ```
 
 ### Install from GitHub
 
 ```bash
 pip install --force-reinstall git+https://github.com/braingeneers/braingeneerspy.git
 ```
 
 ### Install with Optional Dependencies
 
-You can install `braingeneerspy` with specific optional dependencies based on your needs. Use the following command examples:
+You can install `braingeneers` with specific optional dependencies based on your needs. Use the following command examples:
 
-- Install with IoT, analysis, and data access functions (skips machine learning and lab-specific dependencies):
+- Install with machine-learning dependencies:
 
 ```bash
-pip install "braingeneers[iot,analysis,data]"
+pip install "braingeneers[ml]"
+```
+
+- Install with Hengen lab dependencies:
+
+```bash
+pip install "braingeneers[hengenlab]"
+```
+
+- Install with developer dependencies (running tests and building sphinx docs):
+
+```bash
+pip install "braingeneers[dev]"
 ```
 
 - Install with all optional dependencies:
 
 ```bash
 pip install "braingeneers[all]"
 ```
 
 ## Committing Changes to the Repo
 
-To make changes and publish them on GitHub, please refer to the [CONTRIBUTING.md](https://github.com/braingeneers/braingeneerspy/blob/development/.github/CONTRIBUTING.md) file for up-to-date guidelines.
+To make changes and publish them on GitHub, please refer to the [CONTRIBUTING.md](https://github.com/braingeneers/braingeneerspy/blob/master/.github/CONTRIBUTING.md) file for up-to-date guidelines.
 
 ## Modules and Subpackages
 
-`braingeneerspy` includes several subpackages and modules, each serving a specific purpose within the Braingeneers project:
+`braingeneers` includes several subpackages and modules, each serving a specific purpose within the Braingeneers project:
 
 - `braingeneers.analysis`: Contains code for data analysis.
 - `braingeneers.data`: Provides code for basic data access, including subpackages for handling electrophysiology, fluidics, and imaging data.
 - `braingeneers.iot`: Offers code for Internet of Things (IoT) communication, including a messaging interface.
 - `braingeneers.ml`: Contains code related to machine learning, such as a high-performance PyTorch data loader for electrophysiology data.
 - `braingeneers.utils`: Provides utility functions, including S3 access and smart file opening.
```

### Comparing `braingeneers-0.1.0/pyproject.toml` & `braingeneers-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,93 +2,80 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "braingeneers"
 authors = [
-  { name = "Braingeneers", email = "me@example.com" },
+  { name = "UCSC Braingeneers", email = "ucscgi@ucsc.edu" },
+]
+maintainers = [
+  { name = "David", email = "dfparks@ucsc.edu" },
+  { name = "Alex", email = "atspaeth@ucsc.edu" },
+  { name = "Lon", email = "lblauvel@ucsc.edu" },
 ]
 description = "Braingeneers Python utilities"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
-  "License :: OSI Approved :: BSD License",
+  "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-  "typing_extensions >=4.6; python_version<'3.11'",
-  'deprecated',
-  'requests',
-  'numpy',
-  'tenacity',
-  'boto3',
+    'awswrangler==3.*',
+    'boto3',
+    'braingeneers-smart-open==2023.10.6',
+    'deprecated',
+    'h5py',
+    'matplotlib',
+    'nptyping',
+    'numpy',
+    'paho-mqtt>=2',
+    'pandas',
+    'powerlaw',
+    'redis',
+    'requests',
+    'schedule',
+    'scipy>=1.10.0',
+    'tenacity',
+    "typing_extensions>=4.6; python_version<'3.11'",
+    'diskcache',
+    'pytz', 
+    'tzlocal'
 ]
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/braingeneers/_version.py"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [project.optional-dependencies]
 all = [
-  'braingeneers[data]',
-  'braingeneers[analysis]',
   'braingeneers[ml]',
-  'braingeneers[iot]',
-  'braingeneers[hengenlab]',
-  'braingeneers[test]',
-  'braingeneers[docs]',
-]
-data = [
-  'h5py',
-  'braingeneers-smart-open==2023.10.6',  # 'smart_open>=5.1.0',  the hash version fixes the bytes from-to range header issue.
-  'awswrangler==3.*',
-  'pandas',
-  'nptyping',
-  'paho-mqtt'
-]
-iot = [
-  'redis',
-  'schedule',
-  'paho-mqtt'
-]
-analysis = [
-  'scipy>=1.10.0',
-  'pandas',
-  'powerlaw',
-  'matplotlib',
-  # Both of these dependencies are required for read_phy_files
-  'awswrangler==3.*',
-  'braingeneers-smart-open==2023.10.6',  # 'smart_open>=5.1.0',  the hash version fixes the bytes from-to range header issue.
+  'braingeneers[dev]',
 ]
 ml = [
   'torch',
   'scikit-learn',
 ]
-hengenlab = [
-  'neuraltoolkit==0.3.1',  # channel mapping information
-]
-test = [
+dev = [
   "pytest >=6",
   "pytest-cov >=3",
-]
-docs = [
   "sphinx>=4.0",
   "myst_parser>=0.13",
   "sphinx_book_theme>=0.1.0",
   "sphinx_copybutton",
   "sphinx_autodoc_typehints",
   "furo",
 ]
```

### Comparing `braingeneers-0.1.0/PKG-INFO` & `braingeneers-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,74 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: braingeneers
-Version: 0.1.0
+Version: 0.2.0
 Summary: Braingeneers Python utilities
 Project-URL: Homepage, https://github.com/braingeneers/braingeneerspy
 Project-URL: Bug Tracker, https://github.com/braingeneers/braingeneerspy/issues
 Project-URL: Discussions, https://github.com/braingeneers/braingeneerspy/discussions
 Project-URL: Changelog, https://github.com/braingeneers/braingeneerspy/releases
-Author-email: Braingeneers <me@example.com>
+Author-email: UCSC Braingeneers <ucscgi@ucsc.edu>
+Maintainer-email: David <dfparks@ucsc.edu>, Alex <atspaeth@ucsc.edu>, Lon <lblauvel@ucsc.edu>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
+Requires-Dist: awswrangler==3.*
 Requires-Dist: boto3
+Requires-Dist: braingeneers-smart-open==2023.10.6
 Requires-Dist: deprecated
+Requires-Dist: diskcache
+Requires-Dist: h5py
+Requires-Dist: matplotlib
+Requires-Dist: nptyping
 Requires-Dist: numpy
+Requires-Dist: paho-mqtt>=2
+Requires-Dist: pandas
+Requires-Dist: powerlaw
+Requires-Dist: pytz
+Requires-Dist: redis
 Requires-Dist: requests
+Requires-Dist: schedule
+Requires-Dist: scipy>=1.10.0
 Requires-Dist: tenacity
 Requires-Dist: typing-extensions>=4.6; python_version < '3.11'
+Requires-Dist: tzlocal
 Provides-Extra: all
-Requires-Dist: braingeneers[analysis]; extra == 'all'
-Requires-Dist: braingeneers[data]; extra == 'all'
-Requires-Dist: braingeneers[docs]; extra == 'all'
-Requires-Dist: braingeneers[hengenlab]; extra == 'all'
-Requires-Dist: braingeneers[iot]; extra == 'all'
-Requires-Dist: braingeneers[ml]; extra == 'all'
-Requires-Dist: braingeneers[test]; extra == 'all'
-Provides-Extra: analysis
-Requires-Dist: awswrangler==3.*; extra == 'analysis'
-Requires-Dist: braingeneers-smart-open==2023.10.6; extra == 'analysis'
-Requires-Dist: matplotlib; extra == 'analysis'
-Requires-Dist: pandas; extra == 'analysis'
-Requires-Dist: powerlaw; extra == 'analysis'
-Requires-Dist: scipy>=1.10.0; extra == 'analysis'
-Provides-Extra: data
-Requires-Dist: awswrangler==3.*; extra == 'data'
-Requires-Dist: braingeneers-smart-open==2023.10.6; extra == 'data'
-Requires-Dist: h5py; extra == 'data'
-Requires-Dist: nptyping; extra == 'data'
-Requires-Dist: paho-mqtt; extra == 'data'
-Requires-Dist: pandas; extra == 'data'
-Provides-Extra: docs
-Requires-Dist: furo; extra == 'docs'
-Requires-Dist: myst-parser>=0.13; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
-Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'docs'
-Requires-Dist: sphinx-copybutton; extra == 'docs'
-Requires-Dist: sphinx>=4.0; extra == 'docs'
-Provides-Extra: hengenlab
-Requires-Dist: neuraltoolkit==0.3.1; extra == 'hengenlab'
-Provides-Extra: iot
-Requires-Dist: paho-mqtt; extra == 'iot'
-Requires-Dist: redis; extra == 'iot'
-Requires-Dist: schedule; extra == 'iot'
+Requires-Dist: furo; extra == 'all'
+Requires-Dist: myst-parser>=0.13; extra == 'all'
+Requires-Dist: pytest-cov>=3; extra == 'all'
+Requires-Dist: pytest>=6; extra == 'all'
+Requires-Dist: scikit-learn; extra == 'all'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'all'
+Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'all'
+Requires-Dist: sphinx-copybutton; extra == 'all'
+Requires-Dist: sphinx>=4.0; extra == 'all'
+Requires-Dist: torch; extra == 'all'
+Provides-Extra: dev
+Requires-Dist: furo; extra == 'dev'
+Requires-Dist: myst-parser>=0.13; extra == 'dev'
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest>=6; extra == 'dev'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'dev'
+Requires-Dist: sphinx-book-theme>=0.1.0; extra == 'dev'
+Requires-Dist: sphinx-copybutton; extra == 'dev'
+Requires-Dist: sphinx>=4.0; extra == 'dev'
 Provides-Extra: ml
 Requires-Dist: scikit-learn; extra == 'ml'
 Requires-Dist: torch; extra == 'ml'
-Provides-Extra: test
-Requires-Dist: pytest-cov>=3; extra == 'test'
-Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Braingeneers Python Utilities
 
 [![ssec](https://img.shields.io/badge/SSEC-Project-purple?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAOCAQAAABedl5ZAAAACXBIWXMAAAHKAAABygHMtnUxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMNJREFUGBltwcEqwwEcAOAfc1F2sNsOTqSlNUopSv5jW1YzHHYY/6YtLa1Jy4mbl3Bz8QIeyKM4fMaUxr4vZnEpjWnmLMSYCysxTcddhF25+EvJia5hhCudULAePyRalvUteXIfBgYxJufRuaKuprKsbDjVUrUj40FNQ11PTzEmrCmrevPhRcVQai8m1PRVvOPZgX2JttWYsGhD3atbHWcyUqX4oqDtJkJiJHUYv+R1JbaNHJmP/+Q1HLu2GbNoSm3Ft0+Y1YMdPSTSwQAAAABJRU5ErkJggg==&style=plastic)](https://escience.washington.edu/wetai/)
 [![MIT License](https://badgen.net/badge/license/MIT/blue)](LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/braingeneers/badge/?version=latest)](https://braingeneers.readthedocs.io/en/latest/?badge=latest)
@@ -89,51 +86,63 @@
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/braingeneers/braingeneerspy?quickstart=1)
 
 Instruction on how to contribute to this project can be found in the [CONTRIBUTION.md](https://github.com/braingeneers/braingeneerspy/blob/development/.github/CONTRIBUTING.md).
 
 ## Installation
 
-You can install `braingeneerspy` using `pip` with the following commands:
+You can install `braingeneers` using `pip` with the following commands:
 
 ### Install from PyPI (Recommended)
 
 ```bash
-pip install braingeneerspy
+pip install braingeneers
 ```
 
 ### Install from GitHub
 
 ```bash
 pip install --force-reinstall git+https://github.com/braingeneers/braingeneerspy.git
 ```
 
 ### Install with Optional Dependencies
 
-You can install `braingeneerspy` with specific optional dependencies based on your needs. Use the following command examples:
+You can install `braingeneers` with specific optional dependencies based on your needs. Use the following command examples:
 
-- Install with IoT, analysis, and data access functions (skips machine learning and lab-specific dependencies):
+- Install with machine-learning dependencies:
 
 ```bash
-pip install "braingeneers[iot,analysis,data]"
+pip install "braingeneers[ml]"
+```
+
+- Install with Hengen lab dependencies:
+
+```bash
+pip install "braingeneers[hengenlab]"
+```
+
+- Install with developer dependencies (running tests and building sphinx docs):
+
+```bash
+pip install "braingeneers[dev]"
 ```
 
 - Install with all optional dependencies:
 
 ```bash
 pip install "braingeneers[all]"
 ```
 
 ## Committing Changes to the Repo
 
-To make changes and publish them on GitHub, please refer to the [CONTRIBUTING.md](https://github.com/braingeneers/braingeneerspy/blob/development/.github/CONTRIBUTING.md) file for up-to-date guidelines.
+To make changes and publish them on GitHub, please refer to the [CONTRIBUTING.md](https://github.com/braingeneers/braingeneerspy/blob/master/.github/CONTRIBUTING.md) file for up-to-date guidelines.
 
 ## Modules and Subpackages
 
-`braingeneerspy` includes several subpackages and modules, each serving a specific purpose within the Braingeneers project:
+`braingeneers` includes several subpackages and modules, each serving a specific purpose within the Braingeneers project:
 
 - `braingeneers.analysis`: Contains code for data analysis.
 - `braingeneers.data`: Provides code for basic data access, including subpackages for handling electrophysiology, fluidics, and imaging data.
 - `braingeneers.iot`: Offers code for Internet of Things (IoT) communication, including a messaging interface.
 - `braingeneers.ml`: Contains code related to machine learning, such as a high-performance PyTorch data loader for electrophysiology data.
 - `braingeneers.utils`: Provides utility functions, including S3 access and smart file opening.
```

