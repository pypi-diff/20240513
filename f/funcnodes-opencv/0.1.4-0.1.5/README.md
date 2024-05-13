# Comparing `tmp/funcnodes_opencv-0.1.4.tar.gz` & `tmp/funcnodes_opencv-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_opencv-0.1.4.tar", max compression
+gzip compressed data, was "funcnodes_opencv-0.1.5.tar", max compression
```

## Comparing `funcnodes_opencv-0.1.4.tar` & `funcnodes_opencv-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0      101 2024-04-25 11:02:08.723486 funcnodes_opencv-0.1.4/funcnodes_opencv/__init__.py
--rw-r--r--   0        0        0     2956 2024-04-24 13:09:03.909315 funcnodes_opencv-0.1.4/funcnodes_opencv/imageformat.py
--rw-r--r--   0        0        0      381 2024-04-25 11:02:00.504149 funcnodes_opencv-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.4/README.md
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-05-13 05:19:43.219778 funcnodes_opencv-0.1.5/funcnodes_opencv/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-10 03:41:57.002216 funcnodes_opencv-0.1.5/funcnodes_opencv/colormodes.py
+-rw-r--r--   0        0        0     1333 2024-05-10 09:30:00.771338 funcnodes_opencv-0.1.5/funcnodes_opencv/components.py
+-rw-r--r--   0        0        0     6490 2024-05-10 06:28:01.061816 funcnodes_opencv-0.1.5/funcnodes_opencv/filter.py
+-rw-r--r--   0        0        0     8347 2024-05-10 03:41:23.858486 funcnodes_opencv-0.1.5/funcnodes_opencv/image_operations.py
+-rw-r--r--   0        0        0     2818 2024-05-10 06:50:49.080766 funcnodes_opencv-0.1.5/funcnodes_opencv/imageformat.py
+-rw-r--r--   0        0        0     5813 2024-05-13 05:02:48.256439 funcnodes_opencv-0.1.5/funcnodes_opencv/masks.py
+-rw-r--r--   0        0        0      903 2024-05-10 09:28:17.466933 funcnodes_opencv-0.1.5/funcnodes_opencv/utils.py
+-rw-r--r--   0        0        0      404 2024-05-13 05:20:08.370239 funcnodes_opencv-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.5/README.md
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.5/PKG-INFO
```

### Comparing `funcnodes_opencv-0.1.4/funcnodes_opencv/imageformat.py` & `funcnodes_opencv-0.1.5/funcnodes_opencv/imageformat.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,27 @@
     return cv2.cvtColor(data, getattr(cv2, conv))
 
 
 class OpenCVImageFormat(NumpyImageFormat):
     def __init__(self, arr: np.ndarray, colorspace: str = "BGR"):
         if not isinstance(arr, np.ndarray):
             raise TypeError("arr must be a numpy array")
-        if arr.ndim != 3 or (arr.shape[2] != 3 and arr.shape[2] != 1):
-            raise ValueError(
-                "arr must have 3 dimensions and 3 or 1 channels in BGR format"
-            )
+
+        if arr.ndim == 2:
+            colorspace = "GRAY"
 
         if colorspace != "BGR":
             arr = _conv_colorspace(arr, colorspace, "BGR")
 
         super().__init__(arr)
 
     def get_data_copy(self) -> np.ndarray:
         return self._data.copy()
 
-    def to_to_colorspace(self, colorspace: str) -> np.ndarray:
+    def to_colorspace(self, colorspace: str) -> np.ndarray:
         return _conv_colorspace(self.data, "BGR", colorspace)
 
     def to_jpeg(self, quality=0.75) -> bytes:
         return cv2.imencode(
             ".jpg", self.data, [int(cv2.IMWRITE_JPEG_QUALITY), int(quality * 100)]
         )[1].tobytes()
```

