# Comparing `tmp/arrr-1.0.4.tar.gz` & `tmp/arrr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrr-1.0.4.tar", last modified: Sat Dec 17 12:25:43 2022, max compression
+gzip compressed data, was "arrr-1.0.5.tar", last modified: Mon May 13 15:48:54 2024, max compression
```

## Comparing `arrr-1.0.4.tar` & `arrr-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ntoll     (1000) ntoll     (1000)        0 2022-12-17 12:25:43.689399 arrr-1.0.4/
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1080 2022-12-17 12:17:39.000000 arrr-1.0.4/CHANGES.rst
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1066 2020-06-19 10:53:45.000000 arrr-1.0.4/LICENSE
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       55 2022-12-17 12:10:38.000000 arrr-1.0.4/MANIFEST.in
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     6093 2022-12-17 12:25:43.689399 arrr-1.0.4/PKG-INFO
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     3045 2022-12-17 12:10:44.000000 arrr-1.0.4/README.rst
-drwxrwxr-x   0 ntoll     (1000) ntoll     (1000)        0 2022-12-17 12:25:43.689399 arrr-1.0.4/arrr.egg-info/
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     6093 2022-12-17 12:25:43.000000 arrr-1.0.4/arrr.egg-info/PKG-INFO
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)      202 2022-12-17 12:25:43.000000 arrr-1.0.4/arrr.egg-info/SOURCES.txt
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)        1 2022-12-17 12:25:43.000000 arrr-1.0.4/arrr.egg-info/dependency_links.txt
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       38 2022-12-17 12:25:43.000000 arrr-1.0.4/arrr.egg-info/entry_points.txt
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)        5 2022-12-17 12:25:43.000000 arrr-1.0.4/arrr.egg-info/top_level.txt
--rwxrwxr-x   0 ntoll     (1000) ntoll     (1000)     5114 2022-12-17 12:24:32.000000 arrr-1.0.4/arrr.py
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       38 2022-12-17 12:25:43.689399 arrr-1.0.4/setup.cfg
--rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1052 2022-12-17 12:10:38.000000 arrr-1.0.4/setup.py
+drwxrwxr-x   0 ntoll     (1000) ntoll     (1000)        0 2024-05-13 15:48:54.579845 arrr-1.0.5/
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1136 2024-05-13 15:41:21.000000 arrr-1.0.5/CHANGES.rst
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1066 2020-06-19 10:53:45.000000 arrr-1.0.5/LICENSE
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       55 2022-12-17 12:10:38.000000 arrr-1.0.5/MANIFEST.in
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     6189 2024-05-13 15:48:54.579845 arrr-1.0.5/PKG-INFO
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     3045 2022-12-17 12:10:44.000000 arrr-1.0.5/README.rst
+drwxrwxr-x   0 ntoll     (1000) ntoll     (1000)        0 2024-05-13 15:48:54.579845 arrr-1.0.5/arrr.egg-info/
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     6189 2024-05-13 15:48:54.000000 arrr-1.0.5/arrr.egg-info/PKG-INFO
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)      202 2024-05-13 15:48:54.000000 arrr-1.0.5/arrr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)        1 2024-05-13 15:48:54.000000 arrr-1.0.5/arrr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       38 2024-05-13 15:48:54.000000 arrr-1.0.5/arrr.egg-info/entry_points.txt
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)        5 2024-05-13 15:48:54.000000 arrr-1.0.5/arrr.egg-info/top_level.txt
+-rwxrwxr-x   0 ntoll     (1000) ntoll     (1000)     5467 2024-05-13 15:43:25.000000 arrr-1.0.5/arrr.py
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)       38 2024-05-13 15:48:54.579845 arrr-1.0.5/setup.cfg
+-rw-rw-r--   0 ntoll     (1000) ntoll     (1000)     1052 2022-12-17 12:10:38.000000 arrr-1.0.5/setup.py
```

### Comparing `arrr-1.0.4/CHANGES.rst` & `arrr-1.0.5/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+1.0.5
+=====
+
+* New ship in which to sail: MicroPython.
+
 1.0.4
 =====
 
 * Cleaned up blots in the cap'n's log.
 * More piratical ways to mangle English.
 
 1.0.3
```

### Comparing `arrr-1.0.4/LICENSE` & `arrr-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arrr-1.0.4/PKG-INFO` & `arrr-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arrr
-Version: 1.0.4
+Version: 1.0.5
 Summary: A module and command to turn English into Pirate speak.
 Home-page: https://github.com/ntoll/arrr
 Author: Nicholas H.Tollervey
 Author-email: ntoll@ntoll.org
 License: MIT
 Description: Arrr.py - Pirate Speak for Python
         =================================
@@ -104,14 +104,19 @@
         
         If you find any bugs, `submit a new issue <https://github.com/ntoll/arrr/issues/new>`_. Thank you!
         
         
         Release History
         ===============
         
+        1.0.5
+        =====
+        
+        * New ship in which to sail: MicroPython.
+        
         1.0.4
         =====
         
         * Cleaned up blots in the cap'n's log.
         * More piratical ways to mangle English.
         
         1.0.3
```

### Comparing `arrr-1.0.4/README.rst` & `arrr-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `arrr-1.0.4/arrr.egg-info/PKG-INFO` & `arrr-1.0.5/arrr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arrr
-Version: 1.0.4
+Version: 1.0.5
 Summary: A module and command to turn English into Pirate speak.
 Home-page: https://github.com/ntoll/arrr
 Author: Nicholas H.Tollervey
 Author-email: ntoll@ntoll.org
 License: MIT
 Description: Arrr.py - Pirate Speak for Python
         =================================
@@ -104,14 +104,19 @@
         
         If you find any bugs, `submit a new issue <https://github.com/ntoll/arrr/issues/new>`_. Thank you!
         
         
         Release History
         ===============
         
+        1.0.5
+        =====
+        
+        * New ship in which to sail: MicroPython.
+        
         1.0.4
         =====
         
         * Cleaned up blots in the cap'n's log.
         * More piratical ways to mangle English.
         
         1.0.3
```

### Comparing `arrr-1.0.4/arrr.py` & `arrr-1.0.5/arrr.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,29 +19,27 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
-import argparse as arrrgparse  # Geddit..? ;-)
 import random
-import sys
 
 
 #: The help text to be shown when requested.
 _HELP_TEXT = """
 Take English words and turn them into something Pirate-ish.
 
 Documentation here: https://arrr.readthedocs.io/en/latest/
 """
 
 
 #: MAJOR, MINOR, RELEASE, STATUS [alpha, beta, final], VERSION
-_VERSION = (1, 0, 4)
+_VERSION = (1, 0, 5)
 
 
 #: Defines English to Pirate-ish word substitutions.
 _PIRATE_WORDS = {
     "hello": "ahoy",
     "hi": "arrr",
     "my": "me",
@@ -112,44 +110,62 @@
 def get_version():
     """
     Returns a string representation of the version information of this project.
     """
     return ".".join([str(i) for i in _VERSION])
 
 
+def capitalized(word):
+    """
+    A MicroPython compatible means of capitalizing a string.
+    """
+    if word:
+        return word[0].upper() + word[1:]
+
+
 def translate(english):
     """
     Take some English text and return a Pirate-ish version thereof.
     """
     # Normalise a list of words (remove whitespace and make lowercase)
-    words = [w.lower() for w in english.split()]
+    original = english.split()
+    words = [w.lower() for w in original]
     # Substitute some English words with Pirate equivalents.
-    result = [_PIRATE_WORDS.get(word, word) for word in words]
+    result = []
+    for count, word in enumerate(words):
+        if word in _PIRATE_WORDS:
+            result.append(_PIRATE_WORDS.get(word, word))
+        else:
+            result.append(original[count])
     # Capitalize words that begin a sentence and potentially insert a pirate
     # phrase with a chance of 1 in 5.
     capitalize = True
     for i, word in enumerate(result):
         if capitalize:
-            result[i] = word.capitalize()
+            result[i] = capitalized(word)
             capitalize = False
-        if word.endswith((".", "!", "?", ":",)):
+        if word[-1] in (".", "!", "?", ":",):
             # It's a word that ends with a sentence ending character.
             capitalize = True
             if random.randint(0, 5) == 0:
                 result.insert(i + 1, random.choice(_PIRATE_PHRASES))
     return " ".join(result)
 
 
 def main(arrrgv=None):
     """ 
     Entry point for the command line tool 'pirate'.
 
     Will print help text if the optional first argument is "help". Otherwise,
     takes the text passed into the command and prints a pirate version of it.
     """
+    # These imports are here for MicroPython compatibility related reasons.
+    import argparse as arrrgparse  # Geddit..? ;-)
+    import sys
+
     if not arrrgv:
         arrrgv = sys.argv[1:]
 
     parser = arrrgparse.ArgumentParser(description=_HELP_TEXT)
     parser.add_argument("english", nargs="*", default="")
     arrrgs = parser.parse_args(arrrgv)
     if arrrgs.english:
@@ -159,11 +175,7 @@
         except Exception:
             print(
                 "Error processing English. The pirates replied:\n\n"
                 "Shiver me timbers. We're fish bait. "
                 "Summat went awry, me lovely! Arrr..."
             )
             sys.exit(1)
-
-
-if __name__ == "__main__":
-    main(sys.argv[1:])
```

### Comparing `arrr-1.0.4/setup.py` & `arrr-1.0.5/setup.py`

 * *Files identical despite different names*

