# Comparing `tmp/cjtool-0.29.7-py2.py3-none-any.whl.zip` & `tmp/cjtool-0.29.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 20473 bytes, number of entries: 17
+Zip file size: 21832 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat       76 b- defN 22-Oct-06 08:53 cjtool/__init__.py
--rw-rw-rw-  2.0 fat     3501 b- defN 23-Dec-23 11:35 cjtool/cdbtool.py
--rw-rw-rw-  2.0 fat    11909 b- defN 23-Dec-11 13:34 cjtool/common.py
--rw-rw-rw-  2.0 fat    15195 b- defN 24-May-12 01:57 cjtool/debuger.py
--rw-rw-rw-  2.0 fat     1938 b- defN 23-Nov-12 10:47 cjtool/indent.py
--rw-rw-rw-  2.0 fat     2408 b- defN 23-Dec-16 14:20 cjtool/monitor.py
--rw-rw-rw-  2.0 fat     2323 b- defN 23-Dec-10 06:01 cjtool/search.py
+-rw-rw-rw-  2.0 fat      404 b- defN 24-May-13 08:53 cjtool/addconsole.py
+-rw-rw-rw-  2.0 fat     3501 b- defN 24-May-12 10:07 cjtool/cdbtool.py
+-rw-rw-rw-  2.0 fat    12182 b- defN 24-May-13 08:51 cjtool/common.py
+-rw-rw-rw-  2.0 fat    15195 b- defN 24-May-12 10:07 cjtool/debuger.py
+-rw-rw-rw-  2.0 fat     1938 b- defN 24-May-12 10:07 cjtool/indent.py
+-rw-rw-rw-  2.0 fat     2408 b- defN 24-May-12 10:07 cjtool/monitor.py
+-rw-rw-rw-  2.0 fat     2044 b- defN 24-May-13 08:51 cjtool/search.py
 -rw-rw-rw-  2.0 fat     5826 b- defN 22-Oct-06 08:27 cjtool/stl.py
 -rw-rw-rw-  2.0 fat     7180 b- defN 22-Oct-04 06:17 cjtool/stringtool.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-12 09:48 cjtool/gfy/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-12 10:07 cjtool/gfy/__init__.py
+-rw-rw-rw-  2.0 fat     2280 b- defN 24-May-13 13:36 cjtool/gfy/edoinfo.py
 -rw-rw-rw-  2.0 fat     2226 b- defN 24-May-12 02:17 cjtool/gfy/print.py
--rw-rw-rw-  2.0 fat     2309 b- defN 24-May-12 09:45 cjtool/gfy/printedo.py
--rw-rw-rw-  2.0 fat     1935 b- defN 24-May-12 09:48 cjtool-0.29.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-May-12 09:48 cjtool-0.29.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      187 b- defN 24-May-12 09:48 cjtool-0.29.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-12 09:48 cjtool-0.29.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1288 b- defN 24-May-12 09:48 cjtool-0.29.7.dist-info/RECORD
-17 files, 58418 bytes uncompressed, 18397 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat     2309 b- defN 24-May-12 10:07 cjtool/gfy/printedo.py
+-rw-rw-rw-  2.0 fat     1935 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      221 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1442 b- defN 24-May-13 13:37 cjtool-0.29.8.dist-info/RECORD
+19 files, 61284 bytes uncompressed, 19522 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: cjtool/__init__.py
 Comment: 
 
+Filename: cjtool/addconsole.py
+Comment: 
+
 Filename: cjtool/cdbtool.py
 Comment: 
 
 Filename: cjtool/common.py
 Comment: 
 
 Filename: cjtool/debuger.py
@@ -24,29 +27,32 @@
 
 Filename: cjtool/stringtool.py
 Comment: 
 
 Filename: cjtool/gfy/__init__.py
 Comment: 
 
+Filename: cjtool/gfy/edoinfo.py
+Comment: 
+
 Filename: cjtool/gfy/print.py
 Comment: 
 
 Filename: cjtool/gfy/printedo.py
 Comment: 
 
-Filename: cjtool-0.29.7.dist-info/METADATA
+Filename: cjtool-0.29.8.dist-info/METADATA
 Comment: 
 
-Filename: cjtool-0.29.7.dist-info/WHEEL
+Filename: cjtool-0.29.8.dist-info/WHEEL
 Comment: 
 
-Filename: cjtool-0.29.7.dist-info/entry_points.txt
+Filename: cjtool-0.29.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: cjtool-0.29.7.dist-info/top_level.txt
+Filename: cjtool-0.29.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cjtool-0.29.7.dist-info/RECORD
+Filename: cjtool-0.29.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cjtool/common.py

```diff
@@ -330,14 +330,23 @@
     freopen = pykd.typedVar(freopen_Type, pykd.getOffset("ucrtbase!freopen"))
     param = pykd.stackAlloc(100)
     pykd.writeCStr(param, "CON")
     pykd.writeCStr(param + 8, "w")
     freopen(param, param + 8, stdout)
     pykd.stackFree(100)
 
+def attach_process(process_name: str):
+    pykd.initialize()
+    pid = getProcessByName(process_name)
+    if pid == 0:
+        print(f"The app: {process_name} is not found")
+        exit()
+
+    print(f"Attaching to process: pid {pid}")
+    pykd.attachProcess(pid)
 
 def natvis(moduleName, var, depth=1):
     # Need copy the stl.natvis to the site-packages\pykd\Visualizers
     typename = var.type().name()
     addr = var.getAddress()
     desc = pykd.dbgCommand("dx -r{} (*(({}!{} *){:#x}))".format(
         depth, moduleName, typename, addr))
```

## cjtool/search.py

```diff
@@ -1,22 +1,10 @@
 from pykd import *
 from common import *
 
-
-def attach_process(process_name: str):
-    pykd.initialize()
-    pid = getProcessByName(process_name)
-    if pid == 0:
-        print(f"The app: {process_name} is not found")
-        exit()
-
-    print(f"Attaching to process: pid {pid}")
-    pykd.attachProcess(pid)
-
-
 class EntitySearcher:
     def __init__(self, class_name: str) -> None:
         self.class_name = class_name
         self.search_type = BaseType(class_name)
 
     def search(self) -> list[int]:
         self.search_type.print_vftable_methods()
```

## Comparing `cjtool-0.29.7.dist-info/METADATA` & `cjtool-0.29.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjtool
-Version: 0.29.7
+Version: 0.29.8
 Summary: Provide some tools in C++ development
 Home-page: http://github.com/Junch/cjtool
 Author: Jun Chen
 Author-email: junc76@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: colorama
```

## Comparing `cjtool-0.29.7.dist-info/RECORD` & `cjtool-0.29.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 cjtool/__init__.py,sha256=Lh7NOd9-n-o-7iRw3-RIoQCF_F57zhZQktJjCkSYOgA,76
+cjtool/addconsole.py,sha256=K9sOmpNh0pqSghnqGOyRwgshJAfgfnIcjyqCVcmNs9I,404
 cjtool/cdbtool.py,sha256=gKc-NzgsDwCg6yBHOTmQG4IEC0jRtIK1jEmoIbB2PWw,3501
-cjtool/common.py,sha256=GFlIJihR3hYhG3p8_Ogtj1miXqusBlLG04aSFEAIDF4,11909
+cjtool/common.py,sha256=djGMFHGFc8758wQDe9Y8bMlxEsCGZK-Fz2fPBOTRjuo,12182
 cjtool/debuger.py,sha256=3V3YkWiKpTlm70TQIoJXRi6tka21AZRmtKXVFwF30Zw,15195
 cjtool/indent.py,sha256=o8nzbYzfXviUn4f7JayUAtCc5o2c_SZp5PTr1MK8sRg,1938
 cjtool/monitor.py,sha256=qE1sLXBOhcI_AgbdbwOzKqTPqLGsyOKLsjkewuPciWE,2408
-cjtool/search.py,sha256=_c-aOw35jEst5lZsvEZr8ZewBdQiQKr9SxPWNoX0u5I,2323
+cjtool/search.py,sha256=bbz_gpxrlEfDATWv26MbsfN1Pm6yEB-1zoTAZL10kaw,2044
 cjtool/stl.py,sha256=SeNfQubgArMRtByamEIjdn5fuvEKDhhaIeKBeo6cSdM,5826
 cjtool/stringtool.py,sha256=84VYHVPyIPSO51IXxrhDjJdGE-11NJsdCD-EcI7eL0w,7180
 cjtool/gfy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cjtool/gfy/edoinfo.py,sha256=f2-FVzs6INSWm_EOIhtMjSaBK_VRlhS1RQhSvpzcW04,2280
 cjtool/gfy/print.py,sha256=O5VyI3XC2EXjs-HhR2Dv2kA_uEpfeHoIhIJOYaZkaeI,2226
 cjtool/gfy/printedo.py,sha256=E8a_4GG_PBTEdw_9NGqhZTMXIAQlR5t3P7ilKJ8Dtw4,2309
-cjtool-0.29.7.dist-info/METADATA,sha256=Nd4vusj91k2N_awR6Nq6Y9NKXPQbEM0zwVdUpc0eu-o,1935
-cjtool-0.29.7.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-cjtool-0.29.7.dist-info/entry_points.txt,sha256=DGqFVsRfZ6aYDikJHPWEyuQSHATsUhRQswFDlprcO_g,187
-cjtool-0.29.7.dist-info/top_level.txt,sha256=xT9DqEuxuB3mnAq-fVy_mWHaaTT3M-S7J_93pQnE7W8,7
-cjtool-0.29.7.dist-info/RECORD,,
+cjtool-0.29.8.dist-info/METADATA,sha256=NR-qtlYARNDc98_YvNWzzSgDE_YB2THMjuFtAmAWKjA,1935
+cjtool-0.29.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+cjtool-0.29.8.dist-info/entry_points.txt,sha256=AWsqHhznLRvyrE6X5j68-B3xsMz7SRbx6glhSxb36qI,221
+cjtool-0.29.8.dist-info/top_level.txt,sha256=xT9DqEuxuB3mnAq-fVy_mWHaaTT3M-S7J_93pQnE7W8,7
+cjtool-0.29.8.dist-info/RECORD,,
```

