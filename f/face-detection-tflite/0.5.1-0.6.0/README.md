# Comparing `tmp/face-detection-tflite-0.5.1.tar.gz` & `tmp/face-detection-tflite-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face-detection-tflite-0.5.1.tar", last modified: Sat Mar 30 09:29:12 2024, max compression
+gzip compressed data, was "face-detection-tflite-0.6.0.tar", last modified: Mon May 13 21:26:32 2024, max compression
```

## Comparing `face-detection-tflite-0.5.1.tar` & `face-detection-tflite-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.187727 face-detection-tflite-0.5.1/
--rw-rw-rw-   0        0        0     1098 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      334 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4893 2024-03-30 09:29:12.187727 face-detection-tflite-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3797 2024-03-30 09:25:03.000000 face-detection-tflite-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.138767 face-detection-tflite-0.5.1/docs/
--rw-rw-rw-   0        0        0     4949 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/example-explained.md
--rw-rw-rw-   0        0        0     8818 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/example1.jpg
--rw-rw-rw-   0        0        0    12041 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/example2.jpg
--rw-rw-rw-   0        0        0    13618 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/example3.jpg
--rw-rw-rw-   0        0        0     5261 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/example4.jpg
--rw-rw-rw-   0        0        0    17441 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/eyes.jpg
--rw-rw-rw-   0        0        0    93201 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/group.jpg
--rw-rw-rw-   0        0        0    92139 2022-08-20 06:56:32.000000 face-detection-tflite-0.5.1/docs/group_photo.jpg
--rw-rw-rw-   0        0        0    64388 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/docs/portrait.jpg
--rw-rw-rw-   0        0        0    82376 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/docs/portrait_exif.jpg
--rw-rw-rw-   0        0        0    87148 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/docs/portrait_fl.jpg
--rw-rw-rw-   0        0        0    23176 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/docs/recolored.jpg
--rw-rw-rw-   0        0        0    11409 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/docs/tutorial.md
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.186721 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/
--rw-rw-rw-   0        0        0     4893 2024-03-30 09:29:12.000000 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1128 2024-03-30 09:29:12.000000 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 09:29:12.000000 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-03-30 09:29:12.000000 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 09:29:12.000000 face-detection-tflite-0.5.1/face_detection_tflite.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.152832 face-detection-tflite-0.5.1/fdlite/
--rw-rw-rw-   0        0        0     1000 2024-03-30 09:25:03.000000 face-detection-tflite-0.5.1/fdlite/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.183959 face-detection-tflite-0.5.1/fdlite/data/
--rw-rw-rw-   0        0        0    21633 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/camdb.csv
--rw-rw-rw-   0        0        0      272 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/camdb.txt
--rw-rw-rw-   0        0        0   315332 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_detection_back.tflite
--rw-rw-rw-   0        0        0   229032 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_detection_front.tflite
--rw-rw-rw-   0        0        0  1083984 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_detection_full_range.tflite
--rw-rw-rw-   0        0        0   680736 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_detection_full_range_sparse.tflite
--rw-rw-rw-   0        0        0   229032 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_detection_short_range.tflite
--rw-rw-rw-   0        0        0  2439440 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/face_landmark.tflite
--rw-rw-rw-   0        0        0  2640568 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/data/iris_landmark.tflite
--rw-rw-rw-   0        0        0      703 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-30 09:29:12.186721 face-detection-tflite-0.5.1/fdlite/examples/
--rw-rw-rw-   0        0        0        0 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/examples/__init__.py
--rw-rw-rw-   0        0        0     7276 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/examples/iris_recoloring.py
--rw-rw-rw-   0        0        0     3303 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/exif.py
--rw-rw-rw-   0        0        0    12520 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/face_detection.py
--rw-rw-rw-   0        0        0     9701 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/face_landmark.py
--rw-rw-rw-   0        0        0    21165 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/iris_landmark.py
--rw-rw-rw-   0        0        0     4620 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/nms.py
--rw-rw-rw-   0        0        0    11547 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/render.py
--rw-rw-rw-   0        0        0    13747 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/transform.py
--rw-rw-rw-   0        0        0     6567 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/fdlite/types.py
--rw-rw-rw-   0        0        0       41 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/mypy.ini
--rw-rw-rw-   0        0        0      110 2022-08-20 07:17:06.000000 face-detection-tflite-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0     1232 2024-03-30 09:29:12.188727 face-detection-tflite-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1425 2022-08-20 06:56:33.000000 face-detection-tflite-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.455131 face-detection-tflite-0.6.0/
+-rw-rw-rw-   0        0        0     1103 2024-05-13 21:01:04.000000 face-detection-tflite-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      334 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4854 2024-05-13 21:26:32.455131 face-detection-tflite-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3797 2024-03-30 09:25:03.000000 face-detection-tflite-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.430803 face-detection-tflite-0.6.0/docs/
+-rw-rw-rw-   0        0        0     4953 2024-05-13 21:21:12.000000 face-detection-tflite-0.6.0/docs/example-explained.md
+-rw-rw-rw-   0        0        0     8818 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/example1.jpg
+-rw-rw-rw-   0        0        0    12041 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/example2.jpg
+-rw-rw-rw-   0        0        0    13618 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/example3.jpg
+-rw-rw-rw-   0        0        0     5261 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/example4.jpg
+-rw-rw-rw-   0        0        0    17441 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/eyes.jpg
+-rw-rw-rw-   0        0        0    93201 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/group.jpg
+-rw-rw-rw-   0        0        0    92139 2022-08-20 06:56:32.000000 face-detection-tflite-0.6.0/docs/group_photo.jpg
+-rw-rw-rw-   0        0        0    64388 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/docs/portrait.jpg
+-rw-rw-rw-   0        0        0    82376 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/docs/portrait_exif.jpg
+-rw-rw-rw-   0        0        0    87148 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/docs/portrait_fl.jpg
+-rw-rw-rw-   0        0        0    23176 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/docs/recolored.jpg
+-rw-rw-rw-   0        0        0    11409 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/docs/tutorial.md
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.441953 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/
+-rw-rw-rw-   0        0        0     4854 2024-05-13 21:26:32.000000 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1128 2024-05-13 21:26:32.000000 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 21:26:32.000000 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-13 21:26:32.000000 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 21:26:32.000000 face-detection-tflite-0.6.0/face_detection_tflite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.445952 face-detection-tflite-0.6.0/fdlite/
+-rw-rw-rw-   0        0        0     1000 2024-05-13 21:02:51.000000 face-detection-tflite-0.6.0/fdlite/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.453131 face-detection-tflite-0.6.0/fdlite/data/
+-rw-rw-rw-   0        0        0    21633 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/camdb.csv
+-rw-rw-rw-   0        0        0      272 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/camdb.txt
+-rw-rw-rw-   0        0        0   315332 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_detection_back.tflite
+-rw-rw-rw-   0        0        0   229032 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_detection_front.tflite
+-rw-rw-rw-   0        0        0  1083984 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_detection_full_range.tflite
+-rw-rw-rw-   0        0        0   680736 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_detection_full_range_sparse.tflite
+-rw-rw-rw-   0        0        0   229032 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_detection_short_range.tflite
+-rw-rw-rw-   0        0        0  2439440 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/face_landmark.tflite
+-rw-rw-rw-   0        0        0  2640568 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/data/iris_landmark.tflite
+-rw-rw-rw-   0        0        0      703 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:26:32.454131 face-detection-tflite-0.6.0/fdlite/examples/
+-rw-rw-rw-   0        0        0        0 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/examples/__init__.py
+-rw-rw-rw-   0        0        0     7276 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/examples/iris_recoloring.py
+-rw-rw-rw-   0        0        0     3303 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/exif.py
+-rw-rw-rw-   0        0        0    12520 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/face_detection.py
+-rw-rw-rw-   0        0        0     9701 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/face_landmark.py
+-rw-rw-rw-   0        0        0    21165 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/iris_landmark.py
+-rw-rw-rw-   0        0        0     4620 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/nms.py
+-rw-rw-rw-   0        0        0    11547 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/render.py
+-rw-rw-rw-   0        0        0    13805 2024-05-13 21:18:18.000000 face-detection-tflite-0.6.0/fdlite/transform.py
+-rw-rw-rw-   0        0        0     6567 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/fdlite/types.py
+-rw-rw-rw-   0        0        0       41 2022-08-20 06:56:33.000000 face-detection-tflite-0.6.0/mypy.ini
+-rw-rw-rw-   0        0        0      110 2022-08-20 07:17:06.000000 face-detection-tflite-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1233 2024-05-13 21:26:32.456132 face-detection-tflite-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2024-05-13 21:00:44.000000 face-detection-tflite-0.6.0/setup.py
```

### Comparing `face-detection-tflite-0.5.1/LICENSE` & `face-detection-tflite-0.6.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
-Copyright © 2021 Patrick Levin
+Copyright © 2021,2024 Patrick Levin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `face-detection-tflite-0.5.1/PKG-INFO` & `face-detection-tflite-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: face-detection-tflite
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python port of Google MediaPipe Face Detection modules
 Home-page: https://github.com/patlevin/face-detection-tflite
 Author: Patrick Levin
 Author-email: vertical-pink@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/patlevin/face-detection-tflite/issues
 Keywords: AI,face-detection,tensorflow,tflite,face-landmarks,iris-detection,face-mesh
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow>=2.3
-Requires-Dist: Pillow==9.5.0
 
 # Face Detection For Python
 
 This package implements parts of Google®'s [**MediaPipe**](https://mediapipe.dev/#!) models in pure Python (with a little help from Numpy and PIL) without `Protobuf` graphs and with minimal dependencies (just [**TF Lite**](https://www.tensorflow.org/lite/api_docs) and [**Pillow**](https://python-pillow.org/)).
 
 ## Models and Examples
 
@@ -110,7 +109,9 @@
 containing `setup.py` and running
 
 ```sh
 pip install .
 ```
 
 from a shell or command prompt.
+
+
```

### Comparing `face-detection-tflite-0.5.1/README.md` & `face-detection-tflite-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/example-explained.md` & `face-detection-tflite-0.6.0/docs/example-explained.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 An initial attempt might look something like this:
 
 ```python
 ...
 left_eye = detect_iris(image, left_eye_roi)
 # isolate the iris
 iris_location, iris_size = get_iris_position_and_size(left_eye, image)
-iris = image.transform(iris_size, Image.EXTENT, data=iris_location)
+iris = image.transform(iris_size, Transform.EXTENT, data=iris_location)
 # grayscale
 iris = iris.convert('L')
 # create mask
 mask = get_iris_mask(iris_size)
 # apply color
 iris_new = ImageOps.colorize(iris, 'black', 'white', mid=(120, 210, 45))
 # paste results into image
```

### Comparing `face-detection-tflite-0.5.1/docs/example1.jpg` & `face-detection-tflite-0.6.0/docs/example1.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/example2.jpg` & `face-detection-tflite-0.6.0/docs/example2.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/example3.jpg` & `face-detection-tflite-0.6.0/docs/example3.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/example4.jpg` & `face-detection-tflite-0.6.0/docs/example4.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/eyes.jpg` & `face-detection-tflite-0.6.0/docs/eyes.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/group.jpg` & `face-detection-tflite-0.6.0/docs/group.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/group_photo.jpg` & `face-detection-tflite-0.6.0/docs/group_photo.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/portrait.jpg` & `face-detection-tflite-0.6.0/docs/portrait.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/portrait_exif.jpg` & `face-detection-tflite-0.6.0/docs/portrait_exif.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/portrait_fl.jpg` & `face-detection-tflite-0.6.0/docs/portrait_fl.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/recolored.jpg` & `face-detection-tflite-0.6.0/docs/recolored.jpg`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/docs/tutorial.md` & `face-detection-tflite-0.6.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/face_detection_tflite.egg-info/PKG-INFO` & `face-detection-tflite-0.6.0/face_detection_tflite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: face-detection-tflite
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python port of Google MediaPipe Face Detection modules
 Home-page: https://github.com/patlevin/face-detection-tflite
 Author: Patrick Levin
 Author-email: vertical-pink@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/patlevin/face-detection-tflite/issues
 Keywords: AI,face-detection,tensorflow,tflite,face-landmarks,iris-detection,face-mesh
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow>=2.3
-Requires-Dist: Pillow==9.5.0
 
 # Face Detection For Python
 
 This package implements parts of Google®'s [**MediaPipe**](https://mediapipe.dev/#!) models in pure Python (with a little help from Numpy and PIL) without `Protobuf` graphs and with minimal dependencies (just [**TF Lite**](https://www.tensorflow.org/lite/api_docs) and [**Pillow**](https://python-pillow.org/)).
 
 ## Models and Examples
 
@@ -110,7 +109,9 @@
 containing `setup.py` and running
 
 ```sh
 pip install .
 ```
 
 from a shell or command prompt.
+
+
```

### Comparing `face-detection-tflite-0.5.1/face_detection_tflite.egg-info/SOURCES.txt` & `face-detection-tflite-0.6.0/face_detection_tflite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/__init__.py` & `face-detection-tflite-0.6.0/fdlite/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from .iris_landmark import IrisIndex, IrisLandmark, IrisResults   # noqa:F401
 from .iris_landmark import eye_landmarks_to_render_data           # noqa:F401
 from .iris_landmark import iris_depth_in_mm_from_landmarks        # noqa:F401
 from .iris_landmark import iris_landmarks_to_render_data          # noqa:F401
 from .iris_landmark import iris_roi_from_face_landmarks           # noqa:F401
 
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
```

### Comparing `face-detection-tflite-0.5.1/fdlite/data/camdb.csv` & `face-detection-tflite-0.6.0/fdlite/data/camdb.csv`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_detection_back.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_detection_back.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_detection_front.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_detection_front.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_detection_full_range.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_detection_full_range.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_detection_full_range_sparse.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_detection_full_range_sparse.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_detection_short_range.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_detection_short_range.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/face_landmark.tflite` & `face-detection-tflite-0.6.0/fdlite/data/face_landmark.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/data/iris_landmark.tflite` & `face-detection-tflite-0.6.0/fdlite/data/iris_landmark.tflite`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/errors.py` & `face-detection-tflite-0.6.0/fdlite/errors.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/examples/iris_recoloring.py` & `face-detection-tflite-0.6.0/fdlite/examples/iris_recoloring.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/exif.py` & `face-detection-tflite-0.6.0/fdlite/exif.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/face_detection.py` & `face-detection-tflite-0.6.0/fdlite/face_detection.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/face_landmark.py` & `face-detection-tflite-0.6.0/fdlite/face_landmark.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/iris_landmark.py` & `face-detection-tflite-0.6.0/fdlite/iris_landmark.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/nms.py` & `face-detection-tflite-0.6.0/fdlite/nms.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/render.py` & `face-detection-tflite-0.6.0/fdlite/render.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/fdlite/transform.py` & `face-detection-tflite-0.6.0/fdlite/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021 Patrick Levin
 # SPDX-Identifier: MIT
 from enum import IntEnum
 from typing import List, Optional, Sequence, Tuple, Union
 import numpy as np
 from PIL import Image
-from PIL.Image import Image as PILImage
+from PIL.Image import Image as PILImage, Resampling, Transform, Transpose
 from fdlite import ArgumentError, CoordinateRangeError, InvalidEnumError
 from fdlite.types import BBox, Detection, ImageTensor, Landmark, Rect
 """Functions for data transformations that are used by the detection models"""
 
 
 def image_to_tensor(
     image: Union[PILImage, np.ndarray, str],
@@ -58,16 +58,16 @@
     if output_size is None:
         output_size = (int(roi.size[0]), int(roi.size[1]))
     width, height = (roi.size if keep_aspect_ratio      # type: ignore[misc]
                      else output_size)
     src_points = roi.points()
     dst_points = [(0., 0.), (width, 0.), (width, height), (0., height)]
     coeffs = _perspective_transform_coeff(src_points, dst_points)
-    roi_image = img.transform(size=(width, height), method=Image.PERSPECTIVE,
-                              data=coeffs, resample=Image.LINEAR)
+    roi_image = img.transform(size=(width, height), method=Transform.PERSPECTIVE,
+                              data=coeffs, resample=Resampling.BILINEAR)
     # free some memory - we don't need the temporary image anymore
     if img != image:
         img.close()
     pad_x, pad_y = 0., 0.
     if keep_aspect_ratio:
         # perform letterboxing if required
         out_aspect = output_size[1] / output_size[0]    # type: ignore[index]
@@ -78,19 +78,19 @@
             pad_y = (1 - roi_aspect / out_aspect) / 2
         else:
             new_width = int(roi.height / out_aspect)
             pad_x = (1 - out_aspect / roi_aspect) / 2
         if new_width != int(roi.width) or new_height != int(roi.height):
             pad_h, pad_v = int(pad_x * new_width), int(pad_y * new_height)
             roi_image = roi_image.transform(
-                size=(new_width, new_height), method=Image.EXTENT,
+                size=(new_width, new_height), method=Transform.EXTENT,
                 data=(-pad_h, -pad_v, new_width - pad_h, new_height - pad_v))
-        roi_image = roi_image.resize(output_size, resample=Image.BILINEAR)
+        roi_image = roi_image.resize(output_size, resample=Resampling.BILINEAR)
     if flip_horizontal:
-        roi_image = roi_image.transpose(method=Image.FLIP_LEFT_RIGHT)
+        roi_image = roi_image.transpose(method=Transpose.FLIP_LEFT_RIGHT)
     # finally, apply value range transform
     min_val, max_val = output_range
     tensor_data = np.asarray(roi_image, dtype=np.float32)
     tensor_data *= (max_val - min_val) / 255
     tensor_data += min_val
     return ImageTensor(tensor_data,
                        padding=(pad_x, pad_y, pad_x, pad_y),
```

### Comparing `face-detection-tflite-0.5.1/fdlite/types.py` & `face-detection-tflite-0.6.0/fdlite/types.py`

 * *Files identical despite different names*

### Comparing `face-detection-tflite-0.5.1/setup.cfg` & `face-detection-tflite-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 6163 652d 6465 7465 6374 696f   = face-detectio
 00000020: 6e2d 7466 6c69 7465 0d0a 7665 7273 696f  n-tflite..versio
-00000030: 6e20 3d20 302e 352e 310d 0a61 7574 686f  n = 0.5.1..autho
+00000030: 6e20 3d20 302e 362e 300d 0a61 7574 686f  n = 0.6.0..autho
 00000040: 7220 3d20 5061 7472 6963 6b20 4c65 7669  r = Patrick Levi
 00000050: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
 00000060: 3d20 7665 7274 6963 616c 2d70 696e 6b40  = vertical-pink@
 00000070: 7072 6f74 6f6e 6d61 696c 2e63 6f6d 0d0a  protonmail.com..
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000090: 5079 7468 6f6e 2070 6f72 7420 6f66 2047  Python port of G
 000000a0: 6f6f 676c 6520 4d65 6469 6150 6970 6520  oogle MediaPipe 
@@ -58,20 +58,21 @@
 00000390: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
 000003a0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
 000003b0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
 000003c0: 7974 686f 6e20 4d6f 6475 6c65 730d 0a0d  ython Modules...
 000003d0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 000003e0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
 000003f0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000400: 3e3d 2033 2e37 0d0a 696e 636c 7564 655f  >= 3.7..include_
+00000400: 3e3d 2033 2e38 0d0a 696e 636c 7564 655f  >= 3.8..include_
 00000410: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
 00000420: 7275 650d 0a69 6e73 7461 6c6c 5f72 6571  rue..install_req
 00000430: 7569 7265 7320 3d20 0d0a 0974 656e 736f  uires = ...tenso
 00000440: 7266 6c6f 773e 3d32 2e33 0d0a 0950 696c  rflow>=2.3...Pil
-00000450: 6c6f 773d 3d39 2e35 2e30 0d0a 0d0a 5b66  low==9.5.0....[f
-00000460: 6c61 6b65 385d 0d0a 6578 636c 7564 6520  lake8]..exclude 
-00000470: 3d20 0d0a 092e 6567 6773 2c0d 0a09 2e67  = ....eggs,....g
-00000480: 6974 2c0d 0a09 5f5f 7079 6361 6368 655f  it,...__pycache_
-00000490: 5f2c 0d0a 0962 7569 6c64 2c0d 0a09 6469  _,...build,...di
-000004a0: 7374 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  st....[egg_info]
-000004b0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000004c0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000450: 6c6f 773e 3d31 302e 332e 300d 0a0d 0a5b  low>=10.3.0....[
+00000460: 666c 616b 6538 5d0d 0a65 7863 6c75 6465  flake8]..exclude
+00000470: 203d 200d 0a09 2e65 6767 732c 0d0a 092e   = ....eggs,....
+00000480: 6769 742c 0d0a 095f 5f70 7963 6163 6865  git,...__pycache
+00000490: 5f5f 2c0d 0a09 6275 696c 642c 0d0a 0964  __,...build,...d
+000004a0: 6973 740d 0a0d 0a5b 6567 675f 696e 666f  ist....[egg_info
+000004b0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000004c0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000004d0: 0a                                       .
```

### Comparing `face-detection-tflite-0.5.1/setup.py` & `face-detection-tflite-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-Copyright © 2021 Patrick Levin
+Copyright © 2021,2024 Patrick Levin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

