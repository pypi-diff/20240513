# Comparing `tmp/btex-0.2.5.tar.gz` & `tmp/btex-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btex-0.2.5.tar", max compression
+gzip compressed data, was "btex-0.3.tar", max compression
```

## Comparing `btex-0.2.5.tar` & `btex-0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    21987 2024-04-29 17:12:45.552196 btex-0.2.5/btex/__init__.py
--rw-r--r--   0        0        0      362 2024-04-29 17:14:18.595562 btex-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       54 2024-02-14 17:00:31.123256 btex-0.2.5/README.md
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 btex-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    22643 2024-05-13 12:39:10.460180 btex-0.3/btex/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-13 12:40:04.678025 btex-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2115 2024-05-13 12:37:02.730502 btex-0.3/README.md
+-rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 btex-0.3/PKG-INFO
```

### Comparing `btex-0.2.5/btex/__init__.py` & `btex-0.3/btex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,24 @@
     "cong": "\\cong",
     "simeq": "\\simeq",
     "sim": "\\sim",
     "propto": "\\propto",
     "neq": "\\neq"
 }
 
+
+def newEnv():
+    return {
+        "pdftitle": "Document"
+    }
+
+
+ENV = newEnv()
+
+
 main_path = ""
 imports_to_watch = []
 customComponents: list[CustomComponent] = {}
 
 
 def resolve_scope(scope: str, is_math: bool = False):
     t = scope.replace("\n", "").replace("\t", "").replace("@", " \\@")
@@ -206,14 +216,34 @@
     if length == 1:
         docclass = f"\\documentclass{{{args[0]}}}"
     else:
         docclass = f"\\documentclass{args[0]}{{{args[1]}}}"
     return "", True
 
 
+def setenv(_, args):
+    scope = ""
+    txt = " ".join(args)
+    if args[0] == "{":
+        scope = resolve_scope(txt)
+    else:
+        with open(txt) as f:
+            scope = f.read().split("\n")
+
+    for statement in scope:
+        pair: list[str] = statement.split("=")
+        if len(pair) < 2:
+            print("Error in env: not enough information")
+            exit(1)
+        var = pair[0].strip()
+        value = pair[1].strip()
+        ENV[var] = value
+    return "", True
+
+
 def custom_component(_, args):
     name = args[0]
     if name[0] == "(":
         print("Error in component: name can't be null")
         exit(1)
     string, params, _ = getparams(args[1:], False)
     customParams = []
@@ -494,15 +524,15 @@
     p = ','.join(f"{key}={val}" for key, val in parsed.items())
 
     return f"\\lstinputlisting[{p}]{{{string}}}", True
 
 
 def _import(_, args):
     """if len(args) != 1:
-        print("How many fucking parameters did you put?")
+        print("How many parameters did you put?")
         exit(1)
     return f"\\usepackage{{{args[0]}}}", True"""
     filename = args[0]
     text = read(f"{main_path}/{filename}.btex")
     scope = resolve_scope(f"{{{text}}}")
     for line in scope:
         statement = [i for i in line.split(" ") if i != ""]
@@ -573,14 +603,15 @@
     "wrapfigure": wrapfigure,
     "paragraph": section,
     "section": section,
     "subsection": section,
     "subsubsection": section,
     "import": _import,
     "use": use,
+    "env": setenv,
     "graphic": usegraphics,
     "sqrt": sqrt,
     "split": _split,
     "binom": binom,
     "frac": frac,
     "tableofcontents": itselfnewline,
     "maketitle": itselfnewline,
@@ -648,23 +679,23 @@
 
 
 def eval_imports():
     final = ""
     for i in imports:
         label = f"\\usepackage{{{i}}}\n"
         if i == "hyperref":
-            label += """
-\\hypersetup{
+            label += f"""
+\\hypersetup{{
     colorlinks=true,
     linkcolor=blue,
     filecolor=magenta,
     urlcolor=cyan,
-    pdftitle={Overleaf Example},
+    pdftitle={{{ENV["pdftitle"]}}},
     pdfpagemode=FullScreen,
-}\n
+}}\n
 """
         if i == "listings":
             label += """
 \\definecolor{codegreen}{rgb}{0,0.6,0}
 \\definecolor{codegray}{rgb}{0.5,0.5,0.5}
 \\definecolor{codepurple}{rgb}{0.58,0,0.82}
 \\definecolor{backcolour}{rgb}{0.95,0.95,0.92}
@@ -703,14 +734,16 @@
 
     return text
 
 
 def compile_text(text: str, to: str):
     customComponents.clear()
     imports_to_watch.clear()
+    global ENV
+    ENV = newEnv()
     split = resolve_scope(f"{{{text}}}")
 
     compiled = ""
 
     for i in split:
         s, newline = exec_line(i)
         compiled += s
```

