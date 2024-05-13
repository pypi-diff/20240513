# Comparing `tmp/pisahkan_ktp-0.1.6.tar.gz` & `tmp/pisahkan_ktp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.1.6.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.1.7.tar", max compression
```

## Comparing `pisahkan_ktp-0.1.6.tar` & `pisahkan_ktp-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     4971 2024-05-13 03:45:24.672426 pisahkan_ktp-0.1.6/README.md
--rwxr-xr-x   0        0        0      690 2024-05-13 03:38:36.729406 pisahkan_ktp-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.1.6/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    17340 2024-05-13 03:42:21.556697 pisahkan_ktp-0.1.6/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 pisahkan_ktp-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0     4971 2024-05-13 03:45:24.672426 pisahkan_ktp-0.1.7/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-13 03:52:09.534650 pisahkan_ktp-0.1.7/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.1.7/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    17216 2024-05-13 03:52:01.904988 pisahkan_ktp-0.1.7/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 pisahkan_ktp-0.1.7/PKG-INFO
```

### Comparing `pisahkan_ktp-0.1.6/LICENSE` & `pisahkan_ktp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.1.6/README.md` & `pisahkan_ktp-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.1.6/pyproject.toml` & `pisahkan_ktp-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.1.6"
+version = "0.1.7"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pisahkan_ktp-0.1.6/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.1.7/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,17 +389,14 @@
     except Exception as e:
         print(f"ERROR: {e}")
         return None
 
 def getPassPhotoNdarray(image):
     assert isinstance(image, np.ndarray), "image can be ndarray type only"
     try:
-        # Open Image
-        img = cv2.imread(image_path)
-
         # Resize Image to Standard Preprocessing Size
         imgResize = cv2.resize(img, (1000, 700))
 
         # Segment Identity Card (Indonesian IC) based on Image Ratio
         imgHeight, imgWidth = imgResize.shape[:2]
         # Param List Note: Matrix[[y, height], [x, width]]
         # passphoto = imgResize[int(imgHeight*0.16):, int(imgHeight*0.90):]
@@ -409,17 +406,14 @@
     except Exception as e:
         print(f"ERROR: {e}")
         return None
 
 def getSignatureNdarray(image):
     assert isinstance(image, np.ndarray), "image can be ndarray type only"
     try:
-        # Open Image
-        img = cv2.imread(image_path)
-
         # Resize Image to Standard Preprocessing Size
         imgResize = cv2.resize(img, (1000, 700))
 
         # Segment Identity Card (Indonesian IC) based on Image Ratio
         imgHeight, imgWidth = imgResize.shape[:2]
         # Param List Note: Matrix[[y, height], [x, width]]
         signature = imgResize[int(imgHeight*0.745):, int(imgHeight*0.90):]
```

### Comparing `pisahkan_ktp-0.1.6/PKG-INFO` & `pisahkan_ktp-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

