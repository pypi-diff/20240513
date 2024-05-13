# Comparing `tmp/dara_components-1.9.0-py3-none-any.whl.zip` & `tmp/dara_components-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3081751 bytes, number of entries: 86
+Zip file size: 3081753 bytes, number of entries: 86
 -rw-r--r--  2.0 unx      808 b- defN 80-Jan-01 00:00 dara/components/__init__.py
 -rw-r--r--  2.0 unx     3866 b- defN 80-Jan-01 00:00 dara/components/common/__init__.py
 -rw-r--r--  2.0 unx     9487 b- defN 80-Jan-01 00:00 dara/components/common/accordion.py
 -rw-r--r--  2.0 unx     2869 b- defN 80-Jan-01 00:00 dara/components/common/anchor.py
 -rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 dara/components/common/base_component.py
 -rw-r--r--  2.0 unx     1433 b- defN 80-Jan-01 00:00 dara/components/common/bullet_list.py
 -rw-r--r--  2.0 unx     4549 b- defN 80-Jan-01 00:00 dara/components/common/button.py
@@ -77,12 +77,12 @@
 -rw-r--r--  2.0 unx     1345 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/filter_status_button.py
 -rw-r--r--  2.0 unx     8656 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/core.py
 -rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/data_preview.py
 -rw-r--r--  2.0 unx     3313 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/plotting.py
 -rw-r--r--  2.0 unx     2877 b- defN 80-Jan-01 00:00 dara/components/smart/hierarchy.py
 -rw-r--r--  2.0 unx 17002703 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
 -rw-r--r--  2.0 unx    23576 b- defN 80-Jan-01 00:00 dara/components/umd/style.css
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.9.0.dist-info/RECORD
-86 files, 17332365 bytes uncompressed, 3068577 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.9.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.9.1.dist-info/RECORD
+86 files, 17332365 bytes uncompressed, 3068579 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -240,20 +240,20 @@
 
 Filename: dara/components/umd/dara.components.umd.js
 Comment: 
 
 Filename: dara/components/umd/style.css
 Comment: 
 
-Filename: dara_components-1.9.0.dist-info/LICENSE
+Filename: dara_components-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: dara_components-1.9.0.dist-info/METADATA
+Filename: dara_components-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: dara_components-1.9.0.dist-info/WHEEL
+Filename: dara_components-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: dara_components-1.9.0.dist-info/RECORD
+Filename: dara_components-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dara_components-1.9.0.dist-info/LICENSE` & `dara_components-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dara_components-1.9.0.dist-info/METADATA` & `dara_components-1.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dara-components
-Version: 1.9.0
+Version: 1.9.1
 Summary: Components for the Dara Framework
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Patricia Jacob
 Author-email: patricia@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=3.1.0,<3.2.0)
 Requires-Dist: cai-causal-graph (>=0.3.6)
-Requires-Dist: dara-core (==1.9.0)
+Requires-Dist: dara-core (==1.9.1)
 Requires-Dist: dill (>=0.3.0,<0.4.0)
 Requires-Dist: matplotlib (>=2.0.0)
 Requires-Dist: pandas (>=1.1.0,<3.0.0)
 Requires-Dist: plotly (>=5.14.0,<5.15.0)
 Requires-Dist: scipy
 Requires-Dist: seaborn (>=0.11.0)
 Project-URL: Repository, https://github.com/causalens/dara
 Description-Content-Type: text/markdown
 
 # Dara Components
 
-<img src="https://github.com/causalens/dara/blob/VERSION-1.9.0/img/dara_light.svg?raw=true">
+<img src="https://github.com/causalens/dara/blob/VERSION-1.9.1/img/dara_light.svg?raw=true">
 
 ![Master tests](https://github.com/causalens/dara/actions/workflows/tests.yml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![NPM](https://img.shields.io/npm/v/@darajs/components.svg?color=dark-green)](https://www.npmjs.com/package/@darajs/components)
```

## Comparing `dara_components-1.9.0.dist-info/RECORD` & `dara_components-1.9.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -76,11 +76,11 @@
 dara/components/smart/data_slicer/extension/filter_status_button.py,sha256=02CgqHEBgkZg1E9v9HGrnRYvEiMNhYpajyOwGuPNV1M,1345
 dara/components/smart/data_slicer/utils/core.py,sha256=6BrmG-iwQCuwUAKQ-y9zFKLeinnzhXIaUOB58UxCYbc,8656
 dara/components/smart/data_slicer/utils/data_preview.py,sha256=OAphjMrm3F76XmJ09X7sZSeOeKqGJFwN5ooo3qcyrG4,1722
 dara/components/smart/data_slicer/utils/plotting.py,sha256=JYzdQLXdAD0A8k2W-764xUr7zN0Ri5nf3OQ2Nb_iuiY,3313
 dara/components/smart/hierarchy.py,sha256=STkgyZiVB1c6KJtcKnn1r8lnjZAIrWkTCpZ_WCyCI1c,2877
 dara/components/umd/dara.components.umd.js,sha256=7a0IhPt-swT52ZyvJeyVh7khAn6oUZm4ClPLlZs3rDI,17002703
 dara/components/umd/style.css,sha256=cvNU48TRRp73QxBrE9awB-zm3YURFnFlASafeLTNa_U,23576
-dara_components-1.9.0.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-dara_components-1.9.0.dist-info/METADATA,sha256=x8KtEfxQKaB1UK5FQDmJyTTR_lq6AQbB0Q_O4NMrjik,2710
-dara_components-1.9.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-dara_components-1.9.0.dist-info/RECORD,,
+dara_components-1.9.1.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+dara_components-1.9.1.dist-info/METADATA,sha256=81gzq6CzQLGULcJnoI6zzCluQvwpixtTjw9qZWkYsB0,2710
+dara_components-1.9.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+dara_components-1.9.1.dist-info/RECORD,,
```

