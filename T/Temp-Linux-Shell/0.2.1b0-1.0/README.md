# Comparing `tmp/temp_linux_shell-0.2.1b0.tar.gz` & `tmp/temp_linux_shell-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temp_linux_shell-0.2.1b0.tar", last modified: Thu May  9 13:22:44 2024, max compression
+gzip compressed data, was "temp_linux_shell-1.0.tar", last modified: Mon May 13 20:09:10 2024, max compression
```

## Comparing `temp_linux_shell-0.2.1b0.tar` & `temp_linux_shell-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:44.568176 temp_linux_shell-0.2.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-09 13:22:40.000000 temp_linux_shell-0.2.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-09 13:22:44.568176 temp_linux_shell-0.2.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-09 13:22:40.000000 temp_linux_shell-0.2.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:44.564175 temp_linux_shell-0.2.1b0/TLS/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 13:22:40.000000 temp_linux_shell-0.2.1b0/TLS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5992 2024-05-09 13:22:40.000000 temp_linux_shell-0.2.1b0/TLS/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:44.568176 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 13:22:44.000000 temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:22:44.568176 temp_linux_shell-0.2.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-09 13:22:40.000000 temp_linux_shell-0.2.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:09:10.543867 temp_linux_shell-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-13 20:09:05.000000 temp_linux_shell-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-13 20:09:10.543867 temp_linux_shell-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-13 20:09:05.000000 temp_linux_shell-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:09:10.543867 temp_linux_shell-1.0/TLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 20:09:05.000000 temp_linux_shell-1.0/TLS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6226 2024-05-13 20:09:05.000000 temp_linux_shell-1.0/TLS/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:09:10.543867 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 20:09:10.000000 temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:09:10.543867 temp_linux_shell-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 20:09:05.000000 temp_linux_shell-1.0/setup.py
```

### Comparing `temp_linux_shell-0.2.1b0/LICENSE` & `temp_linux_shell-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `temp_linux_shell-0.2.1b0/PKG-INFO` & `temp_linux_shell-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temp-Linux-Shell
-Version: 0.2.1b0
+Version: 1.0
 Summary: Wrapper around Chroot to make it easy to use temporary Linux Shells.
 Home-page: https://github.com/Noriskky/tls
 Author: Noriskky
 Author-email: Noriskky44@proton.me
 License: GPLv3
 Keywords: cli,tls,alpine,temp-system,temp-linux-shell,temp-linux-system
 Platform: Linux
@@ -23,14 +23,26 @@
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Alpine Linux](https://img.shields.io/badge/Alpine_Linux-%230D597F.svg?style=for-the-badge&logo=alpine-linux&logoColor=white)
 
 [![PyPI download month](https://img.shields.io/pypi/dm/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell//)
 
 ![Screenshot of TLS](https://github.com/Noriskky/TLS/blob/main/pictures/screenshot.png?raw=true) 
 
+## Testing
+
+If you just want to test ``TLS`` without installing it you can do that with the following command:
+```bash
+source <(curl -sSL https://raw.githubusercontent.com/Noriskky/TLS/main/scripts/tls.sh)
+```
+
+
+**NOTE**: 
+THIS will not install the script! <br>
+This script only writes to ``/var/tmp`` so the changes will not be permanent, and it's using a temporary VENV.
+
 ## Installation
 
 You can install TLS via Pip:
 
 ```bash
 pip install Temp-Linux-Shell
 ```
```

### Comparing `temp_linux_shell-0.2.1b0/README.md` & `temp_linux_shell-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Alpine Linux](https://img.shields.io/badge/Alpine_Linux-%230D597F.svg?style=for-the-badge&logo=alpine-linux&logoColor=white)
 
 [![PyPI download month](https://img.shields.io/pypi/dm/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell//)
 
 ![Screenshot of TLS](https://github.com/Noriskky/TLS/blob/main/pictures/screenshot.png?raw=true) 
 
+## Testing
+
+If you just want to test ``TLS`` without installing it you can do that with the following command:
+```bash
+source <(curl -sSL https://raw.githubusercontent.com/Noriskky/TLS/main/scripts/tls.sh)
+```
+
+
+**NOTE**: 
+THIS will not install the script! <br>
+This script only writes to ``/var/tmp`` so the changes will not be permanent, and it's using a temporary VENV.
+
 ## Installation
 
 You can install TLS via Pip:
 
 ```bash
 pip install Temp-Linux-Shell
 ```
```

### Comparing `temp_linux_shell-0.2.1b0/TLS/main.py` & `temp_linux_shell-1.0/TLS/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import argparse
 import os
 import subprocess
 import sys
 import uuid
-
+import signal
 import requests
 from tqdm import tqdm
 
 
 def main():
-    tls(sys.argv[1:])
+    try:
+        tls(sys.argv[1:])
+    except KeyboardInterrupt:
+        print('Interrupted by User')
 
 def get_latest_alpine_version():
     try:
         # Construct the URL for the latest version of Alpine Linux
         latest_version_url = "https://dl-cdn.alpinelinux.org/alpine/latest-stable/releases/x86_64/"
         response = requests.get(latest_version_url)
         response.raise_for_status()
@@ -99,23 +102,28 @@
     #    if not persistent:
     #        # Clear the temporary directory after exiting the shell
     #        if os.path.exists(working_directory):
     #            if 
     #            shutil.rmtree(working_directory)
     #            print(f"\033[94mTemp directory cleared.\033[0m")
 
+def signal_handler(sig, frame):
+    print('Interrupted by User')
+    sys.exit(0)
 
 class tls:
     def __init__(self, name):
         parser = argparse.ArgumentParser(description="Start a temporary Alpine Linux shell")
         parser.add_argument("--hostname", "-hn", default="alpine", help="Specify the hostname for the Alpine Linux environment")
         parser.add_argument("--command", "-c", help="Command to execute in the Alpine Linux environment")
         parser.add_argument("--directory", "-d", help="Where the folder of the Shell should be")
         parser.add_argument("--password", "--passwd", "-p", help="Password for the Root User")
         #parser.add_argument("--persistent", "-p", help="A Flag to make the Shell persistent. Make sure to specify a directory.", action="store_true")
         args = parser.parse_args()
 
         #if args.persistent and args.directory == None:
         #    print("Make sure to specify a directory.")
         #    quit()
+        signal.signal(signal.SIGINT, signal_handler)
+        start_temp_alpine_shell(args.hostname, args.command, args.directory, args.password)
 
-        start_temp_alpine_shell(args.hostname, args.command, args.directory, args.password)
+main()
```

### Comparing `temp_linux_shell-0.2.1b0/Temp_Linux_Shell.egg-info/PKG-INFO` & `temp_linux_shell-1.0/Temp_Linux_Shell.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temp-Linux-Shell
-Version: 0.2.1b0
+Version: 1.0
 Summary: Wrapper around Chroot to make it easy to use temporary Linux Shells.
 Home-page: https://github.com/Noriskky/tls
 Author: Noriskky
 Author-email: Noriskky44@proton.me
 License: GPLv3
 Keywords: cli,tls,alpine,temp-system,temp-linux-shell,temp-linux-system
 Platform: Linux
@@ -23,14 +23,26 @@
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Alpine Linux](https://img.shields.io/badge/Alpine_Linux-%230D597F.svg?style=for-the-badge&logo=alpine-linux&logoColor=white)
 
 [![PyPI download month](https://img.shields.io/pypi/dm/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/Temp-Linux-Shell.svg)](https://pypi.python.org/pypi/Temp-Linux-Shell//)
 
 ![Screenshot of TLS](https://github.com/Noriskky/TLS/blob/main/pictures/screenshot.png?raw=true) 
 
+## Testing
+
+If you just want to test ``TLS`` without installing it you can do that with the following command:
+```bash
+source <(curl -sSL https://raw.githubusercontent.com/Noriskky/TLS/main/scripts/tls.sh)
+```
+
+
+**NOTE**: 
+THIS will not install the script! <br>
+This script only writes to ``/var/tmp`` so the changes will not be permanent, and it's using a temporary VENV.
+
 ## Installation
 
 You can install TLS via Pip:
 
 ```bash
 pip install Temp-Linux-Shell
 ```
```

### Comparing `temp_linux_shell-0.2.1b0/setup.py` & `temp_linux_shell-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Temp-Linux-Shell",
-    version="0.2.1-Beta",
+    version="1.0",
     author="Noriskky",
     platforms=["Linux"],
     author_email="Noriskky44@proton.me",
     description="Wrapper around Chroot to make it easy to use temporary Linux Shells.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3",
     url="https://github.com/Noriskky/tls",
     keywords=["cli", "tls", "alpine", "temp-system", "temp-linux-shell", "temp-linux-system"],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: POSIX :: Linux",
+        "Operating System :: POSIX :: Linux"
     ],
     install_requires=[
         "requests",
         "tqdm"
     ],
     python_requires='>=3.6',
     entry_points={
```

