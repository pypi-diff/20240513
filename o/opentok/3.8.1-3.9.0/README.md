# Comparing `tmp/opentok-3.8.1.tar.gz` & `tmp/opentok-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opentok-3.8.1.tar", last modified: Fri Sep  8 12:31:15 2023, max compression
+gzip compressed data, was "dist/opentok-3.9.0.tar", last modified: Mon May 13 13:02:37 2024, max compression
```

## Comparing `opentok-3.8.1.tar` & `opentok-3.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-09-08 12:31:15.000000 opentok-3.8.1/
--rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.8.1/LICENSE.txt
--rw-r--r--   0 mkahan     (503) staff       (20)    28901 2023-09-08 12:31:15.000000 opentok-3.8.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)    27596 2023-09-07 13:19:01.000000 opentok-3.8.1/README.rst
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok/
--rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.8.1/opentok/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.8.1/opentok/archives.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4407 2023-08-21 14:54:23.000000 opentok-3.8.1/opentok/broadcast.py
--rw-r--r--   0 mkahan     (503) staff       (20)      368 2023-09-07 13:19:01.000000 opentok-3.8.1/opentok/captions.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6479 2023-09-07 13:19:01.000000 opentok-3.8.1/opentok/endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3462 2023-09-07 13:19:01.000000 opentok-3.8.1/opentok/exceptions.py
--rw-r--r--   0 mkahan     (503) staff       (20)   101640 2023-09-08 12:24:47.000000 opentok-3.8.1/opentok/opentok.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.8.1/opentok/render.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.8.1/opentok/session.py
--rw-r--r--   0 mkahan     (503) staff       (20)      446 2023-08-16 22:53:58.000000 opentok-3.8.1/opentok/sip_call.py
--rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.8.1/opentok/stream.py
--rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.8.1/opentok/streamlist.py
--rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-09-08 12:28:17.000000 opentok-3.8.1/opentok/version.py
--rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.8.1/opentok/websocket_audio_connection.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)    28901 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      492 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-09-08 12:31:15.000000 opentok-3.8.1/opentok.egg-info/top_level.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-09-08 12:31:15.000000 opentok-3.8.1/setup.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.8.1/setup.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-13 13:02:37.000000 opentok-3.9.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.9.0/LICENSE.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)    30107 2024-05-13 13:02:37.000000 opentok-3.9.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)    28802 2024-01-12 03:41:40.000000 opentok-3.9.0/README.rst
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok/
+-rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.9.0/opentok/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.9.0/opentok/archives.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4407 2023-08-21 14:54:23.000000 opentok-3.9.0/opentok/broadcast.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      368 2023-09-07 13:19:01.000000 opentok-3.9.0/opentok/captions.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     6479 2023-09-07 13:19:01.000000 opentok-3.9.0/opentok/endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3462 2023-09-07 13:19:01.000000 opentok-3.9.0/opentok/exceptions.py
+-rw-r--r--   0 mkahan     (503) staff       (20)   101864 2024-05-13 13:00:43.000000 opentok-3.9.0/opentok/opentok.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.9.0/opentok/render.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.9.0/opentok/session.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      446 2023-08-16 22:53:58.000000 opentok-3.9.0/opentok/sip_call.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.9.0/opentok/stream.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.9.0/opentok/streamlist.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      101 2024-05-13 13:00:43.000000 opentok-3.9.0/opentok/version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.9.0/opentok/websocket_audio_connection.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)    30107 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      492 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       39 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        8 2024-05-13 13:02:37.000000 opentok-3.9.0/opentok.egg-info/top_level.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      103 2024-05-13 13:02:37.000000 opentok-3.9.0/setup.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.9.0/setup.py
```

### Comparing `opentok-3.8.1/LICENSE.txt` & `opentok-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/PKG-INFO` & `opentok-3.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: opentok
-Version: 3.8.1
-Summary: OpenTok server-side SDK
-Home-page: https://github.com/opentok/Opentok-Python-SDK/
-Author: TokBox, Inc.
-Author-email: support@tokbox.com
-License: LICENSE.txt
-Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Communications
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Communications :: Conferencing
-Classifier: Topic :: Multimedia :: Video :: Capture
-Classifier: Topic :: Multimedia :: Video :: Display
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
-Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
 ==================
 OpenTok Python SDK
 ==================
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg 
    :target: CODE_OF_CONDUCT.md
 
@@ -40,14 +10,26 @@
    :alt: Tokbox is now known as Vonage
 
 The OpenTok Python SDK lets you generate
 `sessions <http://tokbox.com/opentok/tutorials/create-session/>`_ and
 `tokens <http://tokbox.com/opentok/tutorials/create-token/>`_ for `OpenTok <http://www.tokbox.com/>`_
 applications, and `archive <http://www.tokbox.com/platform/archiving>`_ OpenTok sessions.
 
+Note!
+-----
+
+This library is designed to work with the Tokbox/OpenTok platform, part of the Vonage Video API. If you are looking to use the Vonage Video API and are using the Vonage Customer Dashboard, you will want to install the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_, which includes support for the Vonage Video API.
+
+Not sure which exact platform you are using? Take a look at `this guide <https://api.support.vonage.com/hc/en-us/articles/10817774782492>`_.
+
+If you are using the Tokbox platform, do not worry! The Tokbox platform is not going away, and this library will continue to be updated. While we encourage customers to check out the new Unified platform, there is no rush to switch. Both platforms run the exact same infrastructure and capabilities. The main difference is a unified billing interface and easier access to `Vonage's other CPaaS APIs <https://www.vonage.com/communications-apis/>`_.
+
+If you are new to the Vonage Video API, head on over to the `Vonage Customer Dashboard <https://dashboard.vonage.com>`_ to sign up for a developer account and check out the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_. 
+
+
 Installation using Pip (recommended):
 -------------------------------------
 
 Pip helps manage dependencies for Python projects using the PyPI index. Find more info here:
 http://www.pip-installer.org/en/latest/
 
 Add the ``opentok`` package as a dependency in your project. The most common way is to add it to your
```

### Comparing `opentok-3.8.1/README.rst` & `opentok-3.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: opentok
+Version: 3.9.0
+Summary: OpenTok server-side SDK
+Home-page: https://github.com/opentok/Opentok-Python-SDK/
+Author: TokBox, Inc.
+Author-email: support@tokbox.com
+License: LICENSE.txt
+Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Communications :: Conferencing
+Classifier: Topic :: Multimedia :: Video :: Capture
+Classifier: Topic :: Multimedia :: Video :: Display
+Classifier: Topic :: Multimedia :: Sound/Audio :: Players
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 ==================
 OpenTok Python SDK
 ==================
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg 
    :target: CODE_OF_CONDUCT.md
 
@@ -10,14 +40,26 @@
    :alt: Tokbox is now known as Vonage
 
 The OpenTok Python SDK lets you generate
 `sessions <http://tokbox.com/opentok/tutorials/create-session/>`_ and
 `tokens <http://tokbox.com/opentok/tutorials/create-token/>`_ for `OpenTok <http://www.tokbox.com/>`_
 applications, and `archive <http://www.tokbox.com/platform/archiving>`_ OpenTok sessions.
 
+Note!
+-----
+
+This library is designed to work with the Tokbox/OpenTok platform, part of the Vonage Video API. If you are looking to use the Vonage Video API and are using the Vonage Customer Dashboard, you will want to install the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_, which includes support for the Vonage Video API.
+
+Not sure which exact platform you are using? Take a look at `this guide <https://api.support.vonage.com/hc/en-us/articles/10817774782492>`_.
+
+If you are using the Tokbox platform, do not worry! The Tokbox platform is not going away, and this library will continue to be updated. While we encourage customers to check out the new Unified platform, there is no rush to switch. Both platforms run the exact same infrastructure and capabilities. The main difference is a unified billing interface and easier access to `Vonage's other CPaaS APIs <https://www.vonage.com/communications-apis/>`_.
+
+If you are new to the Vonage Video API, head on over to the `Vonage Customer Dashboard <https://dashboard.vonage.com>`_ to sign up for a developer account and check out the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_. 
+
+
 Installation using Pip (recommended):
 -------------------------------------
 
 Pip helps manage dependencies for Python projects using the PyPI index. Find more info here:
 http://www.pip-installer.org/en/latest/
 
 Add the ``opentok`` package as a dependency in your project. The most common way is to add it to your
```

### Comparing `opentok-3.8.1/opentok/__init__.py` & `opentok-3.9.0/opentok/__init__.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/archives.py` & `opentok-3.9.0/opentok/archives.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/broadcast.py` & `opentok-3.9.0/opentok/broadcast.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/endpoints.py` & `opentok-3.9.0/opentok/endpoints.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/exceptions.py` & `opentok-3.9.0/opentok/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/opentok.py` & `opentok-3.9.0/opentok/opentok.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 class Roles(Enum):
     """List of valid roles for a token."""
 
     subscriber = u("subscriber")
     """A subscriber can only subscribe to streams."""
     publisher = u("publisher")
     """A publisher can publish streams, subscribe to streams, and signal"""
+    publisher_only = "publisheronly"
+    """A client with the `publisher_only` role can only publish streams. It cannot subscribe to 
+    other clients' streams or send signals."""
     moderator = u("moderator")
     """In addition to the privileges granted to a publisher, a moderator can perform
     moderation functions, such as forcing clients to disconnect, to stop publishing streams,
     or to mute audio in published streams. See the
     `Moderation developer guide <https://tokbox.com/developer/guides/moderation/>`_
     """
 
@@ -102,15 +105,14 @@
     "1080x1920",
 }
 
 logger = logging.getLogger("opentok")
 
 
 class Client(object):
-
     """Use this SDK to create tokens and interface with the server-side portion
     of the Opentok API.
     """
 
     TOKEN_SENTINEL = "T1=="
     """For internal use."""
 
@@ -183,14 +185,17 @@
           class:
 
           * `Roles.subscriber` -- A subscriber can only subscribe to streams.
 
           * `Roles.publisher` -- A publisher can publish streams, subscribe to
             streams, and signal. (This is the default value if you do not specify a role.)
 
+          * `Roles.publisher_only` -- A client with the `publisher_only` role can only publish streams.
+            It cannot subscribe to other clients' streams or send signals.
+
           * `Roles.moderator` -- In addition to the privileges granted to a
             publisher, in clients using the OpenTok.js 2.2 library, a moderator can call the
             `forceUnpublish()` and `forceDisconnect()` method of the
             Session object.
 
         :param int expire_time: The expiration time of the token, in seconds since the UNIX epoch.
           The maximum expiration time is 30 days after the creation time. The default expiration
@@ -495,17 +500,15 @@
                     "Failed to create session (code=%s): %s"
                     % (
                         error.attributes["code"].value,
                         error.firstChild.attributes["message"].value,
                     )
                 )
 
-            session_id = (
-                dom.getElementsByTagName("session_id")[0].childNodes[0].nodeValue
-            )
+            session_id = dom.getElementsByTagName("session_id")[0].childNodes[0].nodeValue
             return Session(
                 self,
                 session_id,
                 location=location,
                 media_mode=media_mode,
                 archive_mode=archive_mode,
                 e2ee=e2ee,
@@ -886,17 +889,15 @@
                     "Your archive is configured with a streamMode that does not support stream manipulation."
                 )
             elif response.status_code == 409:
                 raise ArchiveError(response.json().get("message"))
         else:
             raise RequestError("An unexpected error occurred.", response.status_code)
 
-    def remove_archive_stream(
-        self, archive_id: str, stream_id: str
-    ) -> requests.Response:
+    def remove_archive_stream(self, archive_id: str, stream_id: str) -> requests.Response:
         """
         This method will remove streams from the archive with removeStream.
 
         :param String archive_id: the ID of the archive that will be updated
         :param String stream_id: the ID of the stream that will get added to the archive
         """
 
@@ -1335,17 +1336,15 @@
                 "is invalid JSON. It may also indicate that you passed in invalid layout options."
             )
         elif response.status_code == 403:
             raise AuthError("Authentication error.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
-    def start_broadcast(
-        self, session_id, options, stream_mode=BroadcastStreamModes.auto
-    ):
+    def start_broadcast(self, session_id, options, stream_mode=BroadcastStreamModes.auto):
         """
         Use this method to start a live streaming broadcast for an OpenTok session. This broadcasts
         the session to an HLS (HTTP live streaming) or to RTMP streams. To successfully start
         broadcasting a session, at least one client must be connected to the session. You can only
         start live streaming for sessions that use the OpenTok Media Router (with the media mode set
         to routed); you cannot use live streaming with sessions that have the media mode set to
         relayed
@@ -1572,17 +1571,15 @@
             elif response.status_code == 403:
                 raise AuthError("Authentication error.")
             elif response.status_code == 405:
                 raise BroadcastStreamModeError(
                     "Your broadcast is configured with a streamMode that does not support stream manipulation."
                 )
             elif response.status_code == 409:
-                raise BroadcastError(
-                    "The broadcast has already started for the session."
-                )
+                raise BroadcastError("The broadcast has already started for the session.")
         else:
             raise RequestError("An unexpected error occurred.", response.status_code)
 
     def remove_broadcast_stream(
         self, broadcast_id: str, stream_id: str
     ) -> requests.Response:
         """
@@ -1617,17 +1614,15 @@
             elif response.status_code == 403:
                 raise AuthError("Authentication error.")
             elif response.status_code == 405:
                 raise BroadcastStreamModeError(
                     "Your broadcast is configured with a streamMode that does not support stream manipulation."
                 )
             elif response.status_code == 409:
-                raise BroadcastError(
-                    "The broadcast has already started for the session."
-                )
+                raise BroadcastError("The broadcast has already started for the session.")
         else:
             raise RequestError("OpenTok server error.", response.status_code)
 
     def get_broadcast(self, broadcast_id):
         """
         Use this method to get details on a broadcast that is in-progress.
```

### Comparing `opentok-3.8.1/opentok/render.py` & `opentok-3.9.0/opentok/render.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/session.py` & `opentok-3.9.0/opentok/session.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/stream.py` & `opentok-3.9.0/opentok/stream.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/streamlist.py` & `opentok-3.9.0/opentok/streamlist.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok/websocket_audio_connection.py` & `opentok-3.9.0/opentok/websocket_audio_connection.py`

 * *Files identical despite different names*

### Comparing `opentok-3.8.1/opentok.egg-info/PKG-INFO` & `opentok-3.9.0/opentok.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.8.1
+Version: 3.9.0
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,14 +40,26 @@
    :alt: Tokbox is now known as Vonage
 
 The OpenTok Python SDK lets you generate
 `sessions <http://tokbox.com/opentok/tutorials/create-session/>`_ and
 `tokens <http://tokbox.com/opentok/tutorials/create-token/>`_ for `OpenTok <http://www.tokbox.com/>`_
 applications, and `archive <http://www.tokbox.com/platform/archiving>`_ OpenTok sessions.
 
+Note!
+-----
+
+This library is designed to work with the Tokbox/OpenTok platform, part of the Vonage Video API. If you are looking to use the Vonage Video API and are using the Vonage Customer Dashboard, you will want to install the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_, which includes support for the Vonage Video API.
+
+Not sure which exact platform you are using? Take a look at `this guide <https://api.support.vonage.com/hc/en-us/articles/10817774782492>`_.
+
+If you are using the Tokbox platform, do not worry! The Tokbox platform is not going away, and this library will continue to be updated. While we encourage customers to check out the new Unified platform, there is no rush to switch. Both platforms run the exact same infrastructure and capabilities. The main difference is a unified billing interface and easier access to `Vonage's other CPaaS APIs <https://www.vonage.com/communications-apis/>`_.
+
+If you are new to the Vonage Video API, head on over to the `Vonage Customer Dashboard <https://dashboard.vonage.com>`_ to sign up for a developer account and check out the `Vonage Server SDK for Python <https://github.com/Vonage/vonage-python-sdk>`_. 
+
+
 Installation using Pip (recommended):
 -------------------------------------
 
 Pip helps manage dependencies for Python projects using the PyPI index. Find more info here:
 http://www.pip-installer.org/en/latest/
 
 Add the ``opentok`` package as a dependency in your project. The most common way is to add it to your
```

### Comparing `opentok-3.8.1/setup.py` & `opentok-3.9.0/setup.py`

 * *Files identical despite different names*

