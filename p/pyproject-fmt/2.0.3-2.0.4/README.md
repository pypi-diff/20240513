# Comparing `tmp/pyproject_fmt-2.0.3.tar.gz` & `tmp/pyproject_fmt-2.0.4.tar.gz`

## Comparing `pyproject_fmt-2.0.3.tar` & `pyproject_fmt-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/tox.ini
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/tests/test_cli.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/README.md
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tox.ini
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_cli.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/README.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.4/PKG-INFO
```

### Comparing `pyproject_fmt-2.0.3/tox.ini` & `pyproject_fmt-2.0.4/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -60,17 +60,19 @@
     python -m build --sdist --wheel -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:docs]
 description = build documentation
 extras =
     docs
+set_env =
+    DOCS_OUT = {posargs:{toxworkdir}{/}docs_out}
 commands =
-    sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b html {posargs}
-    python -c 'print(r"documentation available under file://{toxworkdir}{/}docs_out{/}index.html")'
+    sphinx-build -d "{envtmpdir}{/}doctree" docs "{env:DOCS_OUT}" --color -b html
+    python -c 'print(r"documentation available under file://{env:DOCS_OUT}{/}index.html")'
 
 [testenv:dev]
 description = generate a DEV environment
 package = editable
 extras =
     docs
     test
```

### Comparing `pyproject_fmt-2.0.3/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.0.4/src/pyproject_fmt/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.3/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.0.4/src/pyproject_fmt/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     stdout: bool
     check: bool
 
     column_width: int
     indent: int
     keep_full_version: bool
     max_supported_python: tuple[int, int]
-    min_supported_python: tuple[int, int]
 
 
 @dataclass(frozen=True)
 class Config:
     """Configuration flags for the formatting."""
 
     pyproject_toml: Path
@@ -102,40 +101,37 @@
         version=f"%(prog)s ({version('pyproject-fmt')})",
     )
     group = parser.add_mutually_exclusive_group()
     msg = "print the formatted text to the stdout (instead of update in-place)"
     group.add_argument("-s", "--stdout", action="store_true", help=msg)
     msg = "check and fail if any input would be formatted, printing any diffs"
     group.add_argument("--check", action="store_true", help=msg)
-    msg = "keep full dependency versions. For example do not change version 1.0.0 to 1"
-    parser.add_argument("--keep-full-version", action="store_true", help=msg)
     parser.add_argument(
         "--column-width",
         type=int,
         default=1,
         help="max column width in the file",
+        metavar="count",
     )
     parser.add_argument(
         "--indent",
         type=int,
         default=2,
         help="number of spaces to indent",
-    )
-    parser.add_argument(
-        "--min-supported-python",
-        type=_version_argument,
-        default=(3, 8),
-        help="latest Python version the project supports (e.g. 3.8)",
+        metavar="count",
     )
     parser.add_argument(
         "--max-supported-python",
+        metavar="minor.major",
         type=_version_argument,
         default=(3, 12),
         help="latest Python version the project supports (e.g. 3.13)",
     )
+    msg = "keep full dependency versions - do not remove redundant .0 from versions"
+    parser.add_argument("--keep-full-version", action="store_true", help=msg)
     msg = "pyproject.toml file(s) to format"
     parser.add_argument("inputs", nargs="+", type=pyproject_toml_path_creator, help=msg)
     return parser
 
 
 def cli_args(args: Sequence[str]) -> list[Config]:
     """
@@ -149,40 +145,37 @@
     parser.parse_args(namespace=opt, args=args)
     res = []
     for pyproject_toml in opt.inputs:
         column_width = opt.column_width
         indent = opt.indent
         keep_full_version = opt.keep_full_version
         max_supported_python = opt.max_supported_python
-        min_supported_python = opt.min_supported_python
         with pyproject_toml.open("rb") as file_handler:
             config = tomllib.load(file_handler)
             if "tool" in config and "pyproject-fmt" in config["tool"]:
                 for key, entry in config["tool"]["pyproject-fmt"].items():
                     if key == "column_width":
                         column_width = int(entry)
                     elif key == "indent":
                         indent = int(entry)
                     elif key == "keep_full_version":
                         keep_full_version = bool(entry)
                     elif key == "max_supported_python":
                         max_supported_python = _version_argument(entry)
-                    elif key == "min_supported_python":  # pragma: no branch
-                        min_supported_python = _version_argument(entry)
         res.append(
             Config(
                 pyproject_toml=pyproject_toml,
                 stdout=opt.stdout,
                 check=opt.check,
                 settings=Settings(
                     column_width=column_width,
                     indent=indent,
                     keep_full_version=keep_full_version,
                     max_supported_python=max_supported_python,
-                    min_supported_python=min_supported_python,
+                    min_supported_python=(3, 8),  # default for when the user did not specify via requires-python
                 ),
             )
         )
 
     return res
```

### Comparing `pyproject_fmt-2.0.3/tests/test_cli.py` & `pyproject_fmt-2.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.3/tests/test_main.py` & `pyproject_fmt-2.0.4/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,29 +208,28 @@
       "requests>=2.0",
     ]
 
     [tool.pyproject-fmt]
     column_width = 20
     indent = 4
     keep_full_version = true
-    min_supported_python = "3.7"
     max_supported_python = "3.10"
+    ignore_extra = true
     """
     filename = tmp_path / "pyproject.toml"
     filename.write_text(dedent(txt))
     run([str(filename)])
 
     expected = """\
     [project]
     keywords = [
         "A",
     ]
     classifiers = [
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ]
     dynamic = [
         "B",
     ]
@@ -238,15 +237,15 @@
         "requests>=2.0",
     ]
 
     [tool.pyproject-fmt]
     column_width = 20
     indent = 4
     keep_full_version = true
-    min_supported_python = "3.7"
     max_supported_python = "3.10"
+    ignore_extra = true
     """
     got = filename.read_text()
     assert got == dedent(expected)
     out, err = capsys.readouterr()
     assert out
     assert not err
```

### Comparing `pyproject_fmt-2.0.3/LICENSE.txt` & `pyproject_fmt-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.3/README.md` & `pyproject_fmt-2.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,10 @@
 [![PyPI](https://img.shields.io/pypi/v/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![Downloads](https://static.pepy.tech/badge/pyproject-fmt/month)](https://pepy.tech/project/pyproject-fmt)
 [![PyPI - License](https://img.shields.io/pypi/l/pyproject-fmt?style=flat-square)](https://opensource.org/licenses/MIT)
 [![check](https://github.com/tox-dev/pyproject-fmt/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pyproject-fmt/actions/workflows/check.yml)
 
-Apply a consistent format to `pyproject.toml` files.
-[Read the full documentation here](https://pyproject-fmt.readthedocs.io/en/latest/).
+Apply a consistent format to the `pyproject.toml` files.
 
-## add to pre-commit
-
-```yaml
-- repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "1.7.0"
-  hooks:
-    - id: pyproject-fmt
-```
+[For more information on how to use or configure read the documentation here](https://pyproject-fmt.readthedocs.io/en/latest/).
```

### Comparing `pyproject_fmt-2.0.3/pyproject.toml` & `pyproject_fmt-2.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,16 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "pyproject-fmt-rust==1.0.4",
+  "pyproject-fmt-rust==1.0.6",
+  "tomli>=2.0.1; python_version<'3.11'",
 ]
 optional-dependencies.docs = [
   "furo>=2024.5.6",
   "sphinx>=7.3.7",
   "sphinx-argparse-cli>=1.15",
   "sphinx-autodoc-typehints>=2.1",
   "sphinx-copybutton>=0.5.2",
```

### Comparing `pyproject_fmt-2.0.3/PKG-INFO` & `pyproject_fmt-2.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 2.0.3
+Version: 2.0.4
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
@@ -33,15 +33,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: pyproject-fmt-rust==1.0.4
+Requires-Dist: pyproject-fmt-rust==1.0.6
+Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
 Requires-Dist: furo>=2024.5.6; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.15; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints>=2.1; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx>=7.3.7; extra == 'docs'
 Provides-Extra: test
@@ -56,18 +57,10 @@
 [![PyPI](https://img.shields.io/pypi/v/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![Downloads](https://static.pepy.tech/badge/pyproject-fmt/month)](https://pepy.tech/project/pyproject-fmt)
 [![PyPI - License](https://img.shields.io/pypi/l/pyproject-fmt?style=flat-square)](https://opensource.org/licenses/MIT)
 [![check](https://github.com/tox-dev/pyproject-fmt/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pyproject-fmt/actions/workflows/check.yml)
 
-Apply a consistent format to `pyproject.toml` files.
-[Read the full documentation here](https://pyproject-fmt.readthedocs.io/en/latest/).
+Apply a consistent format to the `pyproject.toml` files.
 
-## add to pre-commit
-
-```yaml
-- repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "1.7.0"
-  hooks:
-    - id: pyproject-fmt
-```
+[For more information on how to use or configure read the documentation here](https://pyproject-fmt.readthedocs.io/en/latest/).
```

