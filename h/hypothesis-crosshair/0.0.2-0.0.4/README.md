# Comparing `tmp/hypothesis-crosshair-0.0.2.tar.gz` & `tmp/hypothesis_crosshair-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-crosshair-0.0.2.tar", last modified: Fri Mar 15 19:41:24 2024, max compression
+gzip compressed data, was "hypothesis_crosshair-0.0.4.tar", last modified: Mon May 13 13:06:33 2024, max compression
```

## Comparing `hypothesis-crosshair-0.0.2.tar` & `hypothesis_crosshair-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:41:24.939968 hypothesis-crosshair-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-15 19:41:24.939968 hypothesis-crosshair-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:41:24.939968 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 19:41:24.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:41:24.939968 hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/crosshair_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/crosshair_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:41:24.939968 hypothesis-crosshair-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-15 19:41:20.000000 hypothesis-crosshair-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:06:33.945833 hypothesis_crosshair-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-13 13:06:33.945833 hypothesis_crosshair-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:06:33.945833 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 13:06:33.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:06:33.945833 hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/crosshair_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/crosshair_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/end_to_end_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:06:33.945833 hypothesis_crosshair-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 13:06:27.000000 hypothesis_crosshair-0.0.4/setup.py
```

### Comparing `hypothesis-crosshair-0.0.2/LICENSE` & `hypothesis_crosshair-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis-crosshair-0.0.2/PKG-INFO` & `hypothesis_crosshair-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-crosshair
-Version: 0.0.2
+Version: 0.0.4
 Summary: Level-up your Hypothesis tests with CrossHair.
 Home-page: https://github.com/pschanely/hypothesis-crosshair
 Author: Phillip Schanely
 Author-email: pschanely+B9vk@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Hypothesis
@@ -48,10 +48,10 @@
 @settings(backend="crosshair")
 @given(st.integers())
 def test_needs_solver(x):
     assert x != 123456789
 ```
 
 
-Docs hopefully comming soon. In the meantime, start a
+Docs hopefully coming soon. In the meantime, start a
 [discussion](https://github.com/pschanely/hypothesis-crosshair/discussions)
 or file an [issue](https://github.com/pschanely/hypothesis-crosshair/issues).
```

### Comparing `hypothesis-crosshair-0.0.2/README.md` & `hypothesis_crosshair-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 @settings(backend="crosshair")
 @given(st.integers())
 def test_needs_solver(x):
     assert x != 123456789
 ```
 
 
-Docs hopefully comming soon. In the meantime, start a
+Docs hopefully coming soon. In the meantime, start a
 [discussion](https://github.com/pschanely/hypothesis-crosshair/discussions)
 or file an [issue](https://github.com/pschanely/hypothesis-crosshair/issues).
```

### Comparing `hypothesis-crosshair-0.0.2/hypothesis_crosshair.egg-info/PKG-INFO` & `hypothesis_crosshair-0.0.4/hypothesis_crosshair.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-crosshair
-Version: 0.0.2
+Version: 0.0.4
 Summary: Level-up your Hypothesis tests with CrossHair.
 Home-page: https://github.com/pschanely/hypothesis-crosshair
 Author: Phillip Schanely
 Author-email: pschanely+B9vk@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Hypothesis
@@ -48,10 +48,10 @@
 @settings(backend="crosshair")
 @given(st.integers())
 def test_needs_solver(x):
     assert x != 123456789
 ```
 
 
-Docs hopefully comming soon. In the meantime, start a
+Docs hopefully coming soon. In the meantime, start a
 [discussion](https://github.com/pschanely/hypothesis-crosshair/discussions)
 or file an [issue](https://github.com/pschanely/hypothesis-crosshair/issues).
```

### Comparing `hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/crosshair_provider.py` & `hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/crosshair_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import math
 import os
 import sys
 from contextlib import ExitStack, contextmanager
 from time import monotonic
-from typing import Any, Optional, Sequence
+from typing import Optional, Sequence
 
 import crosshair.core_and_libs  # Needed for patch registrations
 from crosshair import debug, deep_realize
 from crosshair.core import (COMPOSITE_TRACER, DEFAULT_OPTIONS,
                             AnalysisOptionSet, CallAnalysis, IgnoreAttempt,
                             NoTracing, Patched, RootNode, StateSpace,
                             StateSpaceContext, UnexploredPath,
                             VerificationStatus, condition_parser,
-                            get_current_parser,
-                            context_statespace, is_tracing, proxy_for_type)
+                            context_statespace, get_current_parser, is_tracing,
+                            proxy_for_type)
 from crosshair.libimpl.builtinslib import (LazyIntSymbolicStr,
                                            SymbolicBoundedIntTuple)
+from crosshair.statespace import DeatchedPathNode
 from crosshair.util import set_debug, test_stack
 from hypothesis.internal.conjecture.data import PrimitiveProvider
 from hypothesis.internal.intervalsets import IntervalSet
 
 
 class CrossHairPrimitiveProvider(PrimitiveProvider):
     """An implementation of PrimitiveProvider based on CrossHair."""
@@ -28,37 +29,64 @@
         self.iteration_number = 0
         self.current_exit_stack: Optional[ExitStack] = None
         self.search_root = RootNode()
         if len(os.environ.get("DEBUG_CROSSHAIR", "")) > 1:
             set_debug(os.environ["DEBUG_CROSSHAIR"].lower() not in ("0", "false"))
         elif "-vv" in sys.argv:
             set_debug(True)
+        self._previous_space = None
         self._previous_realized_draws = None
+        self.exhausted = False
 
     @contextmanager
-    def per_test_case_context_manager(self):
-        self.iteration_number += 1
-        if self.search_root.child.is_exhausted():
-            debug("Resetting search root")
-            # might be nice to signal that we're done somehow.
-            # But for now, just start over!
-            self.search_root = RootNode()
-        self._previous_realized_draws = None
-        iter_start = monotonic()
+    def post_test_case_context_manager(self):
+        assert self._previous_space is not None
+        with (
+            condition_parser([]),
+            Patched(),
+            StateSpaceContext(self._previous_space),
+            COMPOSITE_TRACER,
+        ):
+            # IgnoreAttempt is possible here in theory, but hopefully won't happen because we've
+            # already fixed the drawn values
+            yield
+
+    def _make_statespace(self):
         options = DEFAULT_OPTIONS.overlay(AnalysisOptionSet(analysis_kind=[]))
-        per_path_timeout = options.get_per_path_timeout()  # TODO: how to set this?
+        per_path_timeout = (
+            2.0  # TODO: use hypothesis.settings.deadline * 10 or something?
+        )
+        iter_start = monotonic()
         space = StateSpace(
             execution_deadline=iter_start + per_path_timeout,
             model_check_timeout=per_path_timeout / 2,
             search_root=self.search_root,
         )
         space._hypothesis_draws = []  # keep a log of drawn values
         space._hypothesis_next_name_id = (
             0  # something to uniqu-ify names for drawn values
         )
+        return space
+
+    @contextmanager
+    def per_test_case_context_manager(self):
+        if self._previous_space is not None:
+            _analysis, _exhausted = self._previous_space.bubble_status(
+                CallAnalysis(VerificationStatus.CONFIRMED)
+            )
+        self.iteration_number += 1
+        if self.search_root.child.is_exhausted():
+            self.exhausted = True
+            debug("Resetting search root")
+            # might be nice to signal that we're done somehow.
+            # But for now, just start over!
+            self.search_root = RootNode()
+        self._previous_realized_draws = None
+        self._previous_space = None
+        space = self._make_statespace()
 
         try:
             with (
                 condition_parser([]),
                 Patched(),
                 StateSpaceContext(space),
                 COMPOSITE_TRACER,
@@ -70,23 +98,22 @@
                     debug("starting iteration", self.iteration_number)
                     try:
                         yield
                     finally:
                         any_choices_made = bool(space.choices_made)
                         if any_choices_made:
                             space.detach_path()
-                            self._previous_realized_draws = {
-                                id(symbolic): deep_realize(symbolic)
-                                for symbolic in space._hypothesis_draws
-                            }
                         else:
-                            # TODO: I can't detach_path here because it will conflict with the
+                            # NOTE: I can't detach_path here because it will conflict with the
                             # top node of a prior "real" execution.
-                            # Should I just generate a dummy concrete value for each of the draws?
-                            self._previous_realized_draws = {}
+                            space._search_position = DeatchedPathNode()
+                        self._previous_realized_draws = {
+                            id(symbolic): deep_realize(symbolic)
+                            for symbolic in space._hypothesis_draws
+                        }
                     debug("ended iteration (normal completion)")
                 except Exception as exc:
                     try:
                         exc.args = deep_realize(exc.args)
                         debug(
                             f"ended iteration (exception: {type(exc).__name__}: {exc})",
                             test_stack(exc.__traceback__),
@@ -94,22 +121,20 @@
                     except Exception:
                         exc.args = ()
                         debug(
                             f"ended iteration ({type(exc)} exception)",
                             test_stack(exc.__traceback__),
                         )
                     raise exc
-        except (IgnoreAttempt, UnexploredPath) as e:
+        except (IgnoreAttempt, UnexploredPath):
             pass
         finally:
+            self._previous_space = space
             if any_choices_made:
                 debug("bubbling status")
-                _analysis, _exhausted = space.bubble_status(
-                    CallAnalysis(VerificationStatus.CONFIRMED)
-                )
             else:
                 debug("no decisions made; ignoring this iteration")
 
     def _next_name(self, prefix: str) -> str:
         space = context_statespace()
         space._hypothesis_next_name_id += 1
         name = f"{prefix}_{space._hypothesis_next_name_id:02d}"
@@ -122,43 +147,48 @@
     def draw_boolean(
         self,
         p: float = 0.5,
         *,
         forced: Optional[bool] = None,
         fake_forced: bool = False,
     ) -> bool:
-        if forced is not None:
-            return forced
+        with NoTracing():
+            if forced is not None:
+                return forced
 
-        symbolic = proxy_for_type(bool, self._next_name("bool"), allow_subtypes=False)
-        self._remember_draw(symbolic)
-        return symbolic
+            symbolic = proxy_for_type(
+                bool, self._next_name("bool"), allow_subtypes=False
+            )
+            self._remember_draw(symbolic)
+            return symbolic
 
     def draw_integer(
         self,
         min_value: Optional[int] = None,
         max_value: Optional[int] = None,
         *,
         # weights are for choosing an element index from a bounded range
         weights: Optional[Sequence[float]] = None,
         shrink_towards: int = 0,
         forced: Optional[int] = None,
         fake_forced: bool = False,
     ) -> int:
-        if forced is not None:
-            return forced
-        symbolic = proxy_for_type(int, self._next_name("int"), allow_subtypes=False)
+        with NoTracing():
+            if forced is not None:
+                return forced
+            symbolic = proxy_for_type(int, self._next_name("int"), allow_subtypes=False)
         conditions = []
         if min_value is not None:
             conditions.append(min_value <= symbolic)
         if max_value is not None:
             conditions.append(symbolic <= max_value)
         if not all(conditions):
             raise IgnoreAttempt
-        self._remember_draw(symbolic)
+        with NoTracing():
+            self._remember_draw(symbolic)
         return symbolic
 
     def draw_float(
         self,
         *,
         min_value: float = -math.inf,
         max_value: float = math.inf,
@@ -170,17 +200,20 @@
         # exclude_min and exclude_max handled higher up
         forced: Optional[float] = None,
         fake_forced: bool = False,
     ) -> float:
         # TODO: all of this is a bit of a ruse - at present, CrossHair approximates
         # floats as real numbers. (though it will attempt +/-inf & nan)
         # See https://github.com/pschanely/CrossHair/issues/230
-        if forced is not None:
-            return forced
-        symbolic = proxy_for_type(float, self._next_name("float"), allow_subtypes=False)
+        with NoTracing():
+            if forced is not None:
+                return forced
+            symbolic = proxy_for_type(
+                float, self._next_name("float"), allow_subtypes=False
+            )
         conditions = []
         if not allow_nan:
             conditions.append(math.isnan(symbolic))
         if min_value is not None:
             conditions.append(min_value <= symbolic)
         if max_value is not None:
             conditions.append(symbolic <= max_value)
@@ -192,15 +225,16 @@
                         symbolic == 0,
                         symbolic > smallest_nonzero_magnitude,
                     ]
                 )
             )
         if not all(conditions):
             raise IgnoreAttempt
-        self._remember_draw(symbolic)
+        with NoTracing():
+            self._remember_draw(symbolic)
         return symbolic
 
     def draw_string(
         self,
         intervals: IntervalSet,
         *,
         min_size: int = 0,
@@ -220,26 +254,33 @@
 
     def draw_bytes(
         self,
         size: int,
         forced: Optional[bytes] = None,
         fake_forced: bool = False,
     ) -> bytes:
-        if forced is not None:
-            return forced
-        symbolic = proxy_for_type(bytes, self._next_name("bytes"), allow_subtypes=False)
+        with NoTracing():
+            if forced is not None:
+                return forced
+            symbolic = proxy_for_type(
+                bytes, self._next_name("bytes"), allow_subtypes=False
+            )
         if len(symbolic) != size:
             raise IgnoreAttempt
-        self._remember_draw(symbolic)
-        return symbolic
+        with NoTracing():
+            self._remember_draw(symbolic)
+            return symbolic
 
     def export_value(self, value):
         if is_tracing():
             return deep_realize(value)
+        elif self._previous_realized_draws is None:
+            debug("WARNING: export_value() requested before test case complered", test_stack())
+            return value
+        elif id(value) in self._previous_realized_draws:
+            return self._previous_realized_draws[id(value)]
         else:
-            if self._previous_realized_draws is None:
-                debug("WARNING: export_value() requested at wrong time", test_stack())
-                return value
-            return self._previous_realized_draws.get(id(value), value)
+            with self.post_test_case_context_manager():
+                return deep_realize(value)
 
     def post_test_case_hook(self, val):
         return self.export_value(val)
```

### Comparing `hypothesis-crosshair-0.0.2/hypothesis_crosshair_provider/crosshair_provider_test.py` & `hypothesis_crosshair-0.0.4/hypothesis_crosshair_provider/crosshair_provider_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,7 +44,33 @@
             assert type(provider.export_value(s_str)) == str
             # NOTE: draw_bytes can raise IgnoreAttempt, which will leave the bytes
             # symbolic without a concrete value:
             assert type(provider.export_value(s_bytes)) in (bytes, types.NoneType)
         except TargetException:
             found_ct += 1
     assert found_ct > 0, "CrossHair could not find the exception"
+
+
+def test_post_run_value_export():
+    provider = CrossHairPrimitiveProvider()
+    with provider.per_test_case_context_manager():
+        s_int = provider.draw_integer()
+        if s_int > 10:
+            pass
+    assert type(provider.export_value(s_int)) is int
+    assert type(provider.export_value([s_int])[0]) is int
+
+
+def test_post_run_decisions_do_not_grow_the_search_tree():
+    provider = CrossHairPrimitiveProvider()
+    # There should only be one real branch; so it will take 2 iterations to exhaust
+    for _ in range(2):
+        with provider.per_test_case_context_manager():
+            s_int = provider.draw_integer()
+            if s_int > 10:
+                pass
+        with provider.post_test_case_context_manager():
+            if s_int + 1 > 100:
+                pass
+        assert not provider.exhausted
+    with provider.per_test_case_context_manager():
+        assert provider.exhausted
```

### Comparing `hypothesis-crosshair-0.0.2/setup.py` & `hypothesis_crosshair-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="hypothesis-crosshair",
-    version="0.0.2",
+    version="0.0.4",
     author="Phillip Schanely",
     author_email="pschanely+B9vk@gmail.com",
     packages=setuptools.find_packages(),
     url="https://github.com/pschanely/hypothesis-crosshair",
     license="MIT",
     description="Level-up your Hypothesis tests with CrossHair.",
     long_description=open("README.md", encoding="utf-8").read(),
```

