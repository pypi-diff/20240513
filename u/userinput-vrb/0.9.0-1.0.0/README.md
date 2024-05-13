# Comparing `tmp/userinput_vrb-0.9.0.tar.gz` & `tmp/userinput_vrb-1.0.0.tar.gz`

## Comparing `userinput_vrb-0.9.0.tar` & `userinput_vrb-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/src/userinput_vrb/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/src/userinput_vrb/__version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/src/userinput_vrb/py.typed
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/LICENSE
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 userinput_vrb-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/src/userinput_vrb/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/src/userinput_vrb/__version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/src/userinput_vrb/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 userinput_vrb-1.0.0/PKG-INFO
```

### Comparing `userinput_vrb-0.9.0/src/userinput_vrb/__init__.py` & `userinput_vrb-1.0.0/src/userinput_vrb/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,117 @@
 """
 # userinput_vrb
 
-Helper functions for console user input.
+Short module description
 
 This module defines:
 
-```function input_with_default()```
+```function ...```
   
-Read string from stdin. If empty, return dflt.
+Description
 
-```function getpass_not_empty()```
-
-Read password from stdin, don't allow empty password.()
-
-```function choose_from()```
+```type ...```
+  
+Description
 
-Read character from stdin. The user must input one of
-the characters passed in choices. A default may be given.
+...
 """
 
 from getpass import getpass
 
-def input_with_default(msg: str, dflt: str) -> str:
-    """read string from stdin. If empty, return dflt.
-
-    Args:
-        msg (str): prompt for input
-        dflt (str): default value (if user enters empty string)
-
-    Returns:
-        str: string read from stdin or dflt, if empty.
-    """
-    return input(f"{msg} [{dflt}]: ").strip() or dflt
-
-def getpass_not_empty(msg: str) -> str:
-    """read password from stdin, don't allow empty password.
-
-    Args:
-        msg (str): prompt for input
-
-    Returns:
-        str: password read from stdin
-    """
-    passwd = ""
-    while not passwd:
-        passwd = getpass(msg)
-    return passwd
+class UserInput:
+    @classmethod
+    def input_with_default(cls, msg: str, dflt: str) -> str:
+        """read string from stdin. If empty, return dflt.
+
+        Args:
+            msg (str): prompt for input
+            dflt (str): default value (if user enters empty string)
+
+        Returns:
+            str: string read from stdin or dflt, if empty.
+        """
+        return input(f"{msg} [{dflt}]: ").strip() or dflt
+
+    @classmethod
+    def getpass_not_empty(cls, msg: str) -> str:
+        """read password from stdid, don't allow empty password.
+
+        Args:
+            msg (str): prompt for input
+
+        Returns:
+            str: password read from stdin
+        """
+        passwd = ""
+        while not passwd:
+            passwd = getpass(msg)
+        return passwd
     
-def choose_from(msg: str = "", choices: str = "yn", 
-                end: str = ":", dflt: str = "") -> str:
-    """read character from stdin. The user must input one of
-    the characters passed in choices (all characters will be
-    converted to lowercase). If dflt is given (and if dftl 
-    is in choices), the corresponding letter will be displayed
-    in uppercase and entering an empty string will result in
-    returning the dflt character.
-    The input prompt is: msg+choices+end, where choices will
-    be displayed with slashes between the allowed characters,
-    e.g. "Do you want to continue "+"y/N" + "? "
-
-    Args:
-        msg (str, optional): prompt for input. Defaults to "".
-        choices (str, optional): allowed chars for input. Defaults to "yn".
-        end (_type_, optional): part of prompt behind choices. Defaults to ":".
-        dflt (str, optional): default choice if just Enter is pressed. Defaults to "".
-
-    Returns:
-        str: character read from stdin
-    """
-    # make all choices lowercase
-    choices = choices.lower()
-
-    # construct message prompt
-    prompt = ""
-    # insert slash between possible answers ("yn" -> "y/n")
-    for pos in range(len(choices)-1):
-        prompt += choices[pos] + "/"
-    prompt += choices[-1]
-    # make default choice uppercase (-> e.g. "y/N")
-    if dflt:
-        pos = prompt.find(dflt.lower())
-        if pos >= 0:
-            prompt = prompt[:pos] + prompt[pos].upper() + prompt[pos+1:]
-    # start prompt with given msg text and append given end
-    prompt = msg + prompt + end
-
-    result = ""
-    while not result:
-        result = input(prompt).lower()
-        # If default is given, empty answer means default value
-        if dflt and (result == ""):
-            result = dflt.lower()
-        # otherwise answer must be one of the given choices
-        elif not result or (result not in choices):
-            result = ""
-    # return character is always lowercase
-    return result
+    @classmethod
+    def choose_from(cls, msg: str = "", choices: str = "yn", 
+                         end: str = ":", dflt: str = "") -> str:
+        """read character from stdin. The user must input one of
+        the characters passed in choices (all characters will be
+        converted to lowercase). If dflt is given (and if dftl 
+        is in choices), the correxponding letter will be displayed
+        in uppercase and entering an empty string will result in
+        returning the dflt character.
+        The input prompt is: msg+choices+end, where choices will
+        be displayed with slashes between the allowed characters,
+        e.g. "Do you want to continue "+"y/N" + "? "
+
+        Args:
+            msg (str, optional): prompt for input. Defaults to "".
+            choices (str, optional): allowed chars for input. Defaults to "yn".
+            end (_type_, optional): part of prompt behind choices. Defaults to ":".
+            dflt (str, optional): default choice if just Enter is pressed. Defaults to "".
+
+        Returns:
+            str: character read from stdin
+        """
+        # make all choices lowercase
+        choices = choices.lower()
+
+        # construct message prompt
+        prompt = ""
+        # insert slash between possible answers ("yn" -> "y/n")
+        for pos in range(len(choices)-1):
+            prompt += choices[pos] + "/"
+        prompt += choices[-1]
+        # make default choice uppercase (-> e.g. "y/N")
+        if dflt:
+            pos = prompt.find(dflt.lower())
+            if pos >= 0:
+                prompt = prompt[:pos] + prompt[pos].upper() + prompt[pos+1:]
+        # start prompt with given msg text and append given end
+        prompt = msg + prompt + end
+
+        result = ""
+        while not result:
+            result = input(prompt).lower()
+            # If default is given, empty answer means default value
+            if dflt and (result == ""):
+                result = dflt.lower()
+            # otherwise answer must be one of the given choices
+            elif not result or (result not in choices):
+                result = ""
+        # return character is always lowercase
+        return result
+    
+
+
+# Sample Usage
+if False:
+    c = UserInput.input_with_default("Input Color", "red")
+    print(f"You have entered '{c}'")
+    p = UserInput.getpass_not_empty("Enter hidden password: ")
+    print(f"You entered '{p}'")
+    if "y" != UserInput.choose_from("Do you want to continue? ", "yn", ": ", "n"):
+        print("ABORTED!")
+    else:
+        print("GO AHEAD!")
+    print("Basic variant", end=", ")
+    c = UserInput.choose_from()
+    print(f"You chose '{c}'")
+
```

### Comparing `userinput_vrb-0.9.0/LICENSE` & `userinput_vrb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userinput_vrb-0.9.0/pyproject.toml` & `userinput_vrb-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 authors = [
   { name="volker", email="volker@vrbdev.eu" },
 ]
 maintainers = [
   { name="volker", email="volker@vrbdev.eu" },
 ]
-description = "Helper functions for console user input"
+description = "Helper class for user input"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -23,15 +23,14 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/v-r-b/userinput_vrb"
-Issues = "https://github.com/v-r-b/userinput_vrb/issues"
 
 [tool.hatch.version]
 path = "./src/userinput_vrb/__version__.py"
 
 [tool.hatch.build]
 exclude = [
   "/.*",
```

