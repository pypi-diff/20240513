# Comparing `tmp/alliance_platform_codegen-0.0.3.tar.gz` & `tmp/alliance_platform_codegen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_codegen-0.0.3.tar", last modified: Wed Apr 10 05:18:09 2024, max compression
+gzip compressed data, was "alliance_platform_codegen-0.0.4.tar", last modified: Mon May 13 01:20:57 2024, max compression
```

## Comparing `alliance_platform_codegen-0.0.3.tar` & `alliance_platform_codegen-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/__init__.py
--rw-r--r--   0        0        0      351 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/apps.py
--rw-r--r--   0        0        0        0 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/post_processors/__init__.py
--rw-r--r--   0        0        0     3587 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/post_processors/js.py
--rw-r--r--   0        0        0    15716 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/printer.py
--rw-r--r--   0        0        0        0 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/py.typed
--rw-r--r--   0        0        0     6352 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/registry.py
--rw-r--r--   0        0        0     1389 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/settings.py
--rw-r--r--   0        0        0    18618 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/alliance_platform/codegen/typescript.py
--rw-r--r--   0        0        0      848 2024-04-10 05:18:09.437297 alliance_platform_codegen-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    14091 2024-04-10 05:17:36.341254 alliance_platform_codegen-0.0.3/tests/test_printer.py
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 alliance_platform_codegen-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/apps.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/post_processors/__init__.py
+-rw-r--r--   0        0        0     3587 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/post_processors/js.py
+-rw-r--r--   0        0        0    24745 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/printer.py
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/py.typed
+-rw-r--r--   0        0        0     7971 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/registry.py
+-rw-r--r--   0        0        0     1389 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/settings.py
+-rw-r--r--   0        0        0    19400 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/alliance_platform/codegen/typescript.py
+-rw-r--r--   0        0        0      848 2024-05-13 01:20:56.979145 alliance_platform_codegen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    21941 2024-05-13 01:20:27.951018 alliance_platform_codegen-0.0.4/tests/test_printer.py
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 alliance_platform_codegen-0.0.4/PKG-INFO
```

### Comparing `alliance_platform_codegen-0.0.3/alliance_platform/codegen/post_processors/js.py` & `alliance_platform_codegen-0.0.4/alliance_platform/codegen/post_processors/js.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.3/alliance_platform/codegen/printer.py` & `alliance_platform_codegen-0.0.4/alliance_platform/codegen/printer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+import dataclasses
+from functools import wraps
 import json
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Callable
+from typing import Sequence
 
 from django.conf import settings
+from django.utils.html import escape
 
 from .settings import ap_codegen_settings
-
-# from codegen.presto.config import CodeGenFile
-# from codegen.presto.get_config import get_codegen_config
 from .typescript import ArrayLiteralExpression
 from .typescript import ArrowFunction
 from .typescript import AsExpression
 from .typescript import AsyncKeyword
 from .typescript import Block
 from .typescript import BooleanLiteral
 from .typescript import CallExpression
 from .typescript import ElementAccessExpression
 from .typescript import ExportKeyword
 from .typescript import FunctionDeclaration
 from .typescript import Identifier
 from .typescript import ImportDeclaration
 from .typescript import ImportDefaultSpecifier
 from .typescript import ImportSpecifier
+from .typescript import JsxAttribute
+from .typescript import JsxElement
+from .typescript import JsxExpression
+from .typescript import JsxText
 from .typescript import Modifier
+from .typescript import MultiLineComment
 from .typescript import NewExpression
 from .typescript import Node
 from .typescript import NodeLike
 from .typescript import NullKeyword
 from .typescript import NumericLiteral
 from .typescript import ObjectLiteralExpression
 from .typescript import ObjectProperty
@@ -45,37 +51,210 @@
 
 # Useful reference: https://babeljs.io/docs/en/babel-types
 
 
 # TODO: Should add a base Printer and TypescriptSourceFileWriter class
 
 
+def push_node_stack(method):
+    """Pushes a node onto the node stack before calling the method and pops it after.
+
+    This is done as a decorator to avoid needing to wrap and indent the entire ``print`` method which is already
+    very large.
+    """
+
+    @wraps(method)
+    def wrapper(self: "TypescriptPrinter", node: NodeLike, *args, **kwargs):
+        self.node_stack.append(node)
+        try:
+            result = method(self, node, *args, **kwargs)
+        finally:
+            self.node_stack.pop()
+        return result
+
+    return wrapper
+
+
+def print_comments(method):
+    """For any node that has leading or trailing comments print them out before or after the node code.
+
+    Intended to decorate the ``print`` method on ``TypescriptPrinter``. This is a decorator to avoid needing to
+    concatenate strings within ``print`` which is already very large. Comments are a special case in that they
+    apply generically to many nodes.
+    """
+
+    @wraps(method)
+    def wrapper(self: "TypescriptPrinter", node: NodeLike, *args, **kwargs):
+        result = method(self, node, *args, **kwargs)
+        if isinstance(node, Node) and (not isinstance(node, JsxElement) or not self.jsx_transform):
+            if node.leading_comments:
+                result = self._print_comments(node.leading_comments) + "\n" + result
+                if self.parent_node():
+                    result = "\n" + result
+            if node.trailing_comments:
+                result = result + "\n" + self._print_comments(node.trailing_comments)
+                if len(self.node_stack) > 1:
+                    # Only do this if not the root node
+                    result += "\n"
+        return result
+
+    return wrapper
+
+
+default_jsx_transform = PropertyAccessExpression(
+    Identifier("React"),
+    Identifier("createElement"),
+)
+
+
 class TypescriptPrinter:
     """Print out code for the specified node
 
     NOTE: This does not generate nicely formatted code - it's expected the code will be passed through prettier.
     """
 
     #: Path any imports are relative to. Only used if a :class:`~pathlib.Path` is received - if a string is encountered it used directly
     relative_to_path: Path
     #: Function used to resolve the URL to use for an import. This can be used to do things like resolve it to a dev server URL or to a built file. If not provided import source is used as is.
     resolve_import_url: Callable[[Path | str], str] | None
+    #: How to treat JSX elements. If specified, JSX elements will be transformed to the equivalent of ``React.createElement`` calls.
+    #: The specific function called is identified by ``jsx_transform``, but the relevant import must be added manually.
+    jsx_transform: Node | None
+    #: Current node stack for printing. As each node is printed it is pushed onto this stack. This can be used to determine the parent node of the current node.
+    node_stack: list[NodeLike]
 
     def __init__(
         self,
         relative_to_path: Path | None = None,
         resolve_import_url: Callable[[Path | str], str] | None = None,
+        jsx_transform: Node | None = default_jsx_transform,
     ):
         if relative_to_path is None:
             relative_to_path = ap_codegen_settings.JS_ROOT_DIR
         self.relative_to_path = relative_to_path.parent if relative_to_path.is_file() else relative_to_path
         self.resolve_import_url = resolve_import_url
+        self.jsx_transform = jsx_transform
+        self.node_stack = []
+
+    def _format_literal(self, value: str | int | float | bool):
+        """Format a literal for printing
+
+        For strings, this will escape them and wrap them in quotes. For booleans, this will convert them to 'true' or 'false'.
+        Numeric values will be converted to strings.
+        """
+        if isinstance(value, str):
+            # use json.dumps to escape strings & quote them
+            return json.dumps(
+                value,
+                # don't escape non-ascii. I added this specifically for generating code for React, e.g. '“I'm in a lquo;“' should
+                # not end up as \u201cI'm in a lquo;\u201c
+                ensure_ascii=False,
+            )
+        if isinstance(value, bool):
+            return "true" if value else "false"
+        return str(value)
+
+    def _print_comments(self, comments: Sequence[SingleLineComment | MultiLineComment]):
+        """Print comments according to the current context
+
+        If within a JSX element, comments will be wrapped in curly braces and SingleLineComment cannot be used.
+        """
+        within_jsx = self.is_within_jsx()
+        comment_strs: list[str] = []
+        for comment in comments:
+            if within_jsx and isinstance(comment, SingleLineComment):
+                comment = MultiLineComment(comment.comment_text)
+            comment_str = self.print(comment)
+            if within_jsx:
+                comment_str = f"{{{comment_str}}}"
+            comment_strs.append(comment_str)
+        return "\n".join(comment_strs)
+
+    def parent_node(self):
+        """Return the parent node of the current node being processed by ``print``. This only makes sense when called from within ``print``.
 
-    def print(self, node: NodeLike):  # noqa: T202
+        This can be used to determine what to do with a node conditionally based on its parent.
+        """
+        if len(self.node_stack) >= 2:
+            return self.node_stack[-2]
+        return None
+
+    @push_node_stack
+    @print_comments
+    def print(self, node: NodeLike) -> str:  # noqa: T202
         """Recursively print the code for the specified ``node``"""
+        if isinstance(node, JsxText) or isinstance(node, StringLiteral) and self.is_within_jsx():
+            if self.jsx_transform:
+                return self._format_literal(node.value)
+            if node.value != escape(node.value):
+                # If escaping is needed, use a JSX expression. For example, if the string is "Hello <World>" then
+                # this will be printed as {"Hello <World>"}
+                return f"{{{self._format_literal(node.value)}}}"
+            return node.value
+        if isinstance(node, JsxExpression):
+            value = ""
+            if node.expression is not None:
+                value = self.print(node.expression)
+            prefix = ""
+            suffix = ""
+            if node.leading_comments:
+                prefix = self.print(node.leading_comments)
+            if node.trailing_comments:
+                suffix = self.print(node.trailing_comments)
+            if self.jsx_transform:
+                return f"{prefix}{value}{suffix}"
+            return f"{{{prefix}{value}{suffix}}}"
+        if isinstance(node, JsxElement):
+            if self.jsx_transform:
+                # Copy comments from the node to the tag name when using JSX transform
+                tag_name = dataclasses.replace(
+                    node.tag_name,
+                    leading_comments=node.leading_comments,
+                    trailing_comments=node.trailing_comments,
+                )
+                element_args: list[NodeLike] = [
+                    tag_name,
+                    ObjectLiteralExpression(
+                        [
+                            ObjectProperty(attr.name, attr.initializer)
+                            if isinstance(attr, JsxAttribute)
+                            else SpreadAssignment(attr.expression)
+                            for attr in node.attributes
+                        ]
+                    ),
+                    *node.children,
+                ]
+                return self.print(
+                    CallExpression(
+                        self.jsx_transform,
+                        element_args,
+                    )
+                )
+            attrs = []
+            for attr in node.attributes:
+                if isinstance(attr, JsxAttribute):
+                    # if attr is e.g. "aria-label" use that as is. Otherwise will be an Identifier.
+                    name = attr.name.value if isinstance(attr.name, StringLiteral) else self.print(attr.name)
+                    # if string use form 'name="value"', otherwise use form 'name={value}'
+                    if isinstance(attr.initializer, StringLiteral):
+                        attrs.append(f"{name}={self._format_literal(attr.initializer.value)}")
+                    else:
+                        attrs.append(f"{name}={{{self.print(attr.initializer)}}}")
+                else:
+                    attrs.append(f"{{...{self.print(attr.expression)}}}")
+            attrs_str = ""
+            if attrs:
+                attrs_str = " " + " ".join(attrs)
+            tag_name_str = (
+                node.tag_name.value if isinstance(node.tag_name, StringLiteral) else self.print(node.tag_name)
+            )
+            if node.children:
+                return f"<{tag_name_str}{attrs_str}>{''.join(self.print(child) for child in node.children)}</{tag_name_str}>"
+            return f"<{tag_name_str}{attrs_str} />"
+
         if isinstance(node, VariableDeclaration):
             return self.apply_modifiers(
                 " ".join(
                     [node.kind, ", ".join(self.print(declaration) for declaration in node.declarations)]
                 ),
                 node.modifiers,
                 node,
@@ -83,16 +262,15 @@
         if isinstance(node, (VariableDeclarator, Parameter)):
             if node.init:
                 return " ".join([self.print(node.name), "=", self.print(node.init)])
             return self.print(node.name)
         if isinstance(node, Identifier):
             return node.name
         if isinstance(node, (NumericLiteral, BooleanLiteral, StringLiteral)):
-            # use json.dumps to escape strings & quote them
-            return json.dumps(node.value)
+            return self._format_literal(node.value)
         if isinstance(node, ImportSpecifier):
             if node.imported == node.local:
                 return self.print(node.imported)
             return f"{self.print(node.imported)} as {self.print(node.local)}"
         if isinstance(node, ImportDeclaration):
             default_specifier = node.get_default_specifier()
             named_specifiers = [
@@ -142,16 +320,23 @@
                 node.modifiers,
                 node,
             )
         if isinstance(node, ReturnStatement):
             return f"return {self.print(node.expression)}"
 
         if isinstance(node, CallExpression):
-            args = ", ".join(self.print(arg) for arg in node.arguments)
-            return f"{self.print(node.expression)}({args})"
+            args: list[str] = []
+            for arg in node.arguments:
+                code = self.print(arg)
+                if isinstance(arg, SingleLineComment):
+                    args.append(f"\n{code}\n")
+                else:
+                    args.append(code)
+            args_str = ", ".join(args)
+            return f"{self.print(node.expression)}({args_str})"
 
         if isinstance(node, AsExpression):
             return f"{self.print(node.expression)} as {self.print(node.type_annotation)}"
 
         if isinstance(node, TypeReference):
             # TODO: need to support type arguments - but this should be based on target. e.g. for code in browser we
             # wouldn't include this, but for codegen ViewModel classes we would.
@@ -174,14 +359,17 @@
                     pieces.append(f"${{{self.print(child)}}}")
             return f"`{''.join(pieces)}`"
 
         if isinstance(node, SingleLineComment):
             lines = "\n// ".join(node.comment_text.split("\n"))
             return f"// {lines}"
 
+        if isinstance(node, MultiLineComment):
+            return f"/* {node.comment_text} */"
+
         if isinstance(node, NullKeyword):
             return "null"
 
         if isinstance(node, NewExpression):
             return (
                 f"new {self.print(node.expression)}({', '.join(self.print(arg) for arg in node.arguments)})"
             )
@@ -221,14 +409,21 @@
             elif isinstance(modifier, AsyncKeyword):
                 prefix += "async "
             else:
                 raise NotImplementedError(f"Do not know how to handle {modifier}")
 
         return prefix + code
 
+    def is_within_jsx(self):
+        """Return True if the current node is within a JSX element. This can be used to determine how to print certain nodes.
+
+        For example, a ``StringLiteral`` within a JSX element would be ``<Element>Text</Element>``, but outside would be ``"Text"``.
+        """
+        return isinstance(self.parent_node(), JsxElement)
+
 
 class TypescriptSourceFileWriter:
     """Source file writer with some helpers
 
     Helps add imports to nodes without needing to manually track duplicates etc. Use ``resolve_import`` to get a valid
     ``Identifier`` to use.
 
@@ -277,19 +472,24 @@
     #: Function used to resolve the URL to use for an import. This can be used to do things like resolve it to a dev server URL or to a built file.
     resolve_import_url: Callable[[Path | str], str] | None
     #: Nodes that will be included at the start of the generated code. This is useful for adding header comments.
     leading_nodes: list[Node]
 
     used_identifiers: list[str]
 
+    #: How to treat JSX elements. If specified, JSX elements will be transformed to the equivalent of ``React.createElement`` calls.
+    #: The specific function called is identified by ``jsx_transform``, but the relevant import must be added manually.
+    jsx_transform: Node | None
+
     def __init__(
         self,
         path: Path | None = None,
         path_base: Path | None = None,
         resolve_import_url: Callable[[Path | str], str] | None = None,
+        jsx_transform: Node | None = default_jsx_transform,
     ):
         """
 
         Args:
             path: If specified, and ``SourceFileWrite`` used as a context then the generated code will be written to this file
             path_base: Path any imports are relative to
             resolve_import_url: Function used to resolve the URL to use for an import. This can be used to do things like resolve
@@ -298,14 +498,15 @@
         self.path = path
         self.resolve_import_url = resolve_import_url
         self.path_base = path_base or path or settings.PROJECT_DIR
         self.nodes = []
         self.leading_nodes = []
         self.required_imports = []
         self.used_identifiers = []
+        self.jsx_transform = jsx_transform
 
     def resolve_import(
         self, source: str | Path, specifier: ImportSpecifier | ImportDefaultSpecifier, import_order_priority=0
     ) -> Identifier:
         """
         Resolve an import. This will make sure the import is included in the final source (while not conflicting with
         other imports) and will return the ``Identifier`` to use to reference it.
@@ -346,15 +547,15 @@
         self.leading_nodes.append(node)
 
     def __enter__(self):
         return self
 
     def get_code(self) -> str:
         """Returns the printed code"""
-        printer = TypescriptPrinter(self.path_base, self.resolve_import_url)
+        printer = TypescriptPrinter(self.path_base, self.resolve_import_url, jsx_transform=self.jsx_transform)
         code = [printer.print(node) for node in self.leading_nodes]
         for imp in self.required_imports:
             code.append(printer.print(imp))
         if code:
             code.append("\n")
         for node in self.nodes:
             code.append(printer.print(node))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alliance_platform_codegen-0.0.3/alliance_platform/codegen/registry.py` & `alliance_platform_codegen-0.0.4/alliance_platform/codegen/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import field
 from functools import lru_cache
 import json
 import logging
 from pathlib import Path
 import tempfile
 import time
+import traceback
 from typing import Callable
 from typing import TypedDict
 
 from alliance_platform.codegen.settings import ap_codegen_settings
 from alliance_platform.core.settings import ap_core_settings
 
 logger = logging.getLogger("alliance_platform.codegen")
@@ -32,14 +33,24 @@
 
     def get_cache_key(self) -> None | CodegenRegistrationCacheKey:
         """
         Returns an identifier and a  list of file paths that this code generation depends on. The code generation should
         be re-triggered if any of these files change.
 
         If the code generation should always run, return ``None``.
+
+        Note that caching is local to your machine.
+
+        .. warning::
+
+            Use this sparingly, as it can lead to cases where code generation does not run when it should. In particular,
+            if details used in the code generation depend on state not captured in the ``cache`` key the cache won't
+            be invalidated when it should be. For example, if you generated code for a specific class that was part
+            of the cache key, but used details from a base class in a different file and that file changed then the
+            cache would not be invalidated.
         """
         return None
 
 
 @dataclass
 class IntermediateArtifact:
     temp_file_path: Path
@@ -93,25 +104,40 @@
             self.cache = {"version": 1, "entries": {}}
         if not isinstance(self.cache["entries"], dict):
             self.cache["entries"] = {}
 
     def register(self, registration: CodegenRegistration):
         self.registrations.append(registration)
 
+    def invalidate_cache(self, registration: CodegenRegistration):
+        cache_key = registration.get_cache_key()
+        if not cache_key:
+            return True
+        registration_id = self._get_cache_registration_id(registration)
+        if registration_id in self.cache["entries"]:
+            del self.cache["entries"][registration_id]
+            self.cache_path.write_text(json.dumps(self.cache, indent=2))
+
+    def _get_cache_registration_id(self, registration: CodegenRegistration) -> str:
+        cache_key = registration.get_cache_key()
+        if not cache_key:
+            raise ValueError("Registration has no cache key")
+        class_id = f"{registration.__class__.__module__}.{registration.__class__.__qualname__}"
+        return f'{class_id}.{cache_key["registration_id"]}'
+
     def has_dependencies_changed(self, registration: CodegenRegistration, stats: CodegenStats) -> bool:
         cache_key = registration.get_cache_key()
         if not cache_key:
             return True
         if not cache_key["dependency_files"]:
             stats.add_warning(
                 f"Codegen registration {registration} `get_cache_key` lists no files; will always run"
             )
             return True
-        class_id = f"{registration.__class__.__module__}.{registration.__class__.__qualname__}"
-        registration_id = f'{class_id}.{cache_key["registration_id"]}'
+        registration_id = self._get_cache_registration_id(registration)
         entry = self.cache["entries"].get(registration_id, {})
         timestamps = {}
         for dependency in cache_key["dependency_files"]:
             dependency = Path(dependency)
             if not dependency.exists():
                 stats.add_warning(f"Dependency file {dependency} does not exist")
                 return True
@@ -131,28 +157,34 @@
                 return False
 
         files_to_write = []
         stats = CodegenStats(len(self.registrations))
         for registration in self.registrations:
             if not self.has_dependencies_changed(registration, stats):
                 continue
-            artifacts = registration.generate_artifacts()
-            if not isinstance(artifacts, list):
-                artifacts = [artifacts]
-            for artifact in artifacts:
-                suffix = Path(artifact.path).suffix
-                temp = tempfile.NamedTemporaryFile(
-                    "w",
-                    suffix=suffix,
-                    delete=False,
-                    dir=ap_codegen_settings.TEMP_DIR,
-                )
-                temp.write(artifact.contents)
-                temp.close()
-                files_to_write.append(IntermediateArtifact(Path(temp.name), artifact.path))
+            try:
+                artifacts = registration.generate_artifacts()
+            except Exception:
+                stats.add_warning(f"Error generating artifacts for {registration}: {traceback.format_exc()}")
+                self.invalidate_cache(registration)
+                continue
+            else:
+                if not isinstance(artifacts, list):
+                    artifacts = [artifacts]
+                for artifact in artifacts:
+                    suffix = Path(artifact.path).suffix
+                    temp = tempfile.NamedTemporaryFile(
+                        "w",
+                        suffix=suffix,
+                        delete=False,
+                        dir=ap_codegen_settings.TEMP_DIR,
+                    )
+                    temp.write(artifact.contents)
+                    temp.close()
+                    files_to_write.append(IntermediateArtifact(Path(temp.name), artifact.path))
 
         def cleanup():
             for intermediate_file in files_to_write:
                 intermediate_file.temp_file_path.unlink(missing_ok=True)
 
         abort_reason = should_abort()
         if abort_reason:
```

### Comparing `alliance_platform_codegen-0.0.3/alliance_platform/codegen/settings.py` & `alliance_platform_codegen-0.0.4/alliance_platform/codegen/settings.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_codegen-0.0.3/alliance_platform/codegen/typescript.py` & `alliance_platform_codegen-0.0.4/alliance_platform/codegen/typescript.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 import re
 from typing import Callable
 from typing import Sequence
+from typing import Union
 
 from django.utils.functional import Promise
 
 # To work out what to name things enter code at https://astexplorer.net/ and see what AST it generates
 # We don't need to be strict so exclude things where it makes it easier to use
 
 
+@dataclass(kw_only=True)
 class Node:
     """Root node everything else should extend from"""
 
-    pass
+    leading_comments: Sequence[Union["SingleLineComment", "MultiLineComment"]] | None = None
+    trailing_comments: Sequence[Union["SingleLineComment", "MultiLineComment"]] | None = None
 
 
 class Modifier:
     """Base class for modifiers"""
 
     pass
 
@@ -583,14 +586,19 @@
 
 @dataclass
 class SingleLineComment(Node):
     comment_text: str
 
 
 @dataclass
+class MultiLineComment(Node):
+    comment_text: str
+
+
+@dataclass
 class NewExpression(Node):
     expression: Node
     arguments: Sequence[NodeLike] = field(default_factory=list)
 
 
 @dataclass
 class Block(Node):
@@ -603,14 +611,42 @@
 class ArrowFunction(Node):
     #: Any parameters to the function
     parameters: list[Parameter]
     #: The body as either a single expression valid for Arrow functions or a ``Block`` node
     body: Node
 
 
+@dataclass
+class JsxAttribute(Node):
+    name: Identifier | StringLiteral
+    initializer: Node
+
+
+@dataclass
+class JsxSpreadAttribute(Node):
+    expression: Identifier
+
+
+@dataclass
+class JsxText(Node):
+    value: str
+
+
+@dataclass
+class JsxExpression(Node):
+    expression: Node | None
+
+
+@dataclass
+class JsxElement(Node):
+    tag_name: Identifier | StringLiteral
+    attributes: Sequence[JsxAttribute | JsxSpreadAttribute]
+    children: list[Union[JsxText, JsxExpression, "JsxElement"]]
+
+
 def construct_object_property_key(
     value: AcceptedPropertyKeyType,
 ) -> Identifier | NumericLiteral | StringLiteral:
     """Construct node to use for a property key
 
     If ``value`` is numeric will return ``NumericLiteral``
         e.g. ``{ 5: "five" }``
```

### Comparing `alliance_platform_codegen-0.0.3/pyproject.toml` & `alliance_platform_codegen-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "alliance-platform-core",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 include = [
     "alliance_platform/codegen/py.typed",
 ]
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [build-system]
 requires = [
     "pdm-backend",
```

