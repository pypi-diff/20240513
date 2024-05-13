# Comparing `tmp/k1usnsst-23.5.26.tar.gz` & `tmp/k1usnsst-24.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k1usnsst-23.5.26.tar", last modified: Fri May 26 16:42:07 2023, max compression
+gzip compressed data, was "k1usnsst-24.5.13.tar", last modified: Mon May 13 19:38:19 2024, max compression
```

## Comparing `k1usnsst-23.5.26.tar` & `k1usnsst-24.5.13.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1071 2022-03-17 15:01:31.000000 k1usnsst-23.5.26/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3883 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.490455 k1usnsst-23.5.26/k1usnsst/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42473 2023-05-26 16:38:40.000000 k1usnsst-23.5.26/k1usnsst/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.496455 k1usnsst-23.5.26/k1usnsst/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      256 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/cwmacros_sst.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7208 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      216 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30121 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22264 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16248 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/settings.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.498455 k1usnsst-23.5.26/k1usnsst/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.499455 k1usnsst-23.5.26/k1usnsst/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1589 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13810 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3957 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/settings.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.493455 k1usnsst-23.5.26/k1usnsst.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      697 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1125 2023-05-26 16:39:22.000000 k1usnsst-23.5.26/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.136917 k1usnsst-24.5.13/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1071 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4889 2024-05-13 19:38:19.136917 k1usnsst-24.5.13/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4050 2024-05-13 19:36:52.000000 k1usnsst-24.5.13/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.126917 k1usnsst-24.5.13/k1usnsst/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43364 2024-05-13 19:29:28.000000 k1usnsst-24.5.13/k1usnsst/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.132917 k1usnsst-24.5.13/k1usnsst/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      256 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/cwmacros_sst.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7208 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      216 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/k6gte-k1usnsst.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30121 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/k6gte-k1usnsst.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22264 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16839 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/data/settings.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.133917 k1usnsst-24.5.13/k1usnsst/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.135917 k1usnsst-24.5.13/k1usnsst/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1589 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13810 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4190 2024-05-13 19:02:02.000000 k1usnsst-24.5.13/k1usnsst/lib/settings.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-13 19:38:19.135917 k1usnsst-24.5.13/k1usnsst.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4889 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      697 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2024-05-13 19:38:19.000000 k1usnsst-24.5.13/k1usnsst.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1125 2024-05-13 19:32:58.000000 k1usnsst-24.5.13/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-05-13 19:38:19.136917 k1usnsst-24.5.13/setup.cfg
```

### Comparing `k1usnsst-23.5.26/LICENSE` & `k1usnsst-24.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/PKG-INFO` & `k1usnsst-24.5.13/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1usnsst
-Version: 23.5.26
+Version: 24.5.13
 Summary: K1USN SST Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/k1usnsst
 Project-URL: Bug Tracker, https://github.com/mbridak/k1usnsst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt5
+Requires-Dist: requests
+Requires-Dist: xmltodict
 
 # K1USN SST Logger
 
 [![License: GPL v3](https://img.shields.io/github/license/mbridak/Tuner)](https://opensource.org/licenses/MIT)  [![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)  [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)  ![PyPI - Downloads](https://img.shields.io/pypi/dm/k1usnsst)
 
 ## What it is
 
@@ -37,14 +40,15 @@
     - [CAT](#cat)
     - [Enabling CW Interface](#enabling-cw-interface)
   - [CW Macros](#cw-macros)
   - [When the event is over](#when-the-event-is-over)
 
 ## Recent Changes
 
+- Can now send CW via rigctld CAT for those radios that support it.
 - Interface is now resizable
 - Repackaged for PyPi and it now pip installable
 
 ## Installing
 
 In a terminal type:
 
@@ -81,14 +85,16 @@
 
 `sudo apt install flrig`
 
 ### Enabling CW Interface
 
 In the setting screen, switch to the CW tab. Set the host that is running either cwdaemon or PyWinkeyer. Most likely `localhost`. Set the port that the service is listening on. cwdaemon defaults to 6789, Pywinkeyer defaults to 8000. And lastly click the bullet next to the service you will be using.
 
+You can now choose Key via CAT to use rigctld to key the radio, negating the need for a winkeyer.
+
 ![CW settings screen](https://github.com/mbridak/k1usnsst/raw/master/pics/cwsettings.png)
 
 ## CW Macros
 
 The program will check in the current working directory for a file called `cwmacros_sst.txt`. If it is not there it will create one. It will parse the file and configure the new row of 12 buttons along the bottom half of the window. The macros can be activated by either pressing the corresponding function key, or by directly clicking on the button. You can check the file to glean it's structure, but it's pretty straight forward. Each line has 3 sections separated by the pipe `|` character. Here's an example line.
 
 `F3|Run TU|tu {HISNAME} 73 ee`
```

### Comparing `k1usnsst-23.5.26/README.md` & `k1usnsst-24.5.13/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     - [CAT](#cat)
     - [Enabling CW Interface](#enabling-cw-interface)
   - [CW Macros](#cw-macros)
   - [When the event is over](#when-the-event-is-over)
 
 ## Recent Changes
 
+- Can now send CW via rigctld CAT for those radios that support it.
 - Interface is now resizable
 - Repackaged for PyPi and it now pip installable
 
 ## Installing
 
 In a terminal type:
 
@@ -62,14 +63,16 @@
 
 `sudo apt install flrig`
 
 ### Enabling CW Interface
 
 In the setting screen, switch to the CW tab. Set the host that is running either cwdaemon or PyWinkeyer. Most likely `localhost`. Set the port that the service is listening on. cwdaemon defaults to 6789, Pywinkeyer defaults to 8000. And lastly click the bullet next to the service you will be using.
 
+You can now choose Key via CAT to use rigctld to key the radio, negating the need for a winkeyer.
+
 ![CW settings screen](https://github.com/mbridak/k1usnsst/raw/master/pics/cwsettings.png)
 
 ## CW Macros
 
 The program will check in the current working directory for a file called `cwmacros_sst.txt`. If it is not there it will create one. It will parse the file and configure the new row of 12 buttons along the bottom half of the window. The macros can be activated by either pressing the corresponding function key, or by directly clicking on the button. You can check the file to glean it's structure, but it's pretty straight forward. Each line has 3 sections separated by the pipe `|` character. Here's an example line.
 
 `F3|Run TU|tu {HISNAME} 73 ee`
```

### Comparing `k1usnsst-23.5.26/k1usnsst/__main__.py` & `k1usnsst-24.5.13/k1usnsst/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """
 Logger for K1USN SST
 """
 
+import datetime as dt
 import logging
 import os
-import pkgutil
 import re
 import socket
 import sqlite3
 import sys
 import xmlrpc.client
 from datetime import datetime
 from json import dumps, loads
@@ -34,14 +34,15 @@
 
 # pylint: disable=c-extension-no-member
 
 if os.environ.get("XDG_CURRENT_DESKTOP", False) == "GNOME":
     os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
     os.environ["QT_STYLE_OVERRIDE"] = "Adwaita-Dark"
 
+
 def load_fonts_from_dir(directory: str) -> set:
     """
     Well it loads fonts from a directory...
     """
     font_families = set()
     for _fi in QDir(directory).entryInfoList(["*.ttf", "*.woff", "*.woff2"]):
         _id = QFontDatabase.addApplicationFont(_fi.absoluteFilePath())
@@ -105,17 +106,15 @@
     cw = None
     keyerserver = "http://localhost:8000"
     pastcontacts = {}
 
     def __init__(self, *args, **kwargs):
         logging.info("MainWindow: __init__")
         super().__init__(*args, **kwargs)
-        self.working_path = os.path.dirname(
-            pkgutil.get_loader("k1usnsst").get_filename()
-        )
+        self.working_path = os.path.dirname(__loader__.get_filename())
         data_path = self.working_path + "/data/main.ui"
         uic.loadUi(data_path, self)
         self.listWidget.itemDoubleClicked.connect(self.qsoclicked)
         self.mycallEntry.textEdited.connect(self.changemycall)
         self.myexchangeEntry.textEdited.connect(self.changemyexchange)
         self.callsign_entry.textEdited.connect(self.calltest)
         self.callsign_entry.returnPressed.connect(self.log_contact)
@@ -349,23 +348,26 @@
                 except socket.error as exception:
                     self.radio_icon.setPixmap(self.radio_red)
                     logging.warning("poll_radio: flrig: %s", exception)
                 return
             else:
                 self.radio_icon.setPixmap(self.radio_red)
         if self.rigonline:
-            self.rigctrlsocket.settimeout(0.5)
-            self.rigctrlsocket.send(b"f")
-            newfreq = self.rigctrlsocket.recv(1024).decode().strip()
-            self.radio_icon.setPixmap(self.radio_green)
-            self.rigctrlsocket.shutdown(socket.SHUT_RDWR)
-            self.rigctrlsocket.close()
-            if newfreq != self.oldfreq:
-                self.oldfreq = newfreq
-                self.setband(str(self.getband(newfreq)))
+            try:
+                self.rigctrlsocket.settimeout(0.5)
+                self.rigctrlsocket.send(b"f")
+                newfreq = self.rigctrlsocket.recv(1024).decode().strip()
+                self.radio_icon.setPixmap(self.radio_green)
+                self.rigctrlsocket.shutdown(socket.SHUT_RDWR)
+                self.rigctrlsocket.close()
+                if newfreq != self.oldfreq:
+                    self.oldfreq = newfreq
+                    self.setband(str(self.getband(newfreq)))
+            except TimeoutError:
+                ...
 
     def check_radio(self) -> None:
         """
         Checks to see if rigctld daemon is running.
         """
         if not (self.flrig or self.userigctl):
             self.radio_icon.setPixmap(self.radio_grey)
@@ -482,15 +484,36 @@
         if event.key() == Qt.Key_F12:
             self.sendf12()
 
     def sendcw(self, texttosend: str) -> None:
         """
         Sends string to k1el keyer.
         """
-        if self.cw:
+        if (
+            self.userigctl is True
+            and self.rigonline is True
+            and self.settings_dict.get("cwtype", 0) == 3
+        ):
+            try:
+                self.rigctrlsocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                self.rigctrlsocket.connect(
+                    (
+                        self.settings_dict["rigcontrolip"],
+                        int(self.settings_dict["rigcontrolport"]),
+                    )
+                )
+                self.rigctrlsocket.settimeout(0.5)
+                self.rigctrlsocket.send(bytes(f"b{texttosend}\n", "utf-8"))
+                _ = self.rigctrlsocket.recv(1024).decode().strip()
+                self.rigctrlsocket.shutdown(socket.SHUT_RDWR)
+                self.rigctrlsocket.close()
+            except (TimeoutError, BrokenPipeError, OSError) as err:
+                print(err)
+
+        elif self.cw:
             self.cw.sendcw(texttosend)
 
     def sendf1(self) -> None:
         """
         Sends the contents of buttons tool tip
         to the k1el keyer.
         """
@@ -585,15 +608,15 @@
         self.exchange_entry.clear()
         self.callsign_entry.setFocus()
 
     def update_time(self) -> None:
         """
         Update local and UTC time on screen.
         """
-        utcnow = datetime.utcnow().isoformat(" ")[5:19].replace("-", "/")
+        utcnow = datetime.now(dt.timezone.utc).isoformat(" ")[5:19].replace("-", "/")
         self.utctime.setText(utcnow)
 
     def flash(self) -> None:
         """
         Flash the screen to give visual indication of a dupe.
         """
         self.setStyleSheet(
@@ -1039,17 +1062,15 @@
     """
 
     theitem = ""
     database = ""
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.working_path = os.path.dirname(
-            pkgutil.get_loader("k1usnsst").get_filename()
-        )
+        self.working_path = os.path.dirname(__loader__.get_filename())
         data_path = self.working_path + "/data/dialog.ui"
         uic.loadUi(data_path, self)
         self.deleteButton.clicked.connect(self.delete_contact)
         self.buttonBox.accepted.connect(self.save_changes)
         self.change = QSOEdit()
 
     def setup(self, linetopass: str, thedatabase: str) -> None:
@@ -1129,15 +1150,15 @@
         ),
         datefmt="%H:%M:%S",
         level=logging.WARNING,
     )
 
 app = QtWidgets.QApplication(sys.argv)
 app.setStyle("Fusion")
-working_path = os.path.dirname(pkgutil.get_loader("k1usnsst").get_filename())
+working_path = os.path.dirname(__loader__.get_filename())
 font_path = working_path + "/data"
 families = load_fonts_from_dir(os.fspath(font_path))
 logging.info(families)
 window = MainWindow()
 window.show()
 window.create_db()
 window.readpreferences()
@@ -1149,15 +1170,15 @@
 timer.timeout.connect(window.update_time)
 
 
 def run():
     """
     Main Entry
     """
-    PATH = os.path.dirname(pkgutil.get_loader("k1usnsst").get_filename())
+    PATH = os.path.dirname(__loader__.get_filename())
     os.system(
         "xdg-icon-resource install --size 64 --context apps --mode user "
         f"{PATH}/data/k6gte-k1usnsst.png k6gte-k1usnsst"
     )
     os.system(f"xdg-desktop-menu install {PATH}/data/k6gte-k1usnsst.desktop")
     timer.start(1000)
     sys.exit(app.exec())
```

### Comparing `k1usnsst-23.5.26/k1usnsst/data/JetBrainsMono-Regular.ttf` & `k1usnsst-24.5.13/k1usnsst/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/data/dialog.ui` & `k1usnsst-24.5.13/k1usnsst/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.png` & `k1usnsst-24.5.13/k1usnsst/data/k6gte-k1usnsst.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/data/main.ui` & `k1usnsst-24.5.13/k1usnsst/data/main.ui`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/data/settings.ui` & `k1usnsst-24.5.13/k1usnsst/data/settings.ui`

 * *Files 5% similar despite different names*

#### Comparing `k1usnsst-23.5.26/k1usnsst/data/settings.ui` & `k1usnsst-24.5.13/k1usnsst/data/settings.ui`

```diff
@@ -53,15 +53,15 @@
             </attribute>
             <layout class="QFormLayout" name="formLayout">
               <item row="0" column="0">
                 <widget class="QLabel" name="label">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>QRZ Name:</string>
                   </property>
                   <property name="alignment">
@@ -70,29 +70,29 @@
                 </widget>
               </item>
               <item row="0" column="1">
                 <widget class="QLineEdit" name="qrzname_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>W1AW</string>
                   </property>
                 </widget>
               </item>
               <item row="2" column="0">
                 <widget class="QLabel" name="label_2">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>QRZ Password:</string>
                   </property>
                   <property name="alignment">
@@ -101,29 +101,29 @@
                 </widget>
               </item>
               <item row="2" column="1">
                 <widget class="QLineEdit" name="qrzpass_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>Secret</string>
                   </property>
                 </widget>
               </item>
               <item row="4" column="0">
                 <widget class="QLabel" name="label_3">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>QRZ URL:</string>
                   </property>
                   <property name="alignment">
@@ -132,15 +132,15 @@
                 </widget>
               </item>
               <item row="4" column="1">
                 <widget class="QLineEdit" name="qrzurl_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>http://xmldata.qrz.com/xml/</string>
                   </property>
                 </widget>
@@ -158,14 +158,15 @@
                       <widget class="QCheckBox" name="usehamdb_checkBox">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>12</pointsize>
                           </font>
                         </property>
                         <property name="styleSheet">
                           <string notr="true">border: 1px solid red;</string>
                         </property>
                         <property name="text">
                           <string>Use HamDB</string>
@@ -176,15 +177,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QCheckBox" name="useqrz_checkBox">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
-                            <pointsize>11</pointsize>
+                            <pointsize>12</pointsize>
                             <bold>false</bold>
                           </font>
                         </property>
                         <property name="autoFillBackground">
                           <bool>false</bool>
                         </property>
                         <property name="styleSheet">
@@ -222,15 +223,15 @@
                 </widget>
               </item>
               <item row="1" column="0">
                 <widget class="QLabel" name="label_6">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>Host:</string>
                   </property>
                   <property name="alignment">
@@ -239,29 +240,29 @@
                 </widget>
               </item>
               <item row="1" column="1">
                 <widget class="QLineEdit" name="rigcontrolip_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>127.0.0.1</string>
                   </property>
                 </widget>
               </item>
               <item row="3" column="0">
                 <widget class="QLabel" name="label_7">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>Port:</string>
                   </property>
                   <property name="alignment">
@@ -270,15 +271,15 @@
                 </widget>
               </item>
               <item row="3" column="1">
                 <widget class="QLineEdit" name="rigcontrolport_field">
                   <property name="font">
                     <font>
                       <family>JetBrains Mono</family>
-                      <pointsize>11</pointsize>
+                      <pointsize>12</pointsize>
                       <bold>false</bold>
                     </font>
                   </property>
                   <property name="text">
                     <string>4532</string>
                   </property>
                 </widget>
@@ -293,14 +294,15 @@
                   </property>
                   <layout class="QHBoxLayout" name="horizontalLayout">
                     <item>
                       <widget class="QRadioButton" name="radioButton_flrig">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>12</pointsize>
                           </font>
                         </property>
                         <property name="toolTip">
                           <string extracomment="Connect to FLRIG XMLRPC Server"/>
                         </property>
                         <property name="text">
                           <string>FLRIG</string>
@@ -308,14 +310,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QRadioButton" name="radioButton_rigctld">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>12</pointsize>
                           </font>
                         </property>
                         <property name="toolTip">
                           <string extracomment="Connect to rigctld daemon"/>
                         </property>
                         <property name="text">
                           <string>rigcltd</string>
@@ -323,14 +326,15 @@
                       </widget>
                     </item>
                     <item>
                       <widget class="QRadioButton" name="radioButton_none">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
+                            <pointsize>12</pointsize>
                           </font>
                         </property>
                         <property name="toolTip">
                           <string extracomment="Use no rig control"/>
                         </property>
                         <property name="text">
                           <string>None</string>
@@ -440,14 +444,27 @@
                         </property>
                         <property name="text">
                           <string>PyWinkeyer</string>
                         </property>
                       </widget>
                     </item>
                     <item>
+                      <widget class="QRadioButton" name="usecatforcw_radioButton">
+                        <property name="font">
+                          <font>
+                            <family>JetBrains Mono</family>
+                            <pointsize>12</pointsize>
+                          </font>
+                        </property>
+                        <property name="text">
+                          <string>Key via CAT</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
                       <widget class="QRadioButton" name="radioButton_5">
                         <property name="font">
                           <font>
                             <family>JetBrains Mono</family>
                             <pointsize>12</pointsize>
                           </font>
                         </property>
@@ -470,15 +487,15 @@
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
             <font>
               <family>JetBrains Mono</family>
-              <pointsize>11</pointsize>
+              <pointsize>12</pointsize>
               <bold>true</bold>
             </font>
           </property>
           <property name="layoutDirection">
             <enum>Qt::LeftToRight</enum>
           </property>
           <property name="orientation">
```

### Comparing `k1usnsst-23.5.26/k1usnsst/icon/gear16x16.png` & `k1usnsst-24.5.13/k1usnsst/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/icon/radio_green.png` & `k1usnsst-24.5.13/k1usnsst/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/icon/radio_grey.png` & `k1usnsst-24.5.13/k1usnsst/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/icon/radio_red.png` & `k1usnsst-24.5.13/k1usnsst/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/lib/cwinterface.py` & `k1usnsst-24.5.13/k1usnsst/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/lib/lookup.py` & `k1usnsst-24.5.13/k1usnsst/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/k1usnsst/lib/settings.py` & `k1usnsst-24.5.13/k1usnsst/lib/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,14 +53,17 @@
                 self.cwport_field.setText(str(self.settings_dict["cwport"]))
                 self.usecwdaemon_radioButton.setChecked(
                     bool(self.settings_dict["cwtype"] == 1)
                 )
                 self.usepywinkeyer_radioButton.setChecked(
                     bool(self.settings_dict["cwtype"] == 2)
                 )
+                self.usecatforcw_radioButton.setChecked(
+                    bool(self.settings_dict["cwtype"] == 3)
+                )
         except IOError as exception:
             logging.critical("%s", exception)
 
     def save_changes(self) -> None:
         """
         Saves settings to the settings file.
         """
@@ -82,14 +85,16 @@
         self.settings_dict["cwip"] = self.cwip_field.text()
         self.settings_dict["cwport"] = int(self.cwport_field.text())
         self.settings_dict["cwtype"] = 0
         if self.usecwdaemon_radioButton.isChecked():
             self.settings_dict["cwtype"] = 1
         if self.usepywinkeyer_radioButton.isChecked():
             self.settings_dict["cwtype"] = 2
+        if self.usecatforcw_radioButton.isChecked():
+            self.settings_dict["cwtype"] = 3
 
         logging.info(self.settings_dict)
         try:
             home = os.path.expanduser("~")
             with open(
                 home + "/.k1usnsst.json", "wt", encoding="utf-8"
             ) as file_descriptor:
```

### Comparing `k1usnsst-23.5.26/k1usnsst.egg-info/PKG-INFO` & `k1usnsst-24.5.13/k1usnsst.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1usnsst
-Version: 23.5.26
+Version: 24.5.13
 Summary: K1USN SST Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/k1usnsst
 Project-URL: Bug Tracker, https://github.com/mbridak/k1usnsst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt5
+Requires-Dist: requests
+Requires-Dist: xmltodict
 
 # K1USN SST Logger
 
 [![License: GPL v3](https://img.shields.io/github/license/mbridak/Tuner)](https://opensource.org/licenses/MIT)  [![Python: 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)  [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)  ![PyPI - Downloads](https://img.shields.io/pypi/dm/k1usnsst)
 
 ## What it is
 
@@ -37,14 +40,15 @@
     - [CAT](#cat)
     - [Enabling CW Interface](#enabling-cw-interface)
   - [CW Macros](#cw-macros)
   - [When the event is over](#when-the-event-is-over)
 
 ## Recent Changes
 
+- Can now send CW via rigctld CAT for those radios that support it.
 - Interface is now resizable
 - Repackaged for PyPi and it now pip installable
 
 ## Installing
 
 In a terminal type:
 
@@ -81,14 +85,16 @@
 
 `sudo apt install flrig`
 
 ### Enabling CW Interface
 
 In the setting screen, switch to the CW tab. Set the host that is running either cwdaemon or PyWinkeyer. Most likely `localhost`. Set the port that the service is listening on. cwdaemon defaults to 6789, Pywinkeyer defaults to 8000. And lastly click the bullet next to the service you will be using.
 
+You can now choose Key via CAT to use rigctld to key the radio, negating the need for a winkeyer.
+
 ![CW settings screen](https://github.com/mbridak/k1usnsst/raw/master/pics/cwsettings.png)
 
 ## CW Macros
 
 The program will check in the current working directory for a file called `cwmacros_sst.txt`. If it is not there it will create one. It will parse the file and configure the new row of 12 buttons along the bottom half of the window. The macros can be activated by either pressing the corresponding function key, or by directly clicking on the button. You can check the file to glean it's structure, but it's pretty straight forward. Each line has 3 sections separated by the pipe `|` character. Here's an example line.
 
 `F3|Run TU|tu {HISNAME} 73 ee`
```

### Comparing `k1usnsst-23.5.26/k1usnsst.egg-info/SOURCES.txt` & `k1usnsst-24.5.13/k1usnsst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.5.26/pyproject.toml` & `k1usnsst-24.5.13/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "k1usnsst" 
-version = "23.5.26"
+version = "24.5.13"
 description = "K1USN SST Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

