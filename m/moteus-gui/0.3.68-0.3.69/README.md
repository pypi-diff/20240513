# Comparing `tmp/moteus_gui-0.3.68-py3-none-any.whl.zip` & `tmp/moteus_gui-0.3.69-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14432 bytes, number of entries: 9
+Zip file size: 14433 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-26 18:29 moteus_gui/__init__.py
 -rw-r--r--  2.0 unx    42094 b- defN 24-Apr-30 01:49 moteus_gui/tview.py
 -rw-rw-r--  2.0 unx     5556 b- defN 24-Feb-26 18:29 moteus_gui/tview_main_window.ui
--rw-r--r--  2.0 unx      627 b- defN 24-Apr-30 11:46 moteus_gui/version.py
--rw-r--r--  2.0 unx     1077 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      731 b- defN 24-May-10 18:16 moteus_gui-0.3.68.dist-info/RECORD
-9 files, 50236 bytes uncompressed, 13164 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx      627 b- defN 24-May-13 13:20 moteus_gui/version.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-13 13:20 moteus_gui-0.3.69.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 13:20 moteus_gui-0.3.69.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-13 13:20 moteus_gui-0.3.69.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-13 13:20 moteus_gui-0.3.69.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      731 b- defN 24-May-13 13:20 moteus_gui-0.3.69.dist-info/RECORD
+9 files, 50236 bytes uncompressed, 13165 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: moteus_gui/tview_main_window.ui
 Comment: 
 
 Filename: moteus_gui/version.py
 Comment: 
 
-Filename: moteus_gui-0.3.68.dist-info/METADATA
+Filename: moteus_gui-0.3.69.dist-info/METADATA
 Comment: 
 
-Filename: moteus_gui-0.3.68.dist-info/WHEEL
+Filename: moteus_gui-0.3.69.dist-info/WHEEL
 Comment: 
 
-Filename: moteus_gui-0.3.68.dist-info/entry_points.txt
+Filename: moteus_gui-0.3.69.dist-info/entry_points.txt
 Comment: 
 
-Filename: moteus_gui-0.3.68.dist-info/top_level.txt
+Filename: moteus_gui-0.3.69.dist-info/top_level.txt
 Comment: 
 
-Filename: moteus_gui-0.3.68.dist-info/RECORD
+Filename: moteus_gui-0.3.69.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## moteus_gui/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION="0.3.68"
+VERSION="0.3.69"
```

## Comparing `moteus_gui-0.3.68.dist-info/METADATA` & `moteus_gui-0.3.69.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moteus-gui
-Version: 0.3.68
+Version: 0.3.69
 Summary: moteus brushless controller graphical user interfaces
 Home-page: https://github.com/mjbots/moteus
 Author: mjbots Robotic Systems
 Author-email: info@mjbots.com
 Keywords: moteus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `moteus_gui-0.3.68.dist-info/RECORD` & `moteus_gui-0.3.69.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 moteus_gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 moteus_gui/tview.py,sha256=IUYQOuB9dE_00bN9wB6mjE50CfaoKkXtyrMYp5CTZ2k,42094
 moteus_gui/tview_main_window.ui,sha256=q_qA1sooIWzprVT8eYAe0EH9lfu7zg-QP1diETCNFh8,5556
-moteus_gui/version.py,sha256=8rx1YUinZCom0pzbiJ3IcLDXrj5FEja3M79tr75nJJM,627
-moteus_gui-0.3.68.dist-info/METADATA,sha256=rUBEN94YcDg8VZuRIVXA0TWtpl96o_Wy14rL1KFViHU,1077
-moteus_gui-0.3.68.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-moteus_gui-0.3.68.dist-info/entry_points.txt,sha256=Y9PnhK_gNxr8CO7_POHieVaK1U_4fgu2EYoS6TyzSgk,48
-moteus_gui-0.3.68.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
-moteus_gui-0.3.68.dist-info/RECORD,,
+moteus_gui/version.py,sha256=FEYQhXwueAJ_XxxIiWQCnSdWVFCa2egsxksGzbElp7g,627
+moteus_gui-0.3.69.dist-info/METADATA,sha256=GPxwyC9bFHU4YAbtPzdXW-FlarC9ajUXdGtPMV1SnXc,1077
+moteus_gui-0.3.69.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+moteus_gui-0.3.69.dist-info/entry_points.txt,sha256=Y9PnhK_gNxr8CO7_POHieVaK1U_4fgu2EYoS6TyzSgk,48
+moteus_gui-0.3.69.dist-info/top_level.txt,sha256=oPOkXR-zpPFhGiDcbnDY6scvNqQQAXWzV7oPD_GHMns,11
+moteus_gui-0.3.69.dist-info/RECORD,,
```

