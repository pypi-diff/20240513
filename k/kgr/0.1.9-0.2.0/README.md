# Comparing `tmp/kgr-0.1.9.tar.gz` & `tmp/kgr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.9.tar", last modified: Tue May  7 22:43:42 2024, max compression
+gzip compressed data, was "kgr-0.2.0.tar", last modified: Mon May 13 15:55:40 2024, max compression
```

## Comparing `kgr-0.1.9.tar` & `kgr-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.1.9/LICENSE
--rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.1.9/README.md
--rw-r--r--   0        0        0      880 2024-05-07 22:43:42.480206 kgr-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 20:46:37.221089 kgr-0.1.9/src/kgr/__init__.py
--rw-r--r--   0        0        0       30 2024-04-13 20:46:37.221251 kgr-0.1.9/src/kgr/__main__.py
--rw-r--r--   0        0        0     9024 2024-05-07 22:02:45.239020 kgr-0.1.9/src/kgr/lib.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 kgr-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.2.0/LICENSE
+-rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.2.0/README.md
+-rw-r--r--   0        0        0      876 2024-05-13 15:55:40.880263 kgr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-05-13 11:07:57.892389 kgr-0.2.0/src/kgr/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-13 15:45:03.297572 kgr-0.2.0/src/kgr/__main__.py
+-rw-r--r--   0        0        0     3096 2024-05-13 15:49:06.693947 kgr-0.2.0/src/kgr/convert.py
+-rw-r--r--   0        0        0     3430 2024-05-13 15:49:00.117401 kgr-0.2.0/src/kgr/geocode.py
+-rw-r--r--   0        0        0     1302 2024-05-13 15:42:53.776396 kgr-0.2.0/src/kgr/lib.py
+-rw-r--r--   0        0        0     2781 2024-05-13 15:46:54.378388 kgr-0.2.0/src/kgr/prepare.py
+-rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 kgr-0.2.0/PKG-INFO
```

### Comparing `kgr-0.1.9/LICENSE` & `kgr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.9/pyproject.toml` & `kgr-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.9"
+version = "0.2.0"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
@@ -18,15 +18,15 @@
 maintainers = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
 ]
 description = "Miltitool for convert data from https://memopzk.org to Google Maps"
 readme = "README.md"
 keywords = []
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 
 [project.license]
```

### Comparing `kgr-0.1.9/PKG-INFO` & `kgr-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.9
+Version: 0.2.0
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Dmitry Luschan
         
@@ -21,15 +21,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Project-URL: Homepage, https://github.com/dluschan/kgr
 Project-URL: Repository, https://github.com/dluschan/kgr.git
 Project-URL: Issues, https://github.com/dluschan/kgr/issues
```

