# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.998.tar", last modified: Fri Oct 13 00:26:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.999.tar", last modified: Mon Oct 16 00:25:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.998.tar` & `tencentcloud-sdk-python-dnspod-3.0.999.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    61922 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   352399 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    24241 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1078 2023-10-13 00:26:43.000000 tencentcloud-sdk-python-dnspod-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    61922 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   352399 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    24241 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-10-16 00:25:54.000000 tencentcloud-sdk-python-dnspod-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.998'
+__version__ = '3.0.999'
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.999/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dnspod-3.0.999/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.998/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.999/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dnspod',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dnspod SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

