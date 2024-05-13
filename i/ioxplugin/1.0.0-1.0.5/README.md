# Comparing `tmp/ioxplugin-1.0.0.tar.gz` & `tmp/ioxplugin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.0.0.tar", last modified: Fri May  3 22:50:25 2024, max compression
+gzip compressed data, was "ioxplugin-1.0.5.tar", last modified: Mon May 13 07:05:12 2024, max compression
```

## Comparing `ioxplugin-1.0.0.tar` & `ioxplugin-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38141 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/nodedef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 22:50:25.000000 ioxplugin-1.0.0/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:50:25.379271 ioxplugin-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 22:50:21.000000 ioxplugin-1.0.0/tests/test_ioxplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.882504 ioxplugin-1.0.5/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_to_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 07:05:12.000000 ioxplugin-1.0.5/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:05:12.886504 ioxplugin-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 07:05:04.000000 ioxplugin-1.0.5/tests/test_ioxplugin.py
```

### Comparing `ioxplugin-1.0.0/PKG-INFO` & `ioxplugin-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.0
+Version: 1.0.5
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.0/ioxplugin/ast_util.py` & `ioxplugin-1.0.5/ioxplugin/ast_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import ast
 
 
 def astComment(comment):
-    return None
-    #return ast.Expr(value=ast.Constant(value=comment))
+    return ast.Expr(value=ast.Constant(value=comment))
 
 def astReturnBoolean(val:bool):
     # Create an AST node for 'return True'
     return ast.Return(
         value=ast.Constant(value=val)  # Using ast.Constant for Python 3.8 and later
     )
 
 def astCreateImports():
     import_node = ast.Import(
         names=[
                 ast.alias(name='udi_interface', asname=None),
                 ast.alias(name='os', asname=None),
                 ast.alias(name='sys', asname=None),
                 ast.alias(name='json', asname=None),
-                ast.alias(name='time', asname=None)
+                ast.alias(name='time', asname=None),
             ]
     )
     return import_node 
 
 def astCreateImport(import_name):
     return ast.Import(
         names=[
@@ -211,16 +210,16 @@
         value=ast.Subscript(
             value=ast.Name(id='jparam', ctx=ast.Load()),  # The dictionary 'jparam'
             slice=ast.Index(value=ast.Constant(value=param_uom)),  # Key 
             ctx=ast.Load()  # Context for the Subscript
         )
     )
 
-def astInitBody():
-    return [ast.Expr(value=ast.Call(
+def astInitBody(impl_class_name:str):
+    out = [ast.Expr(value=ast.Call(
         func=ast.Attribute(
             value=ast.Call(
                 func=ast.Name(id='super', ctx=ast.Load()),
                 args=[],
                 keywords=[]
             ),
             attr='__init__',
@@ -231,37 +230,72 @@
             ast.Name(id='controller', ctx=ast.Load()),
             ast.Name(id='address', ctx=ast.Load()),
             ast.Name(id='name', ctx=ast.Load())
         ],
         keywords=[]
     ))]
 
+    if impl_class_name:
+          # Create AST node for Impl(self) call
+        impl_call_node = ast.Call(
+            func=ast.Name(id=impl_class_name, ctx=ast.Load()),
+            args=[ast.Name(id='self', ctx=ast.Load())],
+        keywords=[]
+        )
+
+        inst_name = impl_class_name[0].lower() + impl_class_name[1:]
+        # Create AST node for self.impl = Impl(self) assignment
+        assign_node = ast.Assign(
+            targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr=inst_name, ctx=ast.Store())],
+            value=impl_call_node
+        )
+        out.append(assign_node)
+
+    #add protocol handler if any.
+    ph_node = ast.Assign(
+            targets=[
+            ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr='protocolHandler',
+                ctx=ast.Store()
+                )
+            ],
+            value=ast.Name(id='protocolHandler', ctx=ast.Load())
+        )
+    out.append(ph_node)
+    return out
+
 def astInitBodyController():
     return [
         ast.Assign(
             targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='Parameters', ctx=ast.Store())],
             value=ast.Call(
                 func=ast.Name(id='Custom', ctx=ast.Load()),
                 args=[
                     ast.Name(id='polyglot', ctx=ast.Load()),
                     ast.Constant(value='customparams')
                 ],
                 keywords=[]
             )
         ),
-        # Setting valid_configuration attribute
+        #Setting oauthService 
         ast.Assign(
-            targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='valid_configuration', ctx=ast.Store())],
-            value=ast.Constant(value=False)
+            targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='oauthService', ctx=ast.Store())],
+            value=ast.Constant(value=None)
         ),
+        # Setting valid_configuration attribute
+        #ast.Assign(
+        #    targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='valid_configuration', ctx=ast.Store())],
+        #    value=ast.Constant(value=False)
+        #),
         # Setting started attribute
-        ast.Assign(
-            targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='started', ctx=ast.Store())],
-            value=ast.Constant(value=False)
-        ),
+        #ast.Assign(
+        #    targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='started', ctx=ast.Store())],
+        #    value=ast.Constant(value=False)
+        #),
         # Multiple subscribe method calls
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
             args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='START', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='start', ctx=ast.Load())],
             keywords=[]
         )),
         ast.Expr(value=ast.Call(
@@ -277,33 +311,117 @@
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
             args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='STOP', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='stop', ctx=ast.Load())],
             keywords=[]
         )),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
-            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CONFIG', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='config', ctx=ast.Load())],
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CONFIG', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='configHandler', ctx=ast.Load())],
+            keywords=[]
+        )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CONFIGDONE', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='configDoneHandler', ctx=ast.Load())],
             keywords=[]
         )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='ADDNODEDONE', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='addNodeDoneHandler', ctx=ast.Load())],
+            keywords=[]
+        )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CUSTOMNS', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='customNSHandler', ctx=ast.Load())],
+            keywords=[]
+        )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='OAUTH', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='oauthHandler', ctx=ast.Load())],
+            keywords=[]
+        )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(value=ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='poly', ctx=ast.Load()), attr='subscribe', ctx=ast.Load()),
+            args=[ast.Attribute(value=ast.Name(id='polyglot', ctx=ast.Load()), attr='CUSTOMDATA', ctx=ast.Load()), ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='customDataHandler', ctx=ast.Load())],
+            keywords=[]
+        )),
+        ast.Expr(value=ast.Call(
+            func=ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr='initOAuth',
+                ctx=ast.Load()
+            ),
+            args=[],  # No arguments are passed to the function
+            keywords=[]  # No keyword arguments
+        ))
     ]   
 
+def astAddImplClassInit():
+    # Create AST node for self.node = node assignment
+    assign_node = ast.Assign(
+        targets=[ast.Attribute(value=ast.Name(id='self', ctx=ast.Load()), attr='plugin', ctx=ast.Store())],
+        value=ast.Name(id='plugin', ctx=ast.Load())
+    )
+
+    # Create AST node for method body
+    body_node = [assign_node]
+    function_def = ast.FunctionDef(
+        name='__init__',
+        args=ast.arguments(
+            posonlyargs=[],
+            args=[
+                ast.arg(arg='self'),
+                ast.arg(arg='plugin')
+            ],
+            defaults=[],
+            kwonlyargs=[],
+            kw_defaults=[],
+            vararg=None,
+            kwarg=None
+        ),
+        body=[
+            assign_node
+        ],
+        decorator_list=[],
+        returns=None
+    )
+
+    return function_def
+
+def astCallImplMethod(impl_instance_name, method_name, args_array):
+     # Create AST node for class attribute access
+    class_node = ast.Name(id=impl_instance_name, ctx=ast.Load())
+    method_node = ast.Attribute(value=class_node, attr=method_name, ctx=ast.Load())
+
+    # Create AST nodes for arguments
+    arg_nodes = [ast.Name(id=arg, ctx=ast.Load()) for arg in args_array] if args_array else []
+
+    # Create AST node for function call
+    call_node = ast.Call(
+        func=method_node,
+        args=arg_nodes,
+        keywords=[]
+    )
 
-def astAddClassInit(is_controller, defaults_array):
-    init_body = astInitBody()
+    # Create AST node for expression statement
+    return ast.Return(value=call_node)
+
+def astAddClassInit(is_controller, defaults_array, impl_class_name):
+    init_body = astInitBody(None if is_controller else impl_class_name)
     if (is_controller):
        init_body += astInitBodyController()
 
     # Function definition with default arguments
     function_def = ast.FunctionDef(
         name='__init__',
         args=ast.arguments(
             posonlyargs=[],
             args=[
                 ast.arg(arg='self'),
                 ast.arg(arg='polyglot'),
+                ast.arg(arg='protocolHandler', annotation=None, type_comment=None),
                 ast.arg(arg='controller', annotation=None, type_comment=None),
                 ast.arg(arg='address', annotation=None, type_comment=None),
                 ast.arg(arg='name', annotation=None, type_comment=None)
             ],
             defaults=[
                ast.Constant(value=d) for d in defaults_array
             ],
@@ -892,14 +1010,31 @@
                                     ),
                                     attr='addNode',
                                     ctx=ast.Load()
                                 ),
                                 args=[ast.Name(id='node', ctx=ast.Load())],
                                 keywords=[]
                             )),
+                            ast.Expr(
+                                value=ast.Call(
+                                    func=ast.Attribute(
+                                    value=ast.Name(id='node', ctx=ast.Load()),
+                                    attr='setProtocolHandler',
+                                    ctx=ast.Load()
+                                ),
+                                args=[
+                                    ast.Attribute(
+                                    value=ast.Name(id='self', ctx=ast.Load()),
+                                    attr='protocolHandler',
+                                    ctx=ast.Load()
+                                    )
+                                ],
+                                keywords=[]
+                                )
+                            ),
                             ast.Return(value=ast.Constant(value=True))
                         ]
                     )
                 ],
                 handlers=[
                     ast.ExceptHandler(
                         type=ast.Name(id='Exception', ctx=ast.Load()),
@@ -927,16 +1062,87 @@
             )
         ],
         decorator_list=[]
     )
 
     return function_def
 
-def astCreateMainFunc(controller):
+def astQueryAllMethod(commands):
+    if commands == None or len(commands) <= 0:
+        return None
+
+    function_def = ast.FunctionDef(
+        name='queryAll',
+        args=ast.arguments(args=[], vararg=None, kwonlyargs=[], kw_defaults=[], kwarg=None, defaults=[]),
+        body=[],
+        decorator_list=[],
+        returns=None
+    )
+
+    # Add a method call for each query to the function body
+    for command in commands:
+        method_call = ast.Expr(
+        value=ast.Call(
+            func=ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr=command,
+                ctx=ast.Load()
+            ),
+            args=[],
+            keywords=[]
+            )
+        )
+        function_def.body.append(method_call)
+    return function_def
+
+
+def astCreateMainFunc(controller, protocolHandler):
     try_body = [
+        # plugin = Plugin(PLUGIN_FILE_NAME)
+        ast.Assign(
+            targets=[ast.Name(id='plugin', ctx=ast.Store())],
+            value=ast.Call(
+                func=ast.Name(id='Plugin', ctx=ast.Load()),
+                args=[ast.Name(id='PLUGIN_FILE_NAME', ctx=ast.Load())],
+                keywords=[]
+            )
+        ),
+        # plugin.toIoX()
+        ast.Expr(
+            value=ast.Call(
+                func=ast.Attribute(
+                    value=ast.Name(id='plugin', ctx=ast.Load()),
+                    attr='toIoX',
+                    ctx=ast.Load()
+                ),
+                args=[],
+                keywords=[]
+            )
+        ),
+        # plugin.generateCode(path='./')
+        ast.Expr(
+            value=ast.Call(
+                func=ast.Attribute(
+                    value=ast.Name(id='plugin', ctx=ast.Load()),
+                    attr='generateCode',
+                    ctx=ast.Load()
+                ),
+                args=[],
+                keywords=[ast.keyword(arg='path', value=ast.Constant(value='./'))]
+            )
+        ),
+        # protocolHandler = ModbusProtocolHandler(plugin)
+        ast.Assign(
+            targets=[ast.Name(id='protocolHandler', ctx=ast.Store())],
+            value=ast.Call(
+                func=ast.Name(id=protocolHandler, ctx=ast.Load()),
+                args=[ast.Name(id='plugin', ctx=ast.Load())],
+                keywords=[]
+            )
+        ),
         ast.Assign(
             targets=[ast.Name(id='polyglot', ctx=ast.Store())],
             value=ast.Call(
                 func=ast.Attribute(value=ast.Name(id='udi_interface', ctx=ast.Load()), attr='Interface', ctx=ast.Load()),
                 args=[ast.List(elts=[], ctx=ast.Load())],
                 keywords=[]
             )
@@ -946,15 +1152,15 @@
             args=[ast.Attribute(value=ast.Name(id='version', ctx=ast.Load()), attr='ud_plugin_version', ctx=ast.Load())],
             keywords=[]
         )),
         ast.Assign(
             targets=[ast.Name(id='controller', ctx=ast.Store())],
             value=ast.Call(
                 func=ast.Name(id=controller, ctx=ast.Load()),
-                args=[ast.Name(id='polyglot', ctx=ast.Load())],
+                args=[ast.Name(id='polyglot', ctx=ast.Load()), ast.Name(id='protocolHandler', ctx=ast.Load())],
                 keywords=[]
             )
         ),
         ast.Expr(value=ast.Call(
             func=ast.Attribute(value=ast.Name(id='controller', ctx=ast.Load()), attr='start', ctx=ast.Load()),
             args=[],
             keywords=[]
@@ -1006,7 +1212,308 @@
             )
         ],
         orelse=[]
     )
 
     return main_if
 
+def astDiscoverControllerCommand():
+    return_statement = ast.Return(
+        value = ast.Call(
+        func=ast.Attribute(
+            value=ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr='protocolHandler',
+                ctx=ast.Load()
+            ),
+            attr='discover',
+            ctx=ast.Load()
+        ),
+        args=[],
+        keywords=[]
+    )
+    )
+    body=[
+       return_statement 
+    ]
+    return body
+
+def astQueryAllControllerCommand():
+    body=[
+        # nodes = self.poly.getNodes()
+        ast.Assign(
+            targets=[ast.Name(id='nodes', ctx=ast.Store())],
+            value=ast.Call(
+                func=ast.Attribute(
+                    value=ast.Attribute(
+                        value=ast.Name(id='self', ctx=ast.Load()),
+                        attr='poly',
+                        ctx=ast.Load()
+                    ),
+                    attr='getNodes',
+                    ctx=ast.Load()
+                ),
+                args=[],
+                keywords=[]
+            )
+        ),
+        # if nodes == None or len(nodes) == 0:
+        ast.If(
+            test=ast.BoolOp(
+                op=ast.Or(),
+                values=[
+                    ast.Compare(
+                        left=ast.Name(id='nodes', ctx=ast.Load()),
+                        ops=[ast.Is()],
+                        comparators=[ast.Constant(value=None)]
+                    ),
+                    ast.Compare(
+                        left=ast.Call(
+                            func=ast.Name(id='len', ctx=ast.Load()),
+                            args=[ast.Name(id='nodes', ctx=ast.Load())],
+                            keywords=[]
+                        ),
+                        ops=[ast.Eq()],
+                        comparators=[ast.Constant(value=0)]
+                    )
+                ]
+            ),
+            body=[
+                # return True
+                ast.Return(value=ast.Constant(value=True))
+            ],
+            orelse=[]
+        ),
+        # for n in nodes:
+        ast.For(
+            target=ast.Name(id='n', ctx=ast.Store()),
+            iter=ast.Name(id='nodes', ctx=ast.Load()),
+            body=[
+                # node = nodes[n]
+                ast.Assign(
+                    targets=[ast.Name(id='node', ctx=ast.Store())],
+                    value=ast.Subscript(
+                        value=ast.Name(id='nodes', ctx=ast.Load()),
+                        slice=ast.Name(id='n', ctx=ast.Load()),
+                        ctx=ast.Load()
+                    )
+                ),
+                # if node == None:
+                ast.If(
+                    test=ast.Compare(
+                        left=ast.Name(id='node', ctx=ast.Load()),
+                        ops=[ast.Is()],
+                        comparators=[ast.Constant(value=None)]
+                    ),
+                    body=[
+                        # continue
+                        ast.Continue()
+                    ],
+                    orelse=[
+                        # node.queryAll()
+                        ast.Expr(
+                            value=ast.Call(
+                                func=ast.Attribute(
+                                    value=ast.Name(id='node', ctx=ast.Load()),
+                                    attr='queryAll',
+                                    ctx=ast.Load()
+                                ),
+                                args=[],
+                                keywords=[]
+                            )
+                        )
+                    ]
+                )
+            ],
+            orelse=[]
+        )
+    ]
+    return body
+
+def astSetPluginFunc():
+    return ast.FunctionDef(
+    name='setProtocolHandler',
+    args=ast.arguments(
+        posonlyargs=[],
+        args=[
+            ast.arg(arg='self', annotation=None),
+            ast.arg(arg='protocolHandler', annotation=None)
+        ],
+        vararg=None,
+        kwonlyargs=[],
+        kw_defaults=[],
+        kwarg=None,
+        defaults=[]
+    ),
+    body=[
+        ast.Assign(
+            targets=[
+                ast.Attribute(
+                    value=ast.Name(id='self', ctx=ast.Load()),
+                    attr='protocolHandler',
+                    ctx=ast.Store()
+                )
+            ],
+            value=ast.Name(id='protocolHandler', ctx=ast.Load())
+        )
+    ],
+    decorator_list=[],
+    returns=None
+    )
+
+#protocol handler
+def astPHQueryPropertyFunc(update_method, property):
+    
+    body=[
+    # Outer if statement
+        ast.If(
+              test=ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr='protocolHandler',
+                ctx=ast.Load()
+        ),
+        body=[
+            # Assignment statement
+            ast.Assign(
+                targets=[ast.Name(id='val', ctx=ast.Store())],
+                value=ast.Call(
+                    func=ast.Attribute(
+                        value=ast.Attribute(
+                            value=ast.Name(id='self', ctx=ast.Load()),
+                            attr='protocolHandler',
+                            ctx=ast.Load()
+                        ),
+                        attr='queryProperty',
+                        ctx=ast.Load()
+                    ),
+                    args=[
+                        ast.Name(id='self', ctx=ast.Load()),
+                        ast.Constant(value=property)
+                    ],
+                    keywords=[]
+                )
+            ),
+            # Inner if statement
+            ast.If(
+                test=ast.Name(id='val', ctx=ast.Load()),
+                body=[
+                    # Method call within the inner if statement
+                    ast.Expr(
+                        value=ast.Call(
+                            func=ast.Attribute(
+                                value=ast.Name(id='self', ctx=ast.Load()),
+                                attr=update_method,
+                                ctx=ast.Load()
+                            ),
+                            args=[
+                                ast.Name(id='val', ctx=ast.Load()),
+                                ast.Constant(value=True)
+                            ],
+                            keywords=[]
+                        )
+                    ),
+                    # Return statement within the inner if statement
+                    ast.Return(value=ast.Constant(value=True))
+                ],
+                orelse=[]
+            )
+        ],
+        orelse=[],
+    ),
+    ast.Return(value=ast.Constant(value=False))
+    ]
+    return body
+
+#protocol handler
+def astPHSetPropertyFunc(update_method, property):
+    
+    body=[
+    # Outer if statement
+        ast.If(
+              test=ast.Attribute(
+                value=ast.Name(id='self', ctx=ast.Load()),
+                attr='protocolHandler',
+                ctx=ast.Load()
+        ),
+        body=[
+            # Inner if statement
+            ast.If(
+                test=ast.Call(
+                    func=ast.Attribute(
+                            value=ast.Attribute(
+                                value=ast.Name(id='self', ctx=ast.Load()),
+                                attr='protocolHandler',
+                                ctx=ast.Load()
+                            ),
+                            attr='setProperty',
+                            ctx=ast.Load()
+                    ),
+                    args=[
+                        ast.Name(id='self', ctx=ast.Load()),
+                        ast.Constant(value=property),
+                        ast.Name(id=property, ctx=ast.Load())
+                    ],
+                    keywords=[]
+                ),
+                body=[
+                    # Method call within the inner if statement
+                    ast.Expr(
+                        value=ast.Call(
+                            func=ast.Attribute(
+                                value=ast.Name(id='self', ctx=ast.Load()),
+                                attr=update_method,
+                                ctx=ast.Load()
+                            ),
+                            args=[
+                                ast.Name(id=property, ctx=ast.Load()),
+                                ast.Constant(value=True)
+                            ],
+                            keywords=[]
+                        )
+                    ),
+                    # Return statement within the inner if statement
+                    ast.Return(value=ast.Constant(value=True))
+                ],
+                orelse=[]
+            )
+        ],
+        orelse=[],
+    ),
+    ast.Return(value=ast.Constant(value=False))
+    ]
+    return body
+
+def astPHProcessCommandFunc(command_name, args):
+
+    arg_nodes = [ast.Constant(value=command_name)] 
+    #for arg in args_array:
+    #    arg_nodes.append(ast.Name(id=arg, ctx=ast.Load))
+    # Create AST node for function call
+    return_statement = ast.Return(
+            value=ast.Call(
+            func=ast.Name(id='self.protocolHandler.processCommand', ctx=ast.Load()),
+            args= arg_nodes,
+            keywords=[
+                ast.keyword(
+                    arg=key,
+                    value=ast.Name(id=val, ctx=ast.Load())
+                ) for key, val in args.items()
+            ]
+        )
+    )
+
+    body=[
+    # Outer if statement
+        ast.If(
+              test=ast.Attribute(
+              value=ast.Name(id='self', ctx=ast.Load()),
+              attr='protocolHandler',
+              ctx=ast.Load()
+        ),
+        body=[
+            return_statement
+        ],
+        orelse=[],
+    ),
+    ast.Return(value=ast.Constant(value=False))
+    ]
+    return body
```

### Comparing `ioxplugin-1.0.0/ioxplugin/commands.py` & `ioxplugin-1.0.5/ioxplugin/commands.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/editor.py` & `ioxplugin-1.0.5/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/iox_node_gen.py` & `ioxplugin-1.0.5/ioxplugin/iox_node_gen.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 from .nodedef import NodeDefDetails, NodeProperties
 from .commands import CommandDetails, CommandParam
 from .log import LOGGER
 from .validator import getValidName
 from ioxplugin import ast_util 
 from .uom import UOMs
 from .editor import Editors
+from .iox_controller_template import CONTROLLER_TEMPLATE_BODY, CONTROLLER_TEMPLATE_HEADER
 
 class IoXNodeGen():
     def __init__(self, nodedef:NodeDefDetails, path:str):
         if nodedef == None or path == None:
             LOGGER.critical("need node def and the path to save the python file")
             raise Exception ("need node def and the path to save the python file")
 
         self.nodedef = nodedef
         self.path = path
-
-
  
-    def create_command_body(self, command:CommandDetails):
+    def create_command_body(self, command:CommandDetails, command_name):
         if command == None:
             return None
         
         if not command.hasParams():
-            return ast_util.astReturnBoolean(True)
+            if command_name == "Query" and command.id == "query":
+                return ast_util.astQueryAllControllerCommand()
+            if command_name == "Discover" and command.id == "discover":
+                return ast_util.astDiscoverControllerCommand()
         
         out = []
         error = []
+        impl_args ={} 
 
         added_jparams=False
+        is_property=command.init_prop != None
 
         params = command.getParams()
         for p in params:
             param = params[p] 
             editor = Editors.getEditors().editors[param.editor.getEditorId()]
             #if UOMs.isIndex(editor.uom):
             #    out.append(ast_util.astIndexAssignment(param.name.replace(' ','_') if param.name else param.id, param.id, 'command'))
@@ -40,40 +44,49 @@
             if not added_jparams:
                 stmts = ast_util.astCommandQueryParams('command')
                 for stmt in stmts:
                     out.append(stmt)
                 added_jparams=True
             
             out.append(ast_util.astCommandParamAssignment(f'{param.id}.uom{editor.uom}', param.id))
+            impl_args[param.name if param.name else param.id]=param.id
+            if is_property:
+                body = ast_util.astPHSetPropertyFunc(command_name.replace('set','update'), param.id)
+                for stmt in body:
+                    out.append(stmt)
+                break
 
-        out.append(ast_util.astReturnBoolean(True))
+        #out.append(ast_util.astReturnBoolean(True))
+        if not is_property:
+            body = ast_util.astPHProcessCommandFunc(command_name, impl_args)
+            if body:
+                for stmt in body:
+                    out.append(stmt)
 
         error.append(ast_util.astLogger("error", "failed parsing parameters ... "))
         error.append(ast_util.astReturnBoolean(False))
 
         return ast_util.astTryExcept(out, error)
 
     def create(self, children):
         file_path=f'{self.path}/{self.nodedef.getPythonFileName()}'
-        imports = ast_util.astCreateImports()
-        python_code = astor.to_source(imports)
         with open(file_path, 'w') as file:
-            file.write(python_code)
-
-        global_defs = ast_util.astCreateGlobals()
-        for global_def in global_defs:
-            python_code = astor.to_source(global_def)
-            with open(file_path, 'a') as file:
-                file.write(python_code) 
-
-        if self.nodedef.isController:
-            for child in children:
-                import_stmt = ast_util.astCreateImportFrom(child['node_class'], child['node_class'])
-                python_code = astor.to_source(import_stmt)
-                with open(file_path, 'a') as file:
+            if not self.nodedef.isController:
+                imports = ast_util.astCreateImports()
+                python_code = astor.to_source(imports)
+                file.write(python_code)
+                global_defs = ast_util.astCreateGlobals()
+                for global_def in global_defs:
+                    python_code = astor.to_source(global_def)
+                    file.write(python_code) 
+            else:
+                file.write(CONTROLLER_TEMPLATE_HEADER)    
+                for child in children:
+                    import_stmt = ast_util.astCreateImportFrom(child['node_class'], child['node_class'])
+                    python_code = astor.to_source(import_stmt)
                     file.write(python_code) 
 
         # Create the class for the node 
         class_def = ast.ClassDef(
             name=f'{self.nodedef.getPythonClassName()}',
             bases=[ast.Attribute(value=ast.Name(id='udi_interface', ctx=ast.Load()), attr='Node', ctx=ast.Load())],
             keywords=[],
@@ -122,26 +135,35 @@
                         keys=[ast.Str(s='node_class'), ast.Str(s='id'), ast.Str(s='name'), ast.Str(s='parent')],
                         values=[ast.Str(s=child['node_class']), ast.Str(s=child['id']), ast.Str(s=child['name']), ast.Str(s=child['parent'])]
                     ) for child in children
                 ], ctx=ast.Load())
             )
             class_def.body.append(children_list)
 
+
         defaults=[self.nodedef.parent if self.nodedef.parent else self.nodedef.id,  self.nodedef.id,  self.nodedef.name]
-        class_def.body.append(ast_util.astAddClassInit(self.nodedef.isController, defaults))
+        class_def.body.append(ast_util.astAddClassInit(self.nodedef.isController, defaults, None))
         if self.nodedef.isController:
-            class_def.body.append(ast_util.astParamHandlerFunc())
-            class_def.body.append(ast_util.astConfigFunc())
-            class_def.body.append(ast_util.astStartFunc())
-            class_def.body.append(ast_util.astStopFunc())
-            class_def.body.append(ast_util.astPollFunc())
-            class_def.body.append(ast_util.astAddAllNodesFunc())
-            class_def.body.append(ast_util.astAddNodeFunc())
+            pass
+            #set protocol handler
+            #class_def.body.append(ast_util.astSetPluginFunc())
+            #class_def.body.append(ast_util.astParamHandlerFunc())
+            #class_def.body.append(ast_util.astConfigFunc())
+            #class_def.body.append(ast_util.astStartFunc())
+            #class_def.body.append(ast_util.astStopFunc())
+            #class_def.body.append(ast_util.astPollFunc())
+            #class_def.body.append(ast_util.astAddAllNodesFunc())
+            #class_def.body.append(ast_util.astAddNodeFunc())
+        else:
+            #set protocol handler
+            class_def.body.append(ast_util.astSetPluginFunc())
 
         #create update and get methods
+        query_commands=[]
+
 
         for driver in drivers:
             set_driver_call=ast.Call(
                         func=ast.Attribute(
                         value=ast.Name(id='self', ctx=ast.Load()),  # 'self' object
                         attr='setDriver',  # Method name 'setDriver'
                         ctx=ast.Load()
@@ -165,16 +187,18 @@
             ),
             body=[
                 return_stmt
             ],
             keywords=[],
             decorator_list=[]
             )
-            class_def.body.append(ast_util.astComment(f"Use this method to update {getValidName(driver['name'])} in IoX"))
-            class_def.body.append(method)
+
+            if not self.nodedef.isController:
+                class_def.body.append(ast_util.astComment(f"Use this method to update {getValidName(driver['name'])} in IoX"))
+                class_def.body.append(method)
 
             ## Now getDriver
             get_driver_call=ast.Call(
                         func=ast.Attribute(
                         value=ast.Name(id='self', ctx=ast.Load()),  # 'self' object
                         attr='getDriver',  # Method name 'getDriver'
                         ctx=ast.Load()
@@ -195,64 +219,86 @@
             ),
             body=[
                 return_stmt
             ],
             keywords=[],
             decorator_list=[]
             )
-            class_def.body.append(method)
+            if not self.nodedef.isController:
+                class_def.body.append(method)
+
+            ## Now queryriver
+            command_name=f"query{getValidName(driver['name'])}"
+            update_name=f"update{getValidName(driver['name'])}"
+            query_commands.append(command_name)
+            body = ast_util.astPHQueryPropertyFunc(update_name, driver['driver'])
+
+            if not isinstance(body, list):
+                body = [body]
+
+            #return_stmt = ast.Return(value=query_driver_call)  # Return the result of update 
+            method = ast.FunctionDef(
+            name=command_name,
+            args=ast.arguments(
+                args=[ast.arg(arg='self')],
+                defaults=[],
+                kwonlyargs=[], kw_defaults=[], vararg=None, kwarg=None
+            ),
+            body=body,
+            keywords=[],
+            decorator_list=[]
+            )
+            if not self.nodedef.isController:
+                class_def.body.append(method)
+
+        if len (query_commands) > 0 and not self.nodedef.isController:
+            class_def.body.append(ast_util.astQueryAllMethod(query_commands)) 
+
 
         #now make the commands
         for command in commands:
-            '''
-            set_driver_call=ast.Call(
-                        func=ast.Attribute(
-                        value=ast.Name(id='self', ctx=ast.Load()),  # 'self' object
-                        attr='setDriver',  # Method name 'setDriver'
-                        ctx=ast.Load()
-                    ),
-                    args=[
-                        ast.Name(id=f"\"{driver['driver']}\"", ctx=ast.Load()),  # First, driver id
-                        ast.Name(id='value', ctx=ast.Load()),        # Second, value
-                        ast.Name(id=f"{driver['uom']}", ctx=ast.Load()) ,    # Third uom
-                        ast.Name(id='force', ctx=ast.Load())          # Whether or not to force update/boolean
-                    ],
-                    keywords=[],
-                    decorator_list=[]
-                )
-            return_stmt = ast.Return( value=set_driver_call)  # Return the result of update 
-            '''
             cmd = self.nodedef.commands.acceptCommands[command['id']]
             pass_stmt = ast.Pass()
+            command_name=getValidName(command['name'],False)
+            body = self.create_command_body(cmd, command_name)
+            if not isinstance(body, list):
+                body = [body]
             method = ast.FunctionDef(
-                name=getValidName(command['name'],False),
+                name=command_name,
                 args=ast.arguments(
                     args=[ast.arg(arg='self'), ast.arg(arg='command')],
                     defaults=[],
                     kwonlyargs=[], kw_defaults=[], vararg=None, kwarg=None
                 ),
-                body=[
-            #        pass_stmt
-                     self.create_command_body(cmd)
-                ],
+                body=body,
+                #body=[
+                #     self.create_command_body(cmd, command_name)
+                #],
                 keywords=[],
                 decorator_list=[]
             )
-            class_def.body.append(method)
+            if not self.nodedef.isController:
+                class_def.body.append(method)
 
         # Print the AST dump to verify
         #print(ast.dump(class_def, indent=4))
-        class_def.body.append(ast_util.astComment('This is a list of commands that were defined in the nodedef'))
-        # Add the drivers list
-        commands_list = ast.Assign(
+        if not self.nodedef.isController:
+            class_def.body.append(ast_util.astComment('This is a list of commands that were defined in the nodedef'))
+            # Add the drivers list
+            commands_list = ast.Assign(
             targets=[ast.Name(id='commands', ctx=ast.Store())],
             value= ast.Dict(
                         keys=[ast.Str(s=f"{command['id']}") for command in commands],
                         values=[ast.Name(id=f"{getValidName(command['name'],False)}", ctx=ast.Load()) for command in commands]
                     ) 
-        )
-        class_def.body.append(commands_list)
+            )
+            class_def.body.append(commands_list)
 
+        with open(file_path, 'a') as file:
+            python_code = astor.to_source(class_def)
+            file.write(python_code)
+            if self.nodedef.isController:
+                file.write(CONTROLLER_TEMPLATE_BODY)
 
         return class_def
```

### Comparing `ioxplugin-1.0.0/ioxplugin/iox_profile.py` & `ioxplugin-1.0.5/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/log.py` & `ioxplugin-1.0.5/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/main_gen.py` & `ioxplugin-1.0.5/ioxplugin/main_gen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import astor
 from .nodedef import NodeDefs, NodeDefDetails, NodeProperties
 from .plugin_meta import PluginMetaData
 from .log import LOGGER
 from ioxplugin import ast_util
 from .iox_node_gen import IoXNodeGen
+import os
 
 
 class PluginMain:
     def __init__(self, path:str, plugin_info:PluginMetaData, node_defs:NodeDefs):
         self.plugin_info=plugin_info
         self.node_defs=node_defs
         self.path = path
@@ -17,23 +18,40 @@
     def create(self):
         exec_name = self.plugin_info.getExecutableName()
         if exec_name == None:
             LOGGER.critical("need the executable name ...") 
             return False
 
         file_path = f'{self.path}/{exec_name}'
-        imports = ast_util.astCreateImports()
-        python_code = astor.to_source(imports)
-        with open(file_path, 'w') as file:
-            file.write(python_code)
-
-        version_import = ast_util.astCreateImport("version")
-        python_code = astor.to_source(version_import)
-        with open(file_path, 'a') as file:
-            file.write(python_code)
+        create_main = not os.path.exists(file_path)
+        if create_main:
+            #do not recreate the main
+            with open(file_path, 'w') as file:
+                imports = ast_util.astCreateImports()
+                python_code = astor.to_source(imports)
+                file.write(python_code)
+                
+                version_import = ast_util.astCreateImport("version")
+                python_code = astor.to_source(version_import)
+                file.write(python_code)
+
+                #ioxplugin_import = ast_util.astCreateImport("ioxplugin")
+                #ioxplugin_code = astor.to_source(ioxplugin_import)
+                #file.write(ioxplugin_code)
+
+                ioxplugin_from_import = ast_util.astCreateImportFrom("ioxplugin","Plugin")
+                ioxplugin_code = astor.to_source(ioxplugin_from_import)
+                file.write(ioxplugin_code)
+
+                imp_from_import = ast_util.astCreateImportFrom(self.plugin_info.getPythonPHClassName(), 
+                        self.plugin_info.getPythonPHClassName())
+                ioxplugin_code = astor.to_source(imp_from_import)
+                file.write(ioxplugin_code)
+                file.write(f"\nPLUGIN_FILE_NAME = \'{self.plugin_info.plugin_file}\'\n")
+
 
         self.controllerNode = None
         children = []
         #add import for each node
         nodedefs = self.node_defs.nodedefs
         for ndi in nodedefs:
             nd = nodedefs[ndi]
@@ -44,34 +62,44 @@
                     {
                         'node_class': nd.getPythonClassName(),
                         'id': nd.id,
                         'name': nd.name,
                         'parent': None
                     }
                 )
-            import_stmt = ast_util.astCreateImportFrom(nd.getPythonClassName(), nd.getPythonClassName())
-            python_code = astor.to_source(import_stmt)
-            with open(file_path, 'a') as file:
-                file.write(python_code)
 
-        global_defs = ast_util.astCreateGlobals(True)
-        for global_def in global_defs:
-            python_code = astor.to_source(global_def)
+        if create_main:
             with open(file_path, 'a') as file:
+                import_stmt = ast_util.astCreateImportFrom(nd.getPythonClassName(), nd.getPythonClassName())
+                python_code = astor.to_source(import_stmt)
                 file.write(python_code)
 
-        main_body = ast_util.astCreateMainFunc(self.controllerNode.getPythonClassName()) 
-        python_code = astor.to_source(main_body)
-        with open(file_path, 'a') as file:
-            file.write(python_code)
+                global_defs = ast_util.astCreateGlobals(True)
+                for global_def in global_defs:
+                    python_code = astor.to_source(global_def)
+                    file.write(python_code)
+
+                main_body = ast_util.astCreateMainFunc(self.controllerNode.getPythonClassName(), self.plugin_info.getPythonPHClassName()) 
+                python_code = astor.to_source(main_body)
+                file.write(python_code)
 
         for child in children:
             child['parent'] = self.controllerNode.id
 
         for ndi in nodedefs:
             ndef = nodedefs[ndi]
-            file_path=f'{self.path}/{ndef.getPythonFileName()}'
+            #file_path=f'{self.path}/{ndef.getPythonFileName()}'
             ngen = IoXNodeGen(ndef, self.path)
             nc = ngen.create(children)
-            python_code = astor.to_source(nc)
-            with open(file_path, 'a') as file:
-                    file.write(python_code)
+    
+    def generateVersion(self):
+        versionFile = os.path.join(self.path, "version.py")
+        with open(versionFile, 'w') as file:
+            file.write(self.plugin_info.getVersion())
+
+    def generateRequirements(self):
+        requirementsFile = os.path.join(self.path, "requirements.txt")
+        with open(requirementsFile, 'w') as file:
+            reqs = self.plugin_info.getRequirements()
+            for req in reqs:
+                file.write(req)
+                file.write('\n')
```

### Comparing `ioxplugin-1.0.0/ioxplugin/new_project.py` & `ioxplugin-1.0.5/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/node_properties.py` & `ioxplugin-1.0.5/ioxplugin/node_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class NodePropertyDetails:
     def __init__(self, node_property):
         self.id = None
         self.name = None
         self.is_settable = False
         self.editor = None
         self.hide = False
+        self.protocol_data = None
 
         if node_property == None:
             return
         try: 
             if 'id' in node_property:
                 val = node_property['id']
                 parsed_list = [item.strip() for item in val.split('|')]
@@ -30,14 +31,16 @@
                 self.name = node_property['name']
             if 'is_settable' in node_property:
                 self.is_settable = node_property['is_settable']
             if 'editor' in node_property:
                 self.editor = Editors.getEditors().addEditor(node_property['editor'])
             if 'hide' in node_property:
                 self.hide = node_property['hide']
+            if 'protocol' in node_property:
+                self.protocol_data = node_property['protocol']
         except Exception as ex:
             LOGGER.critical(str(ex))
             raise
 
     def isSet(self)->bool:
         return self.is_settable 
 
@@ -86,14 +89,22 @@
                 if nls_np:
                     nls += f"\n{nls_np}"
             sts += "\n</sts>"
             return sts, nls
         except Exception as ex:
             LOGGER.critical(str(ex))
 
+    def getProtocolData(self):
+        out = {}
+        for np in self.node_properties:
+            node_property:NodePropertyDetails = self.node_properties[np]
+            out[node_property.id] = node_property.protocol_data
+
+        return out
+
     def getPG3Drivers(self):
         drivers = []
         for np in self.node_properties:
             prop = self.node_properties[np]
             if prop == None:
                 continue
             editor = Editors.getEditors().editors[prop.editor.getEditorId()]
```

### Comparing `ioxplugin-1.0.0/ioxplugin/nodedef.py` & `ioxplugin-1.0.5/ioxplugin/nodedef.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 Copyright (C) 2024 Universal Devices
 """
 
 from .node_properties import NodeProperties
 from .commands import Commands
 from .log import LOGGER
 from .validator import validate_id
-from .protocol import Protocol
 
 
 class NodeDefDetails:
     def __init__(self, node):
         self.id = None
         self.name = None
         self.parent = None
         self.icon = None
         self.isController = False
         self.properties:NodeProperties
         self.commands:Commands
-        self.protocol:Protocol
 
         if node == None:
             LOGGER.critical("no node was given ... ")
             return
         try: 
             if 'id' in node:
                 self.id = node['id']
@@ -35,16 +33,14 @@
                 self.parent = node['parent']
             if 'icon' in node:
                 self.icon = node['icon']
             if 'properties' in node:
                 self.properties = NodeProperties(node['properties']) 
             if 'commands' in node:
                 self.commands=Commands(node['commands'])
-            if 'protocol' in node:
-                self.protocol=Protocol(node['protocol'])
 
         except Exception as ex:
             LOGGER.critical(str(ex))
             raise
 
     def getPG3Commands(self):
         commands = []
@@ -61,32 +57,14 @@
                     
     def getPythonClassName(self):
         return f'{self.name}Node'.replace(' ','').replace('_','')
 
     def getPythonFileName(self):
         return f'{self.getPythonClassName()}.py'
 
-    def isModbus(self):
-        try:
-            return self.protocol.isModbus()    
-        except Exception as ex:
-            return False
-
-    def isShelly(self):
-        try:
-            return self.protocol.isShelly()    
-        except Exception as ex:
-            return False
-
-    def isProprietary(self):
-        try:
-            return self.protocol.isProprietary()    
-        except Exception as ex:
-            return False
-
     def toIoX(self):
         nls = ""
         nodedef = f"<nodedef id=\"{self.id}\" nls=\"{self.id}\">"
         nls += f"\nND-{self.id}-NAME = {self.name}"
         if self.icon != None:
             nls += f"\nND-{self.id}-ICON = {self.icon}"
```

### Comparing `ioxplugin-1.0.0/ioxplugin/plugin.py` & `ioxplugin-1.0.5/ioxplugin/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 """
 Plugin schema processor and validator
 Copyright (C) 2024 Universal Devices
 """
 
 #import fastjsonschema
-import json
+import json,os
 from .nodedef import NodeDefs
 from .editor import Editors
 from .plugin_meta import PluginMetaData
 from .log import init_ext_logging, LOGGER
 from .iox_profile import ProfileWriter
 from .iox_node_gen import IoXNodeGen
 from .main_gen import PluginMain
+from .protocol import Protocol
+from .iox_node_impl_gen import IoXNodeImplGen
 import argparse
 
 
 PLUGIN_SCHEMA_FILE="schemas/plugin.schema.json"
 
 CMD_SCHEMA="schemas/commands.schema.json"
 EDITOR_SCHEMA="schemas/editor.schema.json"
@@ -28,40 +30,47 @@
 PROP_SCHEMA="schemas/properties.schema.json"
 UOM_SCHEMA="schemas/uom.schema.json"
 
 
 
 class Plugin:
 
-    def __init__(self, plugin_file, path:str, schema=PLUGIN_SCHEMA_FILE):
-        init_ext_logging(path)
+    def __init__(self, plugin_file, path:str=None, schema=PLUGIN_SCHEMA_FILE):
+        self.path = os.path.dirname(plugin_file) if path == None else path
+        init_ext_logging(self.path)
         self.meta = None
         self.editors=Editors()
-        self.nodedefs:NodeDefs 
+        self.nodedefs:NodeDefs = None
+        self.protocol:Protocol = None
+        
         self.isValid = False
         if plugin_file == None:
             LOGGER.critical("plugin file does not exist ... ")
             return
-        self.profileWriter=ProfileWriter(True, path)
+
+        self.profileWriter=ProfileWriter(True, self.path)
 
         try:
             self.isValid=self.validate_json(schema, plugin_file)
             if not self.isValid:
                 LOGGER.critical("not a valid plugin configuration file ... ")
                 return
             with open(plugin_file, 'r') as file:
                 plugin_json = json.load(file)
 
             if 'plugin' in plugin_json:
                 self.meta = PluginMetaData(plugin_json['plugin'])
+                self.meta.setPluginFile(plugin_file)
             if 'editors' in plugin_json:
                 self.editors.addEditors(plugin_json['editors'])
             if 'nodedefs' in plugin_json:
                 self.nodedefs = NodeDefs(plugin_json['nodedefs'])
                 self.nodedefs.addController(f"{self.meta.getName().replace(' ','_').capitalize()} Controller")
+            if 'protocol' in plugin_json:
+                self.protocol = Protocol(plugin_json['protocol'])
 
         except Exception as ex:
             raise
 
     def toIoX(self)->bool:
         if not self.validate():
             LOGGER.critical("invalid json file ... ")
@@ -132,14 +141,20 @@
             return False
 
     def validate(self):
         n = self.nodedefs.validate()
         e = self.editors.validate()
 
         return n and e
+    
+    def getPythonPHClassName(self):
+        return self.meta.getPythonPHClassName()
+
+    def getPythonPHFileName(self):
+        return self.meta.getPythonPHFileName()
 
     def generateCode(self, path:str):
         try:
             if path == None:
                 LOGGER.critical("need path to write python files to")
                 raise Exception("path to write python files to")
 
@@ -151,20 +166,27 @@
 
             if self.nodedefs.size() == 0:
                 LOGGER.critical("no nodedefs defined ...")
                 raise Exception("no nodedefs")
 
             main = PluginMain(path, self.meta, self.nodedefs)
             main.create()
+            main.generateRequirements()
+            main.generateVersion()
+
+            #now generate the proto handler/impl
+            node_impl_gen=IoXNodeImplGen(path, self.getPythonPHFileName(), self.getPythonPHClassName())
+            node_impl_gen.create()
+
+
 
         except Exception as ex:
             LOGGER.critical(str(ex))
             raise Exception(ex)
 
-
 def generate_code():
     project_path = "/usr/home/admin/workspace/plugin-dev/ext"
     json_file = f"{project_path}/dimmer.iox_plugin.json"
     try:
         parser = argparse.ArgumentParser(description="the path IoX Plugin json file")
     
         parser.add_argument('project_path', type=str, help='path to the project directory')
```

### Comparing `ioxplugin-1.0.0/ioxplugin/properties.py` & `ioxplugin-1.0.5/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/uom.py` & `ioxplugin-1.0.5/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin/validator.py` & `ioxplugin-1.0.5/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.0/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.0.5/ioxplugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.0
+Version: 1.0.5
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.0/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.0.5/ioxplugin.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 LICENSE
 README.md
 setup.py
 ioxplugin/__init__.py
 ioxplugin/ast_util.py
 ioxplugin/commands.py
 ioxplugin/editor.py
+ioxplugin/iox_controller_template.py
 ioxplugin/iox_node_gen.py
+ioxplugin/iox_node_impl_gen.py
 ioxplugin/iox_profile.py
+ioxplugin/iox_to_modbus.py
+ioxplugin/iox_transport.py
 ioxplugin/log.py
 ioxplugin/main_gen.py
 ioxplugin/new_project.py
 ioxplugin/node_properties.py
 ioxplugin/nodedef.py
+ioxplugin/oauth_service.py
 ioxplugin/plugin.py
 ioxplugin/plugin_meta.py
 ioxplugin/properties.py
 ioxplugin/protocol.py
 ioxplugin/uom.py
 ioxplugin/validator.py
 ioxplugin.egg-info/PKG-INFO
```

### Comparing `ioxplugin-1.0.0/setup.py` & `ioxplugin-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.0.0',
+    version='1.0.5',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

