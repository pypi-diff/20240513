# Comparing `tmp/pyqt-toast-notification-1.0.0.tar.gz` & `tmp/pyqt-toast-notification-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-toast-notification-1.0.0.tar", last modified: Thu Mar 21 20:15:38 2024, max compression
+gzip compressed data, was "pyqt-toast-notification-1.1.0.tar", last modified: Mon Apr  8 15:32:56 2024, max compression
```

## Comparing `pyqt-toast-notification-1.0.0.tar` & `pyqt-toast-notification-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.145732 pyqt-toast-notification-1.0.0/
--rw-rw-rw-   0        0        0     1092 2024-02-27 02:46:39.000000 pyqt-toast-notification-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     8071 2024-03-21 20:15:38.145732 pyqt-toast-notification-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7499 2024-03-21 20:13:08.000000 pyqt-toast-notification-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-21 20:15:38.146730 pyqt-toast-notification-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1029 2024-03-21 20:12:05.000000 pyqt-toast-notification-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.128778 pyqt-toast-notification-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.136756 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/
--rw-rw-rw-   0        0        0     8071 2024-03-21 20:15:38.000000 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2024-03-21 20:15:38.000000 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 20:15:38.000000 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-21 20:15:38.000000 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 20:15:38.000000 pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.139748 pyqt-toast-notification-1.0.0/src/pyqttoast/
--rw-rw-rw-   0        0        0       87 2024-03-21 19:04:06.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.140745 pyqt-toast-notification-1.0.0/src/pyqttoast/css/
--rw-rw-rw-   0        0        0      587 2024-03-15 22:29:37.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/css/toast_notification.css
-drwxrwxrwx   0        0        0        0 2024-03-21 20:15:38.144735 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/
--rw-rw-rw-   0        0        0     2628 2024-03-17 21:02:23.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/close.png
--rw-rw-rw-   0        0        0     3446 2024-03-17 20:57:04.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/error.png
--rw-rw-rw-   0        0        0     4016 2024-03-17 21:13:20.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/information.png
--rw-rw-rw-   0        0        0     3301 2024-03-17 20:52:47.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/success.png
--rw-rw-rw-   0        0        0     5976 2024-03-17 21:10:51.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/icons/warning.png
--rw-rw-rw-   0        0        0    76704 2024-03-21 18:54:08.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/toast.py
--rw-rw-rw-   0        0        0      565 2024-03-21 16:14:13.000000 pyqt-toast-notification-1.0.0/src/pyqttoast/toast_enums.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.540202 pyqt-toast-notification-1.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-02-27 02:46:39.000000 pyqt-toast-notification-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8311 2024-04-08 15:32:56.540202 pyqt-toast-notification-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7741 2024-04-08 15:21:28.000000 pyqt-toast-notification-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:32:56.540202 pyqt-toast-notification-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2024-04-08 15:21:04.000000 pyqt-toast-notification-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.521253 pyqt-toast-notification-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.530229 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/
+-rw-rw-rw-   0        0        0     8311 2024-04-08 15:32:56.000000 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-04-08 15:32:56.000000 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:32:56.000000 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 15:32:56.000000 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 15:32:56.000000 pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.533221 pyqt-toast-notification-1.1.0/src/pyqttoast/
+-rw-rw-rw-   0        0        0       87 2024-03-21 19:04:06.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.534219 pyqt-toast-notification-1.1.0/src/pyqttoast/css/
+-rw-rw-rw-   0        0        0      587 2024-03-15 22:29:37.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/css/toast_notification.css
+drwxrwxrwx   0        0        0        0 2024-04-08 15:32:56.538208 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/
+-rw-rw-rw-   0        0        0     2628 2024-03-17 21:02:23.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/close.png
+-rw-rw-rw-   0        0        0     3446 2024-03-17 20:57:04.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/error.png
+-rw-rw-rw-   0        0        0     4016 2024-03-17 21:13:20.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/information.png
+-rw-rw-rw-   0        0        0     3301 2024-03-17 20:52:47.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/success.png
+-rw-rw-rw-   0        0        0     5976 2024-03-17 21:10:51.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/icons/warning.png
+-rw-rw-rw-   0        0        0    77592 2024-04-08 15:21:04.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/toast.py
+-rw-rw-rw-   0        0        0      581 2024-04-08 15:20:25.000000 pyqt-toast-notification-1.1.0/src/pyqttoast/toast_enums.py
```

### Comparing `pyqt-toast-notification-1.0.0/LICENSE` & `pyqt-toast-notification-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/PKG-INFO` & `pyqt-toast-notification-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-toast-notification
-Version: 1.0.0
+Version: 1.1.0
 Summary: A fully customizable toast notification library for PyQt and PySide
 Home-page: https://github.com/niklashenning/pyqt-toast
 Author: Niklas Henning
 Author-email: business@niklashenning.com
 License: MIT
 Keywords: python,pyqt,qt,toast,notification
 Classifier: Programming Language :: Python :: 3
@@ -13,26 +13,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyQt Toast
 
-[![PyPI](https://img.shields.io/badge/pypi-v1.0.0-blue)](https://github.com/niklashenning/pyqt-toast)
+[![PyPI](https://img.shields.io/badge/pypi-v1.1.0-blue)](https://pypi.org/project/pyqt-toast-notification/)
 [![Python](https://img.shields.io/badge/python-3.7+-blue)](https://github.com/niklashenning/pyqt-toast)
-[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE)
 
 A fully customizable and modern toast notification library for PyQt and PySide
 
 ![pyqt-toast](https://github.com/niklashenning/pyqt-toast/assets/58544929/c104f10e-08df-4665-98d8-3785822a20dc)
 
 ## Features
 * Supports showing multiple toasts at the same time
 * Supports queueing of toasts
-* Supports 6 different positions
+* Supports 7 different positions
 * Supports multiple screens
 * Modern and fully customizable UI
 * Works with `PyQt5`, `PyQt6`, `PySide2`, and `PySide6`
 
 ## Installation
 ```
 pip install pyqt-toast-notification
@@ -70,15 +70,15 @@
 
 ## Customization
 
 * **Setting the position of the toasts (<u>static</u>):**
 ```python
 Toast.setPosition(ToastPosition.BOTTOM_MIDDLE)  # Default: ToastPosition.BOTTOM_RIGHT
 ```
-> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`
+> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`, `CENTER`
 
 
 * **Setting a limit on how many toasts can be shown at the same time (<u>static</u>):**
 ```python
 Toast.setMaximumOnScreen(5)  # Default: 3
 ```
 > If you try to show more toasts than the maximum amount on screen, they will get added to a queue and get shown as soon as one of the currently showing toasts is closed.
@@ -115,25 +115,29 @@
 toast.setShowIcon(True)
 
 # Or setting a custom icon:
 toast.setIcon(QPixmap('path/to/your/icon.png'))
 ```
 > **AVAILABLE ICONS:** <br> `SUCCESS`, `WARNING`, `ERROR`, `INFORMATION`, `CLOSE`
 
-* **Settings the icon size:**
+* **Setting the icon size:**
 ```python
 toast.setIconSize(QSize(14, 14))  # Default: QSize(18, 18)
 ```
 
 * **Setting the close button alignment:**
 ```python
 toast.setCloseButtonAlignment(ToastButtonAlignment.MIDDLE)  # Default: ToastButtonAlignment.TOP
 ```
 > **AVAILABLE ALIGNMENTS:** <br> `TOP`, `MIDDLE`, `BOTTOM`
 
+* **Enabling or disabling the close button:**
+```python
+toast.setShowCloseButton(False)  # Default: True
+```
 
 * **Customizing the duration of the fade animations (milliseconds):**
 ```python
 toast.setFadeInDuration(100)   # Default: 250
 toast.setFadeOutDuration(150)  # Default: 250
 ```
 
@@ -208,8 +212,8 @@
 
 ## Demo
 https://github.com/niklashenning/pyqt-toast/assets/58544929/f4d7f4a4-6d69-4087-ae19-da54b6da499d
 
 The demos for PyQt5, PyQt6, and PySide6 can be found in the [demo](demo) folder.
 
 ## License
-This software is licensed under the [MIT license](LICENSE).
+This software is licensed under the [MIT license](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE).
```

### Comparing `pyqt-toast-notification-1.0.0/README.md` & `pyqt-toast-notification-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # PyQt Toast
 
-[![PyPI](https://img.shields.io/badge/pypi-v1.0.0-blue)](https://github.com/niklashenning/pyqt-toast)
+[![PyPI](https://img.shields.io/badge/pypi-v1.1.0-blue)](https://pypi.org/project/pyqt-toast-notification/)
 [![Python](https://img.shields.io/badge/python-3.7+-blue)](https://github.com/niklashenning/pyqt-toast)
-[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE)
 
 A fully customizable and modern toast notification library for PyQt and PySide
 
 ![pyqt-toast](https://github.com/niklashenning/pyqt-toast/assets/58544929/c104f10e-08df-4665-98d8-3785822a20dc)
 
 ## Features
 * Supports showing multiple toasts at the same time
 * Supports queueing of toasts
-* Supports 6 different positions
+* Supports 7 different positions
 * Supports multiple screens
 * Modern and fully customizable UI
 * Works with `PyQt5`, `PyQt6`, `PySide2`, and `PySide6`
 
 ## Installation
 ```
 pip install pyqt-toast-notification
@@ -53,15 +53,15 @@
 
 ## Customization
 
 * **Setting the position of the toasts (<u>static</u>):**
 ```python
 Toast.setPosition(ToastPosition.BOTTOM_MIDDLE)  # Default: ToastPosition.BOTTOM_RIGHT
 ```
-> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`
+> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`, `CENTER`
 
 
 * **Setting a limit on how many toasts can be shown at the same time (<u>static</u>):**
 ```python
 Toast.setMaximumOnScreen(5)  # Default: 3
 ```
 > If you try to show more toasts than the maximum amount on screen, they will get added to a queue and get shown as soon as one of the currently showing toasts is closed.
@@ -98,25 +98,29 @@
 toast.setShowIcon(True)
 
 # Or setting a custom icon:
 toast.setIcon(QPixmap('path/to/your/icon.png'))
 ```
 > **AVAILABLE ICONS:** <br> `SUCCESS`, `WARNING`, `ERROR`, `INFORMATION`, `CLOSE`
 
-* **Settings the icon size:**
+* **Setting the icon size:**
 ```python
 toast.setIconSize(QSize(14, 14))  # Default: QSize(18, 18)
 ```
 
 * **Setting the close button alignment:**
 ```python
 toast.setCloseButtonAlignment(ToastButtonAlignment.MIDDLE)  # Default: ToastButtonAlignment.TOP
 ```
 > **AVAILABLE ALIGNMENTS:** <br> `TOP`, `MIDDLE`, `BOTTOM`
 
+* **Enabling or disabling the close button:**
+```python
+toast.setShowCloseButton(False)  # Default: True
+```
 
 * **Customizing the duration of the fade animations (milliseconds):**
 ```python
 toast.setFadeInDuration(100)   # Default: 250
 toast.setFadeOutDuration(150)  # Default: 250
 ```
 
@@ -191,8 +195,8 @@
 
 ## Demo
 https://github.com/niklashenning/pyqt-toast/assets/58544929/f4d7f4a4-6d69-4087-ae19-da54b6da499d
 
 The demos for PyQt5, PyQt6, and PySide6 can be found in the [demo](demo) folder.
 
 ## License
-This software is licensed under the [MIT license](LICENSE).
+This software is licensed under the [MIT license](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE).
```

### Comparing `pyqt-toast-notification-1.0.0/setup.py` & `pyqt-toast-notification-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as fh:
     readme = "\n" + fh.read()
 
 setup(
     name='pyqt-toast-notification',
-    version='1.0.0',
+    version='1.1.0',
     author='Niklas Henning',
     author_email='business@niklashenning.com',
     license='MIT',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "pyqttoast.css": ["*.css"],
```

### Comparing `pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/PKG-INFO` & `pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-toast-notification
-Version: 1.0.0
+Version: 1.1.0
 Summary: A fully customizable toast notification library for PyQt and PySide
 Home-page: https://github.com/niklashenning/pyqt-toast
 Author: Niklas Henning
 Author-email: business@niklashenning.com
 License: MIT
 Keywords: python,pyqt,qt,toast,notification
 Classifier: Programming Language :: Python :: 3
@@ -13,26 +13,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyQt Toast
 
-[![PyPI](https://img.shields.io/badge/pypi-v1.0.0-blue)](https://github.com/niklashenning/pyqt-toast)
+[![PyPI](https://img.shields.io/badge/pypi-v1.1.0-blue)](https://pypi.org/project/pyqt-toast-notification/)
 [![Python](https://img.shields.io/badge/python-3.7+-blue)](https://github.com/niklashenning/pyqt-toast)
-[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE)
 
 A fully customizable and modern toast notification library for PyQt and PySide
 
 ![pyqt-toast](https://github.com/niklashenning/pyqt-toast/assets/58544929/c104f10e-08df-4665-98d8-3785822a20dc)
 
 ## Features
 * Supports showing multiple toasts at the same time
 * Supports queueing of toasts
-* Supports 6 different positions
+* Supports 7 different positions
 * Supports multiple screens
 * Modern and fully customizable UI
 * Works with `PyQt5`, `PyQt6`, `PySide2`, and `PySide6`
 
 ## Installation
 ```
 pip install pyqt-toast-notification
@@ -70,15 +70,15 @@
 
 ## Customization
 
 * **Setting the position of the toasts (<u>static</u>):**
 ```python
 Toast.setPosition(ToastPosition.BOTTOM_MIDDLE)  # Default: ToastPosition.BOTTOM_RIGHT
 ```
-> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`
+> **AVAILABLE POSITIONS:** <br> `BOTTOM_LEFT`, `BOTTOM_MIDDLE`, `BOTTOM_RIGHT`, `TOP_LEFT`, `TOP_MIDDLE`, `TOP_RIGHT`, `CENTER`
 
 
 * **Setting a limit on how many toasts can be shown at the same time (<u>static</u>):**
 ```python
 Toast.setMaximumOnScreen(5)  # Default: 3
 ```
 > If you try to show more toasts than the maximum amount on screen, they will get added to a queue and get shown as soon as one of the currently showing toasts is closed.
@@ -115,25 +115,29 @@
 toast.setShowIcon(True)
 
 # Or setting a custom icon:
 toast.setIcon(QPixmap('path/to/your/icon.png'))
 ```
 > **AVAILABLE ICONS:** <br> `SUCCESS`, `WARNING`, `ERROR`, `INFORMATION`, `CLOSE`
 
-* **Settings the icon size:**
+* **Setting the icon size:**
 ```python
 toast.setIconSize(QSize(14, 14))  # Default: QSize(18, 18)
 ```
 
 * **Setting the close button alignment:**
 ```python
 toast.setCloseButtonAlignment(ToastButtonAlignment.MIDDLE)  # Default: ToastButtonAlignment.TOP
 ```
 > **AVAILABLE ALIGNMENTS:** <br> `TOP`, `MIDDLE`, `BOTTOM`
 
+* **Enabling or disabling the close button:**
+```python
+toast.setShowCloseButton(False)  # Default: True
+```
 
 * **Customizing the duration of the fade animations (milliseconds):**
 ```python
 toast.setFadeInDuration(100)   # Default: 250
 toast.setFadeOutDuration(150)  # Default: 250
 ```
 
@@ -208,8 +212,8 @@
 
 ## Demo
 https://github.com/niklashenning/pyqt-toast/assets/58544929/f4d7f4a4-6d69-4087-ae19-da54b6da499d
 
 The demos for PyQt5, PyQt6, and PySide6 can be found in the [demo](demo) folder.
 
 ## License
-This software is licensed under the [MIT license](LICENSE).
+This software is licensed under the [MIT license](https://github.com/niklashenning/pyqt-toast/blob/master/LICENSE).
```

### Comparing `pyqt-toast-notification-1.0.0/src/pyqt_toast_notification.egg-info/SOURCES.txt` & `pyqt-toast-notification-1.1.0/src/pyqt_toast_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/css/toast_notification.css` & `pyqt-toast-notification-1.1.0/src/pyqttoast/css/toast_notification.css`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/icons/close.png` & `pyqt-toast-notification-1.1.0/src/pyqttoast/icons/close.png`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/icons/error.png` & `pyqt-toast-notification-1.1.0/src/pyqttoast/icons/error.png`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/icons/information.png` & `pyqt-toast-notification-1.1.0/src/pyqttoast/icons/information.png`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/icons/success.png` & `pyqt-toast-notification-1.1.0/src/pyqttoast/icons/success.png`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/icons/warning.png` & `pyqt-toast-notification-1.1.0/src/pyqttoast/icons/warning.png`

 * *Files identical despite different names*

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/toast.py` & `pyqt-toast-notification-1.1.0/src/pyqttoast/toast.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         self.__show_duration_bar = True
         self.__title = ''
         self.__text = ''
         self.__icon = self.__get_icon_from_enum(ToastIcon.INFORMATION)
         self.__show_icon = False
         self.__icon_size = QSize(18, 18)
         self.__close_button_icon = self.__get_icon_from_enum(ToastIcon.CLOSE)
+        self.__show_close_button = True
         self.__close_button_icon_size = QSize(10, 10)
         self.__close_button_size = QSize(24, 24)
         self.__close_button_alignment = ToastButtonAlignment.TOP
         self.__fade_in_duration = 250
         self.__fade_out_duration = 250
         self.__reset_duration_on_hover = True
         self.__stay_on_top = True
@@ -287,15 +288,16 @@
                 if (Toast.__position == ToastPosition.BOTTOM_RIGHT
                         or Toast.__position == ToastPosition.BOTTOM_LEFT
                         or Toast.__position == ToastPosition.BOTTOM_MIDDLE):
                     self.move(x, y - int(self.height() / 1.5) - predecessor_target_difference_y)
 
                 elif (Toast.__position == ToastPosition.TOP_RIGHT
                       or Toast.__position == ToastPosition.TOP_LEFT
-                      or Toast.__position == ToastPosition.TOP_MIDDLE):
+                      or Toast.__position == ToastPosition.TOP_MIDDLE
+                      or Toast.__position == ToastPosition.CENTER):
                     self.move(x, y + int(self.height() / 1.5) + predecessor_target_difference_y)
 
                 # Start fade down / up animation
                 self.pos_animation = QPropertyAnimation(self, b"pos")
                 self.pos_animation.setEndValue(QPoint(x, y))
                 self.pos_animation.setDuration(self.__fade_in_duration)
                 self.pos_animation.start()
@@ -476,14 +478,23 @@
         elif Toast.__position == ToastPosition.TOP_MIDDLE:
             x = (current_screen.geometry().x()
                  + current_screen.geometry().width() / 2
                  - self.__notification.width() / 2)
             y = (current_screen.geometry().y()
                  + Toast.__offset_y + y_offset)
 
+        elif Toast.__position == ToastPosition.CENTER:
+            x = (current_screen.geometry().x()
+                 + current_screen.geometry().width() / 2
+                 - self.__notification.width() / 2)
+            y = (current_screen.geometry().y()
+                 + current_screen.geometry().height() / 2
+                 - self.__notification.height() / 2
+                 + y_offset)
+
         x = int(x - Toast.__DROP_SHADOW_SIZE)
         y = int(y - Toast.__DROP_SHADOW_SIZE)
 
         return x, y
 
     def __setup_ui(self):
         """Calculate best toast size and place and move everything correctly"""
@@ -518,24 +529,28 @@
                                   + self.__icon_margins.left() + self.__icon_widget.width()
                                   + self.__icon_margins.right() + self.__icon_separator.width()
                                   + self.__icon_section_margins.right())
             icon_section_height = (self.__icon_section_margins.top() + self.__icon_margins.top()
                                    + self.__icon_widget.height() + self.__icon_margins.bottom()
                                    + self.__icon_section_margins.bottom())
 
-        # Calculate height and close button section
-        close_button_section_height = (self.__close_button_margins.top()
-                                       + self.__close_button.height()
-                                       + self.__close_button_margins.bottom())
+        # Calculate close button section height
+        close_button_width = self.__close_button.width() if self.__show_close_button else 0
+        close_button_height = self.__close_button.height() if self.__show_close_button else 0
+        close_button_margins = self.__close_button_margins if self.__show_close_button else QMargins(0, 0, 0, 0)
+
+        close_button_section_height = (close_button_margins.top()
+                                       + close_button_height
+                                       + close_button_margins.bottom())
 
         # Calculate needed width and height
         width = (self.__margins.left() + icon_section_width + self.__text_section_margins.left()
                  + max(title_width, text_width) + self.__text_section_margins.right()
-                 + self.__close_button_margins.left() + self.__close_button.width()
-                 + self.__close_button_margins.right() + self.__margins.right())
+                 + close_button_margins.left() + close_button_width
+                 + close_button_margins.right() + self.__margins.right())
 
         height = (self.__margins.top()
                   + max(icon_section_height, text_section_height, close_button_section_height)
                   + self.__margins.bottom() + duration_bar_height)
 
         forced_additional_height = 0
         forced_reduced_height = 0
@@ -647,16 +662,16 @@
                 # Exit loop if calculated height is less than min height
                 else:
                     break
 
             # Recalculate width
             width = (self.__margins.left() + icon_section_width + self.__text_section_margins.left()
                      + max(title_width, text_width) + self.__text_section_margins.right()
-                     + self.__close_button_margins.left() + self.__close_button.width()
-                     + self.__close_button_margins.right() + self.__margins.right())
+                     + close_button_margins.left() + close_button_width
+                     + close_button_margins.right() + self.__margins.right())
 
             # If min height not met, set height to min height
             if height < self.minimumHeight():
                 forced_additional_height = self.minimumHeight() - height
                 height = self.minimumHeight()
 
         # Handle width less than minimum width
@@ -794,28 +809,32 @@
 
         elif self.__title != '' and self.__text == '':
             self.__title_label.move(self.__title_label.x(),
                                     int((height - title_height - duration_bar_height) / 2))
 
         # Move close button to top, middle, or bottom position
         if self.__close_button_alignment == ToastButtonAlignment.TOP:
-            self.__close_button.move(width - self.__close_button.width()
-                                     - self.__close_button_margins.right() - self.__margins.right(),
-                                     self.__margins.top() + self.__close_button_margins.top())
+            self.__close_button.move(width - close_button_width
+                                     - close_button_margins.right() - self.__margins.right(),
+                                     self.__margins.top() + close_button_margins.top())
         elif self.__close_button_alignment == ToastButtonAlignment.MIDDLE:
-            self.__close_button.move(width - self.__close_button.width()
-                                     - self.__close_button_margins.right() - self.__margins.right(),
-                                     math.ceil((height - self.__close_button.height()
+            self.__close_button.move(width - close_button_width
+                                     - close_button_margins.right() - self.__margins.right(),
+                                     math.ceil((height - close_button_height
                                                - duration_bar_height) / 2))
         elif self.__close_button_alignment == ToastButtonAlignment.BOTTOM:
-            self.__close_button.move(width - self.__close_button.width()
-                                     - self.__close_button_margins.right() - self.__margins.right(),
-                                     height - self.__close_button.height()
+            self.__close_button.move(width - close_button_width
+                                     - close_button_margins.right() - self.__margins.right(),
+                                     height - close_button_height
                                      - self.__margins.bottom()
-                                     - self.__close_button_margins.bottom() - duration_bar_height)
+                                     - close_button_margins.bottom() - duration_bar_height)
+
+        # Hide close button if disabled
+        if not self.__show_close_button:
+            self.__close_button.setVisible(False)
 
         # Resize, move, and show duration bar if enabled
         if self.__show_duration_bar:
             self.__duration_bar_container.setFixedWidth(width)
             self.__duration_bar_container.move(0, height - duration_bar_height)
             self.__duration_bar.setFixedWidth(width)
             self.__duration_bar_chunk.setFixedWidth(width)
@@ -927,15 +946,15 @@
 
         :return: whether the icon is enabled
         """
 
         return self.__show_icon
 
     def setShowIcon(self, on: bool):
-        """Get whether the icon should be shown
+        """Set whether the icon should be shown
 
         :param on: whether the icon should be shown
         """
 
         if self.__used:
             return
         self.__show_icon = on
@@ -982,14 +1001,32 @@
             self.__close_button_icon = self.__get_icon_from_enum(icon)
         else:
             self.__close_button_icon = icon
 
         self.__close_button.setIcon(QIcon(self.__close_button_icon))
         self.setCloseButtonIconColor(self.__close_button_icon_color)
 
+    def isShowCloseButton(self) -> bool:
+        """Get whether the close button is enabled
+
+        :return: whether the close button is enabled
+        """
+
+        return self.__show_close_button
+
+    def setShowCloseButton(self, show: bool):
+        """Set whether the close button should be shown
+
+        :param show: whether the close button should be shown
+        """
+
+        if self.__used:
+            return
+        self.__show_close_button = show
+
     def getCloseButtonIconSize(self) -> QSize:
         """Get the size of the close button icon
 
         :return: size
         """
 
         return self.__close_button_icon_size
@@ -1255,16 +1292,14 @@
 
         if self.__used:
             return
 
         self.__icon_color = color
         recolored_image = self.__recolor_image(self.__icon_widget.icon().pixmap(
                                                self.__icon_widget.iconSize()).toImage(),
-                                               self.__icon_widget.iconSize().width(),
-                                               self.__icon_widget.iconSize().height(),
                                                color)
         self.__icon_widget.setIcon(QIcon(QPixmap(recolored_image)))
 
     def getIconSeparatorColor(self) -> QColor:
         """Get the color of the icon separator
 
         :return: new color
@@ -1298,16 +1333,14 @@
 
         if self.__used:
             return
 
         self.__close_button_icon_color = color
         recolored_image = self.__recolor_image(self.__close_button.icon().pixmap(
                                                self.__close_button.iconSize()).toImage(),
-                                               self.__close_button.iconSize().width(),
-                                               self.__close_button.iconSize().height(),
                                                color)
         self.__close_button.setIcon(QIcon(QPixmap(recolored_image)))
 
     def getDurationBarColor(self) -> QColor:
         """Get the color of the duration bar
 
         :return: color
@@ -1940,27 +1973,25 @@
         """Show next toast in queue"""
 
         if len(Toast.__queue) > 0:
             next_toast = Toast.__queue.pop(0)
             next_toast.show()
 
     @staticmethod
-    def __recolor_image(image: QImage, width: int, height: int, color: QColor):
+    def __recolor_image(image: QImage, color: QColor):
         """Take an image and return a copy with the colors changed
 
         :param image: image to recolor
-        :param width: width of the image
-        :param height: height of the image
         :param color: new color
         :return: recolored image
         """
 
         # Loop through every pixel
-        for x in range(0, width):
-            for y in range(0, height):
+        for x in range(0, image.width()):
+            for y in range(0, image.height()):
                 # Get current color of the pixel
                 current_color = image.pixelColor(x, y)
                 # Replace the rgb values with rgb of new color and keep alpha the same
                 new_color_r = color.red()
                 new_color_g = color.green()
                 new_color_b = color.blue()
                 new_color = QColor.fromRgba(
@@ -2136,15 +2167,16 @@
         """
 
         if (position == ToastPosition.BOTTOM_RIGHT
                 or position == ToastPosition.BOTTOM_LEFT
                 or position == ToastPosition.BOTTOM_MIDDLE
                 or position == ToastPosition.TOP_RIGHT
                 or position == ToastPosition.TOP_LEFT
-                or position == ToastPosition.TOP_MIDDLE):
+                or position == ToastPosition.TOP_MIDDLE
+                or position == ToastPosition.CENTER):
             Toast.__position = position
             Toast.__update_currently_showing_position_xy()
 
     @staticmethod
     def getCount() -> int:
         """Get the amount of toasts that are either currently visible
         or queued to be shown
```

### Comparing `pyqt-toast-notification-1.0.0/src/pyqttoast/toast_enums.py` & `pyqt-toast-notification-1.1.0/src/pyqttoast/toast_enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 class ToastPosition(Enum):
     BOTTOM_LEFT = 1
     BOTTOM_MIDDLE = 2
     BOTTOM_RIGHT = 3
     TOP_LEFT = 4
     TOP_MIDDLE = 5
     TOP_RIGHT = 6
+    CENTER = 7
 
 
 class ToastButtonAlignment(Enum):
     TOP = 1
     MIDDLE = 2
     BOTTOM = 3
```

