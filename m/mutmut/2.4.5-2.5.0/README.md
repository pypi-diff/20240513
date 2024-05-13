# Comparing `tmp/mutmut-2.4.5.tar.gz` & `tmp/mutmut-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutmut-2.4.5.tar", last modified: Thu Apr  4 07:16:13 2024, max compression
+gzip compressed data, was "mutmut-2.5.0.tar", last modified: Mon May 13 15:30:50 2024, max compression
```

## Comparing `mutmut-2.4.5.tar` & `mutmut-2.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.526012 mutmut-2.4.5/
--rw-r--r--   0 boxed      (501) staff       (20)     1345 2024-04-04 07:15:09.000000 mutmut-2.4.5/AUTHORS.rst
--rw-r--r--   0 boxed      (501) staff       (20)    13241 2024-04-04 07:12:53.000000 mutmut-2.4.5/HISTORY.rst
--rw-r--r--   0 boxed      (501) staff       (20)     1471 2021-07-21 11:45:51.000000 mutmut-2.4.5/LICENSE
--rw-r--r--   0 boxed      (501) staff       (20)      110 2021-07-21 11:45:51.000000 mutmut-2.4.5/MANIFEST.in
--rw-r--r--   0 boxed      (501) staff       (20)    18267 2024-04-04 07:16:13.526171 mutmut-2.4.5/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)    14511 2024-04-04 07:11:00.000000 mutmut-2.4.5/README.rst
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.523447 mutmut-2.4.5/mutmut/
--rw-r--r--   0 boxed      (501) staff       (20)    42440 2024-04-04 07:13:03.000000 mutmut-2.4.5/mutmut/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)    19122 2024-04-04 07:11:00.000000 mutmut-2.4.5/mutmut/__main__.py
--rw-r--r--   0 boxed      (501) staff       (20)    18528 2024-04-04 07:11:00.000000 mutmut-2.4.5/mutmut/cache.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.524667 mutmut-2.4.5/mutmut.egg-info/
--rw-r--r--   0 boxed      (501) staff       (20)    18267 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)      464 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/SOURCES.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/dependency_links.txt
--rw-r--r--   0 boxed      (501) staff       (20)       52 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/entry_points.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2021-07-21 11:54:27.000000 mutmut-2.4.5/mutmut.egg-info/not-zip-safe
--rw-r--r--   0 boxed      (501) staff       (20)      124 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/requires.txt
--rw-r--r--   0 boxed      (501) staff       (20)        7 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/top_level.txt
--rw-r--r--   0 boxed      (501) staff       (20)       46 2024-04-04 07:08:51.000000 mutmut-2.4.5/requirements.txt
--rw-r--r--   0 boxed      (501) staff       (20)      375 2024-04-04 07:16:13.526599 mutmut-2.4.5/setup.cfg
--rwxr-xr-x   0 boxed      (501) staff       (20)     3621 2024-04-04 07:08:54.000000 mutmut-2.4.5/setup.py
--rw-r--r--   0 boxed      (501) staff       (20)       67 2021-07-21 11:45:51.000000 mutmut-2.4.5/test_requirements.txt
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.525750 mutmut-2.4.5/tests/
--rw-r--r--   0 boxed      (501) staff       (20)      914 2021-07-21 11:45:51.000000 mutmut-2.4.5/tests/test_cache.py
--rw-r--r--   0 boxed      (501) staff       (20)     5117 2024-04-04 07:08:54.000000 mutmut-2.4.5/tests/test_init.py
--rw-r--r--   0 boxed      (501) staff       (20)    24908 2024-04-04 07:11:00.000000 mutmut-2.4.5/tests/test_main.py
--rw-r--r--   0 boxed      (501) staff       (20)    13133 2024-04-04 07:08:54.000000 mutmut-2.4.5/tests/test_mutation.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-13 15:30:50.098562 mutmut-2.5.0/
+-rw-r--r--   0 boxed      (501) staff       (20)     1362 2024-05-13 15:28:44.000000 mutmut-2.5.0/AUTHORS.rst
+-rw-r--r--   0 boxed      (501) staff       (20)    13385 2024-05-13 15:28:44.000000 mutmut-2.5.0/HISTORY.rst
+-rw-r--r--   0 boxed      (501) staff       (20)     1471 2024-04-06 10:47:53.000000 mutmut-2.5.0/LICENSE
+-rw-r--r--   0 boxed      (501) staff       (20)      110 2024-04-06 10:47:53.000000 mutmut-2.5.0/MANIFEST.in
+-rw-r--r--   0 boxed      (501) staff       (20)    15704 2024-05-13 15:30:50.098372 mutmut-2.5.0/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)    14715 2024-05-13 15:28:44.000000 mutmut-2.5.0/README.rst
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-13 15:30:50.093785 mutmut-2.5.0/mutmut/
+-rw-r--r--   0 boxed      (501) staff       (20)    42458 2024-05-13 15:28:44.000000 mutmut-2.5.0/mutmut/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)    19240 2024-04-06 10:47:53.000000 mutmut-2.5.0/mutmut/__main__.py
+-rw-r--r--   0 boxed      (501) staff       (20)    18557 2024-04-06 10:47:53.000000 mutmut-2.5.0/mutmut/cache.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-13 15:30:50.097346 mutmut-2.5.0/mutmut.egg-info/
+-rw-r--r--   0 boxed      (501) staff       (20)    15704 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)      498 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/SOURCES.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/dependency_links.txt
+-rw-r--r--   0 boxed      (501) staff       (20)       51 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/entry_points.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2024-04-06 10:48:01.000000 mutmut-2.5.0/mutmut.egg-info/not-zip-safe
+-rw-r--r--   0 boxed      (501) staff       (20)      124 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/requires.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        7 2024-05-13 15:30:50.000000 mutmut-2.5.0/mutmut.egg-info/top_level.txt
+-rw-r--r--   0 boxed      (501) staff       (20)       46 2024-04-06 10:47:53.000000 mutmut-2.5.0/requirements.txt
+-rw-r--r--   0 boxed      (501) staff       (20)      375 2024-05-13 15:30:50.098976 mutmut-2.5.0/setup.cfg
+-rwxr-xr-x   0 boxed      (501) staff       (20)     3621 2024-04-06 10:47:53.000000 mutmut-2.5.0/setup.py
+-rw-r--r--   0 boxed      (501) staff       (20)       67 2024-04-06 10:47:53.000000 mutmut-2.5.0/test_requirements.txt
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-05-13 15:30:50.097085 mutmut-2.5.0/tests/
+-rw-r--r--   0 boxed      (501) staff       (20)      914 2024-04-06 10:47:53.000000 mutmut-2.5.0/tests/test_cache.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5593 2024-04-06 10:47:53.000000 mutmut-2.5.0/tests/test_init.py
+-rw-r--r--   0 boxed      (501) staff       (20)    25701 2024-04-06 10:47:53.000000 mutmut-2.5.0/tests/test_main.py
+-rw-r--r--   0 boxed      (501) staff       (20)    13133 2024-04-06 10:47:53.000000 mutmut-2.5.0/tests/test_mutation.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1600 2024-04-06 10:47:53.000000 mutmut-2.5.0/tests/test_mutmut_config_hooks.py
```

### Comparing `mutmut-2.4.5/AUTHORS.rst` & `mutmut-2.5.0/AUTHORS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 * Eivind Jahren <eivind.jahren@gmail.com>
 * WiredNerd <pbuschmail-gitlab@yahoo.com>
 * Kees Hink <kees@fourdigits.nl>
 * Jim Rybarski <jim@rybarski.com>
 * Christopher J. Brody <chris.brody+brodybits@gmail.com>
 * Century-ss <hgfc7543ggfdch@gmail.com>
 * Michael Champagne <michael.champagne@elapsetech.com>
+* Florian Trudel
```

### Comparing `mutmut-2.4.5/HISTORY.rst` & `mutmut-2.5.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 ---------
 
+2.5.0
+~~~~~
+
+* Add cli option to specify html report directory
+
+* Fix use patch file under Windows
+
+* Improve documentation about cache issues
+
 2.4.5
 ~~~~~
 
 * Add skipped column in html index report
 
 * Untested/skipped in show all does not show skipped
```

### Comparing `mutmut-2.4.5/LICENSE` & `mutmut-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutmut-2.4.5/PKG-INFO` & `mutmut-2.5.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,409 +1,390 @@
-Metadata-Version: 2.1
-Name: mutmut
-Version: 2.4.5
-Summary: mutation testing for Python 3
-Home-page: https://github.com/boxed/mutmut
-Author: Anders Hovmöller
-Author-email: boxed@killingar.net
-License: BSD
-Description: mutmut - python mutation tester
-        ===============================
-        
-        .. image:: https://travis-ci.org/boxed/mutmut.svg?branch=master
-            :target: https://travis-ci.org/boxed/mutmut
-        
-        .. image:: https://readthedocs.org/projects/mutmut/badge/?version=latest
-            :target: https://mutmut.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://codecov.io/gh/boxed/mutmut/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/boxed/mutmut
-        
-        .. image:: https://img.shields.io/discord/767914934016802818.svg
-          :target: https://discord.gg/cwb9uNt
-        
-        Mutmut is a mutation testing system for Python, with a strong focus on ease
-        of use. If you don't know what mutation testing is try starting with
-        `this article <https://hackernoon.com/mutmut-a-python-mutation-testing-system-9b9639356c78>`_.
-        
-        Some highlight features:
-        
-        - Found mutants can be applied on disk with a simple command making it very
-          easy to work with the results
-        - Remembers work that has been done, so you can work incrementally
-        - Supports all test runners (because mutmut only needs an exit code from the
-          test command)
-        - If you use the `hammett <https://github.com/boxed/hammett>`_ test runner
-          you can go extremely fast! There's special handling for this runner
-          that has some pretty dramatic results.
-        - Can use coverage data to only do mutation testing on covered lines
-        - Battle tested on real libraries by multiple companies
-        
-        
-        If you need to run mutmut on a python 2 code base use mutmut ``1.5.0``. Mutmut
-        ``1.9.0`` is the last version to support python ``3.4``, ``3.5`` and ``3.6``.
-        
-        
-        Install and run
-        ---------------
-        
-        You can get started with a simple:
-        
-        .. code-block:: console
-        
-            pip install mutmut
-            mutmut run
-        
-        This will by default run pytest (or unittest if pytest is unavailable)
-        on tests in the "tests" or "test" folder and
-        it will try to figure out where the code to mutate lies.
-        
-        NOTE that mutmut will apply the mutations directly, one at a time;
-        it is **highly** recommended to add all changes to source control
-        before running.
-        
-        Enter
-        
-        .. code-block:: console
-        
-            mutmut run --help
-        
-        for the available flags, to use other runners, etc. The recommended way to use
-        mutmut if the defaults aren't working for you is to add a
-        block in ``setup.cfg`` or ``project.toml``.
-        Then when you come back to mutmut weeks later you don't have to figure out the
-        flags again, just run ``mutmut run`` and it works.
-        Like this in ``setup.cfg``:
-        
-        .. code-block:: ini
-        
-            [mutmut]
-            paths_to_mutate=src/
-            backup=False
-            runner=python -m hammett -x
-            tests_dir=tests/
-            dict_synonyms=Struct, NamedStruct
-        
-        or like this in ``pyproject.toml``:
-        
-        .. code-block:: ini
-        
-            [tool.mutmut]
-            paths_to_mutate="src"
-            runner="python -m hammett -x"
-        
-        To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
-        use a comma or colon separated list. For example:
-        
-        .. code-block:: ini
-        
-            [mutmut]
-            paths_to_mutate=src/,src2/
-            tests_dir=tests/:tests2/
-        
-        You can stop the mutation run at any time and mutmut will restart where you
-        left off. It's also smart enough to retest only the surviving mutants when the
-        test suite changes.
-        
-        To print the results run ``mutmut show``. It will give you a list of the mutants
-        grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
-        all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
-        with ``mutmut show all``.
-        
-        You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
-        have the file you mutate under source code control and committed before you apply
-        a mutant!
-        
-        To generate a HTML report for a web browser: ``mutmut html``
-        
-        Whitelisting
-        ------------
-        
-        You can mark lines like this:
-        
-        .. code-block:: python
-        
-            some_code_here()  # pragma: no mutate
-        
-        to stop mutation on those lines. Some cases we've found where you need to
-        whitelist lines are:
-        
-        - The version string on your library. You really shouldn't have a test for this :P
-        - Optimizing break instead of continue. The code runs fine when mutating break
-          to continue, but it's slower.
-        
-        See also `Advanced whitelisting and configuration`_
-        
-        
-        Example mutations
-        -----------------
-        
-        - Integer literals are changed by adding 1. So 0 becomes 1, 5 becomes 6, etc.
-        - ``<`` is changed to ``<=``
-        - break is changed to continue and vice versa
-        
-        In general the idea is that the mutations should be as subtle as possible.
-        See ``__init__.py`` for the full list.
-        
-        
-        Workflow
-        --------
-        
-        This section describes how to work with mutmut to enhance your test suite.
-        
-        1. Run mutmut with ``mutmut run``. A full run is preferred but if you're just
-           getting started you can exit in the middle and start working with what you
-           have found so far.
-        2. Show the mutants with ``mutmut results``
-        3. Apply a surviving mutant to disk running ``mutmut apply 3`` (replace 3 with
-           the relevant mutant ID from ``mutmut results``)
-        4. Write a new test that fails
-        5. Revert the mutant on disk
-        6. Rerun the new test to see that it now passes
-        7. Go back to point 2.
-        
-        Mutmut keeps a result cache in ``.mutmut-cache`` so if you want to make sure you
-        run a full mutmut run just delete this file.
-        
-        If you want to re-run all survivors after changing a lot of code or even the configuration,
-        you can use `for ID in $(mutmut result-ids survived); do mutmut run $ID; done` (for bash).
-        
-        You can also tell mutmut to just check a single mutant:
-        
-        .. code-block:: console
-        
-            mutmut run 3
-        
-        
-        Advanced whitelisting and configuration
-        ---------------------------------------
-        
-        mutmut has an advanced configuration system. You create a file called
-        ``mutmut_config.py``. You can define two functions there: ``init()`` and
-        ``pre_mutation(context)``. ``init`` gets called when mutmut starts and
-        ``pre_mutation`` gets called before each mutant is applied and tested. You can
-        mutate the ``context`` object as you need. You can modify the test command like
-        this:
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                context.config.test_command = 'python -m pytest -x ' + something_else
-        
-        or skip a mutant:
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                if context.filename == 'foo.py':
-                    context.skip = True
-        
-        or skip logging:
-        
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                line = context.current_source_line.strip()
-                if line.startswith('log.'):
-                    context.skip = True
-        
-        look at the code for the ``Context`` class for what you can modify. Please
-        open a github issue if you need help.
-        
-        It is also possible to disable mutation of specific node types by passing the
-        ``--disable-mutation-types`` option. Multiple types can be specified by separating them
-        by comma:
-        
-        .. code-block:: console
-        
-            mutmut run --disable-mutation-types=string,decorator
-        
-        Inversely, you can also only specify to only run specific mutations with ``--enable-mutation-types``.
-        Note that ``--disable-mutation-types`` and ``--enable-mutation-types`` are exclusive and cannot
-        be combined.
-        
-        
-        Selecting tests to run
-        ----------------------
-        
-        If you have a large test suite or long running tests, it can be beneficial to narrow the set of tests to
-        run for each mutant down to the tests that have a chance of killing it.
-        Determining the relevant subset of tests depends on your project, its structure, and the metadata that you
-        know about your tests.
-        ``mutmut`` provides information like the file to mutate and `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_
-        (if used with the ``--use-coverage`` switch).
-        You can set the ``context.config.test_command`` in the ``pre_mutation(context)`` hook of ``mutmut_config.py``.
-        The ``test_command`` is reset after each mutant, so you don't have to explicitly (re)set it for each mutant.
-        
-        This section gives examples to show how this could be done for some concrete use cases.
-        All examples use the default test runner (``python -m pytest -x --assert=plain``).
-        
-        Selection based on source and test layout
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If the location of the test module has a strict correlation with your source code layout, you can simply
-        construct the path to the corresponding test file from ``context.filename``.
-        Suppose your layout follows the following structure where the test file is always located right beside the
-        production code:
-        
-        .. code-block:: console
-        
-            mypackage
-            ├── production_module.py
-            ├── test_production_module.py
-            └── subpackage
-                ├── submodule.py
-                └── test_submodule.py
-        
-        Your ``mutmut_config.py`` in this case would look like this:
-        
-        .. code-block:: python
-        
-            import os.path
-        
-            def pre_mutation(context):
-                dirname, filename = os.path.split(context.filename)
-                testfile = "test_" + filename
-                context.config.test_command += ' ' + os.path.join(dirname, testfile)
-        
-        Selection based on imports
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If you can't rely on the directory structure or naming of the test files, you may assume that the tests most likely
-        to kill the mutant are located in test files that directly import the module that is affected by the mutant.
-        Using the ``ast`` module of the Python standard library, you can use the ``init()`` hook to build a map which test file
-        imports which module, and then lookup all test files importing the mutated module and only run those:
-        
-        .. code-block:: python
-        
-            import ast
-            from pathlib import Path
-        
-            test_imports = {}
-        
-        
-            class ImportVisitor(ast.NodeVisitor):
-                """Visitor which records which modules are imported."""
-                def __init__(self) -> None:
-                    super().__init__()
-                    self.imports = []
-        
-                def visit_Import(self, node: ast.Import) -> None:
-                    for alias in node.names:
-                        self.imports.append(alias.name)
-        
-                def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
-                    self.imports.append(node.module)
-        
-        
-            def init():
-                """Find all test files located under the 'tests' directory and create an abstract syntax tree for each.
-                Let the ``ImportVisitor`` find out what modules they import and store the information in a global dictionary
-                which can be accessed by ``pre_mutation(context)``."""
-                test_files = (Path(__file__).parent / "tests").rglob("test*.py")
-                for fpath in test_files:
-                    visitor = ImportVisitor()
-                    visitor.visit(ast.parse(fpath.read_bytes()))
-                    test_imports[str(fpath)] = visitor.imports
-        
-        
-            def pre_mutation(context):
-                """Construct the module name from the filename and run all test files which import that module."""
-                tests_to_run = []
-                for testfile, imports in test_imports.items():
-                    module_name = context.filename.rstrip(".py").replace("/", ".")
-                    if module_name in imports:
-                        tests_to_run.append(testfile)
-                context.config.test_command += f"{' '.join(tests_to_run)}"
-        
-        Selection based on coverage contexts
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If you recorded `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_ and use
-        the ``--use-coverage`` switch, you can access this coverage data inside the ``pre_mutation(context)`` hook
-        via the ``context.config.coverage_data`` attribute. This attribute is a dictionary in the form
-        ``{filename: {lineno: [contexts]}}``.
-        
-        Let's say you have used the built-in dynamic context option of ``Coverage.py`` by adding the following to
-        your ``.coveragerc`` file:
-        
-        .. code-block:: console
-        
-            [run]
-            dynamic_context = test_function
-        
-        ``coverage`` will create a new context for each test function that you run in the form ``module_name.function_name``.
-        With ``pytest``, we can use the ``-k`` switch to filter tests that match a given expression.
-        
-        .. code-block:: python
-        
-            import os.path
-        
-            def pre_mutation(context):
-                """Extract the coverage contexts if possible and only run the tests matching this data."""
-                if not context.config.coverage_data:
-                    # mutmut was run without ``--use-coverage``
-                    return
-                fname = os.path.abspath(context.filename)
-                contexts_for_file = context.config.coverage_data.get(fname, {})
-                contexts_for_line = contexts_for_file.get(context.current_line_index, [])
-                test_names = [
-                    ctx.rsplit(".", 1)[-1]  # extract only the final part after the last dot, which is the test function name
-                    for ctx in contexts_for_line
-                    if ctx  # skip empty strings
-                ]
-                if not test_names:
-                    return
-                context.config.test_command += f' -k "{" or ".join(test_names)}"'
-        
-        Pay attention that the format of the context name varies depending on the tool you use for creating the contexts.
-        For example, the ``pytest-cov`` plugin uses ``::`` as separator between module and test function.
-        Furthermore, not all tools are able to correctly pick up the correct contexts. ``coverage.py`` for instance is (at the time of writing)
-        unable to pick up tests that are inside a class when using ``pytest``.
-        You will have to inspect your ``.coverage`` database using the `Coverage.py API <https://coverage.readthedocs.io/en/coverage-5.5/api.html>`_
-        first to determine how you can extract the correct information to use with your test runner.
-        
-        Making things more robust
-        ^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Despite your best efforts in picking the right subset of tests, it may happen that the mutant survives because the test which is able
-        to kill it was not included in the test set. You can tell ``mutmut`` to re-run the full test suite in that case, to verify that this
-        mutant indeed survives.
-        You can do so by passing the ``--rerun-all`` option to ``mutmut run``. This option is disabled by default.
-        
-        
-        JUnit XML support
-        -----------------
-        
-        In order to better integrate with CI/CD systems, ``mutmut`` supports the
-        generation of a JUnit XML report (using https://pypi.org/project/junit-xml/).
-        This option is available by calling ``mutmut junitxml``. In order to define how
-        to deal with suspicious and untested mutants, you can use
-        
-        .. code-block:: console
-        
-            mutmut junitxml --suspicious-policy=ignore --untested-policy=ignore
-        
-        The possible values for these policies are:
-        
-        - ``ignore``: Do not include the results on the report at all
-        - ``skipped``: Include the mutant on the report as "skipped"
-        - ``error``: Include the mutant on the report as "error"
-        - ``failure``: Include the mutant on the report as "failure"
-        
-        If a failed mutant is included in the report, then the unified diff of the
-        mutant will also be included for debugging purposes.
-        
-Keywords: mutmut mutant mutation test testing
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Provides-Extra: pytest
-Provides-Extra: coverage
-Provides-Extra: patch
+mutmut - python mutation tester
+===============================
+
+.. image:: https://travis-ci.org/boxed/mutmut.svg?branch=master
+    :target: https://travis-ci.org/boxed/mutmut
+
+.. image:: https://readthedocs.org/projects/mutmut/badge/?version=latest
+    :target: https://mutmut.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/boxed/mutmut/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/boxed/mutmut
+
+.. image:: https://img.shields.io/discord/767914934016802818.svg
+  :target: https://discord.gg/cwb9uNt
+
+Mutmut is a mutation testing system for Python, with a strong focus on ease
+of use. If you don't know what mutation testing is try starting with
+`this article <https://hackernoon.com/mutmut-a-python-mutation-testing-system-9b9639356c78>`_.
+
+Some highlight features:
+
+- Found mutants can be applied on disk with a simple command making it very
+  easy to work with the results
+- Remembers work that has been done, so you can work incrementally
+- Supports all test runners (because mutmut only needs an exit code from the
+  test command)
+- If you use the `hammett <https://github.com/boxed/hammett>`_ test runner
+  you can go extremely fast! There's special handling for this runner
+  that has some pretty dramatic results.
+- Can use coverage data to only do mutation testing on covered lines
+- Battle tested on real libraries by multiple companies
+
+
+If you need to run mutmut on a python 2 code base use mutmut ``1.5.0``. Mutmut
+``1.9.0`` is the last version to support python ``3.4``, ``3.5`` and ``3.6``.
+
+
+Install and run
+---------------
+
+You can get started with a simple:
+
+.. code-block:: console
+
+    pip install mutmut
+    mutmut run
+
+This will by default run pytest (or unittest if pytest is unavailable)
+on tests in the "tests" or "test" folder and
+it will try to figure out where the code to mutate lies.
+
+NOTE that mutmut will apply the mutations directly, one at a time;
+it is **highly** recommended to add all changes to source control
+before running.
+
+Enter
+
+.. code-block:: console
+
+    mutmut run --help
+
+for the available flags, to use other runners, etc. The recommended way to use
+mutmut if the defaults aren't working for you is to add a
+block in ``setup.cfg`` or ``project.toml``.
+Then when you come back to mutmut weeks later you don't have to figure out the
+flags again, just run ``mutmut run`` and it works.
+Like this in ``setup.cfg``:
+
+.. code-block:: ini
+
+    [mutmut]
+    paths_to_mutate=src/
+    backup=False
+    runner=python -m hammett -x
+    tests_dir=tests/
+    dict_synonyms=Struct, NamedStruct
+
+or like this in ``pyproject.toml``:
+
+.. code-block:: ini
+
+    [tool.mutmut]
+    paths_to_mutate="src"
+    runner="python -m hammett -x"
+
+To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
+use a comma or colon separated list. For example:
+
+.. code-block:: ini
+
+    [mutmut]
+    paths_to_mutate=src/,src2/
+    tests_dir=tests/:tests2/
+
+You can stop the mutation run at any time and mutmut will restart where you
+left off. It's also smart enough to retest only the surviving mutants when the
+test suite changes.
+
+To print the results run ``mutmut show``. It will give you a list of the mutants
+grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
+all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
+with ``mutmut show all``.
+
+You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
+have the file you mutate under source code control and committed before you apply
+a mutant!
+
+To generate a HTML report for a web browser: ``mutmut html``
+
+Whitelisting
+------------
+
+You can mark lines like this:
+
+.. code-block:: python
+
+    some_code_here()  # pragma: no mutate
+
+to stop mutation on those lines. Some cases we've found where you need to
+whitelist lines are:
+
+- The version string on your library. You really shouldn't have a test for this :P
+- Optimizing break instead of continue. The code runs fine when mutating break
+  to continue, but it's slower.
+
+See also `Advanced whitelisting and configuration`_
+
+
+Example mutations
+-----------------
+
+- Integer literals are changed by adding 1. So 0 becomes 1, 5 becomes 6, etc.
+- ``<`` is changed to ``<=``
+- break is changed to continue and vice versa
+
+In general the idea is that the mutations should be as subtle as possible.
+See ``__init__.py`` for the full list.
+
+
+Workflow
+--------
+
+This section describes how to work with mutmut to enhance your test suite.
+
+1. Run mutmut with ``mutmut run``. A full run is preferred but if you're just
+   getting started you can exit in the middle and start working with what you
+   have found so far.
+2. Show the mutants with ``mutmut results``
+3. Apply a surviving mutant to disk running ``mutmut apply 3`` (replace 3 with
+   the relevant mutant ID from ``mutmut results``)
+4. Write a new test that fails
+5. Revert the mutant on disk
+6. Rerun the new test to see that it now passes
+7. Go back to point 2.
+
+Mutmut keeps a result cache in ``.mutmut-cache`` so if you want to make sure you
+run a full mutmut run just delete this file.
+
+If you want to re-run all survivors after changing a lot of code or even the configuration,
+you can use `for ID in $(mutmut result-ids survived); do mutmut run $ID; done` (for bash).
+
+You can also tell mutmut to just check a single mutant:
+
+.. code-block:: console
+
+    mutmut run 3
+
+
+Advanced whitelisting and configuration
+---------------------------------------
+
+mutmut has an advanced configuration system. You create a file called
+``mutmut_config.py``. You can define two functions there: ``init()`` and
+``pre_mutation(context)``. ``init`` gets called when mutmut starts and
+``pre_mutation`` gets called before each mutant is applied and tested. You can
+mutate the ``context`` object as you need. You can modify the test command like
+this:
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        context.config.test_command = 'python -m pytest -x ' + something_else
+
+or skip a mutant:
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        if context.filename == 'foo.py':
+            context.skip = True
+
+or skip logging:
+
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        line = context.current_source_line.strip()
+        if line.startswith('log.'):
+            context.skip = True
+
+look at the code for the ``Context`` class for what you can modify. Please
+open a github issue if you need help.
+
+It is also possible to disable mutation of specific node types by passing the
+``--disable-mutation-types`` option. Multiple types can be specified by separating them
+by comma:
+
+.. code-block:: console
+
+    mutmut run --disable-mutation-types=string,decorator
+
+Inversely, you can also only specify to only run specific mutations with ``--enable-mutation-types``.
+Note that ``--disable-mutation-types`` and ``--enable-mutation-types`` are exclusive and cannot
+be combined.
+
+Changes made to ``mutmut_config.py`` does not invalidate the cache.
+If you modify the configuration file, you will likely need to remove ``.mutmut-cache`` manually to ensure that the changes take effect.
+
+Selecting tests to run
+----------------------
+
+If you have a large test suite or long running tests, it can be beneficial to narrow the set of tests to
+run for each mutant down to the tests that have a chance of killing it.
+Determining the relevant subset of tests depends on your project, its structure, and the metadata that you
+know about your tests.
+``mutmut`` provides information like the file to mutate and `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_
+(if used with the ``--use-coverage`` switch).
+You can set the ``context.config.test_command`` in the ``pre_mutation(context)`` hook of ``mutmut_config.py``.
+The ``test_command`` is reset after each mutant, so you don't have to explicitly (re)set it for each mutant.
+
+This section gives examples to show how this could be done for some concrete use cases.
+All examples use the default test runner (``python -m pytest -x --assert=plain``).
+
+Selection based on source and test layout
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If the location of the test module has a strict correlation with your source code layout, you can simply
+construct the path to the corresponding test file from ``context.filename``.
+Suppose your layout follows the following structure where the test file is always located right beside the
+production code:
+
+.. code-block:: console
+
+    mypackage
+    ├── production_module.py
+    ├── test_production_module.py
+    └── subpackage
+        ├── submodule.py
+        └── test_submodule.py
+
+Your ``mutmut_config.py`` in this case would look like this:
+
+.. code-block:: python
+
+    import os.path
+
+    def pre_mutation(context):
+        dirname, filename = os.path.split(context.filename)
+        testfile = "test_" + filename
+        context.config.test_command += ' ' + os.path.join(dirname, testfile)
+
+Selection based on imports
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you can't rely on the directory structure or naming of the test files, you may assume that the tests most likely
+to kill the mutant are located in test files that directly import the module that is affected by the mutant.
+Using the ``ast`` module of the Python standard library, you can use the ``init()`` hook to build a map which test file
+imports which module, and then lookup all test files importing the mutated module and only run those:
+
+.. code-block:: python
+
+    import ast
+    from pathlib import Path
+
+    test_imports = {}
+
+
+    class ImportVisitor(ast.NodeVisitor):
+        """Visitor which records which modules are imported."""
+        def __init__(self) -> None:
+            super().__init__()
+            self.imports = []
+
+        def visit_Import(self, node: ast.Import) -> None:
+            for alias in node.names:
+                self.imports.append(alias.name)
+
+        def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
+            self.imports.append(node.module)
+
+
+    def init():
+        """Find all test files located under the 'tests' directory and create an abstract syntax tree for each.
+        Let the ``ImportVisitor`` find out what modules they import and store the information in a global dictionary
+        which can be accessed by ``pre_mutation(context)``."""
+        test_files = (Path(__file__).parent / "tests").rglob("test*.py")
+        for fpath in test_files:
+            visitor = ImportVisitor()
+            visitor.visit(ast.parse(fpath.read_bytes()))
+            test_imports[str(fpath)] = visitor.imports
+
+
+    def pre_mutation(context):
+        """Construct the module name from the filename and run all test files which import that module."""
+        tests_to_run = []
+        for testfile, imports in test_imports.items():
+            module_name = context.filename.rstrip(".py").replace("/", ".")
+            if module_name in imports:
+                tests_to_run.append(testfile)
+        context.config.test_command += f"{' '.join(tests_to_run)}"
+
+Selection based on coverage contexts
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you recorded `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_ and use
+the ``--use-coverage`` switch, you can access this coverage data inside the ``pre_mutation(context)`` hook
+via the ``context.config.coverage_data`` attribute. This attribute is a dictionary in the form
+``{filename: {lineno: [contexts]}}``.
+
+Let's say you have used the built-in dynamic context option of ``Coverage.py`` by adding the following to
+your ``.coveragerc`` file:
+
+.. code-block:: console
+
+    [run]
+    dynamic_context = test_function
+
+``coverage`` will create a new context for each test function that you run in the form ``module_name.function_name``.
+With ``pytest``, we can use the ``-k`` switch to filter tests that match a given expression.
+
+.. code-block:: python
+
+    import os.path
+
+    def pre_mutation(context):
+        """Extract the coverage contexts if possible and only run the tests matching this data."""
+        if not context.config.coverage_data:
+            # mutmut was run without ``--use-coverage``
+            return
+        fname = os.path.abspath(context.filename)
+        contexts_for_file = context.config.coverage_data.get(fname, {})
+        contexts_for_line = contexts_for_file.get(context.current_line_index, [])
+        test_names = [
+            ctx.rsplit(".", 1)[-1]  # extract only the final part after the last dot, which is the test function name
+            for ctx in contexts_for_line
+            if ctx  # skip empty strings
+        ]
+        if not test_names:
+            return
+        context.config.test_command += f' -k "{" or ".join(test_names)}"'
+
+Pay attention that the format of the context name varies depending on the tool you use for creating the contexts.
+For example, the ``pytest-cov`` plugin uses ``::`` as separator between module and test function.
+Furthermore, not all tools are able to correctly pick up the correct contexts. ``coverage.py`` for instance is (at the time of writing)
+unable to pick up tests that are inside a class when using ``pytest``.
+You will have to inspect your ``.coverage`` database using the `Coverage.py API <https://coverage.readthedocs.io/en/coverage-5.5/api.html>`_
+first to determine how you can extract the correct information to use with your test runner.
+
+Making things more robust
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Despite your best efforts in picking the right subset of tests, it may happen that the mutant survives because the test which is able
+to kill it was not included in the test set. You can tell ``mutmut`` to re-run the full test suite in that case, to verify that this
+mutant indeed survives.
+You can do so by passing the ``--rerun-all`` option to ``mutmut run``. This option is disabled by default.
+
+
+JUnit XML support
+-----------------
+
+In order to better integrate with CI/CD systems, ``mutmut`` supports the
+generation of a JUnit XML report (using https://pypi.org/project/junit-xml/).
+This option is available by calling ``mutmut junitxml``. In order to define how
+to deal with suspicious and untested mutants, you can use
+
+.. code-block:: console
+
+    mutmut junitxml --suspicious-policy=ignore --untested-policy=ignore
+
+The possible values for these policies are:
+
+- ``ignore``: Do not include the results on the report at all
+- ``skipped``: Include the mutant on the report as "skipped"
+- ``error``: Include the mutant on the report as "error"
+- ``failure``: Include the mutant on the report as "failure"
+
+If a failed mutant is included in the report, then the unified diff of the
+mutant will also be included for debugging purposes.
```

### Comparing `mutmut-2.4.5/README.rst` & `mutmut-2.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mutmut
+Version: 2.5.0
+Summary: mutation testing for Python 3
+Home-page: https://github.com/boxed/mutmut
+Author: Anders Hovmöller
+Author-email: boxed@killingar.net
+License: BSD
+Keywords: mutmut mutant mutation test testing
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: glob2
+Requires-Dist: parso
+Requires-Dist: click
+Requires-Dist: pony
+Requires-Dist: junit-xml<2,>=1.8
+Requires-Dist: toml
+Provides-Extra: pytest
+Requires-Dist: pytest; extra == "pytest"
+Requires-Dist: pytest-cov; extra == "pytest"
+Provides-Extra: coverage
+Requires-Dist: coverage; extra == "coverage"
+Provides-Extra: patch
+Requires-Dist: whatthepatch==0.0.6; extra == "patch"
+
 mutmut - python mutation tester
 ===============================
 
 .. image:: https://travis-ci.org/boxed/mutmut.svg?branch=master
     :target: https://travis-ci.org/boxed/mutmut
 
 .. image:: https://readthedocs.org/projects/mutmut/badge/?version=latest
@@ -211,14 +243,16 @@
 
     mutmut run --disable-mutation-types=string,decorator
 
 Inversely, you can also only specify to only run specific mutations with ``--enable-mutation-types``.
 Note that ``--disable-mutation-types`` and ``--enable-mutation-types`` are exclusive and cannot
 be combined.
 
+Changes made to ``mutmut_config.py`` does not invalidate the cache.
+If you modify the configuration file, you will likely need to remove ``.mutmut-cache`` manually to ensure that the changes take effect.
 
 Selecting tests to run
 ----------------------
 
 If you have a large test suite or long running tests, it can be beneficial to narrow the set of tests to
 run for each mutant down to the tests that have a chance of killing it.
 Determining the relevant subset of tests depends on your project, its structure, and the metadata that you
```

### Comparing `mutmut-2.4.5/mutmut/__init__.py` & `mutmut-2.5.0/mutmut/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 )
 from time import time
 from typing import Callable, Dict, Iterator, List, Optional, Set, Tuple
 
 from parso import parse
 from parso.python.tree import Name, Number, Keyword, FStringStart, FStringEnd
 
-__version__ = '2.4.5'
+__version__ = '2.5.0'
 
 
 if os.getcwd() not in sys.path:
     sys.path.insert(0, os.getcwd())
 try:
     import mutmut_config
 except ImportError:
@@ -1216,15 +1216,15 @@
         import whatthepatch
     except ImportError as e:
         raise ImportError('The --use-patch feature requires the whatthepatch library. Run "pip install --force-reinstall mutmut[patch]"') from e
     with open(patch_file_path) as f:
         diffs = whatthepatch.parse_patch(f.read())
 
     return {
-        diff.header.new_path: {change.new for change in diff.changes if change.old is None}
+        os.path.normpath(diff.header.new_path): {change.new for change in diff.changes if change.old is None}
         for diff in diffs if diff.changes
     }
 
 
 def add_mutations_by_file(
     mutations_by_file: Dict[str, List[RelativeMutationID]],
     filename: str,
```

### Comparing `mutmut-2.4.5/mutmut/__main__.py` & `mutmut-2.5.0/mutmut/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,22 +250,24 @@
     """
     print_result_cache_junitxml(dict_synonyms, suspicious_policy, untested_policy)
     sys.exit(0)
 
 
 @climain.command(context_settings=dict(help_option_names=['-h', '--help']))
 @click.option('--dict-synonyms')
+@click.option('-d', '--directory', help='Write the output files to DIR.')
 @config_from_file(
     dict_synonyms='',
+    directory='html',
 )
-def html(dict_synonyms):
+def html(dict_synonyms, directory):
     """
     Generate a HTML report of surviving mutants.
     """
-    create_html_report(dict_synonyms)
+    create_html_report(dict_synonyms, directory)
     sys.exit(0)
 
 
 def do_run(
     argument,
     paths_to_mutate,
     disable_mutation_types,
```

### Comparing `mutmut-2.4.5/mutmut/cache.py` & `mutmut-2.5.0/mutmut/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,28 +256,28 @@
 
     ts = TestSuite("mutmut", test_cases)
     return to_xml_report_string([ts])
 
 
 @init_db
 @db_session
-def create_html_report(dict_synonyms):
+def create_html_report(dict_synonyms, directory):
     mutants = sorted(list(select(x for x in Mutant)), key=lambda x: x.line.sourcefile.filename)
 
-    os.makedirs('html', exist_ok=True)
+    os.makedirs(directory, exist_ok=True)
 
-    with open('html/index.html', 'w') as index_file:
+    with open(join(directory, 'index.html'), 'w') as index_file:
         index_file.write('<h1>Mutation testing report</h1>')
 
         index_file.write('Killed %s out of %s mutants' % (len([x for x in mutants if x.status == OK_KILLED]), len(mutants)))
 
         index_file.write('<table><thead><tr><th>File</th><th>Total</th><th>Skipped</th><th>Killed</th><th>% killed</th><th>Survived</th></thead>')
 
         for filename, mutants in groupby(mutants, key=lambda x: x.line.sourcefile.filename):
-            report_filename = join('html', filename)
+            report_filename = join(directory, filename)
 
             mutants = list(mutants)
 
             with open(filename) as f:
                 source = f.read()
 
             os.makedirs(dirname(report_filename), exist_ok=True)
```

### Comparing `mutmut-2.4.5/mutmut.egg-info/PKG-INFO` & `mutmut-2.5.0/mutmut.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,409 +1,422 @@
 Metadata-Version: 2.1
 Name: mutmut
-Version: 2.4.5
+Version: 2.5.0
 Summary: mutation testing for Python 3
 Home-page: https://github.com/boxed/mutmut
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
-Description: mutmut - python mutation tester
-        ===============================
-        
-        .. image:: https://travis-ci.org/boxed/mutmut.svg?branch=master
-            :target: https://travis-ci.org/boxed/mutmut
-        
-        .. image:: https://readthedocs.org/projects/mutmut/badge/?version=latest
-            :target: https://mutmut.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://codecov.io/gh/boxed/mutmut/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/boxed/mutmut
-        
-        .. image:: https://img.shields.io/discord/767914934016802818.svg
-          :target: https://discord.gg/cwb9uNt
-        
-        Mutmut is a mutation testing system for Python, with a strong focus on ease
-        of use. If you don't know what mutation testing is try starting with
-        `this article <https://hackernoon.com/mutmut-a-python-mutation-testing-system-9b9639356c78>`_.
-        
-        Some highlight features:
-        
-        - Found mutants can be applied on disk with a simple command making it very
-          easy to work with the results
-        - Remembers work that has been done, so you can work incrementally
-        - Supports all test runners (because mutmut only needs an exit code from the
-          test command)
-        - If you use the `hammett <https://github.com/boxed/hammett>`_ test runner
-          you can go extremely fast! There's special handling for this runner
-          that has some pretty dramatic results.
-        - Can use coverage data to only do mutation testing on covered lines
-        - Battle tested on real libraries by multiple companies
-        
-        
-        If you need to run mutmut on a python 2 code base use mutmut ``1.5.0``. Mutmut
-        ``1.9.0`` is the last version to support python ``3.4``, ``3.5`` and ``3.6``.
-        
-        
-        Install and run
-        ---------------
-        
-        You can get started with a simple:
-        
-        .. code-block:: console
-        
-            pip install mutmut
-            mutmut run
-        
-        This will by default run pytest (or unittest if pytest is unavailable)
-        on tests in the "tests" or "test" folder and
-        it will try to figure out where the code to mutate lies.
-        
-        NOTE that mutmut will apply the mutations directly, one at a time;
-        it is **highly** recommended to add all changes to source control
-        before running.
-        
-        Enter
-        
-        .. code-block:: console
-        
-            mutmut run --help
-        
-        for the available flags, to use other runners, etc. The recommended way to use
-        mutmut if the defaults aren't working for you is to add a
-        block in ``setup.cfg`` or ``project.toml``.
-        Then when you come back to mutmut weeks later you don't have to figure out the
-        flags again, just run ``mutmut run`` and it works.
-        Like this in ``setup.cfg``:
-        
-        .. code-block:: ini
-        
-            [mutmut]
-            paths_to_mutate=src/
-            backup=False
-            runner=python -m hammett -x
-            tests_dir=tests/
-            dict_synonyms=Struct, NamedStruct
-        
-        or like this in ``pyproject.toml``:
-        
-        .. code-block:: ini
-        
-            [tool.mutmut]
-            paths_to_mutate="src"
-            runner="python -m hammett -x"
-        
-        To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
-        use a comma or colon separated list. For example:
-        
-        .. code-block:: ini
-        
-            [mutmut]
-            paths_to_mutate=src/,src2/
-            tests_dir=tests/:tests2/
-        
-        You can stop the mutation run at any time and mutmut will restart where you
-        left off. It's also smart enough to retest only the surviving mutants when the
-        test suite changes.
-        
-        To print the results run ``mutmut show``. It will give you a list of the mutants
-        grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
-        all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
-        with ``mutmut show all``.
-        
-        You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
-        have the file you mutate under source code control and committed before you apply
-        a mutant!
-        
-        To generate a HTML report for a web browser: ``mutmut html``
-        
-        Whitelisting
-        ------------
-        
-        You can mark lines like this:
-        
-        .. code-block:: python
-        
-            some_code_here()  # pragma: no mutate
-        
-        to stop mutation on those lines. Some cases we've found where you need to
-        whitelist lines are:
-        
-        - The version string on your library. You really shouldn't have a test for this :P
-        - Optimizing break instead of continue. The code runs fine when mutating break
-          to continue, but it's slower.
-        
-        See also `Advanced whitelisting and configuration`_
-        
-        
-        Example mutations
-        -----------------
-        
-        - Integer literals are changed by adding 1. So 0 becomes 1, 5 becomes 6, etc.
-        - ``<`` is changed to ``<=``
-        - break is changed to continue and vice versa
-        
-        In general the idea is that the mutations should be as subtle as possible.
-        See ``__init__.py`` for the full list.
-        
-        
-        Workflow
-        --------
-        
-        This section describes how to work with mutmut to enhance your test suite.
-        
-        1. Run mutmut with ``mutmut run``. A full run is preferred but if you're just
-           getting started you can exit in the middle and start working with what you
-           have found so far.
-        2. Show the mutants with ``mutmut results``
-        3. Apply a surviving mutant to disk running ``mutmut apply 3`` (replace 3 with
-           the relevant mutant ID from ``mutmut results``)
-        4. Write a new test that fails
-        5. Revert the mutant on disk
-        6. Rerun the new test to see that it now passes
-        7. Go back to point 2.
-        
-        Mutmut keeps a result cache in ``.mutmut-cache`` so if you want to make sure you
-        run a full mutmut run just delete this file.
-        
-        If you want to re-run all survivors after changing a lot of code or even the configuration,
-        you can use `for ID in $(mutmut result-ids survived); do mutmut run $ID; done` (for bash).
-        
-        You can also tell mutmut to just check a single mutant:
-        
-        .. code-block:: console
-        
-            mutmut run 3
-        
-        
-        Advanced whitelisting and configuration
-        ---------------------------------------
-        
-        mutmut has an advanced configuration system. You create a file called
-        ``mutmut_config.py``. You can define two functions there: ``init()`` and
-        ``pre_mutation(context)``. ``init`` gets called when mutmut starts and
-        ``pre_mutation`` gets called before each mutant is applied and tested. You can
-        mutate the ``context`` object as you need. You can modify the test command like
-        this:
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                context.config.test_command = 'python -m pytest -x ' + something_else
-        
-        or skip a mutant:
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                if context.filename == 'foo.py':
-                    context.skip = True
-        
-        or skip logging:
-        
-        
-        .. code-block:: python
-        
-            def pre_mutation(context):
-                line = context.current_source_line.strip()
-                if line.startswith('log.'):
-                    context.skip = True
-        
-        look at the code for the ``Context`` class for what you can modify. Please
-        open a github issue if you need help.
-        
-        It is also possible to disable mutation of specific node types by passing the
-        ``--disable-mutation-types`` option. Multiple types can be specified by separating them
-        by comma:
-        
-        .. code-block:: console
-        
-            mutmut run --disable-mutation-types=string,decorator
-        
-        Inversely, you can also only specify to only run specific mutations with ``--enable-mutation-types``.
-        Note that ``--disable-mutation-types`` and ``--enable-mutation-types`` are exclusive and cannot
-        be combined.
-        
-        
-        Selecting tests to run
-        ----------------------
-        
-        If you have a large test suite or long running tests, it can be beneficial to narrow the set of tests to
-        run for each mutant down to the tests that have a chance of killing it.
-        Determining the relevant subset of tests depends on your project, its structure, and the metadata that you
-        know about your tests.
-        ``mutmut`` provides information like the file to mutate and `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_
-        (if used with the ``--use-coverage`` switch).
-        You can set the ``context.config.test_command`` in the ``pre_mutation(context)`` hook of ``mutmut_config.py``.
-        The ``test_command`` is reset after each mutant, so you don't have to explicitly (re)set it for each mutant.
-        
-        This section gives examples to show how this could be done for some concrete use cases.
-        All examples use the default test runner (``python -m pytest -x --assert=plain``).
-        
-        Selection based on source and test layout
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If the location of the test module has a strict correlation with your source code layout, you can simply
-        construct the path to the corresponding test file from ``context.filename``.
-        Suppose your layout follows the following structure where the test file is always located right beside the
-        production code:
-        
-        .. code-block:: console
-        
-            mypackage
-            ├── production_module.py
-            ├── test_production_module.py
-            └── subpackage
-                ├── submodule.py
-                └── test_submodule.py
-        
-        Your ``mutmut_config.py`` in this case would look like this:
-        
-        .. code-block:: python
-        
-            import os.path
-        
-            def pre_mutation(context):
-                dirname, filename = os.path.split(context.filename)
-                testfile = "test_" + filename
-                context.config.test_command += ' ' + os.path.join(dirname, testfile)
-        
-        Selection based on imports
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If you can't rely on the directory structure or naming of the test files, you may assume that the tests most likely
-        to kill the mutant are located in test files that directly import the module that is affected by the mutant.
-        Using the ``ast`` module of the Python standard library, you can use the ``init()`` hook to build a map which test file
-        imports which module, and then lookup all test files importing the mutated module and only run those:
-        
-        .. code-block:: python
-        
-            import ast
-            from pathlib import Path
-        
-            test_imports = {}
-        
-        
-            class ImportVisitor(ast.NodeVisitor):
-                """Visitor which records which modules are imported."""
-                def __init__(self) -> None:
-                    super().__init__()
-                    self.imports = []
-        
-                def visit_Import(self, node: ast.Import) -> None:
-                    for alias in node.names:
-                        self.imports.append(alias.name)
-        
-                def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
-                    self.imports.append(node.module)
-        
-        
-            def init():
-                """Find all test files located under the 'tests' directory and create an abstract syntax tree for each.
-                Let the ``ImportVisitor`` find out what modules they import and store the information in a global dictionary
-                which can be accessed by ``pre_mutation(context)``."""
-                test_files = (Path(__file__).parent / "tests").rglob("test*.py")
-                for fpath in test_files:
-                    visitor = ImportVisitor()
-                    visitor.visit(ast.parse(fpath.read_bytes()))
-                    test_imports[str(fpath)] = visitor.imports
-        
-        
-            def pre_mutation(context):
-                """Construct the module name from the filename and run all test files which import that module."""
-                tests_to_run = []
-                for testfile, imports in test_imports.items():
-                    module_name = context.filename.rstrip(".py").replace("/", ".")
-                    if module_name in imports:
-                        tests_to_run.append(testfile)
-                context.config.test_command += f"{' '.join(tests_to_run)}"
-        
-        Selection based on coverage contexts
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If you recorded `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_ and use
-        the ``--use-coverage`` switch, you can access this coverage data inside the ``pre_mutation(context)`` hook
-        via the ``context.config.coverage_data`` attribute. This attribute is a dictionary in the form
-        ``{filename: {lineno: [contexts]}}``.
-        
-        Let's say you have used the built-in dynamic context option of ``Coverage.py`` by adding the following to
-        your ``.coveragerc`` file:
-        
-        .. code-block:: console
-        
-            [run]
-            dynamic_context = test_function
-        
-        ``coverage`` will create a new context for each test function that you run in the form ``module_name.function_name``.
-        With ``pytest``, we can use the ``-k`` switch to filter tests that match a given expression.
-        
-        .. code-block:: python
-        
-            import os.path
-        
-            def pre_mutation(context):
-                """Extract the coverage contexts if possible and only run the tests matching this data."""
-                if not context.config.coverage_data:
-                    # mutmut was run without ``--use-coverage``
-                    return
-                fname = os.path.abspath(context.filename)
-                contexts_for_file = context.config.coverage_data.get(fname, {})
-                contexts_for_line = contexts_for_file.get(context.current_line_index, [])
-                test_names = [
-                    ctx.rsplit(".", 1)[-1]  # extract only the final part after the last dot, which is the test function name
-                    for ctx in contexts_for_line
-                    if ctx  # skip empty strings
-                ]
-                if not test_names:
-                    return
-                context.config.test_command += f' -k "{" or ".join(test_names)}"'
-        
-        Pay attention that the format of the context name varies depending on the tool you use for creating the contexts.
-        For example, the ``pytest-cov`` plugin uses ``::`` as separator between module and test function.
-        Furthermore, not all tools are able to correctly pick up the correct contexts. ``coverage.py`` for instance is (at the time of writing)
-        unable to pick up tests that are inside a class when using ``pytest``.
-        You will have to inspect your ``.coverage`` database using the `Coverage.py API <https://coverage.readthedocs.io/en/coverage-5.5/api.html>`_
-        first to determine how you can extract the correct information to use with your test runner.
-        
-        Making things more robust
-        ^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        Despite your best efforts in picking the right subset of tests, it may happen that the mutant survives because the test which is able
-        to kill it was not included in the test set. You can tell ``mutmut`` to re-run the full test suite in that case, to verify that this
-        mutant indeed survives.
-        You can do so by passing the ``--rerun-all`` option to ``mutmut run``. This option is disabled by default.
-        
-        
-        JUnit XML support
-        -----------------
-        
-        In order to better integrate with CI/CD systems, ``mutmut`` supports the
-        generation of a JUnit XML report (using https://pypi.org/project/junit-xml/).
-        This option is available by calling ``mutmut junitxml``. In order to define how
-        to deal with suspicious and untested mutants, you can use
-        
-        .. code-block:: console
-        
-            mutmut junitxml --suspicious-policy=ignore --untested-policy=ignore
-        
-        The possible values for these policies are:
-        
-        - ``ignore``: Do not include the results on the report at all
-        - ``skipped``: Include the mutant on the report as "skipped"
-        - ``error``: Include the mutant on the report as "error"
-        - ``failure``: Include the mutant on the report as "failure"
-        
-        If a failed mutant is included in the report, then the unified diff of the
-        mutant will also be included for debugging purposes.
-        
 Keywords: mutmut mutant mutation test testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: glob2
+Requires-Dist: parso
+Requires-Dist: click
+Requires-Dist: pony
+Requires-Dist: junit-xml<2,>=1.8
+Requires-Dist: toml
 Provides-Extra: pytest
+Requires-Dist: pytest; extra == "pytest"
+Requires-Dist: pytest-cov; extra == "pytest"
 Provides-Extra: coverage
+Requires-Dist: coverage; extra == "coverage"
 Provides-Extra: patch
+Requires-Dist: whatthepatch==0.0.6; extra == "patch"
+
+mutmut - python mutation tester
+===============================
+
+.. image:: https://travis-ci.org/boxed/mutmut.svg?branch=master
+    :target: https://travis-ci.org/boxed/mutmut
+
+.. image:: https://readthedocs.org/projects/mutmut/badge/?version=latest
+    :target: https://mutmut.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://codecov.io/gh/boxed/mutmut/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/boxed/mutmut
+
+.. image:: https://img.shields.io/discord/767914934016802818.svg
+  :target: https://discord.gg/cwb9uNt
+
+Mutmut is a mutation testing system for Python, with a strong focus on ease
+of use. If you don't know what mutation testing is try starting with
+`this article <https://hackernoon.com/mutmut-a-python-mutation-testing-system-9b9639356c78>`_.
+
+Some highlight features:
+
+- Found mutants can be applied on disk with a simple command making it very
+  easy to work with the results
+- Remembers work that has been done, so you can work incrementally
+- Supports all test runners (because mutmut only needs an exit code from the
+  test command)
+- If you use the `hammett <https://github.com/boxed/hammett>`_ test runner
+  you can go extremely fast! There's special handling for this runner
+  that has some pretty dramatic results.
+- Can use coverage data to only do mutation testing on covered lines
+- Battle tested on real libraries by multiple companies
+
+
+If you need to run mutmut on a python 2 code base use mutmut ``1.5.0``. Mutmut
+``1.9.0`` is the last version to support python ``3.4``, ``3.5`` and ``3.6``.
+
+
+Install and run
+---------------
+
+You can get started with a simple:
+
+.. code-block:: console
+
+    pip install mutmut
+    mutmut run
+
+This will by default run pytest (or unittest if pytest is unavailable)
+on tests in the "tests" or "test" folder and
+it will try to figure out where the code to mutate lies.
+
+NOTE that mutmut will apply the mutations directly, one at a time;
+it is **highly** recommended to add all changes to source control
+before running.
+
+Enter
+
+.. code-block:: console
+
+    mutmut run --help
+
+for the available flags, to use other runners, etc. The recommended way to use
+mutmut if the defaults aren't working for you is to add a
+block in ``setup.cfg`` or ``project.toml``.
+Then when you come back to mutmut weeks later you don't have to figure out the
+flags again, just run ``mutmut run`` and it works.
+Like this in ``setup.cfg``:
+
+.. code-block:: ini
+
+    [mutmut]
+    paths_to_mutate=src/
+    backup=False
+    runner=python -m hammett -x
+    tests_dir=tests/
+    dict_synonyms=Struct, NamedStruct
+
+or like this in ``pyproject.toml``:
+
+.. code-block:: ini
+
+    [tool.mutmut]
+    paths_to_mutate="src"
+    runner="python -m hammett -x"
+
+To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
+use a comma or colon separated list. For example:
+
+.. code-block:: ini
+
+    [mutmut]
+    paths_to_mutate=src/,src2/
+    tests_dir=tests/:tests2/
+
+You can stop the mutation run at any time and mutmut will restart where you
+left off. It's also smart enough to retest only the surviving mutants when the
+test suite changes.
+
+To print the results run ``mutmut show``. It will give you a list of the mutants
+grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
+all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
+with ``mutmut show all``.
+
+You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
+have the file you mutate under source code control and committed before you apply
+a mutant!
+
+To generate a HTML report for a web browser: ``mutmut html``
+
+Whitelisting
+------------
+
+You can mark lines like this:
+
+.. code-block:: python
+
+    some_code_here()  # pragma: no mutate
+
+to stop mutation on those lines. Some cases we've found where you need to
+whitelist lines are:
+
+- The version string on your library. You really shouldn't have a test for this :P
+- Optimizing break instead of continue. The code runs fine when mutating break
+  to continue, but it's slower.
+
+See also `Advanced whitelisting and configuration`_
+
+
+Example mutations
+-----------------
+
+- Integer literals are changed by adding 1. So 0 becomes 1, 5 becomes 6, etc.
+- ``<`` is changed to ``<=``
+- break is changed to continue and vice versa
+
+In general the idea is that the mutations should be as subtle as possible.
+See ``__init__.py`` for the full list.
+
+
+Workflow
+--------
+
+This section describes how to work with mutmut to enhance your test suite.
+
+1. Run mutmut with ``mutmut run``. A full run is preferred but if you're just
+   getting started you can exit in the middle and start working with what you
+   have found so far.
+2. Show the mutants with ``mutmut results``
+3. Apply a surviving mutant to disk running ``mutmut apply 3`` (replace 3 with
+   the relevant mutant ID from ``mutmut results``)
+4. Write a new test that fails
+5. Revert the mutant on disk
+6. Rerun the new test to see that it now passes
+7. Go back to point 2.
+
+Mutmut keeps a result cache in ``.mutmut-cache`` so if you want to make sure you
+run a full mutmut run just delete this file.
+
+If you want to re-run all survivors after changing a lot of code or even the configuration,
+you can use `for ID in $(mutmut result-ids survived); do mutmut run $ID; done` (for bash).
+
+You can also tell mutmut to just check a single mutant:
+
+.. code-block:: console
+
+    mutmut run 3
+
+
+Advanced whitelisting and configuration
+---------------------------------------
+
+mutmut has an advanced configuration system. You create a file called
+``mutmut_config.py``. You can define two functions there: ``init()`` and
+``pre_mutation(context)``. ``init`` gets called when mutmut starts and
+``pre_mutation`` gets called before each mutant is applied and tested. You can
+mutate the ``context`` object as you need. You can modify the test command like
+this:
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        context.config.test_command = 'python -m pytest -x ' + something_else
+
+or skip a mutant:
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        if context.filename == 'foo.py':
+            context.skip = True
+
+or skip logging:
+
+
+.. code-block:: python
+
+    def pre_mutation(context):
+        line = context.current_source_line.strip()
+        if line.startswith('log.'):
+            context.skip = True
+
+look at the code for the ``Context`` class for what you can modify. Please
+open a github issue if you need help.
+
+It is also possible to disable mutation of specific node types by passing the
+``--disable-mutation-types`` option. Multiple types can be specified by separating them
+by comma:
+
+.. code-block:: console
+
+    mutmut run --disable-mutation-types=string,decorator
+
+Inversely, you can also only specify to only run specific mutations with ``--enable-mutation-types``.
+Note that ``--disable-mutation-types`` and ``--enable-mutation-types`` are exclusive and cannot
+be combined.
+
+Changes made to ``mutmut_config.py`` does not invalidate the cache.
+If you modify the configuration file, you will likely need to remove ``.mutmut-cache`` manually to ensure that the changes take effect.
+
+Selecting tests to run
+----------------------
+
+If you have a large test suite or long running tests, it can be beneficial to narrow the set of tests to
+run for each mutant down to the tests that have a chance of killing it.
+Determining the relevant subset of tests depends on your project, its structure, and the metadata that you
+know about your tests.
+``mutmut`` provides information like the file to mutate and `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_
+(if used with the ``--use-coverage`` switch).
+You can set the ``context.config.test_command`` in the ``pre_mutation(context)`` hook of ``mutmut_config.py``.
+The ``test_command`` is reset after each mutant, so you don't have to explicitly (re)set it for each mutant.
+
+This section gives examples to show how this could be done for some concrete use cases.
+All examples use the default test runner (``python -m pytest -x --assert=plain``).
+
+Selection based on source and test layout
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If the location of the test module has a strict correlation with your source code layout, you can simply
+construct the path to the corresponding test file from ``context.filename``.
+Suppose your layout follows the following structure where the test file is always located right beside the
+production code:
+
+.. code-block:: console
+
+    mypackage
+    ├── production_module.py
+    ├── test_production_module.py
+    └── subpackage
+        ├── submodule.py
+        └── test_submodule.py
+
+Your ``mutmut_config.py`` in this case would look like this:
+
+.. code-block:: python
+
+    import os.path
+
+    def pre_mutation(context):
+        dirname, filename = os.path.split(context.filename)
+        testfile = "test_" + filename
+        context.config.test_command += ' ' + os.path.join(dirname, testfile)
+
+Selection based on imports
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you can't rely on the directory structure or naming of the test files, you may assume that the tests most likely
+to kill the mutant are located in test files that directly import the module that is affected by the mutant.
+Using the ``ast`` module of the Python standard library, you can use the ``init()`` hook to build a map which test file
+imports which module, and then lookup all test files importing the mutated module and only run those:
+
+.. code-block:: python
+
+    import ast
+    from pathlib import Path
+
+    test_imports = {}
+
+
+    class ImportVisitor(ast.NodeVisitor):
+        """Visitor which records which modules are imported."""
+        def __init__(self) -> None:
+            super().__init__()
+            self.imports = []
+
+        def visit_Import(self, node: ast.Import) -> None:
+            for alias in node.names:
+                self.imports.append(alias.name)
+
+        def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
+            self.imports.append(node.module)
+
+
+    def init():
+        """Find all test files located under the 'tests' directory and create an abstract syntax tree for each.
+        Let the ``ImportVisitor`` find out what modules they import and store the information in a global dictionary
+        which can be accessed by ``pre_mutation(context)``."""
+        test_files = (Path(__file__).parent / "tests").rglob("test*.py")
+        for fpath in test_files:
+            visitor = ImportVisitor()
+            visitor.visit(ast.parse(fpath.read_bytes()))
+            test_imports[str(fpath)] = visitor.imports
+
+
+    def pre_mutation(context):
+        """Construct the module name from the filename and run all test files which import that module."""
+        tests_to_run = []
+        for testfile, imports in test_imports.items():
+            module_name = context.filename.rstrip(".py").replace("/", ".")
+            if module_name in imports:
+                tests_to_run.append(testfile)
+        context.config.test_command += f"{' '.join(tests_to_run)}"
+
+Selection based on coverage contexts
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you recorded `coverage contexts <https://coverage.readthedocs.io/en/coverage-5.5/contexts.html>`_ and use
+the ``--use-coverage`` switch, you can access this coverage data inside the ``pre_mutation(context)`` hook
+via the ``context.config.coverage_data`` attribute. This attribute is a dictionary in the form
+``{filename: {lineno: [contexts]}}``.
+
+Let's say you have used the built-in dynamic context option of ``Coverage.py`` by adding the following to
+your ``.coveragerc`` file:
+
+.. code-block:: console
+
+    [run]
+    dynamic_context = test_function
+
+``coverage`` will create a new context for each test function that you run in the form ``module_name.function_name``.
+With ``pytest``, we can use the ``-k`` switch to filter tests that match a given expression.
+
+.. code-block:: python
+
+    import os.path
+
+    def pre_mutation(context):
+        """Extract the coverage contexts if possible and only run the tests matching this data."""
+        if not context.config.coverage_data:
+            # mutmut was run without ``--use-coverage``
+            return
+        fname = os.path.abspath(context.filename)
+        contexts_for_file = context.config.coverage_data.get(fname, {})
+        contexts_for_line = contexts_for_file.get(context.current_line_index, [])
+        test_names = [
+            ctx.rsplit(".", 1)[-1]  # extract only the final part after the last dot, which is the test function name
+            for ctx in contexts_for_line
+            if ctx  # skip empty strings
+        ]
+        if not test_names:
+            return
+        context.config.test_command += f' -k "{" or ".join(test_names)}"'
+
+Pay attention that the format of the context name varies depending on the tool you use for creating the contexts.
+For example, the ``pytest-cov`` plugin uses ``::`` as separator between module and test function.
+Furthermore, not all tools are able to correctly pick up the correct contexts. ``coverage.py`` for instance is (at the time of writing)
+unable to pick up tests that are inside a class when using ``pytest``.
+You will have to inspect your ``.coverage`` database using the `Coverage.py API <https://coverage.readthedocs.io/en/coverage-5.5/api.html>`_
+first to determine how you can extract the correct information to use with your test runner.
+
+Making things more robust
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Despite your best efforts in picking the right subset of tests, it may happen that the mutant survives because the test which is able
+to kill it was not included in the test set. You can tell ``mutmut`` to re-run the full test suite in that case, to verify that this
+mutant indeed survives.
+You can do so by passing the ``--rerun-all`` option to ``mutmut run``. This option is disabled by default.
+
+
+JUnit XML support
+-----------------
+
+In order to better integrate with CI/CD systems, ``mutmut`` supports the
+generation of a JUnit XML report (using https://pypi.org/project/junit-xml/).
+This option is available by calling ``mutmut junitxml``. In order to define how
+to deal with suspicious and untested mutants, you can use
+
+.. code-block:: console
+
+    mutmut junitxml --suspicious-policy=ignore --untested-policy=ignore
+
+The possible values for these policies are:
+
+- ``ignore``: Do not include the results on the report at all
+- ``skipped``: Include the mutant on the report as "skipped"
+- ``error``: Include the mutant on the report as "error"
+- ``failure``: Include the mutant on the report as "failure"
+
+If a failed mutant is included in the report, then the unified diff of the
+mutant will also be included for debugging purposes.
```

### Comparing `mutmut-2.4.5/setup.py` & `mutmut-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `mutmut-2.4.5/tests/test_cache.py` & `mutmut-2.5.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `mutmut-2.4.5/tests/test_init.py` & `mutmut-2.5.0/tests/test_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import os
 from pathlib import Path
 from time import sleep
 from pytest import raises, fixture
 from unittest.mock import MagicMock, patch
 
 from mutmut import (
     partition_node_list,
@@ -135,14 +136,26 @@
 
     # act
     file_changes = read_patch_data(file_patch)
 
     # assert
     assert file_name in file_changes
     assert file_changes[file_name] == {2} # line is added between 2nd and 3rd
+
+def test_read_patch_data_edited_line_in_subfolder_is_in_the_list(testpatches_path: Path):
+    # arrange
+    file_name = os.path.join("sub", "existing_file.txt") # unix will use "/", windows "\" to join
+    file_patch = testpatches_path / "edit_existing_line_in_subfolder.patch"
+
+    # act
+    file_changes = read_patch_data(file_patch)
+
+    # assert
+    assert file_name in file_changes
+    assert file_changes[file_name] == {2} # line is added between 2nd and 3rd
 
 def test_read_patch_data_renamed_file_edited_line_is_in_the_list(testpatches_path: Path):
     # arrange
     original_file_name = "existing_file.txt"
     new_file_name = "renamed_existing_file.txt"
     file_patch = testpatches_path / "edit_existing_renamed_file_line.patch"
```

### Comparing `mutmut-2.4.5/tests/test_main.py` & `mutmut-2.5.0/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,7 +700,20 @@
     with open("html/index.html") as f:
         assert f.read() == (
             '<h1>Mutation testing report</h1>'
             'Killed 0 out of 2 mutants'
             '<table><thead><tr><th>File</th><th>Total</th><th>Skipped</th><th>Killed</th><th>% killed</th><th>Survived</th></thead>'
             '<tr><td><a href="foo.py.html">foo.py</a></td><td>2</td><td>0</td><td>0</td><td>0.00</td><td>2</td>'
             '</table></body></html>')
+        
+def test_html_custom_output(surviving_mutants_filesystem):
+    result = CliRunner().invoke(climain, ['run', '--paths-to-mutate=foo.py', "--test-time-base=15.0"], catch_exceptions=False)
+    print(repr(result.output))
+    result = CliRunner().invoke(climain, ['html', '--directory', 'htmlmut'])
+    assert os.path.isfile("htmlmut/index.html")
+    with open("htmlmut/index.html") as f:
+        assert f.read() == (
+            '<h1>Mutation testing report</h1>'
+            'Killed 0 out of 2 mutants'
+            '<table><thead><tr><th>File</th><th>Total</th><th>Skipped</th><th>Killed</th><th>% killed</th><th>Survived</th></thead>'
+            '<tr><td><a href="foo.py.html">foo.py</a></td><td>2</td><td>0</td><td>0</td><td>0.00</td><td>2</td>'
+            '</table></body></html>')
```

### Comparing `mutmut-2.4.5/tests/test_mutation.py` & `mutmut-2.5.0/tests/test_mutation.py`

 * *Files identical despite different names*

