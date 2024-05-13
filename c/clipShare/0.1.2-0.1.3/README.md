# Comparing `tmp/clipShare-0.1.2.tar.gz` & `tmp/clipshare-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipShare-0.1.2.tar", last modified: Wed Dec  6 08:24:39 2023, max compression
+gzip compressed data, was "clipshare-0.1.3.tar", last modified: Mon May 13 18:22:39 2024, max compression
```

## Comparing `clipShare-0.1.2.tar` & `clipshare-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.975617 clipShare-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2023-12-06 08:24:27.000000 clipShare-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-06 08:24:27.000000 clipShare-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-12-06 08:24:39.975617 clipShare-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-06 08:24:27.000000 clipShare-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.971616 clipShare-0.1.2/clipShare/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30995 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/clipShare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.971616 clipShare-0.1.2/clipShare/web-interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.971616 clipShare-0.1.2/clipShare/web-interface/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.975617 clipShare-0.1.2/clipShare/web-interface/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    73502 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/static/images/clipShare.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/static/images/help.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.975617 clipShare-0.1.2/clipShare/web-interface/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48316 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/static/js/crypto-js.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   185790 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/static/js/socket.io.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.975617 clipShare-0.1.2/clipShare/web-interface/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2023-12-06 08:24:27.000000 clipShare-0.1.2/clipShare/web-interface/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:24:39.975617 clipShare-0.1.2/clipShare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-06 08:24:39.000000 clipShare-0.1.2/clipShare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 08:24:39.975617 clipShare-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-06 08:24:27.000000 clipShare-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.784519 clipshare-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-13 18:22:20.000000 clipshare-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 18:22:20.000000 clipshare-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-13 18:22:39.784519 clipshare-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-13 18:22:20.000000 clipshare-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.780519 clipshare-0.1.3/clipShare/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30995 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/clipShare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.780519 clipshare-0.1.3/clipShare/web-interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.780519 clipshare-0.1.3/clipShare/web-interface/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.780519 clipshare-0.1.3/clipShare/web-interface/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    73502 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/static/images/clipShare.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/static/images/help.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.780519 clipshare-0.1.3/clipShare/web-interface/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/static/js/crypto-js.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   185790 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/static/js/socket.io.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.784519 clipshare-0.1.3/clipShare/web-interface/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-13 18:22:20.000000 clipshare-0.1.3/clipShare/web-interface/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:39.784519 clipshare-0.1.3/clipShare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 18:22:39.000000 clipshare-0.1.3/clipShare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:22:39.784519 clipshare-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-13 18:22:20.000000 clipshare-0.1.3/setup.py
```

### Comparing `clipShare-0.1.2/LICENSE` & `clipshare-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/PKG-INFO` & `clipshare-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipShare
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sync clipboard between devices
 Home-page: https://github.com/avinashkarhana/clipShare
 Author: Avinash Karhana
 Author-email: avinashkarhana1@gmail.com
 License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console
@@ -26,19 +26,21 @@
 Requires-Dist: Flask-SocketIO
 Requires-Dist: python-socketio
 Requires-Dist: pyclip
 Requires-Dist: pyperclip
 Requires-Dist: pycryptodome
 Requires-Dist: requests
 Requires-Dist: pyngrok
-Requires-Dist: netifaces
+Requires-Dist: netifaces2
 Requires-Dist: zeroconf
 
 # clipShare
-[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml)
+[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml)
+
+*Check the PyPi Package [here](https://pypi.org/project/clipShare/)*
 
 A single TCP server/client bundle that allows you to sync your clipboard between systems.
 
 ## Features
 1. Sync clipboard between systems.
 2. Has a Web UI. `Server IP:Port` or `ngrok-tunnel-host`
     - To view clipboard on mobile devices.
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: clipShare Version: 0.1.2 Summary: Sync clipboard
+Metadata-Version: 2.1 Name: clipShare Version: 0.1.3 Summary: Sync clipboard
 between devices Home-page: https://github.com/avinashkarhana/clipShare Author:
 Avinash Karhana Author-email: avinashkarhana1@gmail.com License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 (LGPLv2) Classifier: Natural Language :: English Classifier:
 Operating System :: Microsoft :: Windows :: Windows 10 Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Communications Classifier: Topic :: Internet Classifier:
 Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: flask Requires-Dist: Flask-
 SocketIO Requires-Dist: python-socketio Requires-Dist: pyclip Requires-Dist:
 pyperclip Requires-Dist: pycryptodome Requires-Dist: requests Requires-Dist:
-pyngrok Requires-Dist: netifaces Requires-Dist: zeroconf # clipShare [![Publish
-Python Package to PyPi](https://github.com/avinashkarhana/clipboardSync/
+pyngrok Requires-Dist: netifaces2 Requires-Dist: zeroconf # clipShare [!
+[Publish Python Package to PyPi](https://github.com/avinashkarhana/clipShare/
 actions/workflows/python-publish.yml/badge.svg)](https://github.com/
-avinashkarhana/clipboardSync/actions/workflows/python-publish.yml) A single TCP
-server/client bundle that allows you to sync your clipboard between systems. ##
-Features 1. Sync clipboard between systems. 2. Has a Web UI. `Server IP:Port`
-or `ngrok-tunnel-host` - To view clipboard on mobile devices. - To sync
-clipboard if not using the Python client. 2. Advertise the server on the local
-network. 3. Authentication using passcode. (Passcode should be shared via some
-external safe channel) 5. Scan for servers on the local network. 6. The same
-script can be used as a server or client. 7. Encrypted communication for
-clipboard sharing with AES Encryption (Key should be shared via some external
-safe channel) ## Installation pip install clipShare ## Usage Usage: clipShare
-[... OPTIONS] Options: -h, --help Show this help message and exit -s, --server
+avinashkarhana/clipShare/actions/workflows/python-publish.yml) *Check the PyPi
+Package [here](https://pypi.org/project/clipShare/)* A single TCP server/client
+bundle that allows you to sync your clipboard between systems. ## Features 1.
+Sync clipboard between systems. 2. Has a Web UI. `Server IP:Port` or `ngrok-
+tunnel-host` - To view clipboard on mobile devices. - To sync clipboard if not
+using the Python client. 2. Advertise the server on the local network. 3.
+Authentication using passcode. (Passcode should be shared via some external
+safe channel) 5. Scan for servers on the local network. 6. The same script can
+be used as a server or client. 7. Encrypted communication for clipboard sharing
+with AES Encryption (Key should be shared via some external safe channel) ##
+Installation pip install clipShare ## Usage Usage: clipShare [... OPTIONS]
+Options: -h, --help Show this help message and exit -s, --server
 [SERVER_PORT_NUMER], --server [SERVER_PORT_NUMER] Run as server on the
 specified port. -c, --client SERVER_IP:SERVER_PORT_NUMBER, --client SERVER_IP:
 SERVER_PORT_NUMBER Run as a client, that connects to specified server IP and
 port. -t, --serve-on-ngrok-tunnel Enable Serve on ngrok tunnel. This option
 requires ngrok authtoken to be present in {current_dir}/ngrok-auth-token.txt -
 a, --advertise Enable Advertising server on the local network. -n, --name Name
 of the server to be advertised. -p, --passcode Passcode for authentication. -
```

### Comparing `clipShare-0.1.2/README.md` & `clipshare-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # clipShare
-[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml)
+[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml)
+
+*Check the PyPi Package [here](https://pypi.org/project/clipShare/)*
 
 A single TCP server/client bundle that allows you to sync your clipboard between systems.
 
 ## Features
 1. Sync clipboard between systems.
 2. Has a Web UI. `Server IP:Port` or `ngrok-tunnel-host`
     - To view clipboard on mobile devices.
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 # clipShare [![Publish Python Package to PyPi](https://github.com/
-avinashkarhana/clipboardSync/actions/workflows/python-publish.yml/badge.svg)]
-(https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-
-publish.yml) A single TCP server/client bundle that allows you to sync your
-clipboard between systems. ## Features 1. Sync clipboard between systems. 2.
-Has a Web UI. `Server IP:Port` or `ngrok-tunnel-host` - To view clipboard on
-mobile devices. - To sync clipboard if not using the Python client. 2.
-Advertise the server on the local network. 3. Authentication using passcode.
-(Passcode should be shared via some external safe channel) 5. Scan for servers
-on the local network. 6. The same script can be used as a server or client. 7.
-Encrypted communication for clipboard sharing with AES Encryption (Key should
-be shared via some external safe channel) ## Installation pip install clipShare
-## Usage Usage: clipShare [... OPTIONS] Options: -h, --help Show this help
-message and exit -s, --server [SERVER_PORT_NUMER], --server [SERVER_PORT_NUMER]
-Run as server on the specified port. -c, --client SERVER_IP:SERVER_PORT_NUMBER,
---client SERVER_IP:SERVER_PORT_NUMBER Run as a client, that connects to
-specified server IP and port. -t, --serve-on-ngrok-tunnel Enable Serve on ngrok
-tunnel. This option requires ngrok authtoken to be present in {current_dir}/
-ngrok-auth-token.txt -a, --advertise Enable Advertising server on the local
-network. -n, --name Name of the server to be advertised. -p, --passcode
-Passcode for authentication. -ep, --encryption-password Encryption password for
-data transfer. -toh, --tcp-over-https Enable TCP over HTTPS for ngrok tunnel. -
-d, --debug Enable debug mode. Examples: clipShare -s 5000 clipShare -s 5000 -
+avinashkarhana/clipShare/actions/workflows/python-publish.yml/badge.svg)]
+(https://github.com/avinashkarhana/clipShare/actions/workflows/python-
+publish.yml) *Check the PyPi Package [here](https://pypi.org/project/clipShare/
+)* A single TCP server/client bundle that allows you to sync your clipboard
+between systems. ## Features 1. Sync clipboard between systems. 2. Has a Web
+UI. `Server IP:Port` or `ngrok-tunnel-host` - To view clipboard on mobile
+devices. - To sync clipboard if not using the Python client. 2. Advertise the
+server on the local network. 3. Authentication using passcode. (Passcode should
+be shared via some external safe channel) 5. Scan for servers on the local
+network. 6. The same script can be used as a server or client. 7. Encrypted
+communication for clipboard sharing with AES Encryption (Key should be shared
+via some external safe channel) ## Installation pip install clipShare ## Usage
+Usage: clipShare [... OPTIONS] Options: -h, --help Show this help message and
+exit -s, --server [SERVER_PORT_NUMER], --server [SERVER_PORT_NUMER] Run as
+server on the specified port. -c, --client SERVER_IP:SERVER_PORT_NUMBER, --
+client SERVER_IP:SERVER_PORT_NUMBER Run as a client, that connects to specified
+server IP and port. -t, --serve-on-ngrok-tunnel Enable Serve on ngrok tunnel.
+This option requires ngrok authtoken to be present in {current_dir}/ngrok-auth-
+token.txt -a, --advertise Enable Advertising server on the local network. -n, -
+-name Name of the server to be advertised. -p, --passcode Passcode for
+authentication. -ep, --encryption-password Encryption password for data
+transfer. -toh, --tcp-over-https Enable TCP over HTTPS for ngrok tunnel. -d, --
+debug Enable debug mode. Examples: clipShare -s 5000 clipShare -s 5000 -
 d clipShare -s 5000 -a clipShare -s 5000 -p RandomPasscode -ep
 5up3rS3cu3_3ncrY9t1on_P45sw0rd clipShare -s 5000 -p RandomPasscode -ep
 5up3rS3cu3_3ncrY9t1on_P45sw0rd -t -a -d clipShare -c 192.168.0.1:8080 clipShare
 -c -d clipShare -c -d -p RandomPasscode -ep 5up3rS3cu3_3ncrY9t1on_P45sw0rd
 clipShare -c "abc.com" -toh -d -p RandomPasscode -ep
 5up3rS3cu3_3ncrY9t1on_P45sw0rd clipShare -c "abc.com:120" -d -p RandomPasscode
 -ep 5up3rS3cu3_3ncrY9t1on_P45sw0rd clipShare -c -d -p RandomPasscode -ep
```

### Comparing `clipShare-0.1.2/clipShare/clipShare.py` & `clipshare-0.1.3/clipShare/clipShare.py`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/static/images/clipShare.jpeg` & `clipshare-0.1.3/clipShare/web-interface/static/images/clipShare.jpeg`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/static/images/help.png` & `clipshare-0.1.3/clipShare/web-interface/static/images/help.png`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/static/js/crypto-js.min.js` & `clipshare-0.1.3/clipShare/web-interface/static/js/crypto-js.min.js`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/static/js/main.js` & `clipshare-0.1.3/clipShare/web-interface/static/js/main.js`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/static/js/socket.io.js` & `clipshare-0.1.3/clipShare/web-interface/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare/web-interface/templates/index.html` & `clipshare-0.1.3/clipShare/web-interface/templates/index.html`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/clipShare.egg-info/PKG-INFO` & `clipshare-0.1.3/clipShare.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipShare
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sync clipboard between devices
 Home-page: https://github.com/avinashkarhana/clipShare
 Author: Avinash Karhana
 Author-email: avinashkarhana1@gmail.com
 License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console
@@ -26,19 +26,21 @@
 Requires-Dist: Flask-SocketIO
 Requires-Dist: python-socketio
 Requires-Dist: pyclip
 Requires-Dist: pyperclip
 Requires-Dist: pycryptodome
 Requires-Dist: requests
 Requires-Dist: pyngrok
-Requires-Dist: netifaces
+Requires-Dist: netifaces2
 Requires-Dist: zeroconf
 
 # clipShare
-[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipboardSync/actions/workflows/python-publish.yml)
+[![Publish Python Package to PyPi](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml/badge.svg)](https://github.com/avinashkarhana/clipShare/actions/workflows/python-publish.yml)
+
+*Check the PyPi Package [here](https://pypi.org/project/clipShare/)*
 
 A single TCP server/client bundle that allows you to sync your clipboard between systems.
 
 ## Features
 1. Sync clipboard between systems.
 2. Has a Web UI. `Server IP:Port` or `ngrok-tunnel-host`
     - To view clipboard on mobile devices.
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: clipShare Version: 0.1.2 Summary: Sync clipboard
+Metadata-Version: 2.1 Name: clipShare Version: 0.1.3 Summary: Sync clipboard
 between devices Home-page: https://github.com/avinashkarhana/clipShare Author:
 Avinash Karhana Author-email: avinashkarhana1@gmail.com License: LGPLv2.1
 Keywords: clipboardSync clipboard sync share encrypted secure clipShare
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v2 (LGPLv2) Classifier: Natural Language :: English Classifier:
 Operating System :: Microsoft :: Windows :: Windows 10 Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Communications Classifier: Topic :: Internet Classifier:
 Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: flask Requires-Dist: Flask-
 SocketIO Requires-Dist: python-socketio Requires-Dist: pyclip Requires-Dist:
 pyperclip Requires-Dist: pycryptodome Requires-Dist: requests Requires-Dist:
-pyngrok Requires-Dist: netifaces Requires-Dist: zeroconf # clipShare [![Publish
-Python Package to PyPi](https://github.com/avinashkarhana/clipboardSync/
+pyngrok Requires-Dist: netifaces2 Requires-Dist: zeroconf # clipShare [!
+[Publish Python Package to PyPi](https://github.com/avinashkarhana/clipShare/
 actions/workflows/python-publish.yml/badge.svg)](https://github.com/
-avinashkarhana/clipboardSync/actions/workflows/python-publish.yml) A single TCP
-server/client bundle that allows you to sync your clipboard between systems. ##
-Features 1. Sync clipboard between systems. 2. Has a Web UI. `Server IP:Port`
-or `ngrok-tunnel-host` - To view clipboard on mobile devices. - To sync
-clipboard if not using the Python client. 2. Advertise the server on the local
-network. 3. Authentication using passcode. (Passcode should be shared via some
-external safe channel) 5. Scan for servers on the local network. 6. The same
-script can be used as a server or client. 7. Encrypted communication for
-clipboard sharing with AES Encryption (Key should be shared via some external
-safe channel) ## Installation pip install clipShare ## Usage Usage: clipShare
-[... OPTIONS] Options: -h, --help Show this help message and exit -s, --server
+avinashkarhana/clipShare/actions/workflows/python-publish.yml) *Check the PyPi
+Package [here](https://pypi.org/project/clipShare/)* A single TCP server/client
+bundle that allows you to sync your clipboard between systems. ## Features 1.
+Sync clipboard between systems. 2. Has a Web UI. `Server IP:Port` or `ngrok-
+tunnel-host` - To view clipboard on mobile devices. - To sync clipboard if not
+using the Python client. 2. Advertise the server on the local network. 3.
+Authentication using passcode. (Passcode should be shared via some external
+safe channel) 5. Scan for servers on the local network. 6. The same script can
+be used as a server or client. 7. Encrypted communication for clipboard sharing
+with AES Encryption (Key should be shared via some external safe channel) ##
+Installation pip install clipShare ## Usage Usage: clipShare [... OPTIONS]
+Options: -h, --help Show this help message and exit -s, --server
 [SERVER_PORT_NUMER], --server [SERVER_PORT_NUMER] Run as server on the
 specified port. -c, --client SERVER_IP:SERVER_PORT_NUMBER, --client SERVER_IP:
 SERVER_PORT_NUMBER Run as a client, that connects to specified server IP and
 port. -t, --serve-on-ngrok-tunnel Enable Serve on ngrok tunnel. This option
 requires ngrok authtoken to be present in {current_dir}/ngrok-auth-token.txt -
 a, --advertise Enable Advertising server on the local network. -n, --name Name
 of the server to be advertised. -p, --passcode Passcode for authentication. -
```

### Comparing `clipShare-0.1.2/clipShare.egg-info/SOURCES.txt` & `clipshare-0.1.3/clipShare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipShare-0.1.2/setup.py` & `clipshare-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'Flask-SocketIO',
         'python-socketio',
         'pyclip',
         'pyperclip',
         'pycryptodome',
         'requests',
         'pyngrok',
-        'netifaces',
+        'netifaces2',
         'zeroconf'
     ],
 
     entry_points={
         'console_scripts': [
             'clipShare=clipShare.clipShare:main'
         ]
```

