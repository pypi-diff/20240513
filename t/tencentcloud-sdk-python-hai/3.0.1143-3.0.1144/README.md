# Comparing `tmp/tencentcloud-sdk-python-hai-3.0.1143.tar.gz` & `tmp/tencentcloud-sdk-python-hai-3.0.1144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hai-3.0.1143.tar", last modified: Wed May  8 21:05:44 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hai-3.0.1144.tar", last modified: Mon May 13 04:52:22 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hai-3.0.1143.tar` & `tencentcloud-sdk-python-hai-3.0.1144.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/
--rw-r--r--   0 root         (0) root         (0)     4636 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10865 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/hai_client.py
--rw-r--r--   0 root         (0) root         (0)    65205 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-08 21:05:44.000000 tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/
+-rw-r--r--   0 root         (0) root         (0)    65206 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/models.py
+-rw-r--r--   0 root         (0) root         (0)    10865 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/hai_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-13 04:52:22.000000 tencentcloud-sdk-python-hai-3.0.1144/setup.py
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/PKG-INFO` & `tencentcloud-sdk-python-hai-3.0.1144/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hai
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Hai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/errorcodes.py` & `tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/hai_client.py` & `tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/hai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/hai/v20230812/models.py` & `tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/hai/v20230812/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1018,15 +1018,15 @@
 FAILED：表示操作失败
 
 注意：此字段可能返回 null，表示取不到有效值。
         :type LatestOperationState: str
         :param _CreateTime: 实例创建时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
-        :param _MaxOutBandwidth: 公网出带宽上限，默认5Mbps
+        :param _MaxOutBandwidth: 公网出带宽上限，默认10Mbps
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxOutBandwidth: str
         :param _MaxFreeTraffic: 每月免费流量，默认500G
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxFreeTraffic: str
         :param _ConfigurationEnvironment: 应用配置环境
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hai-3.0.1144/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1143'
+__version__ = '3.0.1144'
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/setup.py` & `tencentcloud-sdk-python-hai-3.0.1144/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hai',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1143"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1144"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hai SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/README.rst` & `tencentcloud-sdk-python-hai-3.0.1144/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1143/tencentcloud_sdk_python_hai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hai-3.0.1144/tencentcloud_sdk_python_hai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hai
-Version: 3.0.1143
+Version: 3.0.1144
 Summary: Tencent Cloud Hai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

