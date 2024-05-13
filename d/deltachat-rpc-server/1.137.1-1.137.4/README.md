# Comparing `tmp/deltachat-rpc-server-1.137.1.tar.gz` & `tmp/deltachat-rpc-server-1.137.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-server-1.137.1.tar", last modified: Wed Apr  3 02:19:51 2024, max compression
+gzip compressed data, was "deltachat-rpc-server-1.137.4.tar", last modified: Wed Apr 24 12:29:05 2024, max compression
```

## Comparing `deltachat-rpc-server-1.137.1.tar` & `deltachat-rpc-server-1.137.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.1/PKG-INFO
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.1/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.1/setup.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.1/src/deltachat_rpc_server/__init__.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.4/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.4/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.4/setup.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.137.4/src/deltachat_rpc_server/__init__.py
```

### Comparing `deltachat-rpc-server-1.137.1/PKG-INFO` & `deltachat-rpc-server-1.137.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-server
-Version: 1.137.1
+Version: 1.137.4
 Summary: Delta Chat JSON-RPC server
 Description-Content-Type: text/markdown
 
 # Delta Chat RPC server
 
 This program provides a [JSON-RPC 2.0](https://www.jsonrpc.org/specification) interface to DeltaChat
 over standard I/O.
```

### Comparing `deltachat-rpc-server-1.137.1/setup.py` & `deltachat-rpc-server-1.137.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 "download",
                 "--no-input",
                 "--timeout",
                 "1000",
                 "--platform",
                 "musllinux_1_1_" + platform.machine(),
                 "--only-binary=:all:",
-                "deltachat-rpc-server==1.137.1",
+                "deltachat-rpc-server==1.137.4",
             ],
             cwd=tmpdir,
         )
 
         wheel_path = next(Path(tmpdir).glob("*.whl"))
         with ZipFile(wheel_path, "r") as wheel:
             exe_path = wheel.extract("deltachat_rpc_server/deltachat-rpc-server", "src")
```

