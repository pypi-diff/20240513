# Comparing `tmp/shellcrafter-1.1.3.tar.gz` & `tmp/shellcrafter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.1.3.tar", last modified: Sun May  5 01:32:42 2024, max compression
+gzip compressed data, was "shellcrafter-1.1.5.tar", last modified: Mon May 13 16:59:09 2024, max compression
```

## Comparing `shellcrafter-1.1.3.tar` & `shellcrafter-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.540789 shellcrafter-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.540789 shellcrafter-1.1.3/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/keyst_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/peutils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/shellcode_procedure_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.273474 shellcrafter-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/keyst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/peutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/shellcode_procedure_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.1.3/PKG-INFO` & `shellcrafter-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.3
+Version: 1.1.5
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

### Comparing `shellcrafter-1.1.3/README.md` & `shellcrafter-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.3/setup.py` & `shellcrafter-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.1.3"
+version = "1.1.5"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 REPO_URL = 'https://github.com/totekuh/shellcrafter'
```

### Comparing `shellcrafter-1.1.3/src/shellcrafter/cli.py` & `shellcrafter-1.1.5/src/shellcrafter/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,39 +190,39 @@
         shellcode_assembled, count = ShellcodeCompiler(arch).assemble_instructions(
             get_instructions(instructions, instructions_file))
         shellcode_runner.run_shellcode(shellcode_assembled, interactive)
 
 
 @pe_app.command(name="rva-offset-find", help="Convert RVA to file offset in a PE file.")
 def find_rva_offset_(file: str,
-                     rva: str = typer.Argument(...,
+                     rva: str = Argument(...,
                                                help='RVA to convert. Supports "0x" prefix for hexadecimal values.'),
-                     section_name: Optional[str] = typer.Option(None, "--section-name", "-sn",
+                     section_name: Optional[str] = Option(None, "--section-name", "-sn",
                                                                 help='Optional. The name of the section to search through for the given --rva offset.')):
     find_rva_offset(file=file, rva=rva, section_name=section_name)
 
 
 @pe_app.command(name="iat-print", help="Print the Import Address Table (IAT), "
                                        "optionally filtering by DLL name and/or function name.")
 def iat_print_(file: str,
-               dll: Optional[str] = typer.Option(None, help="Filter by DLL name, case-insensitive."),
-               function: Optional[str] = typer.Option(None, help="Filter by function name, case-insensitive.")):
+               dll: Optional[str] = Option(None, help="Filter by DLL name, case-insensitive."),
+               function: Optional[str] = Option(None, help="Filter by function name, case-insensitive.")):
     iat_print(file=file, dll=dll, function=function)
 
 
 @pe_app.command(name="bytes-display", help="Display bytes from a file starting at a specified offset.")
-def display_bytes_(file: str = typer.Argument(..., help="The path to the binary file."),
-                          offset: str = typer.Option(..., help="Offset in the file to start reading bytes."),
-                          length: int = typer.Option(..., help="Number of bytes to read and display.")):
+def display_bytes_(file: str = Argument(..., help="The path to the binary file."),
+                          offset: str = Option(..., help="Offset in the file to start reading bytes."),
+                          length: int = Option(..., help="Number of bytes to read and display.")):
     display_bytes(file=file, offset=offset, length=length)
 
 @pe_app.command(name="bytes-search", help="Search for a sequence of bytes or ASCII characters in a file.")
-def bytes_search(file: str = typer.Argument(..., help="The path to the binary file."),
-                 bytes_: Optional[str] = typer.Option(None, "--bytes", help="Byte sequence to search for, e.g., '\\x41\\x42\\x43'."),
-                 ascii: Optional[str] = typer.Option(None, "--ascii", help="ASCII text to search for, e.g., 'ABC'. Specify only one of --bytes or --ascii.")):
+def bytes_search(file: str = Argument(..., help="The path to the binary file."),
+                 bytes_: Optional[str] = Option(None, "--bytes", help="Byte sequence to search for, e.g., '\\x41\\x42\\x43'."),
+                 ascii: Optional[str] = Option(None, "--ascii", help="ASCII text to search for, e.g., 'ABC'. Specify only one of --bytes or --ascii.")):
     """
     Search for a sequence of bytes or ASCII text in a file. Specify either --bytes or --ascii.
     """
     if bytes_ and ascii:
         raise Exit("Error: Please specify either a byte sequence or an ASCII string, not both.")
     if not bytes_ and not ascii:
         raise Exit("Error: No search pattern provided. Please specify a byte sequence or an ASCII string.")
@@ -240,13 +240,13 @@
     search_bytes(file=file, search_sequence=search_sequence)
 
 @pe_app.command(name="eat-print", help="Parse the Export Address Table (EAT) and print it.")
 def eat_print_(file: str):
     parse_eat(file=file)
 
 @pe_app.command(name="sections-print", help="Print details of each section in the PE file.")
-def print_sections_(file: str = typer.Argument(..., help="The path to the PE file.")):
+def print_sections_(file: str = Argument(..., help="The path to the PE file.")):
     print_sections(file=file)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `shellcrafter-1.1.3/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.1.5/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.3/src/shellcrafter/keyst_api.py` & `shellcrafter-1.1.5/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.3/src/shellcrafter/peutils.py` & `shellcrafter-1.1.5/src/shellcrafter/peutils.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.3/src/shellcrafter/shellcode_procedure_generator.py` & `shellcrafter-1.1.5/src/shellcrafter/shellcode_procedure_generator.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.3/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.1.5/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.3
+Version: 1.1.5
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

