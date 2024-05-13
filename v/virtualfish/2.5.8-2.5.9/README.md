# Comparing `tmp/virtualfish-2.5.8.tar.gz` & `tmp/virtualfish-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualfish-2.5.8.tar", max compression
+gzip compressed data, was "virtualfish-2.5.9.tar", max compression
```

## Comparing `virtualfish-2.5.8.tar` & `virtualfish-2.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1103 2024-04-25 12:53:13.115721 virtualfish-2.5.8/LICENSE
--rw-r--r--   0        0        0     1758 2024-04-25 12:53:13.119721 virtualfish-2.5.8/README.md
--rw-r--r--   0        0        0     1397 2024-04-25 12:54:23.096047 virtualfish-2.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/__init__.py
--rw-r--r--   0        0        0      376 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/__main__.py
--rw-r--r--   0        0        0     3600 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/auto_activation.fish
--rw-r--r--   0        0        0      927 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/compat_aliases.fish
--rw-r--r--   0        0        0     3455 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/environment.fish
--rw-r--r--   0        0        0      797 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/global_requirements.fish
--rw-r--r--   0        0        0      993 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/__init__.py
--rw-r--r--   0        0        0     1048 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/loader/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2307 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/cli.py
--rw-r--r--   0        0        0     1736 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/loader/installer.py
--rw-r--r--   0        0        0     4789 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/projects.fish
--rw-r--r--   0        0        0        0 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/__init__.py
--rw-r--r--   0        0        0      161 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      897 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     3424 2024-04-25 12:54:01.611952 virtualfish-2.5.8/virtualfish/test/__pycache__/repl.cpython-39.pyc
--rw-r--r--   0        0        0     1344 2024-04-25 12:54:01.615952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1130 2024-04-25 12:54:01.619952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1087 2024-04-25 12:54:01.619952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1369 2024-04-25 12:54:01.623952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1991 2024-04-25 12:54:01.627952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     1799 2024-04-25 12:54:01.627952 virtualfish-2.5.8/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      364 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/conftest.py
--rw-r--r--   0        0        0      328 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/repl.fish
--rw-r--r--   0        0        0     3745 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/repl.py
--rw-r--r--   0        0        0      233 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_activate.py
--rw-r--r--   0        0        0      330 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_addpath.py
--rw-r--r--   0        0        0      193 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_deactivate.py
--rw-r--r--   0        0        0      489 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_loader.py
--rw-r--r--   0        0        0      405 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_repl.py
--rw-r--r--   0        0        0      368 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/test/test_rm.py
--rw-r--r--   0        0        0     1181 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/update_python.fish
--rw-r--r--   0        0        0    32704 2024-04-25 12:53:13.119721 virtualfish-2.5.8/virtualfish/virtual.fish
--rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 virtualfish-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-05-13 18:31:54.254824 virtualfish-2.5.9/LICENSE
+-rw-r--r--   0        0        0     1758 2024-05-13 18:31:54.254824 virtualfish-2.5.9/README.md
+-rw-r--r--   0        0        0     1397 2024-05-13 18:32:50.079898 virtualfish-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/__main__.py
+-rw-r--r--   0        0        0     3600 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/auto_activation.fish
+-rw-r--r--   0        0        0      927 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/compat_aliases.fish
+-rw-r--r--   0        0        0     3455 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/environment.fish
+-rw-r--r--   0        0        0      797 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/global_requirements.fish
+-rw-r--r--   0        0        0      993 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/loader/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-13 18:32:29.675509 virtualfish-2.5.9/virtualfish/loader/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2371 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/loader/cli.py
+-rw-r--r--   0        0        0     1736 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/loader/installer.py
+-rw-r--r--   0        0        0     4789 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/projects.fish
+-rw-r--r--   0        0        0        0 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-13 18:32:29.671509 virtualfish-2.5.9/virtualfish/test/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      897 2024-05-13 18:32:29.671509 virtualfish-2.5.9/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     3424 2024-05-13 18:32:29.671509 virtualfish-2.5.9/virtualfish/test/__pycache__/repl.cpython-39.pyc
+-rw-r--r--   0        0        0     1344 2024-05-13 18:32:29.675509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1130 2024-05-13 18:32:29.679509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1087 2024-05-13 18:32:29.679509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1369 2024-05-13 18:32:29.683509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1991 2024-05-13 18:32:29.683509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0     1799 2024-05-13 18:32:29.687509 virtualfish-2.5.9/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0      364 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/conftest.py
+-rw-r--r--   0        0        0      328 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/repl.fish
+-rw-r--r--   0        0        0     3745 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/repl.py
+-rw-r--r--   0        0        0      233 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_activate.py
+-rw-r--r--   0        0        0      330 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_addpath.py
+-rw-r--r--   0        0        0      193 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_deactivate.py
+-rw-r--r--   0        0        0      489 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_loader.py
+-rw-r--r--   0        0        0      405 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_repl.py
+-rw-r--r--   0        0        0      368 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/test/test_rm.py
+-rw-r--r--   0        0        0     1181 2024-05-13 18:31:54.254824 virtualfish-2.5.9/virtualfish/update_python.fish
+-rw-r--r--   0        0        0    32704 2024-05-13 18:31:54.258824 virtualfish-2.5.9/virtualfish/virtual.fish
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 virtualfish-2.5.9/PKG-INFO
```

### Comparing `virtualfish-2.5.8/LICENSE` & `virtualfish-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/README.md` & `virtualfish-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/pyproject.toml` & `virtualfish-2.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtualfish"
-version = "2.5.8"
+version = "2.5.9"
 description = "Fish shell tool for managing Python virtual environments"
 authors = ["Justin Mayer <entroP@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["fish", "shell", "python", "virtual", "environments", "virtualenv"]
 repository = "https://github.com/justinmayer/virtualfish"
```

### Comparing `virtualfish-2.5.8/virtualfish/auto_activation.fish` & `virtualfish-2.5.9/virtualfish/auto_activation.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/compat_aliases.fish` & `virtualfish-2.5.9/virtualfish/compat_aliases.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/environment.fish` & `virtualfish-2.5.9/virtualfish/environment.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/global_requirements.fish` & `virtualfish-2.5.9/virtualfish/global_requirements.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/loader/__init__.py` & `virtualfish-2.5.9/virtualfish/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/loader/__pycache__/__init__.cpython-39.pyc` & `virtualfish-2.5.9/virtualfish/loader/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 993 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 e103 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 e103 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6500 a005 6506 a101 5a07 6407 6405  ..e...e...Z.d.d.
 00000060: 6406 8401 5a08 6401 5300 2908 e900 0000  d...Z.d.S.).....
 00000070: 004e 2901 da08 6d65 7461 6461 7461 a900  .N)...metadata..
```

### Comparing `virtualfish-2.5.8/virtualfish/loader/cli.py` & `virtualfish-2.5.9/virtualfish/loader/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,23 @@
     installer.install(argv[2:])
 
 
 def check_fish_version():
     """Display a warning if the minimum Fish version is not installed. Bail silently if
     the 'packaging' module is missing or if Fish is not installed."""
     try:
+        import re
         import subprocess
         from packaging import version
 
-        cmd = ["fish", "-N", "-c", "echo $version"]
-        fish_version = subprocess.check_output(cmd).decode("utf-8").strip()
-        # Remove any extraneous hyphen-suffixed bits
-        fish_version = fish_version.partition("-")[0]
+        cmd = ["fish", "--version"]
+        fish_output = subprocess.check_output(cmd).decode("utf-8")
+        # Remove any extraneous prefix and hyphen-suffixed bits
+        fish_matches = re.match(r".*version ([\d\.]+)", fish_output)
+        fish_version = fish_matches.group(1)
         if version.parse(fish_version) < version.parse(minimum_fish_version):
             log.warning(
                 """{}WARNING: VirtualFish requires Fish {} or higher.
                    Current version: {}{}""".format(
                     vcolors.RED, minimum_fish_version, fish_version, vcolors.NORMAL
                 )
             )
```

### Comparing `virtualfish-2.5.8/virtualfish/loader/installer.py` & `virtualfish-2.5.9/virtualfish/loader/installer.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/projects.fish` & `virtualfish-2.5.9/virtualfish/projects.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/conftest.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 6c01 0000  a.......9R*fl...
+00000000: 610d 0d0a 0000 0000 9a5c 4266 6c01 0000  a........\Bfl...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6406 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 6d0d 5a0d 0100 6506 6a0e 6407 6408  Z.m.Z...e.j.d.d.
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/repl.cpython-39.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/repl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 3745 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 a10e 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 a10e 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 fa00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6402 6c07 5a07 7a10 6401 6405  ..d.d.l.Z.z.d.d.
 00000070: 6c08 6d09 5a09 0100 5700 6e1e 0400 650a  l.m.Z...W.n...e.
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_activate.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 233 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 e900 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 e900 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 000d 0000 000c 0000  ................
 00000070: 0043 0000 0073 3201 0000 7c00 a000 6401  .C...s2...|...d.
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_addpath.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 330 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 4a01 0000  a.......9R*fJ...
+00000000: 610d 0d0a 0000 0000 9a5c 4266 4a01 0000  a........\BfJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 0009 0000 0007 0000  ................
 00000070: 0043 0000 0073 0a01 0000 7c00 6a00 9b00  .C...s....|.j...
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_deactivate.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 c100 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 c100 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 8400 5a06  ..m.Z...d.d...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 000b 0000 000a 0000  ................
 00000070: 0043 0000 0073 d800 0000 7c00 a000 6401  .C...s....|...d.
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_loader.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 e901 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 e901 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6506 6a0b 6406 6407  l.m.Z...e.j.d.d.
 00000070: 8400 8301 5a0c 6408 6409 8400 5a0d 640a  ....Z.d.d...Z.d.
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_repl.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 405 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 9501 0000  a.......9R*f....
+00000000: 610d 0d0a 0000 0000 9a5c 4266 9501 0000  a........\Bf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6506 6a09  d.d.l.m.Z...e.j.
 00000060: 6404 6405 8400 8301 5a0a 6406 6407 8400  d.d.....Z.d.d...
 00000070: 5a0b 6408 6409 8400 5a0c 640a 640b 8400  Z.d.d...Z.d.d...
```

### Comparing `virtualfish-2.5.8/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.1.1.pyc` & `virtualfish-2.5.9/virtualfish/test/__pycache__/test_rm.cpython-39-pytest-8.2.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 25 12:53:13 2024 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3952 2a66 7001 0000  a.......9R*fp...
+00000000: 610d 0d0a 0000 0000 9a5c 4266 7001 0000  a........\Bfp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 8400 5a07 6404 6405 8400 5a08  d.d...Z.d.d...Z.
 00000060: 6401 5300 2906 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000070: 0000 0000 0000 0000 000a 0000 000a 0000  ................
```

### Comparing `virtualfish-2.5.8/virtualfish/test/repl.py` & `virtualfish-2.5.9/virtualfish/test/repl.py`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/update_python.fish` & `virtualfish-2.5.9/virtualfish/update_python.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/virtualfish/virtual.fish` & `virtualfish-2.5.9/virtualfish/virtual.fish`

 * *Files identical despite different names*

### Comparing `virtualfish-2.5.8/PKG-INFO` & `virtualfish-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtualfish
-Version: 2.5.8
+Version: 2.5.9
 Summary: Fish shell tool for managing Python virtual environments
 Home-page: https://github.com/justinmayer/virtualfish
 License: MIT
 Keywords: fish,shell,python,virtual,environments,virtualenv
 Author: Justin Mayer
 Author-email: entroP@gmail.com
 Requires-Python: >=3.8,<4.0
```

