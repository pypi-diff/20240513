# Comparing `tmp/pizzoo-0.9.5.tar.gz` & `tmp/pizzoo-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizzoo-0.9.5.tar", last modified: Sat May 11 09:39:47 2024, max compression
+gzip compressed data, was "pizzoo-0.9.6.tar", last modified: Mon May 13 14:22:16 2024, max compression
```

## Comparing `pizzoo-0.9.5.tar` & `pizzoo-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 09:39:47.719416 pizzoo-0.9.5/
--rw-rw-rw-   0        0        0     6982 2024-05-11 09:39:47.718416 pizzoo-0.9.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 09:39:47.714790 pizzoo-0.9.5/pizzoo/
--rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.5/pizzoo/__init__.py
--rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.5/pizzoo/_constants.py
--rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.5/pizzoo/_renderers.py
--rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.5/pizzoo/_utils.py
--rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.5/pizzoo/game.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:39:47.718416 pizzoo-0.9.5/pizzoo.egg-info/
--rw-rw-rw-   0        0        0     6982 2024-05-11 09:39:47.000000 pizzoo-0.9.5/pizzoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-11 09:39:47.000000 pizzoo-0.9.5/pizzoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 09:39:47.000000 pizzoo-0.9.5/pizzoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-11 09:39:47.000000 pizzoo-0.9.5/pizzoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-11 09:39:47.000000 pizzoo-0.9.5/pizzoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 09:39:47.719416 pizzoo-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1103 2024-05-11 09:39:44.000000 pizzoo-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.043040 pizzoo-0.9.6/
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:21:35.000000 pizzoo-0.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7155 2024-05-13 14:22:16.043040 pizzoo-0.9.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.039040 pizzoo-0.9.6/pizzoo/
+-rw-rw-rw-   0        0        0    43264 2024-04-19 15:34:13.000000 pizzoo-0.9.6/pizzoo/MatrixLight6.bdf
+-rw-rw-rw-   0        0        0    21798 2024-05-04 08:50:51.000000 pizzoo-0.9.6/pizzoo/__init__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-19 15:38:24.000000 pizzoo-0.9.6/pizzoo/_constants.py
+-rw-rw-rw-   0        0        0    17046 2024-05-03 00:00:18.000000 pizzoo-0.9.6/pizzoo/_renderers.py
+-rw-rw-rw-   0        0        0      705 2024-04-28 16:47:36.000000 pizzoo-0.9.6/pizzoo/_utils.py
+-rw-rw-rw-   0        0        0    21871 2024-05-10 19:21:17.000000 pizzoo-0.9.6/pizzoo/game.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:16.042040 pizzoo-0.9.6/pizzoo.egg-info/
+-rw-rw-rw-   0        0        0     7155 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 14:22:16.000000 pizzoo-0.9.6/pizzoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:22:16.043040 pizzoo-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2024-05-13 14:22:12.000000 pizzoo-0.9.6/setup.py
```

### Comparing `pizzoo-0.9.5/PKG-INFO` & `pizzoo-0.9.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.5
+Version: 0.9.6
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -54,14 +54,22 @@
 
 * **Flexible integration with any device**:
 	Even with the Pixoo64 being the default target, the Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
+## Install
+
+Just use pip to install the package:
+```bash
+pip install pizzoo
+```
+That's it! Everything should be installed correctly and pizzoo is ready to be used!
+
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
 ```python
 pizzoo.cls()
 pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
 pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.5 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.6 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
@@ -28,24 +28,26 @@
 creating fast and reusable interfaces. * **Flexible integration with any
 device**: Even with the Pixoo64 being the default target, the Renderer class
 can be easily extended to support additional methods and integrate with various
 hardware. This ensures that Pizzoo can adapt to your specific project and
 hardware requirements. * **Game Development Toolkit**: Tap into the
 possibilities of micro game development with our mini game engine. Design,
 develop, and deploy small-scale games that can be played right on your LED
-devices, perfect for creating engaging interactive experiences. ## Drawing on
-your device Frame manipulation is the core of the `pizzoo` library. Every time
-the library is created and the `render` method is called, the buffer is filled
-with a new frame we can use to draw on. Lets start by drawing three pixels on
-the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle((31, 31),
-10, '#00ff00', filled=True) # Green circle, filled pizzoo.draw_rectangle((26,
-26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
-pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line pizzoo.draw_line((0,
-31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
-pizzoo.render() ```
+devices, perfect for creating engaging interactive experiences. ## Install Just
+use pip to install the package: ```bash pip install pizzoo ``` That's it!
+Everything should be installed correctly and pizzoo is ready to be used! ##
+Drawing on your device Frame manipulation is the core of the `pizzoo` library.
+Every time the library is created and the `render` method is called, the buffer
+is filled with a new frame we can use to draw on. Lets start by drawing three
+pixels on the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle(
+(31, 31), 10, '#00ff00', filled=True) # Green circle, filled
+pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
+rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
+line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
+rgb color format pizzoo.render() ```
    [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
                                images/qs-2.png]
 ## Creating animations Aside from simple gif drawing (That is also supported),
 custom animations can be created using frame-by-frame manipulation. As an
 example: ```python ''' This will create a simple diagonal moving circle ''' for
 i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
 '#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
```

### Comparing `pizzoo-0.9.5/pizzoo/__init__.py` & `pizzoo-0.9.6/pizzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.5/pizzoo/_constants.py` & `pizzoo-0.9.6/pizzoo/_constants.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.5/pizzoo/_renderers.py` & `pizzoo-0.9.6/pizzoo/_renderers.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.5/pizzoo/_utils.py` & `pizzoo-0.9.6/pizzoo/_utils.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.5/pizzoo/game.py` & `pizzoo-0.9.6/pizzoo/game.py`

 * *Files identical despite different names*

### Comparing `pizzoo-0.9.5/pizzoo.egg-info/PKG-INFO` & `pizzoo-0.9.6/pizzoo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizzoo
-Version: 0.9.5
+Version: 0.9.6
 Summary: Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.
 Home-page: https://github.com/pabletos/pizzoo#readme
 Author: Pablo Huet
 License: MIT
 Keywords: pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED matrix,LED,raspberry,raspberry pi
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics
@@ -54,14 +54,22 @@
 
 * **Flexible integration with any device**:
 	Even with the Pixoo64 being the default target, the Renderer class can be easily extended to support additional methods and integrate with various hardware. This ensures that Pizzoo can adapt to your specific project and hardware requirements.
 
 * **Game Development Toolkit**:
 	Tap into the possibilities of micro game development with our mini game engine. Design, develop, and deploy small-scale games that can be played right on your LED devices, perfect for creating engaging interactive experiences.
 
+## Install
+
+Just use pip to install the package:
+```bash
+pip install pizzoo
+```
+That's it! Everything should be installed correctly and pizzoo is ready to be used!
+
 ## Drawing on your device
 Frame manipulation is the core of the `pizzoo` library. Every time the library is created and the `render` method is called, the buffer is filled with a new frame we can use to draw on. Lets start by drawing three pixels on the screen and rendering:
 
 ```python
 pizzoo.cls()
 pizzoo.draw_circle((31, 31), 10, '#00ff00', filled=True) # Green circle, filled
 pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pizzoo Version: 0.9.5 Summary: Pizzoo is a easy-to-
+Metadata-Version: 2.1 Name: pizzoo Version: 0.9.6 Summary: Pizzoo is a easy-to-
 use library for rendering on pixel matrix screens like the Pixoo64, featuring
 easy new device integration, animation tools, and XML template rendering
 support. Home-page: https://github.com/pabletos/pizzoo#readme Author: Pablo
 Huet License: MIT Keywords:
 pixoo,pixoo64,divoom,screen,pixel,matrix,render,buffer,LED
 matrix,LED,raspberry,raspberry pi Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics Classifier: License :: OSI Approved
@@ -28,24 +28,26 @@
 creating fast and reusable interfaces. * **Flexible integration with any
 device**: Even with the Pixoo64 being the default target, the Renderer class
 can be easily extended to support additional methods and integrate with various
 hardware. This ensures that Pizzoo can adapt to your specific project and
 hardware requirements. * **Game Development Toolkit**: Tap into the
 possibilities of micro game development with our mini game engine. Design,
 develop, and deploy small-scale games that can be played right on your LED
-devices, perfect for creating engaging interactive experiences. ## Drawing on
-your device Frame manipulation is the core of the `pizzoo` library. Every time
-the library is created and the `render` method is called, the buffer is filled
-with a new frame we can use to draw on. Lets start by drawing three pixels on
-the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle((31, 31),
-10, '#00ff00', filled=True) # Green circle, filled pizzoo.draw_rectangle((26,
-26), 11, 11, '#ff0000', filled=False) # Red rectangle, not filled
-pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue line pizzoo.draw_line((0,
-31), (63, 31), (255, 255, 0)) # Yellow line, tuple rgb color format
-pizzoo.render() ```
+devices, perfect for creating engaging interactive experiences. ## Install Just
+use pip to install the package: ```bash pip install pizzoo ``` That's it!
+Everything should be installed correctly and pizzoo is ready to be used! ##
+Drawing on your device Frame manipulation is the core of the `pizzoo` library.
+Every time the library is created and the `render` method is called, the buffer
+is filled with a new frame we can use to draw on. Lets start by drawing three
+pixels on the screen and rendering: ```python pizzoo.cls() pizzoo.draw_circle(
+(31, 31), 10, '#00ff00', filled=True) # Green circle, filled
+pizzoo.draw_rectangle((26, 26), 11, 11, '#ff0000', filled=False) # Red
+rectangle, not filled pizzoo.draw_line((31, 0), (31, 63), '#0000ff') # Blue
+line pizzoo.draw_line((0, 31), (63, 31), (255, 255, 0)) # Yellow line, tuple
+rgb color format pizzoo.render() ```
    [https://raw.githubusercontent.com/pabletos/pizzoo/main/docs/docs/assets/
                                images/qs-2.png]
 ## Creating animations Aside from simple gif drawing (That is also supported),
 custom animations can be created using frame-by-frame manipulation. As an
 example: ```python ''' This will create a simple diagonal moving circle ''' for
 i in range(0, 54): pizzoo.cls() pizzoo.draw_circle((i + 4, i + 4), 2,
 '#00ff00', filled=True) pizzoo.add_frame() pizzoo.render(frame_speed=100) ```
```

### Comparing `pizzoo-0.9.5/setup.py` & `pizzoo-0.9.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup
 
 long_description = open('%s\\README.md' % 'C:\\Users\\Usuario\\Documents\\Projects\\pizzoo', encoding='utf-8').read()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name="pizzoo",
-    version="0.9.5",
+    version="0.9.6",
     author="Pablo Huet",
     description="Pizzoo is a easy-to-use library for rendering on pixel matrix screens like the Pixoo64, featuring easy new device integration, animation tools, and XML template rendering support.",
     long_description=long_description,
 	long_description_content_type='text/markdown',
 	license="MIT",
     keywords="pixoo, pixoo64, divoom, screen, pixel, matrix, render, buffer, LED matrix, LED, raspberry, raspberry pi",
     url="https://github.com/pabletos/pizzoo#readme",
+	include_package_data=True,
     packages=['pizzoo'],
+	package_dir={'pizzoo': 'pizzoo'},
+	package_data={'pizzoo': ['*.bdf']},
     install_requires=[
         'requests ~= 2.31.0',
         'Pillow ~= 10.0.0',
 		'bdfparser ~= 2.2.0'
     ],
 	classifiers=[
         "Development Status :: 4 - Beta",
```

