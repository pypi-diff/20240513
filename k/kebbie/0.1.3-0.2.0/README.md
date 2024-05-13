# Comparing `tmp/kebbie-0.1.3.tar.gz` & `tmp/kebbie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kebbie-0.1.3.tar", last modified: Fri Apr  5 11:59:36 2024, max compression
+gzip compressed data, was "kebbie-0.2.0.tar", last modified: Mon May 13 09:28:44 2024, max compression
```

## Comparing `kebbie-0.1.3.tar` & `kebbie-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.560562 kebbie-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 11:59:30.000000 kebbie-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-05 11:59:36.560562 kebbie-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-05 11:59:30.000000 kebbie-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.556562 kebbie-0.1.3/kebbie/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/correctors.py
--rw-r--r--   0 runner    (1001) docker     (127)    35066 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/gesture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/noise_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.556562 kebbie-0.1.3/kebbie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 11:59:30.000000 kebbie-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:59:36.560562 kebbie-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 11:59:30.000000 kebbie-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.934783 kebbie-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 09:28:42.000000 kebbie-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:28:44.934783 kebbie-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 09:28:42.000000 kebbie-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.930783 kebbie-0.2.0/kebbie/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46981 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/gesture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-13 09:28:42.000000 kebbie-0.2.0/kebbie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:28:44.934783 kebbie-0.2.0/kebbie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:28:44.000000 kebbie-0.2.0/kebbie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 09:28:42.000000 kebbie-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:28:44.934783 kebbie-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-13 09:28:42.000000 kebbie-0.2.0/setup.py
```

### Comparing `kebbie-0.1.3/LICENSE` & `kebbie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/PKG-INFO` & `kebbie-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.1.3
+Version: 0.2.0
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.1.3/README.md` & `kebbie-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/__init__.py` & `kebbie-0.2.0/kebbie/__init__.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/cmd.py` & `kebbie-0.2.0/kebbie/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
     parser.add_argument(
         "--keyboard",
         "-K",
         dest="keyboard",
         type=str,
         required=True,
-        choices=["gboard", "ios", "tappa"],
+        choices=["gboard", "ios", "kbkitpro", "kbkitoss", "tappa", "fleksy"],
         help="Which keyboard, to be tested, is currently installed on the emulator.",
     )
 
 
 def cli():
     """Entry-point of the `kebbie` command line."""
     # create the top-level parser
```

### Comparing `kebbie-0.1.3/kebbie/correctors.py` & `kebbie-0.2.0/kebbie/correctors.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/gesture.py` & `kebbie-0.2.0/kebbie/gesture.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/layout.py` & `kebbie-0.2.0/kebbie/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,18 @@
                     if char.lower() == SPACE:
                         char = " "
                     elif char == POINT:
                         # Points should be added to our key infos
                         pass
                     else:
                         # Other special characters are ignored
-                        continue
+                        char = None
+
+                if char is None:
+                    continue
 
                 # Save the character and its key information
                 # Save it only if it's not already in a previous klayer
                 if char not in keys_info or keys_info[char].klayer_id > klayer["id"]:
                     keys_info[char] = KeyInfo(
                         klayer["id"],
                         button["boundingRect"]["right"] - button["boundingRect"]["left"],
```

### Comparing `kebbie-0.1.3/kebbie/noise_model.py` & `kebbie-0.2.0/kebbie/noise_model.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/oracle.py` & `kebbie-0.2.0/kebbie/oracle.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/scorer.py` & `kebbie-0.2.0/kebbie/scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,18 +514,21 @@
             "min_memory": min(memories) if memories else 0,
             "max_memory": max(memories) if memories else 0,
             "mean_runtime": stats.mean(runtimes) if runtimes else 0,
             "fastest_runtime": min(runtimes) if runtimes else 0,
             "slowest_runtime": max(runtimes) if runtimes else 0,
         }
 
-        return {
-            name: human_readable_memory(x) if name.endswith("memory") else human_readable_runtime(x)
-            for name, x in perf.items()
-        }
+        if self.human_readable:
+            perf = {
+                name: human_readable_memory(x) if name.endswith("memory") else human_readable_runtime(x)
+                for name, x in perf.items()
+            }
+
+        return perf
 
     def score(self, beta: float = DEFAULT_BETA) -> Dict:  # noqa: C901
         """Method that computes the final scores (as well as some alternative
         metrics that can bring insight in the capabilities of the model), and
         output these in an organized dictionary.
 
         Args:
```

### Comparing `kebbie-0.1.3/kebbie/tokenizer.py` & `kebbie-0.2.0/kebbie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/kebbie/utils.py` & `kebbie-0.2.0/kebbie/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,18 +258,18 @@
 
     Returns:
         Human-readable version of the given number, with the right unit.
     """
     x = round_to_n(x, n=3)
     for unit in ["B", "KB", "MB", "GB"]:
         if x < 1000:
-            return f"{x} {unit}"
+            return f"{x:g} {unit}"
 
         x /= 1000
-    return f"{x} TB"
+    return f"{x:g} TB"
 
 
 def human_readable_runtime(x: int) -> str:
     """Given a number in nanoseconds, return a human-readable string of this
     number, with the right unit.
 
     Args:
@@ -277,18 +277,18 @@
 
     Returns:
         Human-readable version of the given number, with the right unit.
     """
     x = round_to_n(x, n=3)
     for unit in ["ns", "μs", "ms"]:
         if x < 1000:
-            return f"{x} {unit}"
+            return f"{x:g} {unit}"
 
         x /= 1000
-    return f"{x} s"
+    return f"{x:g} s"
 
 
 def get_soda_dataset(max_sentences: int = 2_000, seed: int = 31) -> Dict[str, List[str]]:
     """Load the SODA dataset.
 
     Args:
         max_sentences (int, optional): Maximum number of sentences in total in
```

### Comparing `kebbie-0.1.3/kebbie.egg-info/PKG-INFO` & `kebbie-0.2.0/kebbie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.1.3
+Version: 0.2.0
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.1.3/kebbie.egg-info/requires.txt` & `kebbie-0.2.0/kebbie.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/pyproject.toml` & `kebbie-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.3/setup.py` & `kebbie-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require["all"] = sum(extras_require.values(), [])
 extras_require["dev"] = (
     extras_require["test"] + extras_require["hook"] + extras_require["lint"] + extras_require["docs"]
 )
 
 setuptools.setup(
     name="kebbie",
-    version="0.1.3",
+    version="0.2.0",
     author="Nicolas REMOND",
     author_email="nicolas.remond@thingthing.co",
     description="A small framework to test and compare mobile keyboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FleksySDK/kebbie",
     packages=setuptools.find_packages(),
```

