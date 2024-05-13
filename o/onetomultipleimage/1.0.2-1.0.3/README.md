# Comparing `tmp/onetomultipleimage-1.0.2.tar.gz` & `tmp/onetomultipleimage-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetomultipleimage-1.0.2.tar", last modified: Mon May 13 11:53:15 2024, max compression
+gzip compressed data, was "onetomultipleimage-1.0.3.tar", last modified: Mon May 13 15:48:45 2024, max compression
```

## Comparing `onetomultipleimage-1.0.2.tar` & `onetomultipleimage-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 11:53:15.241294 onetomultipleimage-1.0.2/
--rw-rw-rw-   0        0        0     1111 2024-05-08 08:06:24.000000 onetomultipleimage-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4936 2024-05-13 11:53:15.239302 onetomultipleimage-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4299 2024-05-13 11:43:25.000000 onetomultipleimage-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 11:53:15.213369 onetomultipleimage-1.0.2/onetomultipleimage/
--rw-rw-rw-   0        0        0        2 2024-05-08 10:12:52.000000 onetomultipleimage-1.0.2/onetomultipleimage/__init__.py
--rw-rw-rw-   0        0        0      160 2024-05-13 06:09:54.000000 onetomultipleimage-1.0.2/onetomultipleimage/apps.py
--rw-rw-rw-   0        0        0     2133 2024-05-12 17:32:17.000000 onetomultipleimage-1.0.2/onetomultipleimage/fields.py
--rw-rw-rw-   0        0        0     8353 2024-05-12 13:53:06.000000 onetomultipleimage-1.0.2/onetomultipleimage/methods.py
--rw-rw-rw-   0        0        0     3738 2024-05-12 17:32:17.000000 onetomultipleimage-1.0.2/onetomultipleimage/models.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:53:15.237304 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/
--rw-rw-rw-   0        0        0     4936 2024-05-13 11:53:15.000000 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-05-13 11:53:15.000000 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 11:53:15.000000 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-13 11:53:15.000000 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 11:53:15.000000 onetomultipleimage-1.0.2/onetomultipleimage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 11:53:15.241294 onetomultipleimage-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-13 11:53:05.000000 onetomultipleimage-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:45.327621 onetomultipleimage-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 15:48:45.327621 onetomultipleimage-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:45.327621 onetomultipleimage-1.0.3/onetomultipleimage/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/onetomultipleimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/onetomultipleimage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/onetomultipleimage/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/onetomultipleimage/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/onetomultipleimage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:48:45.327621 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 15:48:45.000000 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-13 15:48:45.000000 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:48:45.000000 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 15:48:45.000000 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 15:48:45.000000 onetomultipleimage-1.0.3/onetomultipleimage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:48:45.327621 onetomultipleimage-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-13 15:48:35.000000 onetomultipleimage-1.0.3/setup.py
```

### Comparing `onetomultipleimage-1.0.2/LICENSE` & `onetomultipleimage-1.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Ahmad Khalili
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of the "onetomultipleimage" software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Ahmad Khalili
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of the "onetomultipleimage" software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `onetomultipleimage-1.0.2/PKG-INFO` & `onetomultipleimage-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,123 @@
-Metadata-Version: 2.1
-Name: onetomultipleimage
-Version: 1.0.2
-Summary: convert one image to several sizes in django REST and django models
-Home-page: https://github.com/ahmadekhalili/onetomultipleimage
-Author: Ahmad Khalili
-Author-email: ahmadkhalili2020@gmail.com
-License: MIT
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: djangorestframework
-Requires-Dist: pillow
-Provides-Extra: jalali
-Requires-Dist: jdatetime; extra == "jalali"
-
-# onetomultipleimage
-
-onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
-
-## installation
-
-1- run: ``` pip install onetomultipleimage[jalali]```  
-
-To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
-`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
-__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
-
-2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
-after makemigrations and migrate, models will be created.
-
-
-&nbsp;
-## Serializer Field: OneToMultipleImage
-
-Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
-
-`OneToMultipleImage` arguments:
-
-- **sizes**:
-list of sizes in str. for generate original image use 'default'. required in writing.
-
-- **upload_to**:
-path in str for uploads image. required in writing.
-
-- **data**:
-it is same `data` pass to serializer in writing, but structure should be:  
-{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
-  - `image` key is required. can be formdata file or Base64 str.
-  - `alt` is optional and will fill auto if left blank.
-
-
-**example 1**:
-```
-from onetomultipleimage.field import OneToMultipleImage
-image = request.FILES['image']
-serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
-serializer.is_valid()
-s.validated_data
-```
-
-`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
-{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
-
-&nbsp;  
-**OneToMultipleImage** can use inside a serializer.  
-**example 2**:  
-```
-class PostSerializer(serializers.Serializer):
-    image = OneToMultipleImage(sizes=['120', '240', 'default'])
-
-data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
-serializer = PostSerializer(data=data)
-serializer.is_valid()
-s.validated_data
-```
-same result...
-
-&nbsp;   
-## onetomultipleimage models
-
-if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
-
-### FatherImage model
-Store original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
-
-&nbsp;  
-### ImageSizes
-Stores different sizes of original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **size**: django **CharField**, represent size of image (in str).
-- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
-
-
-**example 1**:  
-```
-image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
-image.save()
-```
-now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
-
-
-**example 2**:
-image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
-image.save()
-
-after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
-
-```
-image = FatherImage.objects.get(alt='sea_food-default')
-image_sizes = image.imagesizes.all()
-```
-**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
+Metadata-Version: 2.1
+Name: onetomultipleimage
+Version: 1.0.3
+Summary: convert one image to several sizes in django REST and django models
+Home-page: https://github.com/ahmadekhalili/onetomultipleimage
+Author: Ahmad Khalili
+Author-email: ahmadkhalili2020@gmail.com
+License: MIT
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django
+Requires-Dist: djangorestframework
+Requires-Dist: pillow
+Provides-Extra: jalali
+Requires-Dist: jdatetime; extra == "jalali"
+
+# onetomultipleimage
+
+onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
+
+## installation
+
+1- run: ``` pip install onetomultipleimage[jalali]```  
+
+To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
+`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
+__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
+
+2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
+after makemigrations and migrate, models will be created.
+
+
+&nbsp;
+## Serializer Field: OneToMultipleImage
+
+Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
+
+`OneToMultipleImage` arguments:
+
+- **sizes**:
+list of sizes in str. for generate original image use 'default'. required in writing.
+
+- **upload_to**:
+path in str for uploads image. required in writing.
+
+- **data**:
+it is same `data` pass to serializer in writing, but structure should be:  
+{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
+  - `image` key is required. can be formdata file or Base64 str.
+  - `alt` is optional and will fill auto if left blank.
+
+
+**example 1**:
+```
+from onetomultipleimage.field import OneToMultipleImage
+image = request.FILES['image']
+serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
+serializer.is_valid()
+s.validated_data
+```
+
+`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
+{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
+
+&nbsp;  
+**OneToMultipleImage** can use inside a serializer.  
+**example 2**:  
+```
+class PostSerializer(serializers.Serializer):
+    image = OneToMultipleImage(sizes=['120', '240', 'default'])
+
+data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
+serializer = PostSerializer(data=data)
+serializer.is_valid()
+s.validated_data
+```
+same result...
+
+&nbsp;   
+## onetomultipleimage models
+
+if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
+
+### FatherImage model
+Store original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
+
+&nbsp;  
+### ImageSizes
+Stores different sizes of original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **size**: django **CharField**, represent size of image (in str).
+- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
+
+
+**example 1**:  
+```
+image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
+image.save()
+```
+now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
+
+
+**example 2**:
+```
+image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
+image.save()
+```
+after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
+
+```
+image = FatherImage.objects.get(alt='sea_food-default')
+image_sizes = image.imagesizes.all()
+```
+**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
```

### Comparing `onetomultipleimage-1.0.2/README.md` & `onetomultipleimage-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,104 @@
-# onetomultipleimage
-
-onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
-
-## installation
-
-1- run: ``` pip install onetomultipleimage[jalali]```  
-
-To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
-`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
-__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
-
-2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
-after makemigrations and migrate, models will be created.
-
-
-&nbsp;
-## Serializer Field: OneToMultipleImage
-
-Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
-
-`OneToMultipleImage` arguments:
-
-- **sizes**:
-list of sizes in str. for generate original image use 'default'. required in writing.
-
-- **upload_to**:
-path in str for uploads image. required in writing.
-
-- **data**:
-it is same `data` pass to serializer in writing, but structure should be:  
-{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
-  - `image` key is required. can be formdata file or Base64 str.
-  - `alt` is optional and will fill auto if left blank.
-
-
-**example 1**:
-```
-from onetomultipleimage.field import OneToMultipleImage
-image = request.FILES['image']
-serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
-serializer.is_valid()
-s.validated_data
-```
-
-`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
-{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
-
-&nbsp;  
-**OneToMultipleImage** can use inside a serializer.  
-**example 2**:  
-```
-class PostSerializer(serializers.Serializer):
-    image = OneToMultipleImage(sizes=['120', '240', 'default'])
-
-data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
-serializer = PostSerializer(data=data)
-serializer.is_valid()
-s.validated_data
-```
-same result...
-
-&nbsp;   
-## onetomultipleimage models
-
-if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
-
-### FatherImage model
-Store original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
-
-&nbsp;  
-### ImageSizes
-Stores different sizes of original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **size**: django **CharField**, represent size of image (in str).
-- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
-
-
-**example 1**:  
-```
-image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
-image.save()
-```
-now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
-
-
-**example 2**:
-image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
-image.save()
-
-after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
-
-```
-image = FatherImage.objects.get(alt='sea_food-default')
-image_sizes = image.imagesizes.all()
-```
-**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
+# onetomultipleimage
+
+onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
+
+## installation
+
+1- run: ``` pip install onetomultipleimage[jalali]```  
+
+To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
+`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
+__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
+
+2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
+after makemigrations and migrate, models will be created.
+
+
+&nbsp;
+## Serializer Field: OneToMultipleImage
+
+Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
+
+`OneToMultipleImage` arguments:
+
+- **sizes**:
+list of sizes in str. for generate original image use 'default'. required in writing.
+
+- **upload_to**:
+path in str for uploads image. required in writing.
+
+- **data**:
+it is same `data` pass to serializer in writing, but structure should be:  
+{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
+  - `image` key is required. can be formdata file or Base64 str.
+  - `alt` is optional and will fill auto if left blank.
+
+
+**example 1**:
+```
+from onetomultipleimage.field import OneToMultipleImage
+image = request.FILES['image']
+serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
+serializer.is_valid()
+s.validated_data
+```
+
+`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
+{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
+
+&nbsp;  
+**OneToMultipleImage** can use inside a serializer.  
+**example 2**:  
+```
+class PostSerializer(serializers.Serializer):
+    image = OneToMultipleImage(sizes=['120', '240', 'default'])
+
+data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
+serializer = PostSerializer(data=data)
+serializer.is_valid()
+s.validated_data
+```
+same result...
+
+&nbsp;   
+## onetomultipleimage models
+
+if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
+
+### FatherImage model
+Store original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
+
+&nbsp;  
+### ImageSizes
+Stores different sizes of original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **size**: django **CharField**, represent size of image (in str).
+- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
+
+
+**example 1**:  
+```
+image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
+image.save()
+```
+now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
+
+
+**example 2**:
+```
+image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
+image.save()
+```
+after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
+
+```
+image = FatherImage.objects.get(alt='sea_food-default')
+image_sizes = image.imagesizes.all()
+```
+**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
```

### Comparing `onetomultipleimage-1.0.2/onetomultipleimage/fields.py` & `onetomultipleimage-1.0.3/onetomultipleimage/fields.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from django import forms
-from django.db import models
-from rest_framework import serializers
-
-import ast
-
-from .methods import ImageCreationSizes
-
-
-class ListCharField(models.CharField):
-    description = "A CharField that stores a list of strings as a comma-separated string."
-
-    def to_python(self, value):
-        if isinstance(value, list):
-            return value
-        if value is None:
-            return []
-        return value.split(',')
-
-    def get_prep_value(self, value):
-        if isinstance(value, list):
-            return ','.join(str(item) for item in value)
-        return value
-
-    def from_db_value(self, value, expression, connection):
-        if value is None:
-            return []
-        return value.split(',')
-
-
-class ListCharFormField(forms.CharField):
-    def to_python(self, value):
-        # Ensures the value is converted to a list, whether coming from a form or directly from Python code
-        if isinstance(value, str):
-            return [item.strip() for item in value.split(',')]
-        return value
-
-    def clean(self, value):
-        if isinstance(value, str):
-            lis = ast.literal_eval(value)
-            value = ','.join(lis)
-        return value
-
-
-class OneToMultipleImage(serializers.Serializer):
-    def __init__(self, sizes=None, upload_to=None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if not self.instance:      # in writing, sizes and upload_to required
-            if not sizes or not upload_to:
-                raise ValueError("both of 'sizes' and 'upload_to' arguments must be provided")
-            self.sizes = sizes
-            self.upload_to = upload_to
-
-    def to_representation(self, value):
-        result = {}
-        for image_icon in value:
-            size = image_icon.size
-            result[size] = {'image': image_icon.url, 'alt': image_icon.alt}
-        return result
-
-    def to_internal_value(self, data):
-        obj = ImageCreationSizes(data=data, sizes=self.sizes)
-        instances = obj.upload(upload_to=self.upload_to)
-        return instances
+from django import forms
+from django.db import models
+from rest_framework import serializers
+
+import ast
+
+from .methods import ImageCreationSizes
+
+
+class ListCharField(models.CharField):
+    description = "A CharField that stores a list of strings as a comma-separated string."
+
+    def to_python(self, value):
+        if isinstance(value, list):
+            return value
+        if value is None:
+            return []
+        return value.split(',')
+
+    def get_prep_value(self, value):
+        if isinstance(value, list):
+            return ','.join(str(item) for item in value)
+        return value
+
+    def from_db_value(self, value, expression, connection):
+        if value is None:
+            return []
+        return value.split(',')
+
+
+class ListCharFormField(forms.CharField):
+    def to_python(self, value):
+        # Ensures the value is converted to a list, whether coming from a form or directly from Python code
+        if isinstance(value, str):
+            return [item.strip() for item in value.split(',')]
+        return value
+
+    def clean(self, value):
+        if isinstance(value, str):
+            lis = ast.literal_eval(value)
+            value = ','.join(lis)
+        return value
+
+
+class OneToMultipleImage(serializers.Serializer):
+    def __init__(self, sizes=None, upload_to=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not self.instance:      # in writing, sizes and upload_to required
+            if not sizes or not upload_to:
+                raise ValueError("both of 'sizes' and 'upload_to' arguments must be provided")
+            self.sizes = sizes
+            self.upload_to = upload_to
+
+    def to_representation(self, value):
+        result = {}
+        for image_icon in value:
+            size = image_icon.size
+            result[size] = {'image': image_icon.url, 'alt': image_icon.alt}
+        return result
+
+    def to_internal_value(self, data):
+        obj = ImageCreationSizes(data=data, sizes=self.sizes)
+        instances = obj.upload(upload_to=self.upload_to)
+        return instances
```

### Comparing `onetomultipleimage-1.0.2/onetomultipleimage/methods.py` & `onetomultipleimage-1.0.3/onetomultipleimage/methods.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from django.conf import settings
-from django.core.files.uploadedfile import SimpleUploadedFile
-
-import io
-import os
-import uuid
-import itertools
-from datetime import datetime
-from PIL import Image as PilImage
-
-
-class ImageCreationSizes:
-    # in this class we receive image binary/base64 and save it to disk with specified sizes. if a model specified,
-    # that models field will be filled instead, for example: image1.image = size1, image2.image = size2, ...
-    def __init__(self, data, sizes, name=None):
-        # data is like: {'image': InMemoryUploadFIle(..)} (keys are instance fields)
-        # sizes like:
-        self.base_path = str(settings.BASE_DIR)  # is like: /home/akh/eCommerce-web-api/ictsun
-        self.data = data.copy()  # we don't want change outside variables has been passed to our class.
-        self.sizes = sizes
-        self.name = name if name else uuid.uuid4().hex[:12]
-        self.uuid_alt = False
-        # when data is like: {'alt': None, ...}, data['alt'] must be removed and replaced with uuid
-        try:
-            alt = self.data.pop('alt')
-            if not alt:
-                self.uuid_alt = True       # in updating, if alt not provided by user, don't update instance.alt
-                alt = uuid.uuid4().hex[:6]
-        except:
-            alt = uuid.uuid4().hex[:6]
-        self.alt = alt
-
-    @staticmethod
-    def add_size_to_alt(size, text=None):
-        # text == pre alt
-        pre_alt = text if text else uuid.uuid4().hex[:6]
-        return f'{pre_alt}-{size}'
-
-    def get_file_stream(self):
-        file = self.files['file'].read() if self.files.get('file') else self.files['image_icon_set-0-image'].read()
-        return io.BytesIO(file)
-
-    def get_path(self, middle_path=None):
-        # get path like: '/media/posts_images/icons/' returns like: '/media/posts_images/icons/1402/3/15/'
-        if not middle_path:
-            middle_path = 'posts_images/icons/'
-        middle_path = '/media/' + middle_path
-        if getattr(settings, 'IMAGES_PATH_TYPE', None) == 'jalali':
-            try:
-                import jdatetime
-                date = jdatetime.datetime.fromgregorian(date=datetime.now()).strftime('%Y %-m %-d').split()
-            except ImportError:
-                raise ImportError("please install 'jdatetime' package")
-        else:
-            now = datetime.now()
-            date = f"{now.year} {now.month} {now.day}".split()     # %Y %-m %-d format doesn't work in windows
-        return f'{middle_path}{date[0]}/{date[1]}/{date[2]}/'
-
-    def _save(self, opened_image, upload_to, full_name, format, instance, att_name):
-        if isinstance(opened_image, PilImage.Image):
-            if instance:           # save image by image field (need write to disk)
-                buffer = io.BytesIO()
-                opened_image.save(buffer, format=format)
-                setattr(instance, att_name, SimpleUploadedFile(full_name, buffer.getvalue()))
-                # field.upload_to must change to our path, also '/media/' must remove from path otherwise raise error
-                if callable(upload_to):    # if upload_to is function
-                    getattr(instance, att_name).field.upload_to = upload_to
-                else:                      # if is string
-                    getattr(instance, att_name).field.upload_to = upload_to.replace('/media/', '', 1)
-                return None
-            else:                  # save image (write to disk) by pillow.save()
-                opened_image.save(self.base_path + upload_to + full_name)
-                return SimpleUploadedFile(full_name, open(self.base_path + upload_to + full_name, 'rb').read())
-
-    def build(self, model, att_name='image', opened_image=None, upload_to=None):
-        instances = [model(alt=f'{self.alt}-{size}', **self.data) for size in self.sizes]
-        return self.save(opened_image=opened_image, upload_to=upload_to, instances=instances, att_name=att_name)
-
-    def update(self, instances, att_name='image', opened_image=None, upload_to=None):
-        instances = list(instances)[:len(self.sizes)]
-        for size, instance in zip(self.sizes, instances):
-            # if we have alt in our instance and user don't want update it, so don't change alt.
-            instance.alt = f'{self.alt}-{size}' if not self.uuid_alt or not instance.alt else instance.alt
-            [setattr(instance, key, self.data[key]) for key in self.data]
-        return self.save(opened_image=opened_image, upload_to=upload_to, instances=instances, att_name=att_name)
-
-    def upload(self, upload_to, opened_image=None):
-        # upload icons without using any models. returned value is simple python objects. each obj has 4 attr. like:
-        # image=<SimpleUploadedFile image.jpg>, url=/media/../qwer43asd2e4-720.JPG, alt=, size=720
-        return self.save(opened_image=opened_image, upload_to=upload_to)
-
-    def save(self, opened_image=None, upload_to=None, instances=None, att_name='image'):
-        '''
-        - opened_image can be binary (multipart form-data) or base64.
-        - upload_to is like: posts_images/icons/ will be convert to: /media/posts_images/icons/
-        - model is django model class. if you specify model, image will be saved to disk by model field,
-        (instance.att_name.save()) instead of PilImage.save()
-        - instances uses when associating with django models (build and update methods)
-        1- returned value: {model_instance1, model_instance2, ...}
-        2- returned value: {<Upload object 1 - (.image .url .size)>, <Upload object 2 - (.image .url .size)>}
-        '''
-        class Upload:
-            def __init__(self, image, url, alt, size, **kwargs):
-                kwargs['image'], kwargs['url'], kwargs['alt'], kwargs['size'] = image, url, alt, size
-                [setattr(self, key, kwargs[key]) for key in kwargs]
-
-            def __repr__(self):
-                return '<Upload object {} - (.image .url .alt .size)>'.format(self.alt)  # self.alt contain size too
-
-        if not instances:
-            instances = []
-
-        try:         # binary file (multipart form-data)
-            stream = io.BytesIO(self.data['image'].read())
-        except:      # base64 file
-            try:
-                import base64
-                stream = io.BytesIO(base64.b64decode(self.data['image'].split(';base64,')[1]))
-            except:       # when no image provided (like when update 'alt' field only)
-                return instances
-        opened_image = PilImage.open(stream) if not opened_image else opened_image
-
-        if not callable(upload_to):  # upload_to is str or None
-            upload_to = self.get_path(upload_to)
-            if not os.path.exists(self.base_path + upload_to):
-                os.makedirs(self.base_path + upload_to)
-
-        iter_instances, objects = itertools.cycle(instances) if instances else None, []
-        if isinstance(opened_image, PilImage.Image):
-            format = opened_image.format              # opened_image.format is like: "JPG"
-            height, width = opened_image.size                 # opened_image.size is like: (1080, 1920)
-            aspect_ratio = height / width
-            for height in self.sizes:
-                if height.isdigit():
-                    height = int(height)
-                    resized = opened_image.resize((height, int(height / aspect_ratio)))
-                else:
-                    resized = opened_image  # for 'default' size
-                full_name = f'{self.name}-{height}' + f'.{format}'
-                instance = next(iter_instances) if iter_instances else None
-                upload_image = self._save(resized, upload_to, full_name, format, instance, att_name)
-                # url is like: /media/posts_images/1402/3/20/qwer43asd2e4-720.JPG
-                if not instances:
-                    objects += [Upload(image=upload_image, url=upload_to+full_name, alt=f'{self.alt}-{height}', size=height)]
-            return instances or objects
-
-        elif isinstance(opened_image, io.BufferedReader):      # open image by built-in function open()
-            pass
-        else:
-            raise Exception('opened_image is not object of PilImage or python built in .open()')
+from django.conf import settings
+from django.core.files.uploadedfile import SimpleUploadedFile
+
+import io
+import os
+import uuid
+import itertools
+from datetime import datetime
+from PIL import Image as PilImage
+
+
+class ImageCreationSizes:
+    # in this class we receive image binary/base64 and save it to disk with specified sizes. if a model specified,
+    # that models field will be filled instead, for example: image1.image = size1, image2.image = size2, ...
+    def __init__(self, data, sizes, name=None):
+        # data is like: {'image': InMemoryUploadFIle(..)} (keys are instance fields)
+        # sizes like:
+        self.base_path = str(settings.BASE_DIR)  # is like: /home/akh/eCommerce-web-api/ictsun
+        self.data = data.copy()  # we don't want change outside variables has been passed to our class.
+        self.sizes = sizes
+        self.name = name if name else uuid.uuid4().hex[:12]
+        self.uuid_alt = False
+        # when data is like: {'alt': None, ...}, data['alt'] must be removed and replaced with uuid
+        try:
+            alt = self.data.pop('alt')
+            if not alt:
+                self.uuid_alt = True       # in updating, if alt not provided by user, don't update instance.alt
+                alt = uuid.uuid4().hex[:6]
+        except:
+            alt = uuid.uuid4().hex[:6]
+        self.alt = alt
+
+    @staticmethod
+    def add_size_to_alt(size, text=None):
+        # text == pre alt
+        pre_alt = text if text else uuid.uuid4().hex[:6]
+        return f'{pre_alt}-{size}'
+
+    def get_file_stream(self):
+        file = self.files['file'].read() if self.files.get('file') else self.files['image_icon_set-0-image'].read()
+        return io.BytesIO(file)
+
+    def get_path(self, middle_path=None):
+        # get path like: '/media/posts_images/icons/' returns like: '/media/posts_images/icons/1402/3/15/'
+        if not middle_path:
+            middle_path = 'posts_images/icons/'
+        middle_path = '/media/' + middle_path
+        if getattr(settings, 'IMAGES_PATH_TYPE', None) == 'jalali':
+            try:
+                import jdatetime
+                date = jdatetime.datetime.fromgregorian(date=datetime.now()).strftime('%Y %-m %-d').split()
+            except ImportError:
+                raise ImportError("please install 'jdatetime' package")
+        else:
+            now = datetime.now()
+            date = f"{now.year} {now.month} {now.day}".split()     # %Y %-m %-d format doesn't work in windows
+        return f'{middle_path}{date[0]}/{date[1]}/{date[2]}/'
+
+    def _save(self, opened_image, upload_to, full_name, format, instance, att_name):
+        if isinstance(opened_image, PilImage.Image):
+            if instance:           # save image by image field (need write to disk)
+                buffer = io.BytesIO()
+                opened_image.save(buffer, format=format)
+                setattr(instance, att_name, SimpleUploadedFile(full_name, buffer.getvalue()))
+                # field.upload_to must change to our path, also '/media/' must remove from path otherwise raise error
+                if callable(upload_to):    # if upload_to is function
+                    getattr(instance, att_name).field.upload_to = upload_to
+                else:                      # if is string
+                    getattr(instance, att_name).field.upload_to = upload_to.replace('/media/', '', 1)
+                return None
+            else:                  # save image (write to disk) by pillow.save()
+                opened_image.save(self.base_path + upload_to + full_name)
+                return SimpleUploadedFile(full_name, open(self.base_path + upload_to + full_name, 'rb').read())
+
+    def build(self, model, att_name='image', opened_image=None, upload_to=None):
+        instances = [model(alt=f'{self.alt}-{size}', **self.data) for size in self.sizes]
+        return self.save(opened_image=opened_image, upload_to=upload_to, instances=instances, att_name=att_name)
+
+    def update(self, instances, att_name='image', opened_image=None, upload_to=None):
+        instances = list(instances)[:len(self.sizes)]
+        for size, instance in zip(self.sizes, instances):
+            # if we have alt in our instance and user don't want update it, so don't change alt.
+            instance.alt = f'{self.alt}-{size}' if not self.uuid_alt or not instance.alt else instance.alt
+            [setattr(instance, key, self.data[key]) for key in self.data]
+        return self.save(opened_image=opened_image, upload_to=upload_to, instances=instances, att_name=att_name)
+
+    def upload(self, upload_to, opened_image=None):
+        # upload icons without using any models. returned value is simple python objects. each obj has 4 attr. like:
+        # image=<SimpleUploadedFile image.jpg>, url=/media/../qwer43asd2e4-720.JPG, alt=, size=720
+        return self.save(opened_image=opened_image, upload_to=upload_to)
+
+    def save(self, opened_image=None, upload_to=None, instances=None, att_name='image'):
+        '''
+        - opened_image can be binary (multipart form-data) or base64.
+        - upload_to is like: posts_images/icons/ will be convert to: /media/posts_images/icons/
+        - model is django model class. if you specify model, image will be saved to disk by model field,
+        (instance.att_name.save()) instead of PilImage.save()
+        - instances uses when associating with django models (build and update methods)
+        1- returned value: {model_instance1, model_instance2, ...}
+        2- returned value: {<Upload object 1 - (.image .url .size)>, <Upload object 2 - (.image .url .size)>}
+        '''
+        class Upload:
+            def __init__(self, image, url, alt, size, **kwargs):
+                kwargs['image'], kwargs['url'], kwargs['alt'], kwargs['size'] = image, url, alt, size
+                [setattr(self, key, kwargs[key]) for key in kwargs]
+
+            def __repr__(self):
+                return '<Upload object {} - (.image .url .alt .size)>'.format(self.alt)  # self.alt contain size too
+
+        if not instances:
+            instances = []
+
+        try:         # binary file (multipart form-data)
+            stream = io.BytesIO(self.data['image'].read())
+        except:      # base64 file
+            try:
+                import base64
+                stream = io.BytesIO(base64.b64decode(self.data['image'].split(';base64,')[1]))
+            except:       # when no image provided (like when update 'alt' field only)
+                return instances
+        opened_image = PilImage.open(stream) if not opened_image else opened_image
+
+        if not callable(upload_to):  # upload_to is str or None
+            upload_to = self.get_path(upload_to)
+            if not os.path.exists(self.base_path + upload_to):
+                os.makedirs(self.base_path + upload_to)
+
+        iter_instances, objects = itertools.cycle(instances) if instances else None, []
+        if isinstance(opened_image, PilImage.Image):
+            format = opened_image.format              # opened_image.format is like: "JPG"
+            height, width = opened_image.size                 # opened_image.size is like: (1080, 1920)
+            aspect_ratio = height / width
+            for height in self.sizes:
+                if height.isdigit():
+                    height = int(height)
+                    resized = opened_image.resize((height, int(height / aspect_ratio)))
+                else:
+                    resized = opened_image  # for 'default' size
+                full_name = f'{self.name}-{height}' + f'.{format}'
+                instance = next(iter_instances) if iter_instances else None
+                upload_image = self._save(resized, upload_to, full_name, format, instance, att_name)
+                # url is like: /media/posts_images/1402/3/20/qwer43asd2e4-720.JPG
+                if not instances:
+                    objects += [Upload(image=upload_image, url=upload_to+full_name, alt=f'{self.alt}-{height}', size=height)]
+            return instances or objects
+
+        elif isinstance(opened_image, io.BufferedReader):      # open image by built-in function open()
+            pass
+        else:
+            raise Exception('opened_image is not object of PilImage or python built in .open()')
```

### Comparing `onetomultipleimage-1.0.2/onetomultipleimage/models.py` & `onetomultipleimage-1.0.3/onetomultipleimage/models.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from django.db import models
-from django.conf import settings
-from django.utils.translation import gettext_lazy as _
-
-from datetime import datetime
-
-from .methods import ImageCreationSizes
-from .fields import ListCharField
-
-
-def image_path_selector(instance, filename):
-    if getattr(settings, 'IMAGES_PATH_TYPE', None) == 'jalali':
-        try:
-            import jdatetime
-            date = jdatetime.datetime.fromgregorian(date=datetime.now()).strftime('%Y %-m %-d').split()
-        except ImportError:
-            raise ImportError("please install 'jdatetime' package")
-    else:
-        now = datetime.now()
-        date = f"{now.year} {now.month} {now.day}".split()
-    return f'{instance.__class__.__name__}/{date[0]}/{date[1]}/{date[2]}/{filename}'
-
-
-class FatherImage(models.Model):
-    image = models.ImageField(_('image'), upload_to=image_path_selector)
-    alt = models.CharField(_('alt'), max_length=55, unique=True, null=True)
-    sizes = ListCharField(_('sizes'), max_length=255)  # input data like: ['120', '240', '480']
-    # imagesizes, reverse relation
-
-    class Meta:
-        verbose_name = _('Image')
-        verbose_name_plural = _('Images')
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.pre_image = self.image
-        self.pre_alt = self.alt
-
-    def __str__(self):
-        return f'{self.alt}'
-
-    def save(self, *args, **kwargs):
-        alt = self.alt    # self.alt is None for default
-        change = True if self.id else False
-        if not change:      # FatherImage creation
-            self.alt = ImageCreationSizes.add_size_to_alt('default', alt)
-        elif alt != self.pre_alt:         # FatherImage updating, prevent alt overriding like: 'asd32a-default-default'
-            self.alt = ImageCreationSizes.add_size_to_alt('default', alt)
-        super().save(*args, **kwargs)
-        if not change:     # ImageSizes creation
-            img = ImageCreationSizes(data={'image': self.image, 'alt': alt}, sizes=self.sizes)
-            instances = img.build(model=ImageSizes, upload_to=ImageSizes._meta.get_field('image').upload_to)
-            for instance, size in zip(instances, self.sizes):
-                instance.father, instance.size = self, size
-            ImageSizes.objects.bulk_create(instances)
-        else:         # ImageSizes updating
-            data = {'alt': alt, 'image': self.image if self.image is not self.pre_image else None}
-            img = ImageCreationSizes(data=data, sizes=self.sizes)
-            instances = self.imagesizes.all()
-            instances = img.update(instances=instances, upload_to=ImageSizes._meta.get_field('image').upload_to)
-            if data.get('image'):
-                for instance in instances:
-                    image_data = instance.image.file
-                    instance.image.save(instance.image.name, image_data)   # image field isn't saved with bulk_update
-            for instance, size in zip(instances, self.sizes):
-                instance.size, instance.father_id = size, self.id
-            ImageSizes.objects.bulk_update(instances, [*list(data.keys()), *['size', 'father_id']])
-
-
-class ImageSizes(models.Model):
-    image = models.ImageField(_('image'), upload_to=image_path_selector)
-    alt = models.CharField(_('alt'), max_length=55, unique=True, null=True)
-    size = models.CharField(_('size'), max_length=20)
-    father = models.ForeignKey(FatherImage, related_name='imagesizes', on_delete=models.CASCADE, verbose_name=_('image'))
-
-    class Meta:
-        verbose_name = _('Image size')
-        verbose_name_plural = _('Images sizes')
-
-    def __str__(self):
-        return f'{self.alt}'
+from django.db import models
+from django.conf import settings
+from django.utils.translation import gettext_lazy as _
+
+from datetime import datetime
+
+from .methods import ImageCreationSizes
+from .fields import ListCharField
+
+
+def image_path_selector(instance, filename):
+    if getattr(settings, 'IMAGES_PATH_TYPE', None) == 'jalali':
+        try:
+            import jdatetime
+            date = jdatetime.datetime.fromgregorian(date=datetime.now()).strftime('%Y %-m %-d').split()
+        except ImportError:
+            raise ImportError("please install 'jdatetime' package")
+    else:
+        now = datetime.now()
+        date = f"{now.year} {now.month} {now.day}".split()
+    return f'{instance.__class__.__name__}/{date[0]}/{date[1]}/{date[2]}/{filename}'
+
+
+class FatherImage(models.Model):
+    image = models.ImageField(_('image'), upload_to=image_path_selector)
+    alt = models.CharField(_('alt'), max_length=55, unique=True, null=True)
+    sizes = ListCharField(_('sizes'), max_length=255)  # input data like: ['120', '240', '480']
+    # imagesizes, reverse relation
+
+    class Meta:
+        verbose_name = _('Image')
+        verbose_name_plural = _('Images')
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.pre_image = self.image
+        self.pre_alt = self.alt
+
+    def __str__(self):
+        return f'{self.alt}'
+
+    def save(self, *args, **kwargs):
+        alt = self.alt    # self.alt is None for default
+        change = True if self.id else False
+        if not change:      # FatherImage creation
+            self.alt = ImageCreationSizes.add_size_to_alt('default', alt)
+        elif alt != self.pre_alt:         # FatherImage updating, prevent alt overriding like: 'asd32a-default-default'
+            self.alt = ImageCreationSizes.add_size_to_alt('default', alt)
+        super().save(*args, **kwargs)
+        if not change:     # ImageSizes creation
+            img = ImageCreationSizes(data={'image': self.image, 'alt': alt}, sizes=self.sizes)
+            instances = img.build(model=ImageSizes, upload_to=ImageSizes._meta.get_field('image').upload_to)
+            for instance, size in zip(instances, self.sizes):
+                instance.father, instance.size = self, size
+            ImageSizes.objects.bulk_create(instances)
+        else:         # ImageSizes updating
+            data = {'alt': alt, 'image': self.image if self.image is not self.pre_image else None}
+            img = ImageCreationSizes(data=data, sizes=self.sizes)
+            instances = self.imagesizes.all()
+            instances = img.update(instances=instances, upload_to=ImageSizes._meta.get_field('image').upload_to)
+            if data.get('image'):
+                for instance in instances:
+                    image_data = instance.image.file
+                    instance.image.save(instance.image.name, image_data)   # image field isn't saved with bulk_update
+            for instance, size in zip(instances, self.sizes):
+                instance.size, instance.father_id = size, self.id
+            ImageSizes.objects.bulk_update(instances, [*list(data.keys()), *['size', 'father_id']])
+
+
+class ImageSizes(models.Model):
+    image = models.ImageField(_('image'), upload_to=image_path_selector)
+    alt = models.CharField(_('alt'), max_length=55, unique=True, null=True)
+    size = models.CharField(_('size'), max_length=20)
+    father = models.ForeignKey(FatherImage, related_name='imagesizes', on_delete=models.CASCADE, verbose_name=_('image'))
+
+    class Meta:
+        verbose_name = _('Image size')
+        verbose_name_plural = _('Images sizes')
+
+    def __str__(self):
+        return f'{self.alt}'
```

### Comparing `onetomultipleimage-1.0.2/onetomultipleimage.egg-info/PKG-INFO` & `onetomultipleimage-1.0.3/onetomultipleimage.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,123 @@
-Metadata-Version: 2.1
-Name: onetomultipleimage
-Version: 1.0.2
-Summary: convert one image to several sizes in django REST and django models
-Home-page: https://github.com/ahmadekhalili/onetomultipleimage
-Author: Ahmad Khalili
-Author-email: ahmadkhalili2020@gmail.com
-License: MIT
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: djangorestframework
-Requires-Dist: pillow
-Provides-Extra: jalali
-Requires-Dist: jdatetime; extra == "jalali"
-
-# onetomultipleimage
-
-onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
-
-## installation
-
-1- run: ``` pip install onetomultipleimage[jalali]```  
-
-To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
-`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
-__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
-
-2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
-after makemigrations and migrate, models will be created.
-
-
-&nbsp;
-## Serializer Field: OneToMultipleImage
-
-Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
-
-`OneToMultipleImage` arguments:
-
-- **sizes**:
-list of sizes in str. for generate original image use 'default'. required in writing.
-
-- **upload_to**:
-path in str for uploads image. required in writing.
-
-- **data**:
-it is same `data` pass to serializer in writing, but structure should be:  
-{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
-  - `image` key is required. can be formdata file or Base64 str.
-  - `alt` is optional and will fill auto if left blank.
-
-
-**example 1**:
-```
-from onetomultipleimage.field import OneToMultipleImage
-image = request.FILES['image']
-serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
-serializer.is_valid()
-s.validated_data
-```
-
-`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
-{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
-
-&nbsp;  
-**OneToMultipleImage** can use inside a serializer.  
-**example 2**:  
-```
-class PostSerializer(serializers.Serializer):
-    image = OneToMultipleImage(sizes=['120', '240', 'default'])
-
-data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
-serializer = PostSerializer(data=data)
-serializer.is_valid()
-s.validated_data
-```
-same result...
-
-&nbsp;   
-## onetomultipleimage models
-
-if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
-
-### FatherImage model
-Store original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
-
-&nbsp;  
-### ImageSizes
-Stores different sizes of original image. attributes:
-
-- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
-- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
-- **size**: django **CharField**, represent size of image (in str).
-- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
-
-
-**example 1**:  
-```
-image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
-image.save()
-```
-now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
-
-
-**example 2**:
-image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
-image.save()
-
-after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
-
-```
-image = FatherImage.objects.get(alt='sea_food-default')
-image_sizes = image.imagesizes.all()
-```
-**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
+Metadata-Version: 2.1
+Name: onetomultipleimage
+Version: 1.0.3
+Summary: convert one image to several sizes in django REST and django models
+Home-page: https://github.com/ahmadekhalili/onetomultipleimage
+Author: Ahmad Khalili
+Author-email: ahmadkhalili2020@gmail.com
+License: MIT
+Classifier: Framework :: Django
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django
+Requires-Dist: djangorestframework
+Requires-Dist: pillow
+Provides-Extra: jalali
+Requires-Dist: jdatetime; extra == "jalali"
+
+# onetomultipleimage
+
+onetomultipleimage is a django package to convert one image to specified sizes. it can be used in REST or django model.
+
+## installation
+
+1- run: ``` pip install onetomultipleimage[jalali]```  
+
+To install onetomultipleimage with Jalali date support, add ```[jalali]``` part.  
+`IMAGES_PATH_TYPE='jalali'` in settings.py, now jalali date path used (instead default gregorian) like:  
+__/media/FatherImage/1401/12/13/small.jpg__ instead of: __/media/FatherImage/2023/3/4/small.jpg__
+
+2- to install **onetomultipleimage** models, add 'onetomultipleimage' to `INSTALLED_APPS` of project's settings.py
+after makemigrations and migrate, models will be created.
+
+
+&nbsp;
+## Serializer Field: OneToMultipleImage
+
+Receives image in Base64/form-data with list of sizes and generate images with specified sizes.
+
+`OneToMultipleImage` arguments:
+
+- **sizes**:
+list of sizes in str. for generate original image use 'default'. required in writing.
+
+- **upload_to**:
+path in str for uploads image. required in writing.
+
+- **data**:
+it is same `data` pass to serializer in writing, but structure should be:  
+{'image': formdata_file/Base64_str, 'alt': 'some_alt'}  
+  - `image` key is required. can be formdata file or Base64 str.
+  - `alt` is optional and will fill auto if left blank.
+
+
+**example 1**:
+```
+from onetomultipleimage.field import OneToMultipleImage
+image = request.FILES['image']
+serializer = OneToMultipleImage(sizes=['120', '240', 'default'], data={'image': image})
+serializer.is_valid()
+s.validated_data
+```
+
+`.validated_data` here returns 3 object with 120px height, 240px height, and default (original) image sizes. `validated_data` returns like:  
+{'image': [<Upload object 1e2813-120 - (.image .url .alt .size)>, <Upload object 1e2813-240 - (.image .url .alt .size)>, <Upload object 1e2813-default - (.image .url .alt .size)>]}
+
+&nbsp;  
+**OneToMultipleImage** can use inside a serializer.  
+**example 2**:  
+```
+class PostSerializer(serializers.Serializer):
+    image = OneToMultipleImage(sizes=['120', '240', 'default'])
+
+data = {'image': {'image': "data:image/jpeg;base64,/9j/..."}}  # image in Base64 (str)
+serializer = PostSerializer(data=data)
+serializer.is_valid()
+s.validated_data
+```
+same result...
+
+&nbsp;   
+## onetomultipleimage models
+
+if you need django model for one-to-multy process, you have to add `onetomultipleimage` to `INSTALLED_APPS`. after migrate, you have two table **__FatherImage__**, **__ImageSizes__**.
+
+### FatherImage model
+Store original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'FatherImage/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **sizes**: custom **ListCharField**, represent lists of sizes you want to create them. (like: ['120', '240'])
+
+&nbsp;  
+### ImageSizes
+Stores different sizes of original image. attributes:
+
+- **image**: django **ImageField**. `upload_to` path is: _'ImageSizes/year/month/day'_ but can override directly before model initializing.
+- **alt**: django **CharField**, represent image's alt, you can leave it blank to auto generating by uuid.uuid4
+- **size**: django **CharField**, represent size of image (in str).
+- **father**: django **ForeignKey**, reference to **FatherImage**. (FatherImage.imagesizes in reverse relation is accecible)
+
+
+**example 1**:  
+```
+image = FatherImage(image=request.FILES['image'], sizes=['120', '240', '480'])
+image.save()
+```
+now fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt and imagesizes.alt auto generated like: 'db949e-default', ''db949z-120', ...
+
+
+**example 2**:
+```
+image = FatherImage(image=request.FILES['image'], alt='sea_food', sizes=['120', '240', '480'])
+image.save()
+```
+after .save, fatherimage and 3 imagesizes with 120, 240, 480 PXs is created. fatherimage.alt is like: 'sea_food-default'
+
+```
+image = FatherImage.objects.get(alt='sea_food-default')
+image_sizes = image.imagesizes.all()
+```
+**image_sizes** contain 3 different size of original image. ```image_sizes[0].alt``` is like: 'sea_food-120',  ```image_sizes[1].alt```: 'sea_food-240', ...
```

