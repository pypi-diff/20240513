# Comparing `tmp/nanopb-0.4.9.dev1465.tar.gz` & `tmp/nanopb-0.4.9.dev1472.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.9.dev1465.tar", max compression
+gzip compressed data, was "nanopb-0.4.9.dev1472.tar", max compression
```

## Comparing `nanopb-0.4.9.dev1465.tar` & `nanopb-0.4.9.dev1472.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4461 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/README.md
--rw-r--r--   0        0        0        0 2024-04-22 02:09:19.262771 nanopb-0.4.9.dev1465/nanopb/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 02:09:19.262771 nanopb-0.4.9.dev1465/nanopb/generator/__init__.py
--rwxr-xr-x   0        0        0      235 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator
--rw-r--r--   0        0        0      206 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.bat
--rwxr-xr-x   0        0        0   112055 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py
--rwxr-xr-x   0        0        0      460 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py2
--rw-r--r--   0        0        0     5839 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/platformio_generator.py
--rw-r--r--   0        0        0      126 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/Makefile
--rw-r--r--   0        0        0     4851 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/__init__.py
--rw-r--r--   0        0        0     3431 2024-04-22 02:09:19.278771 nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2662 2024-04-22 02:09:19.354771 nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2790 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/_utils.py
--rw-r--r--   0        0        0    36277 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     7139 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb.proto
--rw-r--r--   0        0        0     4443 2024-04-22 02:09:19.362772 nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb_pb2.py
--rwxr-xr-x   0        0        0     1577 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc
--rwxr-xr-x   0        0        0      374 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb
--rwxr-xr-x   0        0        0      554 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb-py2
--rw-r--r--   0        0        0      449 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb.bat
--rw-r--r--   0        0        0      302 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc.bat
--rw-r--r--   0        0        0     1065 2024-04-22 02:09:19.382772 nanopb-0.4.9.dev1465/pyproject.toml
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1465/PKG-INFO
+-rw-r--r--   0        0        0     4461 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 02:09:03.941521 nanopb-0.4.9.dev1472/nanopb/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:09:03.941521 nanopb-0.4.9.dev1472/nanopb/generator/__init__.py
+-rwxr-xr-x   0        0        0      235 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator
+-rw-r--r--   0        0        0      206 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.bat
+-rwxr-xr-x   0        0        0   112055 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py
+-rwxr-xr-x   0        0        0      460 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py2
+-rw-r--r--   0        0        0     5839 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/platformio_generator.py
+-rw-r--r--   0        0        0      126 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/Makefile
+-rw-r--r--   0        0        0     4629 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/__init__.py
+-rw-r--r--   0        0        0     3376 2024-05-13 02:09:03.961521 nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2804 2024-05-13 02:09:04.033520 nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2949 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/_utils.py
+-rw-r--r--   0        0        0    36277 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     7139 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb.proto
+-rw-r--r--   0        0        0     4445 2024-05-13 02:09:04.045520 nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb_pb2.py
+-rwxr-xr-x   0        0        0     1577 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc
+-rwxr-xr-x   0        0        0      374 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb
+-rwxr-xr-x   0        0        0      554 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb-py2
+-rw-r--r--   0        0        0      449 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb.bat
+-rw-r--r--   0        0        0      302 2024-05-06 13:53:00.000000 nanopb-0.4.9.dev1472/nanopb/generator/protoc.bat
+-rw-r--r--   0        0        0     1065 2024-05-13 02:09:04.065520 nanopb-0.4.9.dev1472/pyproject.toml
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1472/PKG-INFO
```

### Comparing `nanopb-0.4.9.dev1465/README.md` & `nanopb-0.4.9.dev1472/README.md`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py` & `nanopb-0.4.9.dev1472/nanopb/generator/nanopb_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/platformio_generator.py` & `nanopb-0.4.9.dev1472/nanopb/generator/platformio_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/__init__.py` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,72 +63,66 @@
     # 3) Use protoc to build it, but store only temporarily in system-wide temp folder
     #
     # By default these are tried in numeric order.
     # If NANOPB_PB2_TEMP_DIR environment variable is defined, the 2) is skipped.
     # If the value of the $NANOPB_PB2_TEMP_DIR exists as a directory, it is used instead
     # of system temp folder.
 
-    build_error = None
-    proto_ok = False
     tmpdir = os.getenv("NANOPB_PB2_TEMP_DIR")
     temporary_only = (tmpdir is not None)
     dirname = os.path.dirname(__file__)
     protosrc = os.path.join(dirname, "nanopb.proto")
     protodst = os.path.join(dirname, "nanopb_pb2.py")
-    proto_ok = False
 
     if tmpdir is not None and not os.path.isdir(tmpdir):
         tmpdir = None # Use system-wide temp dir
 
     no_rebuild = bool(int(os.getenv("NANOPB_PB2_NO_REBUILD", default = 0)))
     if bool(no_rebuild):
         # Don't attempt to autogenerate nanopb_pb2.py, external build rules
         # should have already done so.
         import nanopb_pb2 as nanopb_pb2_mod
-        proto_ok = True
-    elif os.path.isfile(protosrc):
+        return nanopb_pb2_mod
+
+    if os.path.isfile(protosrc):
         src_date = os.path.getmtime(protosrc)
-        if not os.path.isfile(protodst) or os.path.getmtime(protodst) < src_date:
-            # Outdated, rebuild
-            proto_ok = False
-        else:
+        if os.path.isfile(protodst) and os.path.getmtime(protodst) >= src_date:
             try:
                 from . import nanopb_pb2 as nanopb_pb2_mod
-                proto_ok = True
+                return nanopb_pb2_mod
             except Exception as e:
                 sys.stderr.write("Failed to import nanopb_pb2.py: " + str(e) + "\n"
                                 "Will automatically attempt to rebuild this.\n"
                                 "Verify that python-protobuf and protoc versions match.\n")
                 print_versions()
 
     # Try to rebuild into generator/proto directory
-    if not proto_ok and not temporary_only:
-        proto_ok = build_nanopb_proto(protosrc, dirname)
+    if not temporary_only:
+        build_nanopb_proto(protosrc, dirname)
 
         try:
             from . import nanopb_pb2 as nanopb_pb2_mod
+            return nanopb_pb2_mod
         except:
             sys.stderr.write("Failed to import generator/proto/nanopb_pb2.py:\n")
             sys.stderr.write(traceback.format_exc() + "\n")
 
     # Try to rebuild into temporary directory
-    if not proto_ok:
-        with TemporaryDirectory(prefix = 'nanopb-', dir = tmpdir) as protodir:
-            proto_ok = build_nanopb_proto(protosrc, protodir)
+    with TemporaryDirectory(prefix = 'nanopb-', dir = tmpdir) as protodir:
+        build_nanopb_proto(protosrc, protodir)
 
-            if protodir not in sys.path:
-                sys.path.insert(0, protodir)
+        if protodir not in sys.path:
+            sys.path.insert(0, protodir)
 
-            try:
-                import nanopb_pb2 as nanopb_pb2_mod
-            except:
-                sys.stderr.write("Failed to import %s/nanopb_pb2.py:\n" % protodir)
-                sys.stderr.write(traceback.format_exc() + "\n")
+        try:
+            import nanopb_pb2 as nanopb_pb2_mod
+            return nanopb_pb2_mod
+        except:
+            sys.stderr.write("Failed to import %s/nanopb_pb2.py:\n" % protodir)
+            sys.stderr.write(traceback.format_exc() + "\n")
 
     # If everything fails
-    if not proto_ok:
-        sys.stderr.write("\n\nGenerating nanopb_pb2.py failed.\n")
-        sys.stderr.write("Make sure that a protoc generator is available and matches python-protobuf version.\n")
-        print_versions()
-        sys.exit(1)
+    sys.stderr.write("\n\nGenerating nanopb_pb2.py failed.\n")
+    sys.stderr.write("Make sure that a protoc generator is available and matches python-protobuf version.\n")
+    print_versions()
+    sys.exit(1)
 
-    return nanopb_pb2_mod
```

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 19 15:52:04 2024 UTC, .py size: 4851 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2493 2266 f312 0000  U.......$."f....
+00000000: 550d 0d0a 0000 0000 bce0 3866 1512 0000  U.........8f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6404 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
@@ -106,110 +106,106 @@
 00000690: 7569 6c74 696e 5f70 726f 746f 5f69 6e63  uiltin_proto_inc
 000006a0: 6c75 6465 720e 0000 0072 0e00 0000 720f  luder....r....r.
 000006b0: 0000 00da 1262 7569 6c64 5f6e 616e 6f70  .....build_nanop
 000006c0: 625f 7072 6f74 6f1e 0000 0073 1e00 0000  b_proto....s....
 000006d0: 0006 0201 0801 0201 08fc 0407 0603 0c01  ................
 000006e0: 1002 0201 0e01 0601 1a01 1401 0802 722a  ..............r*
 000006f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000700: 0c00 0000 0a00 0000 4300 0000 7324 0200  ........C...s$..
-00000710: 0064 007d 0064 017d 0174 00a0 0164 02a1  .d.}.d.}.t...d..
-00000720: 017d 027c 0264 006b 097d 0374 006a 02a0  .}.|.d.k.}.t.j..
-00000730: 0374 04a1 017d 0474 006a 02a0 057c 0464  .t...}.t.j...|.d
-00000740: 03a1 027d 0574 006a 02a0 057c 0464 04a1  ...}.t.j...|.d..
-00000750: 027d 0664 017d 017c 0264 006b 0972 5e74  .}.d.}.|.d.k.r^t
-00000760: 006a 02a0 067c 02a1 0173 5e64 007d 0274  .j...|...s^d.}.t
-00000770: 0774 0874 006a 0164 0564 0664 078d 0283  .t.t.j.d.d.d....
-00000780: 0183 017d 0774 077c 0783 0172 8a64 0664  ...}.t.|...r.d.d
-00000790: 006c 097d 0864 087d 016e 9474 006a 02a0  .l.}.d.}.n.t.j..
-000007a0: 0a7c 05a1 0190 0172 1e74 006a 02a0 0b7c  .|.....r.t.j...|
-000007b0: 05a1 017d 0974 006a 02a0 0a7c 06a1 0172  ...}.t.j...|...r
-000007c0: c074 006a 02a0 0b7c 06a1 017c 096b 0072  .t.j...|...|.k.r
-000007d0: c664 017d 016e 587a 1464 0964 0a6c 0c6d  .d.}.nXz.d.d.l.m
-000007e0: 097d 0801 0064 087d 0157 006e 4204 0074  .}...d.}.W.nB..t
-000007f0: 0d6b 0a90 0172 1c01 007d 0a01 007a 2274  .k...r...}...z"t
-00000800: 0e6a 0fa0 1064 0b74 117c 0a83 0117 0064  .j...d.t.|.....d
-00000810: 0c17 00a1 0101 0074 1283 0001 0057 0035  .......t.....W.5
-00000820: 0064 007d 0a7e 0a58 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
-00000830: 0190 0173 727c 0390 0173 7274 137c 057c  ...sr|...srt.|.|
-00000840: 0483 027d 017a 1064 0964 0a6c 0c6d 097d  ...}.z.d.d.l.m.}
-00000850: 0801 0057 006e 2c01 0001 0001 0074 0e6a  ...W.n,......t.j
-00000860: 0fa0 1064 0da1 0101 0074 0e6a 0fa0 1074  ...d.....t.j...t
-00000870: 14a0 15a1 0064 0e17 00a1 0101 0059 006e  .....d.......Y.n
-00000880: 0258 007c 0190 0173 f274 1664 0f7c 0264  .X.|...s.t.d.|.d
-00000890: 108d 028f 687d 0b74 137c 057c 0b83 027d  ....h}.t.|.|...}
-000008a0: 017c 0b74 0e6a 026b 0790 0172 aa74 0e6a  .|.t.j.k...r.t.j
-000008b0: 02a0 1764 067c 0ba1 0201 007a 0c64 0664  ...d.|.....z.d.d
-000008c0: 006c 097d 0857 006e 3001 0001 0001 0074  .l.}.W.n0......t
-000008d0: 0e6a 0fa0 1064 117c 0b16 00a1 0101 0074  .j...d.|.......t
-000008e0: 0e6a 0fa0 1074 14a0 15a1 0064 0e17 00a1  .j...t.....d....
-000008f0: 0101 0059 006e 0258 0057 0035 0051 0052  ...Y.n.X.W.5.Q.R
-00000900: 0058 007c 0190 0273 2074 0e6a 0fa0 1064  .X.|...s t.j...d
-00000910: 12a1 0101 0074 0e6a 0fa0 1064 13a1 0101  .....t.j...d....
-00000920: 0074 1283 0001 0074 0ea0 1864 09a1 0101  .t.....t...d....
-00000930: 007c 0853 0029 144e 465a 134e 414e 4f50  .|.S.).NFZ.NANOP
-00000940: 425f 5042 325f 5445 4d50 5f44 4952 7a0c  B_PB2_TEMP_DIRz.
-00000950: 6e61 6e6f 7062 2e70 726f 746f 7a0d 6e61  nanopb.protoz.na
-00000960: 6e6f 7062 5f70 6232 2e70 795a 154e 414e  nopb_pb2.pyZ.NAN
-00000970: 4f50 425f 5042 325f 4e4f 5f52 4542 5549  OPB_PB2_NO_REBUI
-00000980: 4c44 7201 0000 0029 01da 0764 6566 6175  LDr....)...defau
-00000990: 6c74 5472 0300 0000 2901 da0a 6e61 6e6f  ltTr....)...nano
-000009a0: 7062 5f70 6232 7a20 4661 696c 6564 2074  pb_pb2z Failed t
-000009b0: 6f20 696d 706f 7274 206e 616e 6f70 625f  o import nanopb_
-000009c0: 7062 322e 7079 3a20 7a64 0a57 696c 6c20  pb2.py: zd.Will 
-000009d0: 6175 746f 6d61 7469 6361 6c6c 7920 6174  automatically at
-000009e0: 7465 6d70 7420 746f 2072 6562 7569 6c64  tempt to rebuild
-000009f0: 2074 6869 732e 0a56 6572 6966 7920 7468   this..Verify th
-00000a00: 6174 2070 7974 686f 6e2d 7072 6f74 6f62  at python-protob
-00000a10: 7566 2061 6e64 2070 726f 746f 6320 7665  uf and protoc ve
-00000a20: 7273 696f 6e73 206d 6174 6368 2e0a 7a30  rsions match..z0
-00000a30: 4661 696c 6564 2074 6f20 696d 706f 7274  Failed to import
-00000a40: 2067 656e 6572 6174 6f72 2f70 726f 746f   generator/proto
-00000a50: 2f6e 616e 6f70 625f 7062 322e 7079 3a0a  /nanopb_pb2.py:.
-00000a60: 721d 0000 007a 076e 616e 6f70 622d 720a  r....z.nanopb-r.
-00000a70: 0000 007a 2346 6169 6c65 6420 746f 2069  ...z#Failed to i
-00000a80: 6d70 6f72 7420 2573 2f6e 616e 6f70 625f  mport %s/nanopb_
-00000a90: 7062 322e 7079 3a0a 7a23 0a0a 4765 6e65  pb2.py:.z#..Gene
-00000aa0: 7261 7469 6e67 206e 616e 6f70 625f 7062  rating nanopb_pb
-00000ab0: 322e 7079 2066 6169 6c65 642e 0a7a 544d  2.py failed..zTM
-00000ac0: 616b 6520 7375 7265 2074 6861 7420 6120  ake sure that a 
-00000ad0: 7072 6f74 6f63 2067 656e 6572 6174 6f72  protoc generator
-00000ae0: 2069 7320 6176 6169 6c61 626c 6520 616e   is available an
-00000af0: 6420 6d61 7463 6865 7320 7079 7468 6f6e  d matches python
-00000b00: 2d70 726f 746f 6275 6620 7665 7273 696f  -protobuf versio
-00000b10: 6e2e 0a29 19da 026f 73da 0667 6574 656e  n..)...os..geten
-00000b20: 76da 0470 6174 6872 2800 0000 da08 5f5f  v..pathr(.....__
-00000b30: 6669 6c65 5f5f 7224 0000 00da 0569 7364  file__r$.....isd
-00000b40: 6972 da04 626f 6f6c da03 696e 7472 2c00  ir..bool..intr,.
-00000b50: 0000 da06 6973 6669 6c65 da08 6765 746d  ....isfile..getm
-00000b60: 7469 6d65 da00 da09 4578 6365 7074 696f  time....Exceptio
-00000b70: 6e72 2100 0000 7222 0000 0072 2300 0000  nr!...r"...r#...
-00000b80: da03 7374 7272 0600 0000 722a 0000 0072  ..strr....r*...r
-00000b90: 2500 0000 7226 0000 0072 0700 0000 da06  %...r&...r......
-00000ba0: 696e 7365 7274 da04 6578 6974 290c 5a0b  insert..exit).Z.
-00000bb0: 6275 696c 645f 6572 726f 725a 0870 726f  build_errorZ.pro
-00000bc0: 746f 5f6f 6b5a 0674 6d70 6469 725a 0e74  to_okZ.tmpdirZ.t
-00000bd0: 656d 706f 7261 7279 5f6f 6e6c 7972 2800  emporary_onlyr(.
-00000be0: 0000 7227 0000 005a 0870 726f 746f 6473  ..r'...Z.protods
-00000bf0: 745a 0a6e 6f5f 7265 6275 696c 645a 0e6e  tZ.no_rebuildZ.n
-00000c00: 616e 6f70 625f 7062 325f 6d6f 645a 0873  anopb_pb2_modZ.s
-00000c10: 7263 5f64 6174 65da 0165 5a08 7072 6f74  rc_date..eZ.prot
-00000c20: 6f64 6972 720e 0000 0072 0e00 0000 720f  odirr....r....r.
-00000c30: 0000 00da 0f6c 6f61 645f 6e61 6e6f 7062  .....load_nanopb
-00000c40: 5f70 6232 3900 0000 735e 0000 0000 0d04  _pb29...s^......
-00000c50: 0104 010a 0108 010c 010e 010e 0104 0214  ................
-00000c60: 0104 0216 0108 0308 0106 010e 010c 011c  ................
-00000c70: 0206 0202 010c 0108 0112 0118 0318 030c  ................
-00000c80: 010a 0202 0110 0106 010c 011a 0306 010e  ................
-00000c90: 010a 020c 010e 0202 010c 0106 0110 0124  ...............$
-00000ca0: 0306 010c 010c 0106 010a 0272 3c00 0000  ...........r<...
-00000cb0: 2912 7219 0000 005a 0a5f 5f66 7574 7572  ).r....Z.__futur
-00000cc0: 655f 5f72 0200 0000 722d 0000 00da 076f  e__r....r-.....o
-00000cd0: 732e 7061 7468 7221 0000 0072 1100 0000  s.pathr!...r....
-00000ce0: 7213 0000 0072 2500 0000 721f 0000 005a  r....r%...r....Z
-00000cf0: 065f 7574 696c 7372 0400 0000 7205 0000  ._utilsr....r...
-00000d00: 0072 0600 0000 7207 0000 00da 0b49 6d70  .r....r......Imp
-00000d10: 6f72 7445 7272 6f72 722a 0000 0072 3c00  ortErrorr*...r<.
-00000d20: 0000 720e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000d30: 0072 0f00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000d40: 0100 0000 731e 0000 0004 010c 0208 0108  ....s...........
-00000d50: 0108 0108 0108 0108 0108 0114 0302 0110  ................
-00000d60: 010e 0114 0d08 1b                        .......
+00000700: 0a00 0000 0a00 0000 4300 0000 7310 0200  ........C...s...
+00000710: 0074 00a0 0164 01a1 017d 007c 0064 006b  .t...d...}.|.d.k
+00000720: 097d 0174 006a 02a0 0374 04a1 017d 0274  .}.t.j...t...}.t
+00000730: 006a 02a0 057c 0264 02a1 027d 0374 006a  .j...|.d...}.t.j
+00000740: 02a0 057c 0264 03a1 027d 047c 0064 006b  ...|.d...}.|.d.k
+00000750: 0972 5274 006a 02a0 067c 00a1 0173 5264  .rRt.j...|...sRd
+00000760: 007d 0074 0774 0874 006a 0164 0464 0564  .}.t.t.t.j.d.d.d
+00000770: 068d 0283 0183 017d 0574 077c 0583 0172  .......}.t.|...r
+00000780: 7c64 0564 006c 097d 067c 0653 0074 006a  |d.d.l.}.|.S.t.j
+00000790: 02a0 0a7c 03a1 0190 0172 0c74 006a 02a0  ...|.....r.t.j..
+000007a0: 0b7c 03a1 017d 0774 006a 02a0 0a7c 04a1  .|...}.t.j...|..
+000007b0: 0190 0172 0c74 006a 02a0 0b7c 04a1 017c  ...r.t.j...|...|
+000007c0: 076b 0590 0172 0c7a 1264 0764 086c 0c6d  .k...r.z.d.d.l.m
+000007d0: 097d 0601 007c 0657 0053 0004 0074 0d6b  .}...|.W.S...t.k
+000007e0: 0a90 0172 0a01 007d 0801 007a 2274 0e6a  ...r...}...z"t.j
+000007f0: 0fa0 1064 0974 117c 0883 0117 0064 0a17  ...d.t.|.....d..
+00000800: 00a1 0101 0074 1283 0001 0057 0035 0064  .....t.....W.5.d
+00000810: 007d 087e 0858 0059 006e 0258 007c 0190  .}.~.X.Y.n.X.|..
+00000820: 0173 5c74 137c 037c 0283 0201 007a 1264  .s\t.|.|.....z.d
+00000830: 0764 086c 0c6d 097d 0601 007c 0657 0053  .d.l.m.}...|.W.S
+00000840: 0001 0001 0001 0074 0e6a 0fa0 1064 0ba1  .......t.j...d..
+00000850: 0101 0074 0e6a 0fa0 1074 14a0 15a1 0064  ...t.j...t.....d
+00000860: 0c17 00a1 0101 0059 006e 0258 0074 1664  .......Y.n.X.t.d
+00000870: 0d7c 0064 0e8d 028f 767d 0974 137c 037c  .|.d....v}.t.|.|
+00000880: 0983 0201 007c 0974 0e6a 026b 0790 0172  .....|.t.j.k...r
+00000890: 8e74 0e6a 02a0 1764 057c 09a1 0201 007a  .t.j...d.|.....z
+000008a0: 1a64 0564 006c 097d 067c 0657 0057 0002  .d.d.l.}.|.W.W..
+000008b0: 0035 0051 0052 00a3 0053 0001 0001 0001  .5.Q.R...S......
+000008c0: 0074 0e6a 0fa0 1064 0f7c 0916 00a1 0101  .t.j...d.|......
+000008d0: 0074 0e6a 0fa0 1074 14a0 15a1 0064 0c17  .t.j...t.....d..
+000008e0: 00a1 0101 0059 006e 0258 0057 0035 0051  .....Y.n.X.W.5.Q
+000008f0: 0052 0058 0074 0e6a 0fa0 1064 10a1 0101  .R.X.t.j...d....
+00000900: 0074 0e6a 0fa0 1064 11a1 0101 0074 1283  .t.j...d.....t..
+00000910: 0001 0074 0ea0 1864 07a1 0101 0064 0053  ...t...d.....d.S
+00000920: 0029 124e 5a13 4e41 4e4f 5042 5f50 4232  .).NZ.NANOPB_PB2
+00000930: 5f54 454d 505f 4449 527a 0c6e 616e 6f70  _TEMP_DIRz.nanop
+00000940: 622e 7072 6f74 6f7a 0d6e 616e 6f70 625f  b.protoz.nanopb_
+00000950: 7062 322e 7079 5a15 4e41 4e4f 5042 5f50  pb2.pyZ.NANOPB_P
+00000960: 4232 5f4e 4f5f 5245 4255 494c 4472 0100  B2_NO_REBUILDr..
+00000970: 0000 2901 da07 6465 6661 756c 7472 0300  ..)...defaultr..
+00000980: 0000 2901 da0a 6e61 6e6f 7062 5f70 6232  ..)...nanopb_pb2
+00000990: 7a20 4661 696c 6564 2074 6f20 696d 706f  z Failed to impo
+000009a0: 7274 206e 616e 6f70 625f 7062 322e 7079  rt nanopb_pb2.py
+000009b0: 3a20 7a64 0a57 696c 6c20 6175 746f 6d61  : zd.Will automa
+000009c0: 7469 6361 6c6c 7920 6174 7465 6d70 7420  tically attempt 
+000009d0: 746f 2072 6562 7569 6c64 2074 6869 732e  to rebuild this.
+000009e0: 0a56 6572 6966 7920 7468 6174 2070 7974  .Verify that pyt
+000009f0: 686f 6e2d 7072 6f74 6f62 7566 2061 6e64  hon-protobuf and
+00000a00: 2070 726f 746f 6320 7665 7273 696f 6e73   protoc versions
+00000a10: 206d 6174 6368 2e0a 7a30 4661 696c 6564   match..z0Failed
+00000a20: 2074 6f20 696d 706f 7274 2067 656e 6572   to import gener
+00000a30: 6174 6f72 2f70 726f 746f 2f6e 616e 6f70  ator/proto/nanop
+00000a40: 625f 7062 322e 7079 3a0a 721d 0000 007a  b_pb2.py:.r....z
+00000a50: 076e 616e 6f70 622d 720a 0000 007a 2346  .nanopb-r....z#F
+00000a60: 6169 6c65 6420 746f 2069 6d70 6f72 7420  ailed to import 
+00000a70: 2573 2f6e 616e 6f70 625f 7062 322e 7079  %s/nanopb_pb2.py
+00000a80: 3a0a 7a23 0a0a 4765 6e65 7261 7469 6e67  :.z#..Generating
+00000a90: 206e 616e 6f70 625f 7062 322e 7079 2066   nanopb_pb2.py f
+00000aa0: 6169 6c65 642e 0a7a 544d 616b 6520 7375  ailed..zTMake su
+00000ab0: 7265 2074 6861 7420 6120 7072 6f74 6f63  re that a protoc
+00000ac0: 2067 656e 6572 6174 6f72 2069 7320 6176   generator is av
+00000ad0: 6169 6c61 626c 6520 616e 6420 6d61 7463  ailable and matc
+00000ae0: 6865 7320 7079 7468 6f6e 2d70 726f 746f  hes python-proto
+00000af0: 6275 6620 7665 7273 696f 6e2e 0a29 19da  buf version..)..
+00000b00: 026f 73da 0667 6574 656e 76da 0470 6174  .os..getenv..pat
+00000b10: 6872 2800 0000 da08 5f5f 6669 6c65 5f5f  hr(.....__file__
+00000b20: 7224 0000 00da 0569 7364 6972 da04 626f  r$.....isdir..bo
+00000b30: 6f6c da03 696e 7472 2c00 0000 da06 6973  ol..intr,.....is
+00000b40: 6669 6c65 da08 6765 746d 7469 6d65 da00  file..getmtime..
+00000b50: da09 4578 6365 7074 696f 6e72 2100 0000  ..Exceptionr!...
+00000b60: 7222 0000 0072 2300 0000 da03 7374 7272  r"...r#.....strr
+00000b70: 0600 0000 722a 0000 0072 2500 0000 7226  ....r*...r%...r&
+00000b80: 0000 0072 0700 0000 da06 696e 7365 7274  ...r......insert
+00000b90: da04 6578 6974 290a 5a06 746d 7064 6972  ..exit).Z.tmpdir
+00000ba0: 5a0e 7465 6d70 6f72 6172 795f 6f6e 6c79  Z.temporary_only
+00000bb0: 7228 0000 0072 2700 0000 5a08 7072 6f74  r(...r'...Z.prot
+00000bc0: 6f64 7374 5a0a 6e6f 5f72 6562 7569 6c64  odstZ.no_rebuild
+00000bd0: 5a0e 6e61 6e6f 7062 5f70 6232 5f6d 6f64  Z.nanopb_pb2_mod
+00000be0: 5a08 7372 635f 6461 7465 da01 655a 0870  Z.src_date..eZ.p
+00000bf0: 726f 746f 6469 7272 0e00 0000 720e 0000  rotodirr....r...
+00000c00: 0072 0f00 0000 da0f 6c6f 6164 5f6e 616e  .r......load_nan
+00000c10: 6f70 625f 7062 3239 0000 0073 5400 0000  opb_pb29...sT...
+00000c20: 000d 0a01 0801 0c01 0e01 0e02 1401 0402  ................
+00000c30: 1601 0803 0801 0402 0e01 0c01 2001 0201  ............ ...
+00000c40: 0c01 0601 1201 1803 1803 0601 0a02 0201  ................
+00000c50: 0c01 0601 0601 0c01 1a03 0e01 0a02 0c01  ................
+00000c60: 0e02 0201 0801 1201 0601 1001 2403 0c01  ............$...
+00000c70: 0c01 0601 723c 0000 0029 1272 1900 0000  ....r<...).r....
+00000c80: 5a0a 5f5f 6675 7475 7265 5f5f 7202 0000  Z.__future__r...
+00000c90: 0072 2d00 0000 da07 6f73 2e70 6174 6872  .r-.....os.pathr
+00000ca0: 2100 0000 7211 0000 0072 1300 0000 7225  !...r....r....r%
+00000cb0: 0000 0072 1f00 0000 5a06 5f75 7469 6c73  ...r....Z._utils
+00000cc0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000cd0: 0700 0000 da0b 496d 706f 7274 4572 726f  ......ImportErro
+00000ce0: 7272 2a00 0000 723c 0000 0072 0e00 0000  rr*...r<...r....
+00000cf0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00000d00: 083c 6d6f 6475 6c65 3e01 0000 0073 1e00  .<module>....s..
+00000d10: 0000 0401 0c02 0801 0801 0801 0801 0801  ................
+00000d20: 0801 0801 1403 0201 1001 0e01 140d 081b  ................
```

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 19 15:52:04 2024 UTC, .py size: 2790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,167 +1,176 @@
-00000000: 550d 0d0a 0000 0000 2493 2266 e60a 0000  U.......$."f....
+00000000: 550d 0d0a 0000 0000 bce0 3866 850b 0000  U.........8f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
+00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 6402 6403 8400 5a04 6404  d.l.Z.d.d...Z.d.
-00000050: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
-00000060: 6409 8400 5a07 6508 640a 6b02 7246 6507  d...Z.e.d.k.rFe.
-00000070: 8300 0100 6401 5300 290b e900 0000 004e  ....d.S.)......N
-00000080: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00000090: 0008 0000 0043 0000 0073 2800 0000 7a0c  .....C...s(...z.
-000000a0: 6401 6402 6c00 7d00 5700 6e16 0400 7401  d.d.l.}.W.n...t.
-000000b0: 6b0a 7222 0100 0100 0100 5900 6403 5300  k.r"......Y.d.S.
-000000c0: 5800 6404 5300 2905 7a2b 2063 6865 636b  X.d.S.).z+ check
-000000d0: 7320 6966 2067 7270 6369 6f2d 746f 6f6c  s if grpcio-tool
-000000e0: 7320 7072 6f74 6f63 2069 7320 696e 7374  s protoc is inst
-000000f0: 616c 6c65 6472 0100 0000 4e46 5429 02da  alledr....NFT)..
-00000100: 1167 7270 635f 746f 6f6c 732e 7072 6f74  .grpc_tools.prot
-00000110: 6f63 da0b 496d 706f 7274 4572 726f 7229  oc..ImportError)
-00000120: 01da 0a67 7270 635f 746f 6f6c 73a9 0072  ...grpc_tools..r
-00000130: 0500 0000 fa5a 2f68 6f6d 652f 7275 6e6e  .....Z/home/runn
-00000140: 6572 2f77 6f72 6b2f 6e61 6e6f 7062 2f6e  er/work/nanopb/n
-00000150: 616e 6f70 622f 6e61 6e6f 7062 2f65 7874  anopb/nanopb/ext
-00000160: 7261 2f70 6f65 7472 792f 6275 696c 642f  ra/poetry/build/
-00000170: 6e61 6e6f 7062 2f67 656e 6572 6174 6f72  nanopb/generator
-00000180: 2f70 726f 746f 2f5f 7574 696c 732e 7079  /proto/_utils.py
-00000190: da11 6861 735f 6772 7063 696f 5f70 726f  ..has_grpcio_pro
-000001a0: 746f 6305 0000 0073 0a00 0000 0004 0201  toc....s........
-000001b0: 0c01 0e01 0801 7207 0000 0063 0000 0000  ......r....c....
-000001c0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-000001d0: 4300 0000 738a 0000 0074 0074 0164 0164  C...s....t.t.d.d
-000001e0: 0283 0372 5074 026a 03a0 0474 026a 03a0  ...rPt.j...t.j..
-000001f0: 0574 026a 03a0 0674 016a 07a1 01a1 0164  .t.j...t.j.....d
-00000200: 03a1 0274 026a 03a0 0474 026a 03a0 0574  ...t.j...t.j...t
-00000210: 026a 03a0 0674 016a 07a1 01a1 0164 0464  .j...t.j.....d.d
-00000220: 05a1 0367 027d 006e 3674 026a 03a0 0574  ...g.}.n6t.j...t
-00000230: 026a 03a0 0674 08a1 01a1 0167 017d 0074  .j...t.....g.}.t
-00000240: 0983 0072 8664 0664 076c 0a7d 017c 00a0  ...r.d.d.l.}.|..
-00000250: 0b7c 01a0 0c64 0464 05a1 02a1 0101 007c  .|...d.d.......|
-00000260: 0053 0029 087a 5646 696e 6420 696e 636c  .S.).zVFind incl
-00000270: 7564 6520 7061 7468 2066 6f72 2073 7461  ude path for sta
-00000280: 6e64 6172 6420 676f 6f67 6c65 2f70 726f  ndard google/pro
-00000290: 746f 6275 6620 696e 636c 7564 6573 2061  tobuf includes a
-000002a0: 6e64 2066 6f72 0a20 2020 206e 616e 6f70  nd for.    nanop
-000002b0: 622e 7072 6f74 6f2e 0a20 2020 20da 0666  b.proto..    ..f
-000002c0: 726f 7a65 6e46 da05 7072 6f74 6f72 0400  rozenF..protor..
-000002d0: 0000 da06 5f70 726f 746f 7201 0000 004e  ...._protor....N
-000002e0: 290d da07 6765 7461 7474 72da 0373 7973  )...getattr..sys
-000002f0: da02 6f73 da04 7061 7468 da04 6a6f 696e  ..os..path..join
-00000300: da07 6469 726e 616d 65da 0761 6273 7061  ..dirname..abspa
-00000310: 7468 da0a 6578 6563 7574 6162 6c65 da08  th..executable..
-00000320: 5f5f 6669 6c65 5f5f 7207 0000 00da 0d70  __file__r......p
-00000330: 6b67 5f72 6573 6f75 7263 6573 da06 6170  kg_resources..ap
-00000340: 7065 6e64 da11 7265 736f 7572 6365 5f66  pend..resource_f
-00000350: 696c 656e 616d 6529 02da 0570 6174 6873  ilename)...paths
-00000360: 7214 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-00000370: 0600 0000 da1e 6765 745f 7072 6f74 6f5f  ......get_proto_
-00000380: 6275 696c 7469 6e5f 696e 636c 7564 655f  builtin_include_
-00000390: 7061 7468 0f00 0000 7314 0000 0000 050c  path....s.......
-000003a0: 031e 0120 fe06 0812 ff04 0406 0108 0112  ... ............
-000003b0: 0272 1800 0000 6301 0000 0000 0000 0000  .r....c.........
-000003c0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000003d0: 5c00 0000 6401 6402 8400 7c00 4400 8301  \...d.d...|.D...
-000003e0: 7318 7c00 a000 6403 a101 0100 7401 8300  s.|...d.....t...
-000003f0: 4400 5d12 7d01 7c00 a000 6404 7c01 1700  D.].}.|...d.|...
-00000400: a101 0100 711e 7402 8300 724e 6405 6406  ....q.t...rNd.d.
-00000410: 6c03 6d04 7d02 0100 7c02 a005 7c00 a101  l.m.}...|...|...
-00000420: 5300 7406 a007 7c00 a101 5300 6406 5300  S.t...|...S.d.S.
-00000430: 2907 7ad5 0a20 2020 2049 6e76 6f6b 6520  ).z..    Invoke 
-00000440: 7072 6f74 6f63 2e0a 0a20 2020 2054 6869  protoc...    Thi
-00000450: 7320 726f 7574 696e 6520 7769 6c6c 2075  s routine will u
-00000460: 7365 2067 7270 6369 6f2d 7072 6f76 6964  se grpcio-provid
-00000470: 6564 2070 726f 746f 6320 6966 2069 7420  ed protoc if it 
-00000480: 6578 6973 7473 2c0a 2020 2020 7573 696e  exists,.    usin
-00000490: 6720 7379 7374 656d 2d69 6e73 7461 6c6c  g system-install
-000004a0: 6564 2070 726f 746f 6320 6173 2061 2066  ed protoc as a f
-000004b0: 616c 6c62 6163 6b2e 0a0a 2020 2020 4172  allback...    Ar
-000004c0: 6773 3a0a 2020 2020 2020 2020 6172 6776  gs:.        argv
-000004d0: 3a20 7072 6f74 6f63 2043 4c49 2069 6e76  : protoc CLI inv
-000004e0: 6f63 6174 696f 6e2c 2066 6972 7374 2069  ocation, first i
-000004f0: 7465 6d20 6d75 7374 2062 6520 2770 726f  tem must be 'pro
-00000500: 746f 6327 0a20 2020 2063 0100 0000 0000  toc'.    c......
-00000510: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00000520: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
-00000530: 01a0 0064 00a1 0172 047c 0191 0271 0453  ...d...r.|...q.S
-00000540: 0029 01fa 022d 4929 01da 0a73 7461 7274  .)...-I)...start
-00000550: 7377 6974 6829 02da 022e 30da 0178 7205  swith)....0..xr.
-00000560: 0000 0072 0500 0000 7206 0000 00da 0a3c  ...r....r......<
-00000570: 6c69 7374 636f 6d70 3e34 0000 0073 0600  listcomp>4...s..
-00000580: 0000 0600 0200 0a00 7a21 696e 766f 6b65  ........z!invoke
-00000590: 5f70 726f 746f 632e 3c6c 6f63 616c 733e  _protoc.<locals>
-000005a0: 2e3c 6c69 7374 636f 6d70 3e7a 032d 492e  .<listcomp>z.-I.
-000005b0: 7219 0000 0072 0100 0000 4e29 0872 1500  r....r....N).r..
-000005c0: 0000 7218 0000 0072 0700 0000 7202 0000  ..r....r....r...
-000005d0: 00da 0670 726f 746f 63da 046d 6169 6eda  ...protoc..main.
-000005e0: 0a73 7562 7072 6f63 6573 73da 0463 616c  .subprocess..cal
-000005f0: 6c29 03da 0461 7267 765a 0769 6e63 7061  l)...argvZ.incpa
-00000600: 7468 721e 0000 0072 0500 0000 7205 0000  thr....r....r...
-00000610: 0072 0600 0000 da0d 696e 766f 6b65 5f70  .r......invoke_p
-00000620: 726f 746f 6327 0000 0073 1000 0000 000d  rotoc'...s......
-00000630: 0e01 0a03 0a01 1002 0601 0c01 0a02 7223  ..............r#
-00000640: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000650: 0300 0000 0a00 0000 4300 0000 736e 0100  ........C...sn..
-00000660: 007a 4474 0083 0072 2a64 0164 006c 017d  .zDt...r*d.d.l.}
-00000670: 0074 026a 03a0 0464 027c 006a 056a 0617  .t.j...d.|.j.j..
-00000680: 0064 0317 00a1 0101 006e 0c74 026a 03a0  .d.......n.t.j..
-00000690: 0464 04a1 0101 0074 0764 0564 0667 0283  .d.....t.d.d.g..
-000006a0: 0101 0057 006e 3a04 0074 086b 0a72 7e01  ...W.n:..t.k.r~.
-000006b0: 007d 0101 007a 1c74 026a 03a0 0464 0774  .}...z.t.j...d.t
-000006c0: 097c 0183 0117 0064 0317 00a1 0101 0057  .|.....d.......W
-000006d0: 0035 0064 007d 017e 0158 0059 006e 0258  .5.d.}.~.X.Y.n.X
-000006e0: 007a 1e74 026a 03a0 0464 0874 0974 0a83  .z.t.j...d.t.t..
-000006f0: 0083 0117 0064 0317 00a1 0101 0057 006e  .....d.......W.n
-00000700: 3a04 0074 086b 0a72 d801 007d 0101 007a  :..t.k.r...}...z
-00000710: 1c74 026a 03a0 0464 0974 097c 0183 0117  .t.j...d.t.|....
-00000720: 0064 0317 00a1 0101 0057 0035 0064 007d  .d.......W.5.d.}
-00000730: 017e 0158 0059 006e 0258 007a 5264 0164  .~.X.Y.n.X.zRd.d
-00000740: 006c 0b7d 0274 026a 03a0 0464 0a74 026a  .l.}.t.j...d.t.j
-00000750: 0c17 0064 0317 00a1 0101 0074 026a 03a0  ...d.......t.j..
-00000760: 0464 0b7c 026a 0d6a 0617 0064 0317 00a1  .d.|.j.j...d....
-00000770: 0101 0074 026a 03a0 0464 0c7c 026a 0d6a  ...t.j...d.|.j.j
-00000780: 0e17 0064 0317 00a1 0101 0057 006e 3c04  ...d.......W.n<.
-00000790: 0074 086b 0a90 0172 6801 007d 0101 007a  .t.k...rh..}...z
-000007a0: 1c74 026a 03a0 0464 0d74 097c 0183 0117  .t.j...d.t.|....
-000007b0: 0064 0317 00a1 0101 0057 0035 0064 007d  .d.......W.5.d.}
-000007c0: 017e 0158 0059 006e 0258 0064 0053 0029  .~.X.Y.n.X.d.S.)
-000007d0: 0e4e 7201 0000 007a 1f55 7369 6e67 2067  .Nr....z.Using g
-000007e0: 7270 6369 6f2d 746f 6f6c 7320 7072 6f74  rpcio-tools prot
-000007f0: 6f63 2066 726f 6d20 da01 0a7a 1e55 7369  oc from ...z.Usi
-00000800: 6e67 2070 726f 746f 6320 6672 6f6d 2073  ng protoc from s
-00000810: 7973 7465 6d20 7061 7468 0a72 1e00 0000  ystem path.r....
-00000820: 7a09 2d2d 7665 7273 696f 6e7a 2446 6169  z.--versionz$Fai
-00000830: 6c65 6420 746f 2064 6574 6572 6d69 6e65  led to determine
-00000840: 2070 726f 746f 6320 7665 7273 696f 6e3a   protoc version:
-00000850: 207a 1d70 726f 746f 6320 6275 696c 7469   z.protoc builti
-00000860: 6e20 696e 636c 7564 6520 7061 7468 3a20  n include path: 
-00000870: 7a29 4661 696c 6564 2074 6f20 636f 6e73  z)Failed to cons
-00000880: 7472 7563 7420 7072 6f74 6f63 2069 6e63  truct protoc inc
-00000890: 6c75 6465 2070 6174 683a 207a 0f50 7974  lude path: z.Pyt
-000008a0: 686f 6e20 7665 7273 696f 6e20 7a1b 5573  hon version z.Us
-000008b0: 696e 6720 7079 7468 6f6e 2d70 726f 746f  ing python-proto
-000008c0: 6275 6620 6672 6f6d 207a 1950 7974 686f  buf from z.Pytho
-000008d0: 6e2d 7072 6f74 6f62 7566 2076 6572 7369  n-protobuf versi
-000008e0: 6f6e 3a20 7a2d 4661 696c 6564 2074 6f20  on: z-Failed to 
-000008f0: 6465 7465 726d 696e 6520 7079 7468 6f6e  determine python
-00000900: 2d70 726f 746f 6275 6620 7665 7273 696f  -protobuf versio
-00000910: 6e3a 2029 0f72 0700 0000 7202 0000 0072  n: ).r....r....r
-00000920: 0c00 0000 da06 7374 6465 7272 da05 7772  ......stderr..wr
-00000930: 6974 6572 1e00 0000 7213 0000 0072 2300  iter....r....r#.
-00000940: 0000 da09 4578 6365 7074 696f 6eda 0373  ....Exception..s
-00000950: 7472 7218 0000 005a 0f67 6f6f 676c 652e  trr....Z.google.
-00000960: 7072 6f74 6f62 7566 da07 7665 7273 696f  protobuf..versio
-00000970: 6e5a 0870 726f 746f 6275 66da 0b5f 5f76  nZ.protobuf..__v
-00000980: 6572 7369 6f6e 5f5f 2903 7204 0000 00da  ersion__).r.....
-00000990: 0165 5a06 676f 6f67 6c65 7205 0000 0072  .eZ.googler....r
-000009a0: 0500 0000 7206 0000 00da 0e70 7269 6e74  ....r......print
-000009b0: 5f76 6572 7369 6f6e 7341 0000 0073 2600  _versionsA...s&.
-000009c0: 0000 0001 0201 0601 0801 1a02 0c02 1001  ................
-000009d0: 1001 2a02 0201 1e01 1001 2a02 0201 0801  ..*.......*.....
-000009e0: 1601 1801 1c01 1201 722c 0000 00da 085f  ........r,....._
-000009f0: 5f6d 6169 6e5f 5f29 0972 0c00 0000 7220  _main__).r....r 
-00000a00: 0000 00da 076f 732e 7061 7468 720d 0000  .....os.pathr...
-00000a10: 0072 0700 0000 7218 0000 0072 2300 0000  .r....r....r#...
-00000a20: 722c 0000 00da 085f 5f6e 616d 655f 5f72  r,.....__name__r
-00000a30: 0500 0000 7205 0000 0072 0500 0000 7206  ....r....r....r.
-00000a40: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000a50: 0073 1000 0000 0801 0801 0802 080a 0818  .s..............
-00000a60: 081a 0819 0801                           ......
+00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 640c  d.l.Z.d.d.l.Z.d.
+00000050: 6403 6404 8401 5a05 6405 6406 8400 5a06  d.d...Z.d.d...Z.
+00000060: 6407 6408 8400 5a07 6409 640a 8400 5a08  d.d...Z.d.d...Z.
+00000070: 6509 640b 6b02 7250 6508 8300 0100 6401  e.d.k.rPe.....d.
+00000080: 5300 290d e900 0000 004e 4663 0100 0000  S.)......NFc....
+00000090: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+000000a0: 4300 0000 7340 0000 007a 0c64 0164 026c  C...s@...z.d.d.l
+000000b0: 007d 0157 006e 2e04 0074 016b 0a72 3a01  .}.W.n...t.k.r:.
+000000c0: 0001 0001 007c 0072 3474 026a 03a0 0464  .....|.r4t.j...d
+000000d0: 0374 05a0 06a1 0016 00a1 0101 0059 0064  .t...........Y.d
+000000e0: 0453 0058 0064 0553 0029 067a 2b20 6368  .S.X.d.S.).z+ ch
+000000f0: 6563 6b73 2069 6620 6772 7063 696f 2d74  ecks if grpcio-t
+00000100: 6f6f 6c73 2070 726f 746f 6320 6973 2069  ools protoc is i
+00000110: 6e73 7461 6c6c 6564 7201 0000 004e 7a20  nstalledr....Nz 
+00000120: 4661 696c 6564 2074 6f20 696d 706f 7274  Failed to import
+00000130: 2067 7270 635f 746f 6f6c 733a 2025 730a   grpc_tools: %s.
+00000140: 4654 2907 da11 6772 7063 5f74 6f6f 6c73  FT)...grpc_tools
+00000150: 2e70 726f 746f 63da 0b49 6d70 6f72 7445  .protoc..ImportE
+00000160: 7272 6f72 da03 7379 73da 0673 7464 6572  rror..sys..stder
+00000170: 72da 0577 7269 7465 da09 7472 6163 6562  r..write..traceb
+00000180: 6163 6bda 0a66 6f72 6d61 745f 6578 6329  ack..format_exc)
+00000190: 02da 0776 6572 626f 7365 da0a 6772 7063  ...verbose..grpc
+000001a0: 5f74 6f6f 6c73 a900 720b 0000 00fa 5a2f  _tools..r.....Z/
+000001b0: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
+000001c0: 2f6e 616e 6f70 622f 6e61 6e6f 7062 2f6e  /nanopb/nanopb/n
+000001d0: 616e 6f70 622f 6578 7472 612f 706f 6574  anopb/extra/poet
+000001e0: 7279 2f62 7569 6c64 2f6e 616e 6f70 622f  ry/build/nanopb/
+000001f0: 6765 6e65 7261 746f 722f 7072 6f74 6f2f  generator/proto/
+00000200: 5f75 7469 6c73 2e70 79da 1168 6173 5f67  _utils.py..has_g
+00000210: 7270 6369 6f5f 7072 6f74 6f63 0700 0000  rpcio_protoc....
+00000220: 730e 0000 0000 0402 010c 010e 0104 0114  s...............
+00000230: 0108 0272 0d00 0000 6300 0000 0000 0000  ...r....c.......
+00000240: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
+00000250: 0073 8a00 0000 7400 7401 6401 6402 8303  .s....t.t.d.d...
+00000260: 7250 7402 6a03 a004 7402 6a03 a005 7402  rPt.j...t.j...t.
+00000270: 6a03 a006 7401 6a07 a101 a101 6403 a102  j...t.j.....d...
+00000280: 7402 6a03 a004 7402 6a03 a005 7402 6a03  t.j...t.j...t.j.
+00000290: a006 7401 6a07 a101 a101 6404 6405 a103  ..t.j.....d.d...
+000002a0: 6702 7d00 6e36 7402 6a03 a005 7402 6a03  g.}.n6t.j...t.j.
+000002b0: a006 7408 a101 a101 6701 7d00 7409 8300  ..t.....g.}.t...
+000002c0: 7286 6406 6407 6c0a 7d01 7c00 a00b 7c01  r.d.d.l.}.|...|.
+000002d0: a00c 6404 6405 a102 a101 0100 7c00 5300  ..d.d.......|.S.
+000002e0: 2908 7a56 4669 6e64 2069 6e63 6c75 6465  ).zVFind include
+000002f0: 2070 6174 6820 666f 7220 7374 616e 6461   path for standa
+00000300: 7264 2067 6f6f 676c 652f 7072 6f74 6f62  rd google/protob
+00000310: 7566 2069 6e63 6c75 6465 7320 616e 6420  uf includes and 
+00000320: 666f 720a 2020 2020 6e61 6e6f 7062 2e70  for.    nanopb.p
+00000330: 726f 746f 2e0a 2020 2020 da06 6672 6f7a  roto..    ..froz
+00000340: 656e 46da 0570 726f 746f 720a 0000 00da  enF..protor.....
+00000350: 065f 7072 6f74 6f72 0100 0000 4e29 0dda  ._protor....N)..
+00000360: 0767 6574 6174 7472 7204 0000 00da 026f  .getattrr......o
+00000370: 73da 0470 6174 68da 046a 6f69 6eda 0764  s..path..join..d
+00000380: 6972 6e61 6d65 da07 6162 7370 6174 68da  irname..abspath.
+00000390: 0a65 7865 6375 7461 626c 65da 085f 5f66  .executable..__f
+000003a0: 696c 655f 5f72 0d00 0000 da0d 706b 675f  ile__r......pkg_
+000003b0: 7265 736f 7572 6365 73da 0661 7070 656e  resources..appen
+000003c0: 64da 1172 6573 6f75 7263 655f 6669 6c65  d..resource_file
+000003d0: 6e61 6d65 2902 da05 7061 7468 7372 1900  name)...pathsr..
+000003e0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+000003f0: 00da 1e67 6574 5f70 726f 746f 5f62 7569  ...get_proto_bui
+00000400: 6c74 696e 5f69 6e63 6c75 6465 5f70 6174  ltin_include_pat
+00000410: 6814 0000 0073 1400 0000 0005 0c03 1e01  h....s..........
+00000420: 20fe 0608 12ff 0404 0601 0801 1202 721d   .............r.
+00000430: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000440: 0300 0000 0500 0000 4300 0000 735c 0000  ........C...s\..
+00000450: 0064 0164 0284 007c 0044 0083 0173 187c  .d.d...|.D...s.|
+00000460: 00a0 0064 03a1 0101 0074 0183 0044 005d  ...d.....t...D.]
+00000470: 127d 017c 00a0 0064 047c 0117 00a1 0101  .}.|...d.|......
+00000480: 0071 1e74 0283 0072 4e64 0564 066c 036d  .q.t...rNd.d.l.m
+00000490: 047d 0201 007c 02a0 057c 00a1 0153 0074  .}...|...|...S.t
+000004a0: 06a0 077c 00a1 0153 0064 0653 0029 077a  ...|...S.d.S.).z
+000004b0: d50a 2020 2020 496e 766f 6b65 2070 726f  ..    Invoke pro
+000004c0: 746f 632e 0a0a 2020 2020 5468 6973 2072  toc...    This r
+000004d0: 6f75 7469 6e65 2077 696c 6c20 7573 6520  outine will use 
+000004e0: 6772 7063 696f 2d70 726f 7669 6465 6420  grpcio-provided 
+000004f0: 7072 6f74 6f63 2069 6620 6974 2065 7869  protoc if it exi
+00000500: 7374 732c 0a20 2020 2075 7369 6e67 2073  sts,.    using s
+00000510: 7973 7465 6d2d 696e 7374 616c 6c65 6420  ystem-installed 
+00000520: 7072 6f74 6f63 2061 7320 6120 6661 6c6c  protoc as a fall
+00000530: 6261 636b 2e0a 0a20 2020 2041 7267 733a  back...    Args:
+00000540: 0a20 2020 2020 2020 2061 7267 763a 2070  .        argv: p
+00000550: 726f 746f 6320 434c 4920 696e 766f 6361  rotoc CLI invoca
+00000560: 7469 6f6e 2c20 6669 7273 7420 6974 656d  tion, first item
+00000570: 206d 7573 7420 6265 2027 7072 6f74 6f63   must be 'protoc
+00000580: 270a 2020 2020 6301 0000 0000 0000 0000  '.    c.........
+00000590: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+000005a0: 1a00 0000 6700 7c00 5d12 7d01 7c01 a000  ....g.|.].}.|...
+000005b0: 6400 a101 7204 7c01 9102 7104 5300 2901  d...r.|...q.S.).
+000005c0: fa02 2d49 2901 da0a 7374 6172 7473 7769  ..-I)...startswi
+000005d0: 7468 2902 da02 2e30 da01 7872 0b00 0000  th)....0..xr....
+000005e0: 720b 0000 0072 0c00 0000 da0a 3c6c 6973  r....r......<lis
+000005f0: 7463 6f6d 703e 3900 0000 7306 0000 0006  tcomp>9...s.....
+00000600: 0002 000a 007a 2169 6e76 6f6b 655f 7072  .....z!invoke_pr
+00000610: 6f74 6f63 2e3c 6c6f 6361 6c73 3e2e 3c6c  otoc.<locals>.<l
+00000620: 6973 7463 6f6d 703e 7a03 2d49 2e72 1e00  istcomp>z.-I.r..
+00000630: 0000 7201 0000 004e 2908 721a 0000 0072  ..r....N).r....r
+00000640: 1d00 0000 720d 0000 0072 0200 0000 da06  ....r....r......
+00000650: 7072 6f74 6f63 da04 6d61 696e da0a 7375  protoc..main..su
+00000660: 6270 726f 6365 7373 da04 6361 6c6c 2903  bprocess..call).
+00000670: da04 6172 6776 5a07 696e 6370 6174 6872  ..argvZ.incpathr
+00000680: 2300 0000 720b 0000 0072 0b00 0000 720c  #...r....r....r.
+00000690: 0000 00da 0d69 6e76 6f6b 655f 7072 6f74  .....invoke_prot
+000006a0: 6f63 2c00 0000 7310 0000 0000 0d0e 010a  oc,...s.........
+000006b0: 030a 0110 0206 010c 010a 0272 2800 0000  ...........r(...
+000006c0: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+000006d0: 000a 0000 0043 0000 0073 7201 0000 7a48  .....C...sr...zH
+000006e0: 7400 6401 6402 8d01 722e 6403 6400 6c01  t.d.d...r.d.d.l.
+000006f0: 7d00 7402 6a03 a004 6404 7c00 6a05 6a06  }.t.j...d.|.j.j.
+00000700: 1700 6405 1700 a101 0100 6e0c 7402 6a03  ..d.......n.t.j.
+00000710: a004 6406 a101 0100 7407 6407 6408 6702  ..d.....t.d.d.g.
+00000720: 8301 0100 5700 6e3a 0400 7408 6b0a 7282  ....W.n:..t.k.r.
+00000730: 0100 7d01 0100 7a1c 7402 6a03 a004 6409  ..}...z.t.j...d.
+00000740: 7409 7c01 8301 1700 6405 1700 a101 0100  t.|.....d.......
+00000750: 5700 3500 6400 7d01 7e01 5800 5900 6e02  W.5.d.}.~.X.Y.n.
+00000760: 5800 7a1e 7402 6a03 a004 640a 7409 740a  X.z.t.j...d.t.t.
+00000770: 8300 8301 1700 6405 1700 a101 0100 5700  ......d.......W.
+00000780: 6e3a 0400 7408 6b0a 72dc 0100 7d01 0100  n:..t.k.r...}...
+00000790: 7a1c 7402 6a03 a004 640b 7409 7c01 8301  z.t.j...d.t.|...
+000007a0: 1700 6405 1700 a101 0100 5700 3500 6400  ..d.......W.5.d.
+000007b0: 7d01 7e01 5800 5900 6e02 5800 7a52 6403  }.~.X.Y.n.X.zRd.
+000007c0: 6400 6c0b 7d02 7402 6a03 a004 640c 7402  d.l.}.t.j...d.t.
+000007d0: 6a0c 1700 6405 1700 a101 0100 7402 6a03  j...d.......t.j.
+000007e0: a004 640d 7c02 6a0d 6a06 1700 6405 1700  ..d.|.j.j...d...
+000007f0: a101 0100 7402 6a03 a004 640e 7c02 6a0d  ....t.j...d.|.j.
+00000800: 6a0e 1700 6405 1700 a101 0100 5700 6e3c  j...d.......W.n<
+00000810: 0400 7408 6b0a 9001 726c 0100 7d01 0100  ..t.k...rl..}...
+00000820: 7a1c 7402 6a03 a004 640f 7409 7c01 8301  z.t.j...d.t.|...
+00000830: 1700 6405 1700 a101 0100 5700 3500 6400  ..d.......W.5.d.
+00000840: 7d01 7e01 5800 5900 6e02 5800 6400 5300  }.~.X.Y.n.X.d.S.
+00000850: 2910 4e54 2901 7209 0000 0072 0100 0000  ).NT).r....r....
+00000860: 7a1f 5573 696e 6720 6772 7063 696f 2d74  z.Using grpcio-t
+00000870: 6f6f 6c73 2070 726f 746f 6320 6672 6f6d  ools protoc from
+00000880: 20da 010a 7a1e 5573 696e 6720 7072 6f74   ...z.Using prot
+00000890: 6f63 2066 726f 6d20 7379 7374 656d 2070  oc from system p
+000008a0: 6174 680a 7223 0000 007a 092d 2d76 6572  ath.r#...z.--ver
+000008b0: 7369 6f6e 7a24 4661 696c 6564 2074 6f20  sionz$Failed to 
+000008c0: 6465 7465 726d 696e 6520 7072 6f74 6f63  determine protoc
+000008d0: 2076 6572 7369 6f6e 3a20 7a1d 7072 6f74   version: z.prot
+000008e0: 6f63 2062 7569 6c74 696e 2069 6e63 6c75  oc builtin inclu
+000008f0: 6465 2070 6174 683a 207a 2946 6169 6c65  de path: z)Faile
+00000900: 6420 746f 2063 6f6e 7374 7275 6374 2070  d to construct p
+00000910: 726f 746f 6320 696e 636c 7564 6520 7061  rotoc include pa
+00000920: 7468 3a20 7a0f 5079 7468 6f6e 2076 6572  th: z.Python ver
+00000930: 7369 6f6e 207a 1b55 7369 6e67 2070 7974  sion z.Using pyt
+00000940: 686f 6e2d 7072 6f74 6f62 7566 2066 726f  hon-protobuf fro
+00000950: 6d20 7a19 5079 7468 6f6e 2d70 726f 746f  m z.Python-proto
+00000960: 6275 6620 7665 7273 696f 6e3a 207a 2d46  buf version: z-F
+00000970: 6169 6c65 6420 746f 2064 6574 6572 6d69  ailed to determi
+00000980: 6e65 2070 7974 686f 6e2d 7072 6f74 6f62  ne python-protob
+00000990: 7566 2076 6572 7369 6f6e 3a20 290f 720d  uf version: ).r.
+000009a0: 0000 0072 0200 0000 7204 0000 0072 0500  ...r....r....r..
+000009b0: 0000 7206 0000 0072 2300 0000 7218 0000  ..r....r#...r...
+000009c0: 0072 2800 0000 da09 4578 6365 7074 696f  .r(.....Exceptio
+000009d0: 6eda 0373 7472 721d 0000 005a 0f67 6f6f  n..strr....Z.goo
+000009e0: 676c 652e 7072 6f74 6f62 7566 da07 7665  gle.protobuf..ve
+000009f0: 7273 696f 6e5a 0870 726f 746f 6275 66da  rsionZ.protobuf.
+00000a00: 0b5f 5f76 6572 7369 6f6e 5f5f 2903 720a  .__version__).r.
+00000a10: 0000 00da 0165 5a06 676f 6f67 6c65 720b  .....eZ.googler.
+00000a20: 0000 0072 0b00 0000 720c 0000 00da 0e70  ...r....r......p
+00000a30: 7269 6e74 5f76 6572 7369 6f6e 7346 0000  rint_versionsF..
+00000a40: 0073 2600 0000 0001 0201 0a01 0801 1a02  .s&.............
+00000a50: 0c02 1001 1001 2a02 0201 1e01 1001 2a02  ......*.......*.
+00000a60: 0201 0801 1601 1801 1c01 1201 722f 0000  ............r/..
+00000a70: 00da 085f 5f6d 6169 6e5f 5f29 0146 290a  ...__main__).F).
+00000a80: 7204 0000 0072 2500 0000 da07 6f73 2e70  r....r%.....os.p
+00000a90: 6174 6872 1200 0000 7207 0000 0072 0d00  athr....r....r..
+00000aa0: 0000 721d 0000 0072 2800 0000 722f 0000  ..r....r(...r/..
+00000ab0: 00da 085f 5f6e 616d 655f 5f72 0b00 0000  ...__name__r....
+00000ac0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00000ad0: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00000ae0: 0000 0801 0801 0802 0802 0a0d 0818 081a  ................
+00000af0: 0819 0801                                ....
```

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/_utils.py` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import sys
 import subprocess
 import os.path
 
-def has_grpcio_protoc():
+import traceback
+
+def has_grpcio_protoc(verbose = False):
     # type: () -> bool
     """ checks if grpcio-tools protoc is installed"""
 
     try:
         import grpc_tools.protoc
     except ImportError:
+        if verbose:
+            sys.stderr.write("Failed to import grpc_tools: %s\n" % traceback.format_exc())
         return False
+
     return True
 
 def get_proto_builtin_include_path():
     """Find include path for standard google/protobuf includes and for
     nanopb.proto.
     """
 
@@ -60,15 +65,15 @@
         import grpc_tools.protoc as protoc
         return protoc.main(argv)
     else:
         return subprocess.call(argv)
 
 def print_versions():
     try:
-        if has_grpcio_protoc():
+        if has_grpcio_protoc(verbose = True):
             import grpc_tools.protoc
             sys.stderr.write("Using grpcio-tools protoc from " + grpc_tools.protoc.__file__ + "\n")
         else:
             sys.stderr.write("Using protoc from system path\n")
 
         invoke_protoc(['protoc', '--version'])
     except Exception as e:
```

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/google/protobuf/descriptor.proto` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb.proto` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb_pb2.py` & `nanopb-0.4.9.dev1472/nanopb/generator/proto/nanopb_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: nanopb.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +16,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cnanopb.proto\x1a google/protobuf/descriptor.proto\"\xb9\x07\n\rNanoPBOptions\x12\x10\n\x08max_size\x18\x01 \x01(\x05\x12\x12\n\nmax_length\x18\x0e \x01(\x05\x12\x11\n\tmax_count\x18\x02 \x01(\x05\x12&\n\x08int_size\x18\x07 \x01(\x0e\x32\x08.IntSize:\nIS_DEFAULT\x12$\n\x04type\x18\x03 \x01(\x0e\x32\n.FieldType:\nFT_DEFAULT\x12\x18\n\nlong_names\x18\x04 \x01(\x08:\x04true\x12\x1c\n\rpacked_struct\x18\x05 \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0bpacked_enum\x18\n \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0cskip_message\x18\x06 \x01(\x08:\x05\x66\x61lse\x12\x18\n\tno_unions\x18\x08 \x01(\x08:\x05\x66\x61lse\x12\r\n\x05msgid\x18\t \x01(\r\x12\x1e\n\x0f\x61nonymous_oneof\x18\x0b \x01(\x08:\x05\x66\x61lse\x12\x15\n\x06proto3\x18\x0c \x01(\x08:\x05\x66\x61lse\x12#\n\x14proto3_singular_msgs\x18\x15 \x01(\x08:\x05\x66\x61lse\x12\x1d\n\x0e\x65num_to_string\x18\r \x01(\x08:\x05\x66\x61lse\x12\x1b\n\x0c\x66ixed_length\x18\x0f \x01(\x08:\x05\x66\x61lse\x12\x1a\n\x0b\x66ixed_count\x18\x10 \x01(\x08:\x05\x66\x61lse\x12\x1e\n\x0fsubmsg_callback\x18\x16 \x01(\x08:\x05\x66\x61lse\x12/\n\x0cmangle_names\x18\x11 \x01(\x0e\x32\x11.TypenameMangling:\x06M_NONE\x12(\n\x11\x63\x61llback_datatype\x18\x12 \x01(\t:\rpb_callback_t\x12\x34\n\x11\x63\x61llback_function\x18\x13 \x01(\t:\x19pb_default_field_callback\x12\x30\n\x0e\x64\x65scriptorsize\x18\x14 \x01(\x0e\x32\x0f.DescriptorSize:\x07\x44S_AUTO\x12\x1a\n\x0b\x64\x65\x66\x61ult_has\x18\x17 \x01(\x08:\x05\x66\x61lse\x12\x0f\n\x07include\x18\x18 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x1a \x03(\t\x12\x0f\n\x07package\x18\x19 \x01(\t\x12\x41\n\rtype_override\x18\x1b \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.Type\x12\x19\n\x0bsort_by_tag\x18\x1c \x01(\x08:\x04true\x12.\n\rfallback_type\x18\x1d \x01(\x0e\x32\n.FieldType:\x0b\x46T_CALLBACK\x12\x13\n\x0binitializer\x18\x1e \x01(\t*i\n\tFieldType\x12\x0e\n\nFT_DEFAULT\x10\x00\x12\x0f\n\x0b\x46T_CALLBACK\x10\x01\x12\x0e\n\nFT_POINTER\x10\x04\x12\r\n\tFT_STATIC\x10\x02\x12\r\n\tFT_IGNORE\x10\x03\x12\r\n\tFT_INLINE\x10\x05*D\n\x07IntSize\x12\x0e\n\nIS_DEFAULT\x10\x00\x12\x08\n\x04IS_8\x10\x08\x12\t\n\x05IS_16\x10\x10\x12\t\n\x05IS_32\x10 \x12\t\n\x05IS_64\x10@*Z\n\x10TypenameMangling\x12\n\n\x06M_NONE\x10\x00\x12\x13\n\x0fM_STRIP_PACKAGE\x10\x01\x12\r\n\tM_FLATTEN\x10\x02\x12\x16\n\x12M_PACKAGE_INITIALS\x10\x03*E\n\x0e\x44\x65scriptorSize\x12\x0b\n\x07\x44S_AUTO\x10\x00\x12\x08\n\x04\x44S_1\x10\x01\x12\x08\n\x04\x44S_2\x10\x02\x12\x08\n\x04\x44S_4\x10\x04\x12\x08\n\x04\x44S_8\x10\x08:E\n\x0enanopb_fileopt\x12\x1c.google.protobuf.FileOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:G\n\rnanopb_msgopt\x12\x1f.google.protobuf.MessageOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:E\n\x0enanopb_enumopt\x12\x1c.google.protobuf.EnumOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptions:>\n\x06nanopb\x12\x1d.google.protobuf.FieldOptions\x18\xf2\x07 \x01(\x0b\x32\x0e.NanoPBOptionsB\x1a\n\x18\x66i.kapsi.koti.jpa.nanopb')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nanopb_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\030fi.kapsi.koti.jpa.nanopb'
   _globals['_FIELDTYPE']._serialized_start=1006
   _globals['_FIELDTYPE']._serialized_end=1111
   _globals['_INTSIZE']._serialized_start=1113
   _globals['_INTSIZE']._serialized_end=1181
   _globals['_TYPENAMEMANGLING']._serialized_start=1183
   _globals['_TYPENAMEMANGLING']._serialized_end=1273
```

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/protoc` & `nanopb-0.4.9.dev1472/nanopb/generator/protoc`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb-py2` & `nanopb-0.4.9.dev1472/nanopb/generator/protoc-gen-nanopb-py2`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1465/pyproject.toml` & `nanopb-0.4.9.dev1472/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanopb"
-version = "0.4.9-dev1465"
+version = "0.4.9-dev1472"
 description = "Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system."
 authors = ["Petteri Aimonen <jpa@npb.mail.kapsi.fi>"]
 license = "Zlib"
 repository = "https://github.com/nanopb/nanopb/"
 readme = "README.md"
 homepage = "https://jpa.kapsi.fi/nanopb/"
 documentation = "https://jpa.kapsi.fi/nanopb/docs/index.html"
```

### Comparing `nanopb-0.4.9.dev1465/PKG-INFO` & `nanopb-0.4.9.dev1472/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanopb
-Version: 0.4.9.dev1465
+Version: 0.4.9.dev1472
 Summary: Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system.
 Home-page: https://jpa.kapsi.fi/nanopb/
 License: Zlib
 Keywords: protobuf,protoc
 Author: Petteri Aimonen
 Author-email: jpa@npb.mail.kapsi.fi
 Requires-Python: >=2.7
```

