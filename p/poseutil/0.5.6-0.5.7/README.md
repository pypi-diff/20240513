# Comparing `tmp/poseutil-0.5.6.tar.gz` & `tmp/poseutil-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.5.6.tar", last modified: Wed Jan 31 00:43:54 2024, max compression
+gzip compressed data, was "poseutil-0.5.7.tar", last modified: Mon May 13 00:34:38 2024, max compression
```

## Comparing `poseutil-0.5.6.tar` & `poseutil-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-01-31 00:43:54.406531 poseutil-0.5.6/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-01-31 00:43:54.406320 poseutil-0.5.6/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-01-31 00:43:54.403817 poseutil-0.5.6/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-01-31 00:43:54.000000 poseutil-0.5.6/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-01-31 00:43:54.000000 poseutil-0.5.6/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-01-31 00:43:54.000000 poseutil-0.5.6/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-01-31 00:43:54.000000 poseutil-0.5.6/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-01-31 00:43:54.000000 poseutil-0.5.6/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-01-31 00:43:54.406572 poseutil-0.5.6/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-01-31 00:43:47.000000 poseutil-0.5.6/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-01-31 00:43:54.406096 poseutil-0.5.6/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/canvas_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-01-31 00:43:24.000000 poseutil-0.5.6/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/cv_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-01-31 00:43:20.000000 poseutil-0.5.6/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    82667 2024-01-31 00:43:18.000000 poseutil-0.5.6/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-01-31 00:43:16.000000 poseutil-0.5.6/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2031 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/qt_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    16668 2024-01-31 00:42:36.000000 poseutil-0.5.6/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.705937 poseutil-0.5.7/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-13 00:34:38.705674 poseutil-0.5.7/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.701094 poseutil-0.5.7/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-05-13 00:34:38.705991 poseutil-0.5.7/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-05-13 00:30:52.000000 poseutil-0.5.7/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.705287 poseutil-0.5.7/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/canvas_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/cv_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    82667 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2276 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/qt_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19250 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/version.py
```

### Comparing `poseutil-0.5.6/setup.py` & `poseutil-0.5.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.5.6',
+    version='0.5.7',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle', 'pyqt6'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.5.6/utils/ReadFrameData.py` & `poseutil-0.5.7/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/canvas_model.py` & `poseutil-0.5.7/utils/canvas_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/common_component.py` & `poseutil-0.5.7/utils/common_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/const.py` & `poseutil-0.5.7/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/csvHelper.py` & `poseutil-0.5.7/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/cv_model.py` & `poseutil-0.5.7/utils/cv_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/cv_util.py` & `poseutil-0.5.7/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/math_util.py` & `poseutil-0.5.7/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/normarlize.py` & `poseutil-0.5.7/utils/normarlize.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/poseMeasure.py` & `poseutil-0.5.7/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/poseMeasureFormat.py` & `poseutil-0.5.7/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/pose_util.py` & `poseutil-0.5.7/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/qt_component.py` & `poseutil-0.5.7/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.6/utils/qt_model.py` & `poseutil-0.5.7/utils/qt_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,17 +35,22 @@
             print("==================================")
 
 class BaseQDialog(QDialog):
     def __init__(self, width, height, mode):
         super().__init__()
         self.mode = mode
         if mode == AppMode.normal:
-            self.monitor = QGuiApplication.primaryScreen().availableGeometry()
+            self.monitor = QGuiApplication.screens()[0].geometry()
         elif mode == AppMode.debug:
-            self.monitor = QGuiApplication.primaryScreen().availableGeometry()
+            if len(QGuiApplication.screens()) > 1:
+                self.monitor = QGuiApplication.screens()[2].geometry()
+            elif len(QGuiApplication.screens()) > 0:
+                self.monitor = QGuiApplication.screens()[1].geometry()
+            else :
+                self.monitor = QGuiApplication.screens()[0].geometry()
         self.setGeometry(self.monitor.left(), self.monitor.top(), width, height)
 
 class StoppableThread(threading.Thread):
     
     def __init__(self,  *args, **kwargs):
         super(StoppableThread, self).__init__(*args, **kwargs)
         self._stop_event = threading.Event()
```

### Comparing `poseutil-0.5.6/utils/version.py` & `poseutil-0.5.7/utils/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     for cell in range(0, int(len(data)), 4):
         unpack_data.append(struct.unpack('i', data[cell : cell+4])[0])
     return unpack_data
 
 def pop_header(data):
     casting_data = []
     header = data.pop(0)
-    if header > 2213:    
+    if header == 2213 or header == 2314:    
         width = data.pop(0)
         height = data.pop(0)
     else:
         width = 480
         height = 640
     version = get_version(f"Version{header}")()
     line = version.row_len
@@ -138,14 +138,15 @@
         if type(frame_data) is dict:
             return frame_data
         frame_data = frame_data.to_numpy()
         frame_data = np.reshape(frame_data, (-1, self.row_len))
         info_index = self.info_index
         info_data = {i: [] for i in info_index.keys()}
         for frame in frame_data:
+            print(frame)
             for key in info_index.keys():
                 if key == "pose":
                     zip_pose = frame[info_index[key][0]: info_index[key][1]]
                     zip_idx = 0
                     pose = []
                     for idx in range(33):
                         if idx in self.body_list:
@@ -280,22 +281,75 @@
                         if idx in self.body_list:
                             pose.append(Coordinate(zip_pose[zip_idx * 3], zip_pose[zip_idx * 3 + 1], zip_pose[zip_idx * 3 + 2]))
                             zip_idx += 1
                         else:
                             pose.append(Coordinate(0, 0, 0))
                     info_data[key].append(pose)
                 elif key == "mlp_label":
-                    info_data[key].append(self.mlp_kind[frame[info_index[key]]])
+                    info_data[key].append(self.mlp_kind[int(frame[info_index[key]])])
                 elif key == "lstm_label":
-                    info_data[key].append(self.lstm_kind[frame[info_index[key]]])
+                    info_data[key].append(self.lstm_kind[int(frame[info_index[key]])])
                 else:
-                    info_data[key].append(frame[info_index[key]])
+                    info_data[key].append(int(frame[info_index[key]]))
+        info_data['header'] = self.header
+        info_data['width'] = self.width
+        info_data['height'] = self.height
+        return info_data
+    
+class Version2320(Version):
+    def __init__(self):
+        super().__init__()
+        self.header = 2320
+        self.width = 480
+        self.height = 640
+        self.info_index = {"time": 0, "mlp_label": 1, "lstm_label": 2, "reps": 3, "caoching_label": 4,  "pose": (5, 74)}
+        self.row_len = 74
+        self.mlp_kind = ["UP", "MIDDLE", "DOWN"]
+        self.lstm_kind = ["EXERCISING", "RESTING"]
+        self.body_list = [
+            NOSE,
+            LEFT_SHOULDER, RIGHT_SHOULDER, LEFT_ELBOW, RIGHT_ELBOW, LEFT_WRIST, RIGHT_WRIST, 
+            LEFT_PINKY, RIGHT_PINKY, LEFT_INDEX, RIGHT_INDEX, LEFT_THUMB, RIGHT_THUMB, 
+            LEFT_HIP, RIGHT_HIP, LEFT_KNEE, RIGHT_KNEE, LEFT_ANKLE, RIGHT_ANKLE,
+            LEFT_HEEL, RIGHT_HEEL, LEFT_FOOT_INDEX, RIGHT_FOOT_INDEX]
+    def setScale(self, width, height):
+        return super().setScale(width, height)
+    def get_data(self, frame_data):
+        if type(frame_data) is dict:
+            return frame_data
+        frame_data = frame_data.to_numpy()
+        frame_data = np.reshape(frame_data, (-1, self.row_len))
+        info_index = self.info_index
+        info_data = {i: [] for i in info_index.keys()}
+        for frame in frame_data:
+            for key in info_index.keys():
+                if key == "pose":
+                    zip_pose = frame[info_index[key][0]: info_index[key][1]]
+                    zip_idx = 0
+                    pose = []
+                    for idx in range(33):
+                        if idx in self.body_list:
+                            pose.append(Coordinate(zip_pose[zip_idx * 3], zip_pose[zip_idx * 3 + 1], zip_pose[zip_idx * 3 + 2]))
+                            zip_idx += 1
+                        else:
+                            pose.append(Coordinate(0, 0, 0))
+                    info_data[key].append(pose)
+                elif key == "mlp_label":
+                    info_data[key].append(self.mlp_kind[int(frame[info_index[key]])])
+                elif key == "lstm_label":
+                    print(int(frame[info_index[key]]))
+                    info_data[key].append(self.lstm_kind[int(frame[info_index[key]])])
+                elif key == "caoching_label":
+                    info_data[key].append(int(frame[info_index[key]]))
+                else:
+                    info_data[key].append(int(frame[info_index[key]]))
         info_data['header'] = self.header
         info_data['width'] = self.width
         info_data['height'] = self.height
+        print(frame_data[1])
         return info_data
 
 # 태권도 헤더
 
 class Version9999(Version):
     def __init__(self):
         super().__init__()
```

