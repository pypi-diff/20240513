# Comparing `tmp/RepoAuditor-0.1.6-py3-none-any.whl.zip` & `tmp/RepoAuditor-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,22 @@
-Zip file size: 14269 bytes, number of entries: 15
--rw-r--r--  2.0 unx     3592 b- defN 24-May-10 20:04 BuildBinary.py
--rw-r--r--  2.0 unx     1912 b- defN 24-May-10 20:04 RepoAuditor/EntryPoint.py
--rw-r--r--  2.0 unx    11014 b- defN 24-May-10 20:04 RepoAuditor/ExecuteModules.py
--rw-r--r--  2.0 unx     7539 b- defN 24-May-10 20:04 RepoAuditor/Module.py
--rw-r--r--  2.0 unx     4984 b- defN 24-May-10 20:04 RepoAuditor/Query.py
--rw-r--r--  2.0 unx     3363 b- defN 24-May-10 20:04 RepoAuditor/Requirement.py
--rw-r--r--  2.0 unx      600 b- defN 24-May-10 20:04 RepoAuditor/__init__.py
--rw-r--r--  2.0 unx     4511 b- defN 24-May-10 20:04 RepoAuditor/Impl/ParallelSequentialProcessor.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 20:04 RepoAuditor/Impl/__init__.py
--rw-r--r--  2.0 unx     1132 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2104 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1252 b- defN 24-May-10 20:05 RepoAuditor-0.1.6.dist-info/RECORD
-15 files, 42178 bytes uncompressed, 12187 bytes compressed:  71.1%
+Zip file size: 19725 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     3592 b- defN 24-May-13 17:08 BuildBinary.py
+-rw-r--r--  2.0 unx     5745 b- defN 24-May-13 17:08 RepoAuditor/CommandLineProcessor.py
+-rw-r--r--  2.0 unx     7706 b- defN 24-May-13 17:08 RepoAuditor/EntryPoint.py
+-rw-r--r--  2.0 unx    11014 b- defN 24-May-13 17:08 RepoAuditor/ExecuteModules.py
+-rw-r--r--  2.0 unx     7539 b- defN 24-May-13 17:08 RepoAuditor/Module.py
+-rw-r--r--  2.0 unx      860 b- defN 24-May-13 17:08 RepoAuditor/Plugin.py
+-rw-r--r--  2.0 unx     4984 b- defN 24-May-13 17:08 RepoAuditor/Query.py
+-rw-r--r--  2.0 unx     3363 b- defN 24-May-13 17:08 RepoAuditor/Requirement.py
+-rw-r--r--  2.0 unx      626 b- defN 24-May-13 17:08 RepoAuditor/__init__.py
+-rw-r--r--  2.0 unx     4511 b- defN 24-May-13 17:08 RepoAuditor/Impl/ParallelSequentialProcessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 17:08 RepoAuditor/Impl/__init__.py
+-rw-r--r--  2.0 unx     3657 b- defN 24-May-13 17:08 RepoAuditor/Plugins/Plugin1.py
+-rw-r--r--  2.0 unx     1896 b- defN 24-May-13 17:08 RepoAuditor/Plugins/Plugin2.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-13 17:08 RepoAuditor/Plugins/__init__.py
+-rw-r--r--  2.0 unx     1132 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2104 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      150 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1681 b- defN 24-May-13 17:08 RepoAuditor-0.1.7.dist-info/RECORD
+20 files, 60676 bytes uncompressed, 16969 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: BuildBinary.py
 Comment: 
 
+Filename: RepoAuditor/CommandLineProcessor.py
+Comment: 
+
 Filename: RepoAuditor/EntryPoint.py
 Comment: 
 
 Filename: RepoAuditor/ExecuteModules.py
 Comment: 
 
 Filename: RepoAuditor/Module.py
 Comment: 
 
+Filename: RepoAuditor/Plugin.py
+Comment: 
+
 Filename: RepoAuditor/Query.py
 Comment: 
 
 Filename: RepoAuditor/Requirement.py
 Comment: 
 
 Filename: RepoAuditor/__init__.py
@@ -21,26 +27,35 @@
 
 Filename: RepoAuditor/Impl/ParallelSequentialProcessor.py
 Comment: 
 
 Filename: RepoAuditor/Impl/__init__.py
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/LICENSE.txt
+Filename: RepoAuditor/Plugins/Plugin1.py
+Comment: 
+
+Filename: RepoAuditor/Plugins/Plugin2.py
+Comment: 
+
+Filename: RepoAuditor/Plugins/__init__.py
+Comment: 
+
+Filename: RepoAuditor-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/METADATA
+Filename: RepoAuditor-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/WHEEL
+Filename: RepoAuditor-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/entry_points.txt
+Filename: RepoAuditor-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/top_level.txt
+Filename: RepoAuditor-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: RepoAuditor-0.1.6.dist-info/RECORD
+Filename: RepoAuditor-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RepoAuditor/EntryPoint.py

```diff
@@ -3,20 +3,34 @@
 # |  Copyright (c) 2024 Scientific Software Engineering Center at Georgia Tech
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """This file serves as an example of how to create scripts that can be invoked from the command line once the package is installed."""
 
 import sys
+import textwrap
 
+from typing import Annotated
+
+import pluggy
 import typer
 
+from click.exceptions import UsageError
+from dbrownell_Common.Streams.DoneManager import DoneManager, Flags as DoneManagerFlags  # type: ignore [import-untyped]
+from dbrownell_Common import TextwrapEx  # type: ignore [import-untyped]
+from dbrownell_Common import TyperEx  # type: ignore [import-untyped]
 from typer.core import TyperGroup  # type: ignore [import-untyped]
 
-from RepoAuditor import __version__
+from RepoAuditor import APP_NAME, __version__
+from RepoAuditor.CommandLineProcessor import CommandLineProcessor, Module
+from RepoAuditor import Plugin
+
+
+# ----------------------------------------------------------------------
+ARGUMENT_SEPARATOR = "-"
 
 
 # ----------------------------------------------------------------------
 class NaturalOrderGrouper(TyperGroup):
     # pylint: disable=missing-class-docstring
     # ----------------------------------------------------------------------
     def list_commands(self, *args, **kwargs):  # pylint: disable=unused-argument
@@ -30,26 +44,190 @@
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     pretty_exceptions_enable=False,
 )
 
 
 # ----------------------------------------------------------------------
-@app.command("Placeholder")
-def Placeholder() -> None:
-    """This is a placeholder command that should be removed once actual functionality is added."""
-    pass
+def _GetModules() -> list[Module]:
+    plugin_manager = pluggy.PluginManager(APP_NAME)
 
+    plugin_manager.add_hookspecs(Plugin)
+    plugin_manager.load_setuptools_entrypoints(APP_NAME)
 
-# ----------------------------------------------------------------------
-@app.command("Version")
-def Version() -> None:
-    """Prints the version of the package."""
+    return plugin_manager.hook.GetModule()
+
+
+_all_modules = _GetModules()
+del _GetModules
+
+
+# ----------------------------------------------------------------------
+def _HelpEpilog() -> str:
+    content: list[str] = []
+
+    for module in _all_modules:
+        arguments: list[str] = []
+
+        for arg_name, type_info in module.GetDynamicArgDefinitions().items():
+            if isinstance(type_info, TyperEx.TypeDefinitionItem):
+                python_type = type_info.python_type
+                parameter_info = type_info.parameter_info
+            elif isinstance(type_info, tuple):
+                python_type = type_info[0]
+                parameter_info = type_info[1]
+            else:
+                python_type = type_info
+                parameter_info = None
+
+            arguments.append(
+                "    {arg_name:<32} {type_description:<8} {help}".format(
+                    arg_name=f"--{module.name}{ARGUMENT_SEPARATOR}{arg_name}",
+                    type_description=python_type.__name__,
+                    help="" if parameter_info is None else parameter_info.help,
+                ),
+            )
+
+        final_arguments = TextwrapEx.Indent(
+            "\n".join(arguments),
+            4,
+            skip_first_line=True,
+        )
+
+        content.append(
+            textwrap.dedent(
+                f"""\
+                {module.name}
+                {"-" * len(module.name)}
+                {module.description}
+
+                Command Line Arguments:
+                    {final_arguments}
+                """,
+            ),
+        )
+
+    return (
+        textwrap.dedent(
+            """\
+        Module Information
+        ==================
+
+        {}
+        """,
+        )
+        .format(
+            "\n".join(content),
+        )
+        .replace("\n", "\n\n")
+    )
+
+
+# ----------------------------------------------------------------------
+def _VersionCallback(value: bool) -> None:
+    if value:
+        sys.stdout.write(f"RepoAuditor v{__version__}\n")
+        raise typer.Exit()
+
+
+# ----------------------------------------------------------------------
+@app.command(
+    "EntryPoint",
+    context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
+    help=__doc__,
+    epilog=_HelpEpilog(),
+    no_args_is_help=False,
+)
+def EntryPoint(
+    ctx: typer.Context,
+    version: Annotated[  # pylint: disable=unused-argument
+        bool,
+        typer.Option(
+            "--version",
+            help="Display the version of this tool and exit.",
+            callback=_VersionCallback,
+            is_eager=True,
+        ),
+    ] = False,
+    excludes: Annotated[
+        list[str],
+        typer.Option(
+            "--exclude",
+            help=f"Module or requirement names to exclude from execution; like other command line arguments, requirement names must include the module name as a prefix (e.g. 'ModuleName{ARGUMENT_SEPARATOR}RequirementName'). This value can be provided multiple times.",
+        ),
+    ] = [],
+    warnings_as_error: Annotated[
+        list[str],
+        typer.Option(
+            "--warnings-as-error",
+            help="Name of a module whose warnings should be treated as errors. This value can be provided multiple times.",
+        ),
+    ] = [],
+    ignore_warnings: Annotated[
+        list[str],
+        typer.Option(
+            "--ignore-warnings",
+            help="Name of a module whose warnings should be ignored. This value can be provided multiple times.",
+        ),
+    ] = [],
+    all_warnings_as_error: Annotated[
+        bool, typer.Option("--all-warnings-as-error", help="Treat all warnings as errors.")
+    ] = False,
+    ignore_all_warnings: Annotated[
+        bool, typer.Option("--ignore-all-warnings", help="Ignore all warnings.")
+    ] = False,
+    single_threaded: Annotated[
+        bool,
+        typer.Option(
+            "--single-threaded", help="Do not use multiple threads when evaluating requirements."
+        ),
+    ] = False,
+    verbose: Annotated[
+        bool,
+        typer.Option(
+            "--verbose",
+            help="Write verbose information to the terminal.",
+        ),
+    ] = False,
+    debug: Annotated[
+        bool,
+        typer.Option(
+            "--debug",
+            help="Write debug information to the terminal.",
+        ),
+    ] = False,
+) -> None:
+    with DoneManager.CreateCommandLine(
+        sys.stdout,
+        flags=DoneManagerFlags.Create(verbose=verbose, debug=debug),
+    ) as dm:
+        try:
+            executor = CommandLineProcessor.Create(
+                lambda dynamic_arg_definitions: TyperEx.ProcessDynamicArgs(
+                    ctx, dynamic_arg_definitions
+                ),
+                _all_modules,
+                excludes,
+                set(warnings_as_error),
+                set(ignore_warnings),
+                all_warnings_as_error=all_warnings_as_error,
+                ignore_all_warnings=ignore_all_warnings,
+                single_threaded=single_threaded,
+                argument_separator=ARGUMENT_SEPARATOR,
+            )
+
+        except Exception as ex:
+            if dm.is_debug:
+                raise
+
+            raise UsageError(str(ex)) from ex
+
+        dm.WriteLine("")
 
-    sys.stdout.write(__version__)
+        executor(dm)
 
 
 # ----------------------------------------------------------------------
 # ----------------------------------------------------------------------
 # ----------------------------------------------------------------------
 if __name__ == "__main__":
     app()  # pragma: no cover
```

## RepoAuditor/__init__.py

```diff
@@ -2,11 +2,13 @@
 # |
 # |  Copyright (c) 2024 Scientific Software Engineering Center at Georgia Tech
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
+APP_NAME = "RepoAuditor"
+
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

## Comparing `RepoAuditor-0.1.6.dist-info/LICENSE.txt` & `RepoAuditor-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `RepoAuditor-0.1.6.dist-info/METADATA` & `RepoAuditor-0.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepoAuditor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Audits repositories for best practices.
 Author-email: Scientific Software Engineering Center at Georgia Tech <sse-center@gatech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Documentation, https://github.com/gt-sse-center/RepoAuditor
 Project-URL: Repository, https://github.com/gt-sse-center/RepoAuditor
 Classifier: License :: OSI Approved :: MIT License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.6 Summary: Audits
+Metadata-Version: 2.1 Name: RepoAuditor Version: 0.1.7 Summary: Audits
 repositories for best practices. Author-email: Scientific Software Engineering
 Center at Georgia Tech
 gatech.edu> License: MIT Project-URL: Homepage, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Documentation, https://github.com/gt-sse-
 center/RepoAuditor Project-URL: Repository, https://github.com/gt-sse-center/
 RepoAuditor Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
```

