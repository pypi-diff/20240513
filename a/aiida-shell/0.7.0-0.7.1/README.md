# Comparing `tmp/aiida_shell-0.7.0.tar.gz` & `tmp/aiida_shell-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_shell-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_shell-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_shell-0.7.0.tar` & `aiida_shell-0.7.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      198 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0    17618 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      448 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/CITATION.cff
--rw-r--r--   0        0        0     1076 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/README.md
--rw-r--r--   0        0        0      638 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/Makefile
--rw-r--r--   0        0        0     1994 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/source/_static/custom.css
--rw-r--r--   0        0        0    25440 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/source/_static/logo-column.png
--rw-r--r--   0        0        0   164551 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/source/_static/logo-column.svg
--rw-r--r--   0        0        0   160798 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/source/_static/logo-shell.svg
--rw-r--r--   0        0        0   168321 2024-03-22 09:45:09.492963 aiida_shell-0.7.0/docs/source/_static/logo-text-light.svg
--rw-r--r--   0        0        0   168272 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/_static/logo-text.svg
--rw-r--r--   0        0        0    41343 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/_static/provenance-pdb-tools.svg
--rw-r--r--   0        0        0       36 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/changelog.md
--rw-r--r--   0        0        0     1875 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/conf.py
--rw-r--r--   0        0        0     1903 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/examples.md
--rw-r--r--   0        0        0     9528 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/examples/gromacs.md
--rw-r--r--   0        0        0    51065 2024-03-22 09:45:09.496963 aiida_shell-0.7.0/docs/source/examples/include/images/gromacs/potential_energy.png
--rw-r--r--   0        0        0  1178644 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/include/images/gromacs/provenance.png
--rw-r--r--   0        0        0   104698 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/include/images/qe/band_structure.png
--rwxr-xr-x   0        0        0     5895 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/include/scripts/gromacs.py
--rwxr-xr-x   0        0        0     1046 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/include/scripts/lammps.py
--rwxr-xr-x   0        0        0     4232 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/include/scripts/qe.py
--rw-r--r--   0        0        0     5737 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/lammps.md
--rw-r--r--   0        0        0    10681 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/examples/qe.md
--rw-r--r--   0        0        0    27961 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/howto.rst
--rw-r--r--   0        0        0     3890 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/index.rst
--rw-r--r--   0        0        0      590 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/docs/source/installation.rst
--rw-r--r--   0        0        0     2885 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      376 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/__init__.py
--rw-r--r--   0        0        0      103 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/calculations/__init__.py
--rw-r--r--   0        0        0    21789 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/calculations/shell.py
--rw-r--r--   0        0        0      201 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/data/__init__.py
--rw-r--r--   0        0        0     1646 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/data/code.py
--rw-r--r--   0        0        0     4703 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/data/entry_point.py
--rw-r--r--   0        0        0     5652 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/data/pickled.py
--rw-r--r--   0        0        0    10590 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/launch.py
--rw-r--r--   0        0        0      104 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/parsers/__init__.py
--rw-r--r--   0        0        0     6017 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/parsers/shell.py
--rw-r--r--   0        0        0       26 2024-03-22 09:45:09.504963 aiida_shell-0.7.0/src/aiida_shell/py.typed
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 aiida_shell-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      198 2024-05-13 14:22:49.446898 aiida_shell-0.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0    17996 2024-05-13 14:22:49.446898 aiida_shell-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2024-05-13 14:22:49.446898 aiida_shell-0.7.1/CITATION.cff
+-rw-r--r--   0        0        0     1076 2024-05-13 14:22:49.446898 aiida_shell-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0      729 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/README.md
+-rw-r--r--   0        0        0      638 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0     1994 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/custom.css
+-rw-r--r--   0        0        0    25440 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/logo-column.png
+-rw-r--r--   0        0        0   164551 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/logo-column.svg
+-rw-r--r--   0        0        0   160798 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/logo-shell.svg
+-rw-r--r--   0        0        0   168321 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/logo-text-light.svg
+-rw-r--r--   0        0        0   168272 2024-05-13 14:22:49.450898 aiida_shell-0.7.1/docs/source/_static/logo-text.svg
+-rw-r--r--   0        0        0    41343 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/_static/provenance-pdb-tools.svg
+-rw-r--r--   0        0        0       36 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/changelog.md
+-rw-r--r--   0        0        0     1875 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1903 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/examples.md
+-rw-r--r--   0        0        0     9528 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/examples/gromacs.md
+-rw-r--r--   0        0        0    51065 2024-05-13 14:22:49.454898 aiida_shell-0.7.1/docs/source/examples/include/images/gromacs/potential_energy.png
+-rw-r--r--   0        0        0  1178644 2024-05-13 14:22:49.458898 aiida_shell-0.7.1/docs/source/examples/include/images/gromacs/provenance.png
+-rw-r--r--   0        0        0   104698 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/include/images/qe/band_structure.png
+-rwxr-xr-x   0        0        0     5895 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/include/scripts/gromacs.py
+-rwxr-xr-x   0        0        0     1046 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/include/scripts/lammps.py
+-rwxr-xr-x   0        0        0     4232 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/include/scripts/qe.py
+-rw-r--r--   0        0        0     5737 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/lammps.md
+-rw-r--r--   0        0        0    10681 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/examples/qe.md
+-rw-r--r--   0        0        0    28093 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/howto.rst
+-rw-r--r--   0        0        0     3890 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/index.rst
+-rw-r--r--   0        0        0      590 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     2885 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      376 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/calculations/__init__.py
+-rw-r--r--   0        0        0    21789 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/calculations/shell.py
+-rw-r--r--   0        0        0      201 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/data/__init__.py
+-rw-r--r--   0        0        0     1646 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/data/code.py
+-rw-r--r--   0        0        0     4703 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/data/entry_point.py
+-rw-r--r--   0        0        0     5652 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/data/pickled.py
+-rw-r--r--   0        0        0    10590 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/launch.py
+-rw-r--r--   0        0        0      104 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/parsers/__init__.py
+-rw-r--r--   0        0        0     6229 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/parsers/shell.py
+-rw-r--r--   0        0        0       26 2024-05-13 14:22:49.462898 aiida_shell-0.7.1/src/aiida_shell/py.typed
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 aiida_shell-0.7.1/PKG-INFO
```

### Comparing `aiida_shell-0.7.0/CHANGELOG.md` & `aiida_shell-0.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Change log
 
+## `v0.7.1` - 2024-05-13
+
+### Fixes
+- `ShellParser`: Prefix output filenames starting with a number [[352c309]](https://github.com/sphuber/aiida-shell/commit/352c309c0b4b5fd2c6af78dcf01013bfb6def6a6)
+
+### Docs
+- Docs: Add hint on retrieving outputs from daemon submitted jobs [[31ebfbc]](https://github.com/sphuber/aiida-shell/commit/31ebfbcde77f30a34a5495f349c19424d8dc1984)
+
+
 ## `v0.7.0` - 2024-03-22
 
 ### Features
 - `PickledData`: Allow passing kwargs to pickler [[f94f030]](https://github.com/sphuber/aiida-shell/commit/f94f030abb36fd8f0dee60190c71b9df5e0a8a6c)
 - `ShellJob`: Automatically serialize string for `arguments` [[4518221]](https://github.com/sphuber/aiida-shell/commit/451822157d9bc585254fded0352863258a7a7290)
 - `launch_shell_job`: Add option to keep skip resolving of `command` [[d4ad9e7]](https://github.com/sphuber/aiida-shell/commit/d4ad9e72b26b3fd6591501e29fab2c9d70046d88)
```

### Comparing `aiida_shell-0.7.0/LICENSE.txt` & `aiida_shell-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/README.md` & `aiida_shell-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/Makefile` & `aiida_shell-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/custom.css` & `aiida_shell-0.7.1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/logo-column.png` & `aiida_shell-0.7.1/docs/source/_static/logo-column.png`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/logo-column.svg` & `aiida_shell-0.7.1/docs/source/_static/logo-column.svg`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/logo-shell.svg` & `aiida_shell-0.7.1/docs/source/_static/logo-shell.svg`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/logo-text-light.svg` & `aiida_shell-0.7.1/docs/source/_static/logo-text-light.svg`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/logo-text.svg` & `aiida_shell-0.7.1/docs/source/_static/logo-text.svg`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/_static/provenance-pdb-tools.svg` & `aiida_shell-0.7.1/docs/source/_static/provenance-pdb-tools.svg`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/conf.py` & `aiida_shell-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples.md` & `aiida_shell-0.7.1/docs/source/examples.md`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/gromacs.md` & `aiida_shell-0.7.1/docs/source/examples/gromacs.md`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/images/gromacs/potential_energy.png` & `aiida_shell-0.7.1/docs/source/examples/include/images/gromacs/potential_energy.png`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/images/gromacs/provenance.png` & `aiida_shell-0.7.1/docs/source/examples/include/images/gromacs/provenance.png`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/images/qe/band_structure.png` & `aiida_shell-0.7.1/docs/source/examples/include/images/qe/band_structure.png`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/scripts/gromacs.py` & `aiida_shell-0.7.1/docs/source/examples/include/scripts/gromacs.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/scripts/lammps.py` & `aiida_shell-0.7.1/docs/source/examples/include/scripts/lammps.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/include/scripts/qe.py` & `aiida_shell-0.7.1/docs/source/examples/include/scripts/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/lammps.md` & `aiida_shell-0.7.1/docs/source/examples/lammps.md`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/examples/qe.md` & `aiida_shell-0.7.1/docs/source/examples/qe.md`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/howto.rst` & `aiida_shell-0.7.1/docs/source/howto.rst`

 * *Files 2% similar despite different names*

```diff
@@ -547,14 +547,16 @@
         if all(node.is_terminated for node in nodes):
             break
         time.sleep(1)
 
     for node in nodes:
         if node.is_finished_ok:
             print(f'{node} finished successfully')
+            # The outputs of each node can be accessed through `node.outputs`:
+            print(node.outputs.stdout.get_content())
         else:
             print(f'{node} failed')
 
 
 Custom output parsing
 =====================
```

### Comparing `aiida_shell-0.7.0/docs/source/index.rst` & `aiida_shell-0.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/docs/source/installation.rst` & `aiida_shell-0.7.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/pyproject.toml` & `aiida_shell-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/calculations/shell.py` & `aiida_shell-0.7.1/src/aiida_shell/calculations/shell.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/data/code.py` & `aiida_shell-0.7.1/src/aiida_shell/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/data/entry_point.py` & `aiida_shell-0.7.1/src/aiida_shell/data/entry_point.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/data/pickled.py` & `aiida_shell-0.7.1/src/aiida_shell/data/pickled.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/launch.py` & `aiida_shell-0.7.1/src/aiida_shell/launch.py`

 * *Files identical despite different names*

### Comparing `aiida_shell-0.7.0/src/aiida_shell/parsers/shell.py` & `aiida_shell-0.7.1/src/aiida_shell/parsers/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,21 +53,25 @@
         exit_code: ExitCode = getattr(self.exit_codes, key).format(**kwargs)
         return exit_code
 
     @staticmethod
     def format_link_label(filename: str) -> str:
         """Format the link label from a given filename.
 
-        Valid link labels can only contain alphanumeric characters and underscores, without consecutive underscores. So
-        all characters that are not alphanumeric or an underscore are converted to underscores, where consecutive
-        underscores are merged into one.
+        Valid link labels can only contain alphanumeric characters and underscores, without consecutive underscores.
+        They can also not start with a number. So all characters that are not alphanumeric or an underscore are
+        converted to underscores, where consecutive underscores are merged into one. Filenames that start with a number
+        are prefixed with ``aiida_shell_``.
 
         :param filename: The filename.
         :returns: The link label.
         """
+        if re.match('^[0-9]+.*', filename):
+            filename = f'aiida_shell_{filename}'
+
         alphanumeric = re.sub('[^0-9a-zA-Z_]+', '_', filename)
         link_label = re.sub('_[_]+', '_', alphanumeric)
         return link_label
 
     def parse_default_outputs(self, dirpath: pathlib.Path) -> ExitCode:
         """Parse the output files that should have been retrieved by default.
```

### Comparing `aiida_shell-0.7.0/PKG-INFO` & `aiida_shell-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-shell
-Version: 0.7.0
+Version: 0.7.1
 Summary: AiiDA plugin that makes running shell commands easy.
 Keywords: aiida,workflows
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
```

