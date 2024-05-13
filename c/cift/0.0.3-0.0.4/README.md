# Comparing `tmp/cift-0.0.3.tar.gz` & `tmp/cift-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cift-0.0.3.tar", last modified: Sun May 12 18:25:25 2024, max compression
+gzip compressed data, was "cift-0.0.4.tar", last modified: Mon May 13 10:13:31 2024, max compression
```

## Comparing `cift-0.0.3.tar` & `cift-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.236869 cift-0.0.3/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-12 18:25:25.236869 cift-0.0.3/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.3/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      487 2024-05-12 18:24:38.000000 cift-0.0.3/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-12 18:25:25.236869 cift-0.0.3/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.231869 cift-0.0.3/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.233869 cift-0.0.3/src/cift/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.3/src/cift/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.3/src/cift/err.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     6744 2024-05-12 18:24:22.000000 cift-0.0.3/src/cift/parser.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      881 2024-05-12 18:22:45.000000 cift-0.0.3/src/cift/re.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      195 2024-05-10 18:04:44.000000 cift-0.0.3/src/cift/types.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.235869 cift-0.0.3/src/cift.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      331 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-12 18:25:25.000000 cift-0.0.3/src/cift.egg-info/top_level.txt
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-12 18:25:25.235869 cift-0.0.3/tests/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      696 2024-05-12 18:23:58.000000 cift-0.0.3/tests/test_comment.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2501 2024-05-10 18:06:15.000000 cift-0.0.3/tests/test_poly.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.3/tests/test_regex.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.3/tests/test_rout.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 10:13:31.304264 cift-0.0.4/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-13 10:13:31.304264 cift-0.0.4/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1418 2024-05-11 10:35:09.000000 cift-0.0.4/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      487 2024-05-13 10:13:02.000000 cift-0.0.4/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      373 2024-05-13 10:13:31.304264 cift-0.0.4/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 10:13:31.299264 cift-0.0.4/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 10:13:31.302264 cift-0.0.4/src/cift/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      155 2024-05-10 08:03:12.000000 cift-0.0.4/src/cift/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      496 2024-05-10 11:58:02.000000 cift-0.0.4/src/cift/err.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     7080 2024-05-13 10:11:38.000000 cift-0.0.4/src/cift/parser.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      881 2024-05-12 18:22:45.000000 cift-0.0.4/src/cift/re.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      195 2024-05-10 18:04:44.000000 cift-0.0.4/src/cift/types.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 10:13:31.303264 cift-0.0.4/src/cift.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     1672 2024-05-13 10:13:31.000000 cift-0.0.4/src/cift.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      331 2024-05-13 10:13:31.000000 cift-0.0.4/src/cift.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-13 10:13:31.000000 cift-0.0.4/src/cift.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        5 2024-05-13 10:13:31.000000 cift-0.0.4/src/cift.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-13 10:13:31.303264 cift-0.0.4/tests/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      696 2024-05-12 18:23:58.000000 cift-0.0.4/tests/test_comment.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4411 2024-05-13 10:12:39.000000 cift-0.0.4/tests/test_poly.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     2766 2024-05-09 15:50:10.000000 cift-0.0.4/tests/test_regex.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3527 2024-05-11 10:51:04.000000 cift-0.0.4/tests/test_rout.py
```

### Comparing `cift-0.0.3/PKG-INFO` & `cift-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cift
-Version: 0.0.3
+Version: 0.0.4
 Summary: Caltech Intermediate Form parser in pure Python
 Author-email: maybetree <no@email.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # CIFT
```

### Comparing `cift-0.0.3/README.md` & `cift-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cift-0.0.3/src/cift/parser.py` & `cift-0.0.4/src/cift/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,28 +158,40 @@
                 self._traceback(),
                 "Error: tried adding geometry before any layer was selected."
                 )))
 
     def _handle_box(self, match):
         self._assert_layer()
 
-        length, width, xpos, ypos = map(to_int, match.groups())
+        width, height, xpos, ypos = map(to_int, match.groups()[:4])
+        rot_x, rot_y = match.groups()[4:]
 
-        x1 = xpos - width / 2
-        y1 = ypos - length / 2
-        x2 = xpos + width / 2
-        y2 = ypos + length / 2
+        x1 = -width / 2
+        y1 = -height / 2
+        x2 = width / 2
+        y2 = height / 2
 
         points = (
             (x1, y1),
             (x2, y1),
             (x2, y2),
             (x1, y2),
             )
 
+        if rot_x is not None:
+            assert rot_y is not None
+            rot_x = to_int(rot_x)
+            rot_y = to_int(rot_y)
+            points = Rotate(rot_x, rot_y).transform_points(points)
+
+        points = (
+            (point[0] + xpos, point[1] + ypos)
+            for point in points
+            )
+
         points = self._frame.transform.transform_points(points)
 
         self.layers[self._frame.layer].append(points)
 
     def _handle_polygon(self, match):
         self._assert_layer()
```

### Comparing `cift-0.0.3/src/cift/re.py` & `cift-0.0.4/src/cift/re.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.3/src/cift.egg-info/PKG-INFO` & `cift-0.0.4/src/cift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cift
-Version: 0.0.3
+Version: 0.0.4
 Summary: Caltech Intermediate Form parser in pure Python
 Author-email: maybetree <no@email.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # CIFT
```

### Comparing `cift-0.0.3/tests/test_comment.py` & `cift-0.0.4/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.3/tests/test_regex.py` & `cift-0.0.4/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `cift-0.0.3/tests/test_rout.py` & `cift-0.0.4/tests/test_rout.py`

 * *Files identical despite different names*

