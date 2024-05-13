# Comparing `tmp/dummynet-2.5.0-py2.py3-none-any.whl.zip` & `tmp/dummynet-2.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 12479 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      454 b- defN 23-Sep-04 10:12 dummynet/__init__.py
--rw-rw-r--  2.0 unx     9719 b- defN 23-Aug-25 12:16 dummynet/dummy_net.py
--rw-rw-r--  2.0 unx     1898 b- defN 23-Sep-04 10:12 dummynet/errors.py
--rw-rw-r--  2.0 unx     3802 b- defN 23-Sep-04 10:12 dummynet/host_shell.py
--rw-rw-r--  2.0 unx     1050 b- defN 23-Sep-04 10:12 dummynet/namespace_shell.py
--rw-rw-r--  2.0 unx      508 b- defN 23-Aug-25 12:16 dummynet/process.py
--rw-rw-r--  2.0 unx     9613 b- defN 23-Aug-28 09:35 dummynet/process_monitor.py
--rw-rw-r--  2.0 unx     4610 b- defN 23-Aug-28 09:35 dummynet/run_info.py
--rw-rw-r--  2.0 unx     1505 b- defN 23-Sep-04 10:13 dummynet-2.5.0.dist-info/LICENSE.rst
--rw-rw-r--  2.0 unx     1928 b- defN 23-Sep-04 10:13 dummynet-2.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Sep-04 10:13 dummynet-2.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Sep-04 10:13 dummynet-2.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1023 b- defN 23-Sep-04 10:13 dummynet-2.5.0.dist-info/RECORD
-13 files, 36229 bytes uncompressed, 10785 bytes compressed:  70.2%
+Zip file size: 15056 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      482 b- defN 24-May-13 06:53 dummynet/__init__.py
+-rw-rw-r--  2.0 unx     7006 b- defN 24-May-13 08:33 dummynet/cgroups.py
+-rw-rw-r--  2.0 unx    11034 b- defN 24-May-13 06:53 dummynet/dummy_net.py
+-rw-rw-r--  2.0 unx     1898 b- defN 24-May-13 06:47 dummynet/errors.py
+-rw-rw-r--  2.0 unx     3802 b- defN 24-May-13 06:47 dummynet/host_shell.py
+-rw-rw-r--  2.0 unx     1050 b- defN 24-May-13 06:47 dummynet/namespace_shell.py
+-rw-rw-r--  2.0 unx      508 b- defN 24-May-13 06:47 dummynet/process.py
+-rw-rw-r--  2.0 unx     9613 b- defN 24-May-13 06:47 dummynet/process_monitor.py
+-rw-rw-r--  2.0 unx     4610 b- defN 24-May-13 06:47 dummynet/run_info.py
+-rw-rw-r--  2.0 unx     1505 b- defN 24-May-13 08:34 dummynet-2.6.0.dist-info/LICENSE.rst
+-rw-rw-r--  2.0 unx     1928 b- defN 24-May-13 08:34 dummynet-2.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-May-13 08:34 dummynet-2.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-13 08:34 dummynet-2.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1100 b- defN 24-May-13 08:34 dummynet-2.6.0.dist-info/RECORD
+14 files, 44655 bytes uncompressed, 13248 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: dummynet/__init__.py
 Comment: 
 
+Filename: dummynet/cgroups.py
+Comment: 
+
 Filename: dummynet/dummy_net.py
 Comment: 
 
 Filename: dummynet/errors.py
 Comment: 
 
 Filename: dummynet/host_shell.py
@@ -18,23 +21,23 @@
 
 Filename: dummynet/process_monitor.py
 Comment: 
 
 Filename: dummynet/run_info.py
 Comment: 
 
-Filename: dummynet-2.5.0.dist-info/LICENSE.rst
+Filename: dummynet-2.6.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: dummynet-2.5.0.dist-info/METADATA
+Filename: dummynet-2.6.0.dist-info/METADATA
 Comment: 
 
-Filename: dummynet-2.5.0.dist-info/WHEEL
+Filename: dummynet-2.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: dummynet-2.5.0.dist-info/top_level.txt
+Filename: dummynet-2.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dummynet-2.5.0.dist-info/RECORD
+Filename: dummynet-2.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dummynet/__init__.py

```diff
@@ -1,13 +1,14 @@
 from .dummy_net import DummyNet
 from .run_info import RunInfo
 from .namespace_shell import NamespaceShell
 from .host_shell import HostShell
 from .process_monitor import ProcessMonitor
 from .process import Process
+from .cgroups import CGroup
 
 from .errors import DummyNetError
 from .errors import RunInfoError
 from .errors import TimeoutError
 from .errors import MatchError
 from .errors import DaemonExitError
 from .errors import AllDaemonsError
```

## dummynet/dummy_net.py

```diff
@@ -1,24 +1,27 @@
 import re
 from subprocess import CalledProcessError
 from . import namespace_shell
+from dummynet.cgroups import CGroup
+from logging import Logger
 
 
 class DummyNet(object):
 
     """A DummyNet object is used to create a network of virtual ethernet
     devices and bind them to namespaces.
     """
 
     def __init__(self, shell):
         """Creates a new DummyNet object.
 
         :param shell: The shell to use for running commands
         """
         self.shell = shell
+        self.cgroups = []
         self.cleaners = []
 
     def link_veth_add(self, p1_name, p2_name):
         """Adds a virtual ethernet between two endpoints.
 
         Name of the link will be 'p1_name@p2_name' when you look at 'ip addr'
         in the terminal
@@ -293,7 +296,37 @@
         return self.link_list(link_type="bridge")
 
     def cleanup(self):
         """Cleans up all the created network namespaces and bridges"""
 
         for cleaner in self.cleaners:
             cleaner()
+
+    def add_cgroup(self,
+                   name: str,
+                   shell,
+                   log: Logger,
+                   default_path: str = "/sys/fs/cgroup",
+                   controllers: dict = {"cpu.max": None,
+                                      "memory.high": None},
+                   pid=None):
+        """
+        Creates a new cgroup object.
+
+        :param name: The name of the cgroup.
+        :param shell: The shell object used for executing shell commands.
+        :param log: The log object used for logging messages.
+        :param default_path: The default path for cgroups. Defaults to "/sys/fs/cgroup".
+        :param controllers: Dictionary of controllers as keys and limits as values. Defaults to {"cpu.max": None, "memory.high": None}.
+        :param pid: The process ID to add to the cgroup. Defaults to None.
+        
+        :return: A CGroup object.
+        """
+        cgroup = CGroup(name=name, shell=shell, log=log, default_path=default_path, controllers=controllers, pid=pid)
+        self.cgroups.append(cgroup)
+        return cgroup
+    
+    def cgroup_cleanup(self):
+        """Cleans up all the created cgroups."""
+        for c in self.cgroups:
+            c.hard_clean()
+
```

## Comparing `dummynet-2.5.0.dist-info/LICENSE.rst` & `dummynet-2.6.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `dummynet-2.5.0.dist-info/METADATA` & `dummynet-2.6.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummynet
-Version: 2.5.0
+Version: 2.6.0
 Summary: A tool for creating dummy networks using network namespaces.
 Home-page: https://github.com/steinwurf/dummynet
 Author: Steinwurf ApS
 Author-email: contact@steinwurf.com
 License: BSD 3-clause "New" or "Revised" License
 Keywords: dummynet,network,namespace
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `dummynet-2.5.0.dist-info/RECORD` & `dummynet-2.6.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-dummynet/__init__.py,sha256=gvUx5nPsVAPy8mfb-sY6xJqH_hX9nnnx52LuQmZp4U8,454
-dummynet/dummy_net.py,sha256=BfDXzxL4UKeMzIvO4VwjIsB2udjqksFnGE8Kchs8aQQ,9719
+dummynet/__init__.py,sha256=TQb99uwzM9N1RKQ1ydqqMEE7rBP25K2dJWC2loWbuYA,482
+dummynet/cgroups.py,sha256=_QUl7-wrFxCv4jubVG_7DuUNRfEAO4wQdF2SKE-ZnLQ,7006
+dummynet/dummy_net.py,sha256=MAgaXX20e-n_bclItnfLmXAXzRWl1rm5EQHxNcA20Eo,11034
 dummynet/errors.py,sha256=1edjgwEyG5sxV1Z5trHOsL_cOlwe4IeCP7L9AbSdw6g,1898
 dummynet/host_shell.py,sha256=loz0BRSEXYoTVD0TJfuL9bbcJpqvtONvFDo0pwD2G_A,3802
 dummynet/namespace_shell.py,sha256=rmu0opiBsLVqKrmpFSecVtmupW11C4Exoetzb3YDsYI,1050
 dummynet/process.py,sha256=_ip-Q46ho2BRtELcO8P-_1x0o_fCjfy3Yj56mPVLwlk,508
 dummynet/process_monitor.py,sha256=78yhnwbq7H6jBQmm4G3QJGSMIS7dbrd56Ql4-2Hm6bs,9613
 dummynet/run_info.py,sha256=Xug4AVXC3uee7pCB8TBw7RLP07VroOccgCKegQV7gR4,4610
-dummynet-2.5.0.dist-info/LICENSE.rst,sha256=lnhVy333OpPgt8lKvpJs9jdfAOTpzAhlk0Z2e4V2BDs,1505
-dummynet-2.5.0.dist-info/METADATA,sha256=N0ljgOXDa5eTCyJAJ0Jv3Rht8_U0Urh4C2RfzetYkCo,1928
-dummynet-2.5.0.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-dummynet-2.5.0.dist-info/top_level.txt,sha256=beQt5cynnx7cpYC2J9i11U2IBQdl-bVPaINnhozkRoM,9
-dummynet-2.5.0.dist-info/RECORD,,
+dummynet-2.6.0.dist-info/LICENSE.rst,sha256=lnhVy333OpPgt8lKvpJs9jdfAOTpzAhlk0Z2e4V2BDs,1505
+dummynet-2.6.0.dist-info/METADATA,sha256=tF1VrIui-SiMSbof2Bi2j2-6Iqos6v-sk8_L37mv79w,1928
+dummynet-2.6.0.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+dummynet-2.6.0.dist-info/top_level.txt,sha256=beQt5cynnx7cpYC2J9i11U2IBQdl-bVPaINnhozkRoM,9
+dummynet-2.6.0.dist-info/RECORD,,
```

