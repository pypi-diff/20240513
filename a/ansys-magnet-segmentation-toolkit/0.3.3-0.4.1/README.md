# Comparing `tmp/ansys_magnet_segmentation_toolkit-0.3.3.tar.gz` & `tmp/ansys_magnet_segmentation_toolkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_magnet_segmentation_toolkit-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_magnet_segmentation_toolkit-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_magnet_segmentation_toolkit-0.3.3.tar` & `ansys_magnet_segmentation_toolkit-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1089 2024-03-05 15:29:57.961016 ansys_magnet_segmentation_toolkit-0.3.3/LICENSE
--rw-r--r--   0        0        0     3118 2024-03-05 15:29:57.961016 ansys_magnet_segmentation_toolkit-0.3.3/README.rst
--rw-r--r--   0        0        0     2290 2024-03-05 15:29:57.961016 ansys_magnet_segmentation_toolkit-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py
--rw-r--r--   0        0        0     1206 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py
--rw-r--r--   0        0        0      287 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/aedt_properties.json
--rw-r--r--   0        0        0     1749 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py
--rw-r--r--   0        0        0     1213 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/__init__.py
--rw-r--r--   0        0        0     1649 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/constants.py
--rw-r--r--   0        0        0     2416 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/logger_handler.py
--rw-r--r--   0        0        0     1905 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/models.py
--rw-r--r--   0        0        0     3257 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/multithreading_server.py
--rw-r--r--   0        0        0     5402 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/rest_api.py
--rw-r--r--   0        0        0     3395 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/thread_manager.py
--rw-r--r--   0        0        0    26936 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/toolkit.py
--rw-r--r--   0        0        0      345 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common_properties.json
--rw-r--r--   0        0        0     2615 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py
--rw-r--r--   0        0        0     3608 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/rest_api.py
--rw-r--r--   0        0        0     1233 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py
--rw-r--r--   0        0        0    16992 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py
--rw-r--r--   0        0        0     6651 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py
--rw-r--r--   0        0        0     1153 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py
--rw-r--r--   0        0        0     1153 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/__init__.py
--rw-r--r--   0        0        0    18229 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/frontend_api_generic.py
--rw-r--r--   0        0        0    27763 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/frontend_ui.py
--rw-r--r--   0        0        0      113 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/general_properties.json
--rw-r--r--   0        0        0    35360 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/images/logo_cropped.png
--rw-r--r--   0        0        0     2410 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/logger_handler.py
--rw-r--r--   0        0        0     1923 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/models.py
--rw-r--r--   0        0        0     4727 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/thread_manager.py
--rw-r--r--   0        0        0    27061 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/toolkit.ui
--rw-r--r--   0        0        0     4797 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_actions.py
--rw-r--r--   0        0        0    10219 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_api.py
--rw-r--r--   0        0        0     1525 2024-03-05 15:29:57.965016 ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/utils.py
--rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 ansys_magnet_segmentation_toolkit-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-13 08:02:46.757867 ansys_magnet_segmentation_toolkit-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3174 2024-05-13 08:02:46.757867 ansys_magnet_segmentation_toolkit-0.4.1/README.rst
+-rw-r--r--   0        0        0     1711 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1234 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/aedt_properties.toml
+-rw-r--r--   0        0        0     1949 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py
+-rw-r--r--   0        0        0     2986 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/models.py
+-rw-r--r--   0        0        0     3791 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py
+-rw-r--r--   0        0        0     1233 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py
+-rw-r--r--   0        0        0    17731 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py
+-rw-r--r--   0        0        0     4100 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/run_toolkit.py
+-rw-r--r--   0        0        0     1153 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py
+-rw-r--r--   0        0        0    11628 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py
+-rw-r--r--   0        0        0     1219 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_properties.toml
+-rw-r--r--   0        0        0     2471 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/models.py
+-rw-r--r--   0        0        0     7558 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/run_frontend.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.py
+-rw-r--r--   0        0        0     1961 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_column.ui
+-rw-r--r--   0        0        0     6616 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_menu.py
+-rw-r--r--   0        0        0     2958 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.py
+-rw-r--r--   0        0        0     2125 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/plot_design/plot_design_page.ui
+-rw-r--r--   0        0        0     2536 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.py
+-rw-r--r--   0        0        0     1967 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_column.ui
+-rw-r--r--   0        0        0    10286 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_menu.py
+-rw-r--r--   0        0        0     5658 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.py
+-rw-r--r--   0        0        0     5227 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/post_processing/post_processing_page.ui
+-rw-r--r--   0        0        0     1153 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.py
+-rw-r--r--   0        0        0     1963 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_column.ui
+-rw-r--r--   0        0        0    15672 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_menu.py
+-rw-r--r--   0        0        0    15823 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.py
+-rw-r--r--   0        0        0    16820 2024-05-13 08:02:46.765868 ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ansys_magnet_segmentation_toolkit-0.4.1/PKG-INFO
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/LICENSE` & `ansys_magnet_segmentation_toolkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/README.rst` & `ansys_magnet_segmentation_toolkit-0.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Magnet Segmentation Toolkit
-===========================
+Magnet Segmentation ToolkitBackend
+==================================
 
 |pyansys| |PythonVersion| |GH-CI| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
@@ -18,39 +18,39 @@
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
   :target: https://github.com/psf/black
   :alt: black
 
 .. reuse_start
 
-The Magnet Segmentation Toolkit is a Python wrapper for automating the segmentation
+The Magnet Segmentation ToolkitBackend is a Python wrapper for automating the segmentation
 and skew of interior permanent magnet (IPM) and surface permanent magnet (SPM)
 motors using Ansys Electronics Desktop (AEDT). You can launch this toolkit
 from the AEDT UI or launch it directly from a Python console.
 
 Requirements
 ~~~~~~~~~~~~
 In addition to the runtime dependencies listed in
 `Getting started <https://magnet.segmentation.toolkit.docs.pyansys.com/version/stable/Getting_started.html>`_,
-the Magnet Segmentation Toolkit requires AEDT 2023 R1 or later. This toolkit also supports the AEDT
+the Magnet Segmentation ToolkitBackend requires AEDT 2023 R1 or later. This toolkit also supports the AEDT
 Student Version for 2023 R1 or later.
 
 Documentation and issues
 ~~~~~~~~~~~~~~~~~~~~~~~~
-Documentation for the latest stable release of the Magnet Segmentation Toolkit is hosted at
-`Magnet Segmentation Toolkit documentation <https://magnet.segmentation.toolkit.docs.pyansys.com/version/stable/index.html>`_.
+Documentation for the latest stable release of the Magnet Segmentation ToolkitBackend is hosted at
+`Magnet Segmentation ToolkitBackend documentation <https://magnet.segmentation.toolkit.docs.pyansys.com/version/stable/index.html>`_.
 
 In the upper right corner of the documentation's title bar, there is an option for switching from
 viewing the documentation for the latest stable release to viewing the documentation for the
 development version or previously released versions.
 
-On the `Magnet Segmentation Toolkit Issues <https://github.com/ansys/magnet-segmentation-toolkit/issues>`_
+On the `Magnet Segmentation ToolkitBackend Issues <https://github.com/ansys/magnet-segmentation-toolkit/issues>`_
 page, you can create issues to report bugs and request new features. On the `Discussions <https://discuss.ansys.com/>`_
 page on the Ansys Developer portal, you can post questions, share ideas, and get community feedback.
 
 License
 ~~~~~~~
-The Magnet Segmentation Toolkit is licensed under the MIT license.
+The Magnet Segmentation ToolkitBackend is licensed under the MIT license.
 
 This toolkit makes no commercial claim over Ansys whatsoever. The use of this toolkit
 requires a legally licensed copy of AEDT. For more information, see the
 `Ansys Electronics <https://www.ansys.com/products/electronics>`_ page on the Ansys website.
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Toolkit dedicated to magnet segmentation.
+ToolkitBackend dedicated to magnet segmentation.
 """
 
-__version__ = "0.3.3"
+__version__ = "0.4.1"
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-"""
-Magnet Segmentation Toolkit backend module.
-"""
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from ansys.aedt.toolkits.common.backend.api import AEDTCommon
+
+from ansys.aedt.toolkits.magnet_segmentation.backend.models import properties
 from ansys.aedt.toolkits.magnet_segmentation.backend.workflows.aedt import AEDTWorkflow
 
 
-class Toolkit(AEDTWorkflow):
+class ToolkitBackend(AEDTWorkflow, AEDTCommon):
     """Provides methods for controlling the toolkit workflow.
 
     This class provides methods for creating an AEDT session, connecting to an existing
     AEDT session, and automating the segmentation and skew of a 3D motor model.
 
     Examples
     --------
-    >>> from ansys.aedt.toolkits.magnet_segmentation.backend.api import Toolkit
-    >>> import time
-    >>> toolkit = Toolkit()
+    >>> from ansys.aedt.toolkits.magnet_segmentation.backend.api import ToolkitBackend
+    >>> toolkit = ToolkitBackend()
     >>> toolkit.launch_aedt()
     """
 
     def __init__(self):
+        AEDTCommon.__init__(self, properties)
         super().__init__()
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,11 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-"""
-Magnet Segmentation Toolkit backend common module.
-"""
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/common/constants.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,27 +16,11 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""Backend constants.
 """
-
-
-# Mapping from name to its associated AEDT application
-NAME_TO_AEDT_APP = {
-    "Circuit Design": "Circuit",
-    "HFSS": "Hfss",
-    "EMIT": "Emit",
-    "HFSS 3D Layout Design": "Hfss3dLayout",
-    "Icepak": "Icepak",
-    "Maxwell 2D": "Maxwell2d",
-    "Maxwell 3D": "Maxwell3d",
-    "Maxwell Circuit": "MaxwellCircuit",
-    "2D Extractor": "Q2d",
-    "Q3D Extractor": "Q3d",
-    "RMxprt": "Rmxprt",
-    "Twin Builder": "Simplorer",
-    "Mechanical": "Mechanical",
-}
+Modules extending the toolkit workflow.
+By default it focuses on aedt.
+"""
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/rest_api.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/run_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,88 +16,95 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from ansys.aedt.toolkits.magnet_segmentation.backend.api import Toolkit
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.multithreading_server import MultithreadingServer
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.rest_api import app
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.rest_api import jsonify
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.rest_api import logger
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.rest_api import settings
+from ansys.aedt.toolkits.common.backend.multithreading_server import MultithreadingServer
+from ansys.aedt.toolkits.common.backend.rest_api import app
+from ansys.aedt.toolkits.common.backend.rest_api import jsonify
+from ansys.aedt.toolkits.common.backend.rest_api import logger
+from api import ToolkitBackend
 
-service = Toolkit()
+toolkit_api = ToolkitBackend()
 
 
-# Toolkit entrypoints
+# ToolkitBackend entrypoints
 
 
 @app.route("/project_materials", methods=["GET"])
 def get_materials():
     logger.info("[GET] /Get project materials.")
 
-    response = service._get_project_materials()
+    response = toolkit_api._get_project_materials()
     if response:
         return response
     else:
         return jsonify("Get project material was unsuccessful."), 500
 
 
+@app.route("/design_setups", methods=["GET"])
+def get_design_setups():
+    logger.info("[GET] /Get design setups.")
+
+    response = toolkit_api._get_design_setup_names()
+    if response:
+        return response
+    else:
+        return jsonify("Get design setups was unsuccessful."), 500
+
+
 @app.route("/apply_segmentation", methods=["POST"])
 def magnets_segmentation():
     logger.info("[POST] /Apply magnets segmentation.")
 
-    response = service.segmentation()
+    response = toolkit_api.segmentation()
     if response:
         return (
             jsonify("Magnets segmentation applied successfully."),
             200,
         )
     else:
         return jsonify("Failure: Magnets segmentation application was unsuccessful."), 500
 
 
 @app.route("/apply_skew", methods=["POST"])
 def apply_skew():
     logger.info("[POST] /Apply skew.")
 
-    response = service.apply_skew()
+    response = toolkit_api.apply_skew()
     if response:
         return (
             jsonify("Skew angle applied successfully."),
             200,
         )
     else:
         return jsonify("Failure: Skew angle application was unsuccessful."), 500
 
 
 @app.route("/validate_analyze", methods=["POST"])
 def analyze_model():
     logger.info("[POST] /Validate and analyze AEDT model.")
 
-    response = service.validate_and_analyze()
+    response = toolkit_api.validate_and_analyze()
     if response:
         return jsonify("AEDT model analyzed successfully."), 200
     else:
         return jsonify("Failure: AEDT model analysis was unsuccessful."), 500
 
 
 @app.route("/magnet_loss", methods=["GET"])
 def get_magnet_loss():
     logger.info("[GET] /Get magnet loss.")
 
-    response = service.get_magnet_loss()
-    if response[0]:
-        return (
-            jsonify(response[1]),
-            200,
-        )
+    response = toolkit_api.get_magnet_loss()
+    if response:
+        return jsonify("Magnet Loss (avg)[W] = {}".format(response["SolidLoss"]["Value"])), 200
     else:
         return jsonify("Failure: Magnet loss calculation was unsuccessful."), 500
 
 
 if __name__ == "__main__":
-    app.debug = True
+    app.debug = toolkit_api.properties.debug
     server = MultithreadingServer()
-    server.run(host=settings["url"], port=settings["port"], app=app)
+    server.run(host=toolkit_api.properties.url, port=toolkit_api.properties.port, app=app)
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/__init__.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,10 +17,9 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Modules extending the toolkit workflow.
-By default it focuses on aedt.
+Magnet Segmentation ToolkitBackend backend module.
 """
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/backend/workflows/aedt.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,43 +18,44 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from operator import attrgetter
 
+from ansys.aedt.toolkits.common.backend.api import AEDTCommon
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import unit_converter
 from pyaedt.modeler.cad.Modeler import CoordinateSystem
 from pyaedt.modeler.cad.Modeler import FaceCoordinateSystem
 from pyaedt.modeler.geometry_operators import GeometryOperators as go
 
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.toolkit import AEDTCommonToolkit
 from ansys.aedt.toolkits.magnet_segmentation.backend.models import properties
 
 
-class AEDTWorkflow(AEDTCommonToolkit):
+class AEDTWorkflow(AEDTCommon):
     """Controls the AEDT toolkit workflow.
 
     This class provides methods for connecting to a selected design,
     segment and skew the motor.
 
     Examples
     --------
-        >>> from ansys.aedt.toolkits.magnet_segmentation.backend.api import Toolkit
-        >>> toolkit = Toolkit()
+        >>> from ansys.aedt.toolkits.magnet_segmentation.backend.api import AEDTWorkflow
+        >>> toolkit = AEDTWorkflow()
         >>> msg1 = toolkit.launch_aedt()
         >>> toolkit.wait_to_be_idle()
         >>> toolkit.segmentation()
         >>> toolkit.apply_skew()
         >>> toolkit.release_aedt(True, True)
     """
 
     def __init__(self):
-        super().__init__()
+        AEDTCommon.__init__(self, properties)
+        self.properties = properties
 
     # @thread.launch_thread
     def segmentation(self):
         """Apply object segmentation.
 
         This method automatically segments the rotor, rotor pockets, and magnets.
 
@@ -63,65 +64,65 @@
             ``SymmetryFactor`` and ``HalfAxial`` design settings defined.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
-        self.connect_design(app_name=list(properties.active_design.keys())[0])
+        self.connect_design()
 
         # Requirements: Design needs  a design variable "HalfAxial"
         if self.aedtapp["HalfAxial"] == "1":
             self.aedtapp["HalfAxial"] = "0"
 
         for obj in self.aedtapp.modeler.unclassified_objects:
             obj.model = False
 
-        self.aedtapp.set_active_design(properties.active_design["Maxwell3d"])
-        self.aedtapp.duplicate_design(properties.active_design["Maxwell3d"])
-        properties.active_design = {"Maxwell3d": self.aedtapp.design_name}
-        self.aedtapp.set_active_design(properties.active_design["Maxwell3d"])
-        properties.designs_by_project_name[self.aedtapp.project_name].append(properties.active_design)
-        self.set_properties(properties.model_dump())
+        self.aedtapp.set_active_design(self.properties.active_design)
+        self.aedtapp.duplicate_design(self.properties.active_design)
+        self.properties.active_design = self.aedtapp.design_name
+        self.aedtapp.set_active_design(self.properties.active_design)
+        self.properties.design_list[self.aedtapp.project_name].append(self.properties.active_design)
+        self.set_properties(self.properties.model_dump())
 
         # try:
         if [bound for bound in self.aedtapp.boundaries if bound.type == "Insulating"]:
             for bound in self.aedtapp.boundaries[:]:
                 if (
                     bound.type == "Insulating"
                     and bound.name in self.aedtapp.odesign.GetChildObject("Boundaries").GetChildNames()
                 ):
                     bound.delete()
 
         vacuum_objects = [x for x in self.aedtapp.modeler.get_objects_by_material("vacuum") if x.object_type == "Solid"]
         rotor_pockets = self._get_rotor_pockets(vacuum_objects)
 
         # If model is already skewed only magnets can be segmented
-        if not properties.is_skewed:
-            magnets = self.aedtapp.modeler.get_objects_by_material(properties.magnets_material)
-            if properties.rotor_material == properties.stator_material:
-                if properties.motor_type == "IPM":
-                    for obj in self.aedtapp.modeler.get_objects_by_material(properties.rotor_material):
+        if not self.properties.is_skewed:
+            magnets = self.aedtapp.modeler.get_objects_by_material(self.properties.magnets_material)
+            if self.properties.rotor_material == self.properties.stator_material:
+                if self.properties.motor_type == "IPM":
+                    for obj in self.aedtapp.modeler.get_objects_by_material(self.properties.rotor_material):
                         if [i for i in magnets if i in self.aedtapp.modeler.objects_in_bounding_box(obj.bounding_box)]:
                             rotor = obj
-                elif properties.motor_type == "SPM":
-                    for obj in self.aedtapp.modeler.get_objects_by_material(properties.rotor_material):
+                elif self.properties.motor_type == "SPM":
+                    for obj in self.aedtapp.modeler.get_objects_by_material(self.properties.rotor_material):
                         if not [
                             i for i in magnets if i in self.aedtapp.modeler.objects_in_bounding_box(obj.bounding_box)
                         ]:
                             rotor = obj
                 else:
-                    raise RuntimeError(f"Motor type {properties.motor_type} is not yet handled.")
+                    raise RuntimeError(f"Motor type {self.properties.motor_type} is not yet handled.")
             else:
-                rotor = self.aedtapp.modeler.get_objects_by_material(properties.rotor_material)[0]
+                rotor = self.aedtapp.modeler.get_objects_by_material(self.properties.rotor_material)[0]
 
-            if properties.rotor_slices > 1:
+            if self.properties.rotor_slices > 1:
                 # rotor segmentation
                 rotor_slices = self.aedtapp.modeler.objects_segmentation(
-                    rotor.id, segments_number=properties.rotor_slices, apply_mesh_sheets=False
+                    rotor.id, segments_number=self.properties.rotor_slices, apply_mesh_sheets=False
                 )
                 # rotor and rotor pockets split
                 rotor_objs = [rotor.name]
                 magnets_names = [x.name for x in magnets]
                 if len(rotor_pockets) > 0:
                     rotor_pockets_names = [x.name for x in rotor_pockets]
                 for slice in rotor_slices[rotor.name]:
@@ -130,43 +131,51 @@
                     if len(rotor_pockets) > 0:
                         rotor_pockets_names = self.aedtapp.modeler.split(
                             rotor_pockets_names, sides="Both", tool=slice.faces[0]
                         )
                     self.aedtapp.modeler.delete_objects_containing(slice.name)
                 rotor_slices.clear()
 
-        magnets = self.aedtapp.modeler.get_objects_by_material(properties.magnets_material)
+        magnets = self.aedtapp.modeler.get_objects_by_material(self.properties.magnets_material)
         for magnet in magnets:
+            faces = []
+            mesh_sheets = []
             cs = self.aedtapp.modeler.duplicate_coordinate_system_to_global(magnet.part_coordinate_system)
             magnet.part_coordinate_system = cs.name
             self.aedtapp.modeler.set_working_coordinate_system("Global")
             objects_segmentation = self.aedtapp.modeler.objects_segmentation(
                 magnet.id,
-                segments_number=properties.magnet_segments_per_slice,
-                apply_mesh_sheets=properties.apply_mesh_sheets,
-                mesh_sheets_number=properties.mesh_sheets_number,
+                segments_number=self.properties.magnet_segments_per_slice,
+                apply_mesh_sheets=self.properties.apply_mesh_sheets,
+                mesh_sheets_number=self.properties.mesh_sheets_number,
             )
-            faces = []
-            if properties.apply_mesh_sheets:
+            if self.properties.apply_mesh_sheets:
                 magnet_segments = objects_segmentation[0]
+                mesh_sheets.extend([s.name for s in objects_segmentation[1][magnet.name]])
             else:
                 magnet_segments = objects_segmentation
             for face in magnet_segments[magnet.name]:
                 obj = self.aedtapp.modeler.create_object_from_face(face.top_face_z)
                 faces.append(obj.top_face_z)
             [face.delete() for face in magnet_segments[magnet.name]]
             self.aedtapp.assign_insulating(faces, "{}_segments".format(magnet.name))
             if isinstance(cs, CoordinateSystem):
                 self._update_cs(cs)
 
+        magnets = self.aedtapp.modeler.get_objects_by_material(self.properties.magnets_material)
+        segments = self.aedtapp.modeler.get_objects_in_group("Insulating")
+
+        self.properties.objects.extend([m.name for m in magnets])
+        self.properties.objects.extend(segments)
+        # self.properties.objects.extend(mesh_sheets)
+        self.set_properties(self.properties.model_dump())
+
         self.aedtapp.save_project()
         self.release_aedt(False, False)
         return True
-        # except:
-        #     return False
 
     # @thread.launch_thread
     def apply_skew(self):
         """Apply skew to rotor slices.
 
         .. warning::
             This method only works if the active AEDT project contains a shaft
@@ -174,18 +183,18 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         try:
-            self.connect_design(app_name=list(properties.active_design.keys())[0])
+            self.connect_design()
 
-            magnets = self.aedtapp.modeler.get_objects_by_material(properties.magnets_material)
-            rotor_objects = self.aedtapp.modeler.get_objects_by_material(properties.rotor_material)
+            magnets = self.aedtapp.modeler.get_objects_by_material(self.properties.magnets_material)
+            rotor_objects = self.aedtapp.modeler.get_objects_by_material(self.properties.rotor_material)
             # Independent and dependent boundary conditions can be assigned either to an object or an object face
             independent = [bound for bound in self.aedtapp.boundaries if bound.type == "Independent"]
             dependent = [bound for bound in self.aedtapp.boundaries if bound.type == "Dependent"]
             # If no indep. o dep. boundary are found it means that the symmetry factor is 1 -> whole motor.
             if independent or dependent:
                 bound_indep_props = independent[0].props
                 if "Objects" in bound_indep_props:
@@ -201,19 +210,19 @@
                     dep = self.aedtapp.modeler.objects[bound_dep_id]
                 elif "Faces" in bound_indep_props:
                     bound_dep_id = bound_dep_props["Faces"][0]
                     obj = [o for o in self.aedtapp.modeler.object_list for f in o.faces if f.id == bound_dep_id][0]
                     dep = [f for f in obj.faces if f.id == bound_dep_id][0]
 
             # check whether stator has same rotor material
-            if properties.rotor_material == properties.stator_material:
+            if self.properties.rotor_material == self.properties.stator_material:
                 stator_obj = max(rotor_objects, key=attrgetter("volume"))
                 rotor_objects = [
                     x
-                    for x in self.aedtapp.modeler.get_objects_by_material(properties.rotor_material)
+                    for x in self.aedtapp.modeler.get_objects_by_material(self.properties.rotor_material)
                     if x != stator_obj and x.name != "Shaft"
                 ]
             objs_in_bb = {}
             rotor_skew_ang = 0
             # rotate objects and apply skew
             for rotor_object in rotor_objects:
                 if rotor_skew_ang != 0:
@@ -233,67 +242,71 @@
                                 magnet_cs.props["ZRotationAngle"] = "{}deg".format(rotor_skew_ang)
                         self.aedtapp.modeler.set_working_coordinate_system("Global")
                         obj.rotate(cs_axis="Z", angle=rotor_skew_ang)
 
                     # It means that indep. and dep. boundaries exist -> symmetry factor != 1
                     if independent and dependent:
                         split = self.aedtapp.modeler.split(objects=rotor_object, sides="Both", tool=indep.id)
-                        if not all([self.aedtapp.modeler[o] for o in split]):
+                        if [s for s in split if s not in self.aedtapp.modeler.objects_by_name]:
                             self.aedtapp.odesign.Undo()
                         split = self.aedtapp.modeler.split(objects=rotor_object, sides="Both", tool=dep.id)
                         split_objects = [self.aedtapp.modeler.objects_by_name[obj] for obj in split]
                         # Get object with minimum volume
                         min_vol_object = min(split_objects, key=lambda x: x.volume).volume
                         # Get object whose volume is equal to min_vol_object
-                        obj_rotate = [obj for obj in split_objects if obj.volume == min_vol_object][0]
+                        obj_rotate = [obj for obj in split_objects if round(obj.volume, 4) == round(min_vol_object, 4)][
+                            0
+                        ]
                         # duplicate around z axis (-360/symmetry_multiplier)
-                        obj_rotate.rotate(cs_axis=self.aedtapp.AXIS.Z, angle=-360 / self.aedtapp.symmetry_multiplier)
+                        self.aedtapp.modeler.rotate(
+                            obj_rotate, self.aedtapp.AXIS.Z, -360 / self.aedtapp.symmetry_multiplier
+                        )
                         self.aedtapp.modeler.unite([split_objects[0], split_objects[1]])
-                rotor_skew_ang += decompose_variable_value(properties.skew_angle)[0]
+                rotor_skew_ang += decompose_variable_value(self.properties.skew_angle)[0]
 
             self.release_aedt(False, False)
             return True
         except:
             return False
 
     def validate_and_analyze(self):
         """Validate and analyze the design.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
-        self.connect_design(app_name=list(properties.active_design.keys())[0])
+        self.connect_design()
 
         if self.aedtapp.validate_simple():
-            self.aedtapp.analyze_setup(properties.setup_to_analyze, use_auto_settings=False)
-            self.aedtapp.release_desktop(False, False)
+            self.aedtapp.analyze_setup(self.properties.setup_to_analyze, use_auto_settings=False)
+            self.release_aedt(False, False)
             return True
         else:
             return False
 
     def get_magnet_loss(self):
         """Get magnet loss.
 
         Returns
         -------
         dict
             dictionary containing the average magnet loss value when successful, ``False`` when failed.
         """
-        self.connect_design(app_name=list(properties.active_design.keys())[0])
+        self.connect_design()
 
         try:
             report_dict = {}
             self.aedtapp.post.create_report(expressions="SolidLoss", plotname="Losses", primary_sweep_variable="Time")
             data = self.aedtapp.post.get_solution_data(expressions="SolidLoss", primary_sweep_variable="Time")
             avg = sum(data.data_magnitude()) / len(data.data_magnitude())
             avg = unit_converter(avg, "Power", data.units_data["SolidLoss"], "W")
             report_dict["SolidLoss"] = {"Value": round(avg, 4), "Unit": "W"}
-            self.aedtapp.release_desktop(False, False)
+            self.release_aedt(False, False)
             return report_dict
         except:
             return False
 
     def _get_rotor_pockets(self, vacuum_objects):
         """Get the rotor pockets if any.
 
@@ -352,15 +365,26 @@
             return True
         except:
             return False
 
     # @thread.launch_thread
     def _get_project_materials(self):
         """Get the project materials."""
-        self.connect_design(app_name=list(properties.active_design.keys())[0])
+        self.connect_design()
 
+        if not self.aedtapp:
+            return
         mats = self.aedtapp.materials.get_used_project_material_names()
 
-        self.aedtapp.release_desktop(False, False)
-        self.aedtapp = None
+        self.release_aedt(False, False)
 
         return mats
+
+    def _get_design_setup_names(self):
+        """Get the design setup names."""
+        self.connect_design()
+
+        setup_names = [setup.name for setup in self.aedtapp.setups]
+
+        self.release_aedt(False, False)
+
+        return setup_names
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/toolkit.ui` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui`

 * *Files 26% similar despite different names*

#### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/common/toolkit.ui` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/windows/segmentation/segmentation_page.ui`

```diff
@@ -1,816 +1,568 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>MainWindow</class>
-  <widget class="QMainWindow" name="MainWindow">
+  <class>Segmentation</class>
+  <widget class="QWidget" name="Segmentation">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>890</width>
-        <height>1178</height>
+        <width>627</width>
+        <height>456</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
     </property>
     <property name="windowTitle">
-      <string>MainWindow</string>
+      <string>Form</string>
     </property>
-    <widget class="QWidget" name="centralwidget">
-      <property name="sizePolicy">
-        <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-          <horstretch>0</horstretch>
-          <verstretch>0</verstretch>
-        </sizepolicy>
-      </property>
-      <layout class="QVBoxLayout" name="verticalLayout">
-        <item>
-          <widget class="QWidget" name="main_menu" native="true">
-            <property name="sizePolicy">
-              <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                <horstretch>0</horstretch>
-                <verstretch>0</verstretch>
-              </sizepolicy>
-            </property>
-            <layout class="QGridLayout" name="gridLayout">
-              <item row="3" column="2">
-                <widget class="QPushButton" name="release_button">
-                  <property name="minimumSize">
-                    <size>
-                      <width>0</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                  <property name="text">
-                    <string>Close Toolkit</string>
-                  </property>
-                </widget>
+    <property name="segmentation" stdset="0">
+      <rect>
+        <x>0</x>
+        <y>0</y>
+        <width>890</width>
+        <height>1178</height>
+      </rect>
+    </property>
+    <layout class="QVBoxLayout" name="verticalLayout">
+      <item>
+        <layout class="QHBoxLayout" name="horizontalLayout_">
+          <item>
+            <layout class="QVBoxLayout" name="verticalLayout_2">
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_66">
+                  <item>
+                    <widget class="QLabel" name="motor_type_combo_label">
+                      <property name="text">
+                        <string>Motor Type</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="motor_type_combo">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <property name="currentText">
+                        <string>--Select Motor Type--</string>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>--Select Motor Type--</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
               </item>
-              <item row="3" column="1">
-                <spacer name="horizontalSpacer">
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_32">
+                  <item>
+                    <widget class="QLabel" name="apply_mesh_sheets_label">
+                      <property name="text">
+                        <string>Apply Mesh Sheets</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_2">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="apply_mesh_sheets">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>False</string>
+                        </property>
+                      </item>
+                      <item>
+                        <property name="text">
+                          <string>True</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_4">
+                  <item>
+                    <widget class="QLabel" name="is_skewed_label">
+                      <property name="text">
+                        <string>Is Skewed</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_5">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="is_skewed">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>False</string>
+                        </property>
+                      </item>
+                      <item>
+                        <property name="text">
+                          <string>True</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_7">
+                  <item>
+                    <widget class="QLabel" name="magnets_material_label">
+                      <property name="text">
+                        <string>Magnet Material</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_6">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="magnets_material">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>--Select Material--</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_20">
+                  <item>
+                    <widget class="QLabel" name="rotor_material_label">
+                      <property name="text">
+                        <string>Rotor Material</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_7">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="rotor_material">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>--Select Material--</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_20a">
+                  <item>
+                    <widget class="QLabel" name="stator_material_label">
+                      <property name="text">
+                        <string>Stator Material</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_8">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QComboBox" name="stator_material">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                      <item>
+                        <property name="text">
+                          <string>--Select Material--</string>
+                        </property>
+                      </item>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_21">
+                  <item>
+                    <widget class="QLabel" name="rotor_slices_label">
+                      <property name="text">
+                        <string>Rotor Slices</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_21">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QLineEdit" name="rotor_slices">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_22">
+                  <item>
+                    <widget class="QLabel" name="magnet_segments_per_slice_label">
+                      <property name="text">
+                        <string>Magnet Segments Per Slice</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_22">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QLineEdit" name="magnet_segments_per_slice">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_33">
+                  <item>
+                    <widget class="QLabel" name="mesh_sheets_number_label">
+                      <property name="text">
+                        <string>Mesh Sheets Number</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_3">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QLineEdit" name="mesh_sheets_number">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_23">
+                  <item>
+                    <widget class="QLabel" name="skew_angle_label">
+                      <property name="text">
+                        <string>Skew Angle (deg)</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <spacer name="horizontalSpacer_23">
+                      <property name="orientation">
+                        <enum>Qt::Horizontal</enum>
+                      </property>
+                      <property name="sizeHint" stdset="0">
+                        <size>
+                          <width>40</width>
+                          <height>20</height>
+                        </size>
+                      </property>
+                    </spacer>
+                  </item>
+                  <item>
+                    <widget class="QLineEdit" name="skew_angle">
+                      <property name="sizePolicy">
+                        <sizepolicy hsizetype="Preferred" vsizetype="Expanding">
+                          <horstretch>0</horstretch>
+                          <verstretch>0</verstretch>
+                        </sizepolicy>
+                      </property>
+                      <property name="minimumSize">
+                        <size>
+                          <width>300</width>
+                          <height>0</height>
+                        </size>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </item>
+              <item>
+                <spacer name="verticalSpacer">
                   <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
+                    <enum>Qt::Vertical</enum>
+                  </property>
+                  <property name="sizeType">
+                    <enum>QSizePolicy::Maximum</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
-                      <width>40</width>
-                      <height>20</height>
+                      <width>20</width>
+                      <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
-              <item row="3" column="3">
-                <widget class="QPushButton" name="release_and_exit_button">
+              <item>
+                <widget class="QPushButton" name="perform_segmentation">
+                  <property name="enabled">
+                    <bool>true</bool>
+                  </property>
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
+                  </property>
                   <property name="minimumSize">
                     <size>
                       <width>0</width>
                       <height>40</height>
                     </size>
                   </property>
+                  <property name="maximumSize">
+                    <size>
+                      <width>16777215</width>
+                      <height>16777215</height>
+                    </size>
+                  </property>
                   <property name="text">
-                    <string>Close AEDT and Toolkit</string>
+                    <string>Perform Segmentation</string>
                   </property>
                 </widget>
               </item>
-              <item row="0" column="0" colspan="5">
-                <widget class="QTabWidget" name="toolkit_tab">
+              <item>
+                <widget class="QPushButton" name="skew">
+                  <property name="enabled">
+                    <bool>true</bool>
+                  </property>
                   <property name="sizePolicy">
-                    <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                    <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
-                  <property name="tabShape">
-                    <enum>QTabWidget::Triangular</enum>
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>40</height>
+                    </size>
                   </property>
-                  <property name="currentIndex">
-                    <number>0</number>
+                  <property name="text">
+                    <string>Apply Skew</string>
                   </property>
-                  <widget class="QWidget" name="AEDTsettings">
-                    <attribute name="title">
-                      <string>AEDT Settings</string>
-                    </attribute>
-                    <layout class="QHBoxLayout" name="horizontalLayout_25">
-                      <item>
-                        <layout class="QVBoxLayout" name="settings_layout">
-                          <item>
-                            <layout class="QHBoxLayout" name="cores_layout">
-                              <item>
-                                <widget class="QLabel" name="cores_label">
-                                  <property name="text">
-                                    <string>Number of Cores</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_30">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="numcores">
-                                  <property name="text">
-                                    <string>4</string>
-                                  </property>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="graphical_layout">
-                              <item>
-                                <widget class="QLabel" name="graphical_label">
-                                  <property name="text">
-                                    <string>Non Graphical</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="non_graphical_combo">
-                                  <item>
-                                    <property name="text">
-                                      <string>False</string>
-                                    </property>
-                                  </item>
-                                  <item>
-                                    <property name="text">
-                                      <string>True</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="aedt_version_layout">
-                              <item>
-                                <widget class="QLabel" name="version_label">
-                                  <property name="text">
-                                    <string>AEDT Version</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="aedt_version_combo"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="aedt_sessions_layout">
-                              <item>
-                                <widget class="QLabel" name="aedt_sessions_label">
-                                  <property name="text">
-                                    <string>Available AEDT Sessions</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="process_id_combo">
-                                  <item>
-                                    <property name="text">
-                                      <string>Create New Session</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="project_path_layout">
-                              <item>
-                                <widget class="QLabel" name="project_path_label">
-                                  <property name="text">
-                                    <string>Project Name</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_2">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeType">
-                                    <enum>QSizePolicy::Minimum</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="project_name"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="select_aedt_proj_layout">
-                              <item>
-                                <spacer name="horizontalSpacer_5">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QPushButton" name="browse_project">
-                                  <property name="text">
-                                    <string>Select AEDT project</string>
-                                  </property>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_5"/>
-                          </item>
-                          <item>
-                            <spacer name="verticalSpacer_8">
-                              <property name="orientation">
-                                <enum>Qt::Vertical</enum>
-                              </property>
-                              <property name="sizeHint" stdset="0">
-                                <size>
-                                  <width>20</width>
-                                  <height>40</height>
-                                </size>
-                              </property>
-                            </spacer>
-                          </item>
-                          <item>
-                            <widget class="QPushButton" name="connect_aedtapp">
-                              <property name="enabled">
-                                <bool>true</bool>
-                              </property>
-                              <property name="minimumSize">
-                                <size>
-                                  <width>0</width>
-                                  <height>40</height>
-                                </size>
-                              </property>
-                              <property name="text">
-                                <string>Launch AEDT</string>
-                              </property>
-                            </widget>
-                          </item>
-                        </layout>
-                      </item>
-                      <item>
-                        <spacer name="horizontalSpacer_29">
-                          <property name="orientation">
-                            <enum>Qt::Horizontal</enum>
-                          </property>
-                          <property name="sizeType">
-                            <enum>QSizePolicy::Preferred</enum>
-                          </property>
-                          <property name="sizeHint" stdset="0">
-                            <size>
-                              <width>40</width>
-                              <height>20</height>
-                            </size>
-                          </property>
-                        </spacer>
-                      </item>
-                    </layout>
-                  </widget>
-                  <widget class="QWidget" name="Segmentation">
-                    <attribute name="title">
-                      <string>Segmentation</string>
-                    </attribute>
-                    <layout class="QHBoxLayout" name="horizontalLayout_">
-                      <item>
-                        <layout class="QVBoxLayout" name="verticalLayout_2">
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_3">
-                              <item>
-                                <widget class="QLabel" name="projects_label_2">
-                                  <property name="text">
-                                    <string>Projects</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="projects_aedt_combo">
-                                  <property name="currentIndex">
-                                    <number>0</number>
-                                  </property>
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Project--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_6">
-                              <item>
-                                <widget class="QLabel" name="designs_label">
-                                  <property name="text">
-                                    <string>Designs</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="design_aedt_combo">
-                                  <property name="currentText">
-                                    <string>--Select Design--</string>
-                                  </property>
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Design--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_66">
-                              <item>
-                                <widget class="QLabel" name="motor_type">
-                                  <property name="text">
-                                    <string>Motor Type</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="motor_type_combo">
-                                  <property name="currentText">
-                                    <string>--Select Motor Type--</string>
-                                  </property>
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Motor Type--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_32">
-                              <item>
-                                <widget class="QLabel" name="label_19">
-                                  <property name="text">
-                                    <string>Apply Mesh Sheets</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="apply_mesh_sheets">
-                                  <item>
-                                    <property name="text">
-                                      <string>False</string>
-                                    </property>
-                                  </item>
-                                  <item>
-                                    <property name="text">
-                                      <string>True</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_4">
-                              <item>
-                                <widget class="QLabel" name="label_12">
-                                  <property name="text">
-                                    <string>Is Skewed</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="is_skewed">
-                                  <item>
-                                    <property name="text">
-                                      <string>False</string>
-                                    </property>
-                                  </item>
-                                  <item>
-                                    <property name="text">
-                                      <string>True</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_7">
-                              <item>
-                                <widget class="QLabel" name="label_13">
-                                  <property name="text">
-                                    <string>Magnets Material</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="magnets_material">
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Material--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_20">
-                              <item>
-                                <widget class="QLabel" name="label_14">
-                                  <property name="text">
-                                    <string>Rotor Material</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="rotor_material">
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Material--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_20a">
-                              <item>
-                                <widget class="QLabel" name="label_14a">
-                                  <property name="text">
-                                    <string>Stator Material</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QComboBox" name="stator_material">
-                                  <item>
-                                    <property name="text">
-                                      <string>--Select Material--</string>
-                                    </property>
-                                  </item>
-                                </widget>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_21">
-                              <item>
-                                <widget class="QLabel" name="label_15">
-                                  <property name="text">
-                                    <string>Rotor Slices</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_21">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="rotor_slices"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_22">
-                              <item>
-                                <widget class="QLabel" name="label_16">
-                                  <property name="text">
-                                    <string>Magnet Segments Per Slice</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_22">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="magnet_segments_per_slice"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_33">
-                              <item>
-                                <widget class="QLabel" name="label_20">
-                                  <property name="text">
-                                    <string>Mesh Sheets Number</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_3">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="mesh_sheets_number"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <layout class="QHBoxLayout" name="horizontalLayout_23">
-                              <item>
-                                <widget class="QLabel" name="label_17">
-                                  <property name="text">
-                                    <string>Skew Angle (deg)</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <spacer name="horizontalSpacer_23">
-                                  <property name="orientation">
-                                    <enum>Qt::Horizontal</enum>
-                                  </property>
-                                  <property name="sizeHint" stdset="0">
-                                    <size>
-                                      <width>40</width>
-                                      <height>20</height>
-                                    </size>
-                                  </property>
-                                </spacer>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="skew_angle"/>
-                              </item>
-                            </layout>
-                          </item>
-                          <item>
-                            <widget class="QPushButton" name="perform_segmentation">
-                              <property name="enabled">
-                                <bool>true</bool>
-                              </property>
-                              <property name="minimumSize">
-                                <size>
-                                  <width>0</width>
-                                  <height>40</height>
-                                </size>
-                              </property>
-                              <property name="maximumSize">
-                                <size>
-                                  <width>16777215</width>
-                                  <height>16777215</height>
-                                </size>
-                              </property>
-                              <property name="text">
-                                <string>Perform Segmentation</string>
-                              </property>
-                            </widget>
-                          </item>
-                          <item>
-                            <widget class="QPushButton" name="skew">
-                              <property name="enabled">
-                                <bool>true</bool>
-                              </property>
-                              <property name="minimumSize">
-                                <size>
-                                  <width>0</width>
-                                  <height>40</height>
-                                </size>
-                              </property>
-                              <property name="text">
-                                <string>Apply Skew</string>
-                              </property>
-                            </widget>
-                          </item>
-                        </layout>
-                      </item>
-                      <item>
-                        <spacer name="horizontalSpacer_4">
-                          <property name="orientation">
-                            <enum>Qt::Horizontal</enum>
-                          </property>
-                          <property name="sizeType">
-                            <enum>QSizePolicy::Preferred</enum>
-                          </property>
-                          <property name="sizeHint" stdset="0">
-                            <size>
-                              <width>40</width>
-                              <height>20</height>
-                            </size>
-                          </property>
-                        </spacer>
-                      </item>
-                    </layout>
-                  </widget>
-                  <widget class="QWidget" name="Post-Processing">
-                    <attribute name="title">
-                      <string>Post-Processing</string>
-                    </attribute>
-                    <widget class="QWidget" name="verticalLayoutWidget">
-                      <property name="geometry">
-                        <rect>
-                          <x>9</x>
-                          <y>9</y>
-                          <width>701</width>
-                          <height>441</height>
-                        </rect>
-                      </property>
-                      <layout class="QVBoxLayout" name="verticalLayout_3">
-                        <item>
-                          <layout class="QHBoxLayout" name="horizontalLayout">
-                            <item>
-                              <widget class="QLabel" name="label">
-                                <property name="sizePolicy">
-                                  <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                                    <horstretch>0</horstretch>
-                                    <verstretch>0</verstretch>
-                                  </sizepolicy>
-                                </property>
-                                <property name="minimumSize">
-                                  <size>
-                                    <width>0</width>
-                                    <height>0</height>
-                                  </size>
-                                </property>
-                                <property name="text">
-                                  <string>Setup to analyze</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <spacer name="horizontalSpacer_6">
-                                <property name="orientation">
-                                  <enum>Qt::Horizontal</enum>
-                                </property>
-                                <property name="sizeHint" stdset="0">
-                                  <size>
-                                    <width>40</width>
-                                    <height>20</height>
-                                  </size>
-                                </property>
-                              </spacer>
-                            </item>
-                            <item>
-                              <widget class="QLineEdit" name="setup_name"/>
-                            </item>
-                          </layout>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="validate_and_analyze">
-                            <property name="minimumSize">
-                              <size>
-                                <width>0</width>
-                                <height>40</height>
-                              </size>
-                            </property>
-                            <property name="maximumSize">
-                              <size>
-                                <width>16777215</width>
-                                <height>16777215</height>
-                              </size>
-                            </property>
-                            <property name="text">
-                              <string>Validate and Analyze</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="get_magnet_loss">
-                            <property name="minimumSize">
-                              <size>
-                                <width>0</width>
-                                <height>40</height>
-                              </size>
-                            </property>
-                            <property name="maximumSize">
-                              <size>
-                                <width>16777215</width>
-                                <height>16777215</height>
-                              </size>
-                            </property>
-                            <property name="text">
-                              <string>Get Magnet Loss</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
-                    </widget>
-                  </widget>
                 </widget>
               </item>
             </layout>
-          </widget>
-        </item>
-        <item>
-          <widget class="QPlainTextEdit" name="log_text">
-            <property name="sizePolicy">
-              <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-                <horstretch>0</horstretch>
-                <verstretch>0</verstretch>
-              </sizepolicy>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QProgressBar" name="progress_bar">
-            <property name="focusPolicy">
-              <enum>Qt::NoFocus</enum>
-            </property>
-            <property name="maximum">
-              <number>100</number>
-            </property>
-            <property name="value">
-              <number>0</number>
-            </property>
-            <property name="textVisible">
-              <bool>true</bool>
-            </property>
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-            <property name="textDirection">
-              <enum>QProgressBar::TopToBottom</enum>
-            </property>
-          </widget>
-        </item>
-      </layout>
-    </widget>
-    <widget class="QMenuBar" name="top_menu_bar">
-      <property name="geometry">
-        <rect>
-          <x>0</x>
-          <y>0</y>
-          <width>890</width>
-          <height>28</height>
-        </rect>
-      </property>
-      <property name="font">
-        <font>
-          <pointsize>12</pointsize>
-        </font>
-      </property>
-      <widget class="QMenu" name="top_menu">
-        <property name="font">
-          <font>
-            <pointsize>12</pointsize>
-          </font>
-        </property>
-        <property name="title">
-          <string>File</string>
-        </property>
-        <addaction name="action_save_project"/>
-      </widget>
-      <addaction name="top_menu"/>
-    </widget>
-    <widget class="QStatusBar" name="status_bar"/>
-    <action name="action_save_project">
-      <property name="text">
-        <string>Save project</string>
-      </property>
-    </action>
+          </item>
+          <item>
+            <spacer name="horizontalSpacer_4">
+              <property name="orientation">
+                <enum>Qt::Horizontal</enum>
+              </property>
+              <property name="sizeType">
+                <enum>QSizePolicy::Preferred</enum>
+              </property>
+              <property name="sizeHint" stdset="0">
+                <size>
+                  <width>40</width>
+                  <height>20</height>
+                </size>
+              </property>
+            </spacer>
+          </item>
+        </layout>
+      </item>
+    </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `ansys_magnet_segmentation_toolkit-0.3.3/src/ansys/aedt/toolkits/magnet_segmentation/ui/frontend_api.py` & `ansys_magnet_segmentation_toolkit-0.4.1/src/ansys/aedt/toolkits/magnet_segmentation/ui/actions.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,39 +16,43 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# import os.path
+from ansys.aedt.toolkits.common.ui.actions_generic import FrontendGeneric
+from ansys.aedt.toolkits.common.ui.logger_handler import logger
 
-from pyaedt.generic.general_methods import _to_boolean
+# import os.path
 import requests
 
-from ansys.aedt.toolkits.magnet_segmentation.backend.common.toolkit import ToolkitThreadStatus
-from ansys.aedt.toolkits.magnet_segmentation.ui.common.frontend_api_generic import FrontendGeneric
-from ansys.aedt.toolkits.magnet_segmentation.ui.common.logger_handler import logger
-from ansys.aedt.toolkits.magnet_segmentation.ui.common.models import be_properties
 
-
-class ToolkitFrontend(FrontendGeneric):
+class Frontend(FrontendGeneric):
     def __init__(self):
         FrontendGeneric.__init__(self)
 
     def check_segmentation_compatibility(self):
         """Check compatibility with segmentation call.
 
         An AEDT file is compatible with the segmentation call if it has defined
         design settings 'SymmetryFactor' and 'HalfAxial'.
         """
         SYMMETRY_FACTOR_BEGIN = "VariableProp('SymmetryFactor'"
         HALF_AXIAL_BEGIN = "VariableProp('HalfAxial'"
         found_data = {target: False for target in [SYMMETRY_FACTOR_BEGIN, HALF_AXIAL_BEGIN]}
 
+        be_properties = self.get_properties()
+        if not be_properties.active_project:
+            return
+        else:
+            with open(be_properties.active_project, "r") as file:
+                lines = file.readlines()
+            lines = [line.strip() for line in lines]
+        be_properties = self.get_properties()
         with open(be_properties.active_project, "r") as file:
             lines = file.readlines()
         lines = [line.strip() for line in lines]
 
         for line in lines:
             for target in [SYMMETRY_FACTOR_BEGIN, HALF_AXIAL_BEGIN]:
                 if line.lstrip().startswith(target):
@@ -64,175 +68,204 @@
     def check_skew_compatibility(self):
         """Check compatibility with skew call.
 
         An AEDT file is compatible with the skew call if the name of the shaft
         is 'Shaft'.
         """
         SHAFT_LINES = ["$begin 'GeometryPart'", "$begin 'Attributes'", "Name='Shaft'"]
+
+        be_properties = self.get_properties()
         with open(be_properties.active_project, "r") as file:
             lines = file.readlines()
         lines = [line.strip() for line in lines]
 
         for i in range(len(lines) - len(SHAFT_LINES) + 1):
             if lines[i : i + len(SHAFT_LINES)] == SHAFT_LINES:
                 logger.debug("Selected AEDT file is compatible with skew call")
                 return True
 
         logger.debug("Selected AEDT file is not compatible with skew call")
         return False
 
     def browse_and_check_for_aedt_project(self):
+        be_properties = self.get_properties()
         super().browse_for_aedt_project()
         segmentation_compatibility = self.check_segmentation_compatibility()
-        if not segmentation_compatibility:
+        if not segmentation_compatibility and segmentation_compatibility is not None:
             self.write_log_line(
                 f"[Warning] AEDT file '{be_properties.active_project}' is not compatible with segmentation."
             )
             self.write_log_line("Please, ensure that 'SymmetryFactor' and 'HalfAxial' are defined")
-        skew_compatibility = self.check_skew_compatibility()
-        if not skew_compatibility:
-            self.write_log_line(f"[Warning] AEDT file '{be_properties.active_project}' is not compatible with skew.")
-            self.write_log_line("Please, ensure that the name of the shaft is 'Shaft'")
-
-    def apply_segmentation(self):
-        if self.backend_busy():
-            msg = ToolkitThreadStatus.BUSY.value
-            logger.debug(msg)
-            self.write_log_line(msg)
-            return
+        elif segmentation_compatibility:
+            skew_compatibility = self.check_skew_compatibility()
+            if not skew_compatibility:
+                self.write_log_line(
+                    f"[Warning] AEDT file '{be_properties.active_project}' is not compatible with skew."
+                )
+                self.write_log_line("Please, ensure that the name of the shaft is 'Shaft'")
 
-        self.get_properties()
-        be_properties.motor_type = self.motor_type_combo.currentText()
-        be_properties.is_skewed = _to_boolean(self.is_skewed.currentText())
-        if not be_properties.is_skewed:
-            be_properties.rotor_material = self.rotor_material.currentText()
-            be_properties.stator_material = self.stator_material.currentText()
-            be_properties.rotor_slices = int(self.rotor_slices.text())
-            be_properties.skew_angle = self.skew_angle.text()
-        be_properties.apply_mesh_sheets = _to_boolean(self.apply_mesh_sheets.currentText())
-        be_properties.magnets_material = self.magnets_material.currentText()
-        be_properties.magnet_segments_per_slice = int(self.magnet_segments_per_slice.text())
-        be_properties.mesh_sheets_number = int(self.mesh_sheets_number.text())
-        # be_properties.setup_to_analyze = self.setup_to_analyze.text()
-        be_properties.active_design = {"Maxwell3d": self.design_aedt_combo.currentText()}
-        self.set_properties()
+    def apply_segmentation(self, project_selected=None, design_selected=None):
+        be_properties = self.get_properties()
+        if project_selected and design_selected:
+            for project in be_properties["project_list"]:
+                if self.get_project_name(project) == project_selected:
+                    be_properties["active_project"] = project
+                    if project_selected in list(be_properties["design_list"].keys()):
+                        designs = be_properties["design_list"][project_selected]
+                        for design in designs:
+                            if design_selected == design:
+                                be_properties["active_design"] = design
+                                break
+                    break
+        else:
+            msg = "Please load a valid AEDT project."
+            logger.info(msg)
 
-        self.update_progress(0)
+        self.set_properties(be_properties)
         try:
             segmentation_response = requests.post(self.url + "/apply_segmentation")
             if segmentation_response.ok:
-                self.find_design_names()
-                self.skew.setEnabled(True)
+                # self.find_design_names()
+                # self.skew.setEnabled(True)
                 msg = "Apply segmentation call successful"
+                logger.info(msg)
+                return True
             else:
                 msg = f"Apply segmentation call failed"
-            logger.debug(msg)
-            self.write_log_line(msg)
-            self.update_progress(100)
+                logger.error(msg)
+                return False
         except requests.exceptions.RequestException:
             logger.error("Apply segmentation call failed")
 
-    def apply_skew(self):
-        if self.backend_busy():
-            msg = ToolkitThreadStatus.BUSY.value
-            logger.debug(msg)
-            self.write_log_line(msg)
-            return
+    def apply_skew(self, project_selected=None, design_selected=None):
+        be_properties = self.get_properties()
+        if project_selected and design_selected:
+            for project in be_properties["project_list"]:
+                if self.get_project_name(project) == project_selected:
+                    be_properties["active_project"] = project
+                    if project_selected in list(be_properties["design_list"].keys()):
+                        designs = be_properties["design_list"][project_selected]
+                        for design in designs:
+                            if design_selected == design:
+                                be_properties["active_design"] = design
+                                break
+                    break
+        else:
+            msg = "Please load a valid AEDT project."
+            logger.info(msg)
+
+        self.set_properties(be_properties)
 
-        # FIXME: do we need that call ?
-        self.get_properties()
-        if be_properties.is_skewed:
+        if be_properties["is_skewed"]:
             msg = "Model is already skewed."
-            logger.debug(msg)
-            self.write_log_line(msg)
-            self.update_progress(100)
+            logger.info(msg)
             return
 
-        if be_properties.skew_angle:
-            self.update_progress(0)
+        if be_properties["skew_angle"]:
             try:
                 response = requests.post(self.url + "/apply_skew")
                 if response.ok:
-                    self.is_skewed.setCurrentText("True")
-                    msg = "Apply skew call successful"
+                    msg = "Apply skew call successful."
+                    logger.info(msg)
+                    return True
                 else:
-                    msg = "Apply skew call failed"
-                logger.debug(msg)
-                self.write_log_line(msg)
-                self.update_progress(100)
+                    msg = "Apply skew call failed."
+                    logger.error(msg)
+                    return False
             except requests.exceptions.RequestException:
-                logger.error("Apply skew call failed")
+                logger.error("Apply skew call failed.")
 
-    def val_check_and_analysis(self):
-        if self.backend_busy():
-            msg = ToolkitThreadStatus.BUSY.value
-            logger.debug(msg)
-            self.write_log_line(msg)
-            return
+    def val_check_and_analysis(self, project_selected=None, design_selected=None):
+        be_properties = self.get_properties()
+        if project_selected and design_selected:
+            for project in be_properties["project_list"]:
+                if self.get_project_name(project) == project_selected:
+                    be_properties["active_project"] = project
+                    if project_selected in list(be_properties["design_list"].keys()):
+                        designs = be_properties["design_list"][project_selected]
+                        for design in designs:
+                            if design_selected == design:
+                                be_properties["active_design"] = design
+                                break
+                    break
+        else:
+            msg = "Please load a valid AEDT project."
+            logger.info(msg)
 
-        self.get_properties()
-        # check box name setup
-        be_properties.setup_to_analyze = self.setup_name.text()
-        self.set_properties()
+        self.set_properties(be_properties)
 
         try:
             response = requests.post(self.url + "/validate_analyze")
             if response.ok:
                 msg = "Validate and analyze call successful"
+                logger.info(msg)
+                return True
             else:
                 msg = "Validate and analyze call failed"
-                logger.debug(msg)
-                self.write_log_line(msg)
-                self.update_progress(100)
+                logger.error(msg)
+                return False
         except requests.exceptions.RequestException:
             logger.error("Validate and analyze call failed")
 
-    def get_report(self):
-        if self.backend_busy():
-            msg = ToolkitThreadStatus.BUSY.value
-            logger.debug(msg)
-            self.write_log_line(msg)
-            return
+    def get_report(self, project_selected=None, design_selected=None):
+        be_properties = self.get_properties()
+        if project_selected and design_selected:
+            for project in be_properties["project_list"]:
+                if self.get_project_name(project) == project_selected:
+                    be_properties["active_project"] = project
+                    if project_selected in list(be_properties["design_list"].keys()):
+                        designs = be_properties["design_list"][project_selected]
+                        for design in designs:
+                            if design_selected == design:
+                                be_properties["active_design"] = design
+                                break
+                    break
+        else:
+            msg = "Please load a valid AEDT project."
+            logger.info(msg)
+
+        self.set_properties(be_properties)
 
         try:
             response = requests.get(self.url + "/magnet_loss")
             if response.ok:
-                msg = "Magnet loss call successful"
+                msg = "Magnet loss call successful."
+                logger.info(msg)
+                return True
             else:
-                msg = "Magnet loss call failed"
-                logger.debug(msg)
-                self.write_log_line(msg)
-                self.update_progress(100)
+                msg = "Magnet loss call failed."
+                logger.error(msg)
+                return False
         except requests.exceptions.RequestException:
-            logger.error("Magnet loss call failed")
-
-    def hide_options(self):
-        if self.is_skewed.currentText() == "True":
-            self.rotor_material.setEnabled(False)
-            self.stator_material.setEnabled(False)
-            self.rotor_slices.setEnabled(False)
-            self.skew_angle.setEnabled(False)
-        else:
-            self.rotor_material.setEnabled(True)
-            self.stator_material.setEnabled(True)
-            self.rotor_slices.setEnabled(True)
-            self.skew_angle.setEnabled(True)
+            logger.error("Magnet loss call failed.")
 
     def get_materials(self):
         try:
-            response = requests.get(self.url + "/status")
-            if response.ok and response.json() == ToolkitThreadStatus.BUSY.value:
-                self.write_log_line("Please wait, toolkit running")
-            elif response.ok and response.json() == ToolkitThreadStatus.IDLE.value:
-                self.update_progress(0)
-                response = requests.get(self.url + "/health")
-                if response.ok and response.json() == "Toolkit is not connected to AEDT.":
-                    response = requests.get(self.url + "/project_materials")
-                    if response.ok:
-                        return response.json()
+            thread_response = self.wait_thread(60)
+            if thread_response:
+                response = requests.get(self.url + "/project_materials")
+                if response.ok:
+                    msg = "Load materials call successful."
+                    logger.info(msg)
+                    return response.json()
+                else:
+                    msg = "Load materials call failed."
+                    logger.error(msg)
+                    return False
+            # else toolkit busy
+
+        except requests.exceptions.RequestException:
+            logger.error("Load materials call failed.")
+
+    def get_design_setups(self):
+        try:
+            response = requests.get(self.url + "/design_setups")
+            if response.ok:
+                msg = "Get design setups call successful."
+                logger.info(msg)
+                return response.json()
             else:
-                self.write_log_line(
-                    f"Something is wrong, either the {ToolkitThreadStatus.CRASHED.value} "
-                    f"or {ToolkitThreadStatus.UNKNOWN.value}"
-                )
+                msg = "Get design setups call failed."
+                logger.error(msg)
+                return False
         except requests.exceptions.RequestException:
-            logger.error(f"Get materials call failed")
+            logger.error("Get design setups call failed.")
```

