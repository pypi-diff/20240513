# Comparing `tmp/pisahkan_ktp-0.0.6.tar.gz` & `tmp/pisahkan_ktp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.0.6.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.1.6.tar", max compression
```

## Comparing `pisahkan_ktp-0.0.6.tar` & `pisahkan_ktp-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.6/LICENSE
--rwxr-xr-x   0        0        0     4280 2024-05-07 09:12:01.464028 pisahkan_ktp-0.0.6/README.md
--rwxr-xr-x   0        0        0      690 2024-05-07 09:13:17.320765 pisahkan_ktp-0.0.6/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.6/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    14550 2024-05-07 09:11:32.848560 pisahkan_ktp-0.0.6/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     4971 2024-05-13 03:45:24.672426 pisahkan_ktp-0.1.6/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-13 03:38:36.729406 pisahkan_ktp-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.1.6/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    17340 2024-05-13 03:42:21.556697 pisahkan_ktp-0.1.6/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 pisahkan_ktp-0.1.6/PKG-INFO
```

### Comparing `pisahkan_ktp-0.0.6/LICENSE` & `pisahkan_ktp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.6/README.md` & `pisahkan_ktp-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,33 +31,51 @@
 ### Installation Using Pip
 1. Installation
     ```sh
     pip install pisahkan-ktp
     ```
 ### Inference
 1. Usage
-    ```py
-    # Input ==> Image Path
-    from pisahkan_ktp.ktp_segmenter import segmenter
-
-    image_path = "./tests/sample.jpg"
-    result = segmenter(image_path)
-    print(result)
-
-    # Input ==> Numpy Array Image ==> cv2.imread(image_path)
-    from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
-
-    image_path = "./tests/sample.jpg"
-    image = cv2.imread(image_path)
-    result = segmenter_ndarray(image)
-    print(result)
-    ```
+    - Text Area
+        ```py
+        # Input ==> Image Path
+        from pisahkan_ktp.ktp_segmenter import segmenter
+
+        image_path = "./tests/sample.jpg"
+        result = segmenter(image_path)
+        print(result)
+
+        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+        from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+
+        image_path = "./tests/sample.jpg"
+        image = cv2.imread(image_path)
+        result = segmenter_ndarray(image)
+        print(result)
+        ```
+    - Pass-Photo & Signature
+        ```py
+        # Input ==> Image Path
+        from pisahkan_ktp.ktp_segmenter import getPassPhoto, getSignature
+
+        image_path = "./tests/sample.jpg"
+        result = getPassPhoto(image_path)
+        # Output Image Numpy Array
+
+        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+        from pisahkan_ktp.ktp_segmenter import getPassPhotoNdarray, getSignatureNdarray
+
+        image_path = "./tests/sample.jpg"
+        image = cv2.imread(image_path)
+        result = getPassPhotoNdarray(image)
+        # Output Image Numpy Array
+        ```
     > NOTE!!! Input image must be a clear Indonesian ID Card (KTP) no/less background noise for optimal performance
 
-3. Result
+3. Result Text Area
     ```json
     {
         "image": [originalImage],
         "provinsiArea": [segmented_provinsi_img_matrix_list],
         "nikArea": [segmented_nik_img_matrix_list],
         "detailArea": [segmented_detail_img_matrix_list],
     }
```

### Comparing `pisahkan_ktp-0.0.6/pyproject.toml` & `pisahkan_ktp-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.0.6"
+version = "0.1.6"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pisahkan_ktp-0.0.6/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.1.6/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -345,8 +345,86 @@
             "image": [originalImage],
             "provinsiArea": segmented_provinsi,
             "nikArea": segmented_nik,
             "detailArea": segmented_detail,
         }
     except Exception as e:
         # If the file does not exist, FileNotFoundError is raised
-        raise f"ERROR: {e}"
+        raise f"ERROR: {e}"
+
+def getPassPhoto(image_path):
+    assert isinstance(image_path, str), "Image Path"
+    try:
+        # Open Image
+        img = cv2.imread(image_path)
+
+        # Resize Image to Standard Preprocessing Size
+        imgResize = cv2.resize(img, (1000, 700))
+
+        # Segment Identity Card (Indonesian IC) based on Image Ratio
+        imgHeight, imgWidth = imgResize.shape[:2]
+        # Param List Note: Matrix[[y, height], [x, width]]
+        # passphoto = imgResize[int(imgHeight*0.16):, int(imgHeight*0.90):]
+        passphoto = imgResize[int(imgHeight*0.16):int(imgHeight*0.70), int(imgHeight*0.93):]
+        
+        return passphoto
+    except Exception as e:
+        print(f"ERROR: {e}")
+        return None
+
+def getSignature(image_path):
+    assert isinstance(image_path, str), "Image Path"
+    try:
+        # Open Image
+        img = cv2.imread(image_path)
+
+        # Resize Image to Standard Preprocessing Size
+        imgResize = cv2.resize(img, (1000, 700))
+
+        # Segment Identity Card (Indonesian IC) based on Image Ratio
+        imgHeight, imgWidth = imgResize.shape[:2]
+        # Param List Note: Matrix[[y, height], [x, width]]
+        signature = imgResize[int(imgHeight*0.745):, int(imgHeight*0.90):]
+        
+        return signature
+    except Exception as e:
+        print(f"ERROR: {e}")
+        return None
+
+def getPassPhotoNdarray(image):
+    assert isinstance(image, np.ndarray), "image can be ndarray type only"
+    try:
+        # Open Image
+        img = cv2.imread(image_path)
+
+        # Resize Image to Standard Preprocessing Size
+        imgResize = cv2.resize(img, (1000, 700))
+
+        # Segment Identity Card (Indonesian IC) based on Image Ratio
+        imgHeight, imgWidth = imgResize.shape[:2]
+        # Param List Note: Matrix[[y, height], [x, width]]
+        # passphoto = imgResize[int(imgHeight*0.16):, int(imgHeight*0.90):]
+        passphoto = imgResize[int(imgHeight*0.16):int(imgHeight*0.70), int(imgHeight*0.93):]
+        
+        return passphoto
+    except Exception as e:
+        print(f"ERROR: {e}")
+        return None
+
+def getSignatureNdarray(image):
+    assert isinstance(image, np.ndarray), "image can be ndarray type only"
+    try:
+        # Open Image
+        img = cv2.imread(image_path)
+
+        # Resize Image to Standard Preprocessing Size
+        imgResize = cv2.resize(img, (1000, 700))
+
+        # Segment Identity Card (Indonesian IC) based on Image Ratio
+        imgHeight, imgWidth = imgResize.shape[:2]
+        # Param List Note: Matrix[[y, height], [x, width]]
+        signature = imgResize[int(imgHeight*0.745):, int(imgHeight*0.90):]
+        
+        return signature
+    except Exception as e:
+        print(f"ERROR: {e}")
+        return None
```

### Comparing `pisahkan_ktp-0.0.6/PKG-INFO` & `pisahkan_ktp-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.0.6
+Version: 0.1.6
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: opencv-contrib-python (==4.9.0.80)
 Requires-Dist: opencv-python (==4.8.0.76)
 Requires-Dist: pythonRLSA (==1.0.0)
 Description-Content-Type: text/markdown
 
 # **PISAHKAN KTP: Indonesian ID Card (KTP) Information Segmentation**
 
@@ -51,33 +52,51 @@
 ### Installation Using Pip
 1. Installation
     ```sh
     pip install pisahkan-ktp
     ```
 ### Inference
 1. Usage
-    ```py
-    # Input ==> Image Path
-    from pisahkan_ktp.ktp_segmenter import segmenter
-
-    image_path = "./tests/sample.jpg"
-    result = segmenter(image_path)
-    print(result)
-
-    # Input ==> Numpy Array Image ==> cv2.imread(image_path)
-    from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
-
-    image_path = "./tests/sample.jpg"
-    image = cv2.imread(image_path)
-    result = segmenter_ndarray(image)
-    print(result)
-    ```
+    - Text Area
+        ```py
+        # Input ==> Image Path
+        from pisahkan_ktp.ktp_segmenter import segmenter
+
+        image_path = "./tests/sample.jpg"
+        result = segmenter(image_path)
+        print(result)
+
+        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+        from pisahkan_ktp.ktp_segmenter import segmenter_ndarray
+
+        image_path = "./tests/sample.jpg"
+        image = cv2.imread(image_path)
+        result = segmenter_ndarray(image)
+        print(result)
+        ```
+    - Pass-Photo & Signature
+        ```py
+        # Input ==> Image Path
+        from pisahkan_ktp.ktp_segmenter import getPassPhoto, getSignature
+
+        image_path = "./tests/sample.jpg"
+        result = getPassPhoto(image_path)
+        # Output Image Numpy Array
+
+        # Input ==> Numpy Array Image ==> cv2.imread(image_path)
+        from pisahkan_ktp.ktp_segmenter import getPassPhotoNdarray, getSignatureNdarray
+
+        image_path = "./tests/sample.jpg"
+        image = cv2.imread(image_path)
+        result = getPassPhotoNdarray(image)
+        # Output Image Numpy Array
+        ```
     > NOTE!!! Input image must be a clear Indonesian ID Card (KTP) no/less background noise for optimal performance
 
-3. Result
+3. Result Text Area
     ```json
     {
         "image": [originalImage],
         "provinsiArea": [segmented_provinsi_img_matrix_list],
         "nikArea": [segmented_nik_img_matrix_list],
         "detailArea": [segmented_detail_img_matrix_list],
     }
```

