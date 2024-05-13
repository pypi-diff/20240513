# Comparing `tmp/ast_grep_py-0.22.2.tar.gz` & `tmp/ast_grep_py-0.22.3.tar.gz`

## Comparing `ast_grep_py-0.22.2.tar` & `ast_grep_py-0.22.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0     1001      127      682 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     8074 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5244 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     8987 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    17978 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     8432 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    19521 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5481 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    17934 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    13810 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127     3341 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    11131 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127    11870 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/config/src/transform/transformation.rs
--rw-r--r--   0     1001      127      692 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    15102 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    15050 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17457 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127     2472 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1450 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/haskell.rs
--rw-r--r--   0     1001      127     1142 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13779 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3523 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2147 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/language/src/swift.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.2/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7731 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61831 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/Cargo.lock
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.2/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.2/pyproject.toml
--rw-r--r--   0     1001      127     1933 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1356 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1459 2024-05-12 08:31:19.000000 ast_grep_py-0.22.2/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.2/PKG-INFO
+-rw-r--r--   0     1001      127      692 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15050 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    18135 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/core/src/traversal.rs
+-rw-r--r--   0     1001      127      682 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     8074 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5244 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     8987 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    17978 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     8432 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    19521 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5481 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    17934 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    13810 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127     3341 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    11131 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127    11870 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/config/src/transform/transformation.rs
+-rw-r--r--   0     1001      127     2472 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1450 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/haskell.rs
+-rw-r--r--   0     1001      127     1142 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13779 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3523 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2147 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/language/src/swift.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.3/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61831 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/Cargo.lock
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.3/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.3/pyproject.toml
+-rw-r--r--   0     1001      127     1933 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1356 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1459 2024-05-13 06:19:49.000000 ast_grep_py-0.22.3/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.3/PKG-INFO
```

### Comparing `ast_grep_py-0.22.2/crates/config/Cargo.toml` & `ast_grep_py-0.22.3/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/check_var.rs` & `ast_grep_py-0.22.3/crates/config/src/check_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/combined.rs` & `ast_grep_py-0.22.3/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/fixer.rs` & `ast_grep_py-0.22.3/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/lib.rs` & `ast_grep_py-0.22.3/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/maybe.rs` & `ast_grep_py-0.22.3/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.22.3/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule/mod.rs` & `ast_grep_py-0.22.3/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.22.3/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.22.3/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.22.3/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule_collection.rs` & `ast_grep_py-0.22.3/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule_config.rs` & `ast_grep_py-0.22.3/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/rule_core.rs` & `ast_grep_py-0.22.3/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/transform/mod.rs` & `ast_grep_py-0.22.3/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.22.3/crates/config/src/transform/rewrite.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.22.3/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/config/src/transform/transformation.rs` & `ast_grep_py-0.22.3/crates/config/src/transform/transformation.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/Cargo.toml` & `ast_grep_py-0.22.3/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/language.rs` & `ast_grep_py-0.22.3/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/lib.rs` & `ast_grep_py-0.22.3/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/match_tree.rs` & `ast_grep_py-0.22.3/crates/core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.22.3/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.22.3/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.22.3/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/matcher/text.rs` & `ast_grep_py-0.22.3/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/matcher.rs` & `ast_grep_py-0.22.3/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/meta_var.rs` & `ast_grep_py-0.22.3/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/node.rs` & `ast_grep_py-0.22.3/crates/core/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -375,51 +375,77 @@
     })
   }
 
   /// Returns all sibling nodes next to `self`.
   // NOTE: Need go to parent first, then move to current node by byte offset.
   // This is because tree_sitter cursor is scoped to the starting node.
   // See https://github.com/tree-sitter/tree-sitter/issues/567
+  #[cfg(not(target_arch = "wasm32"))]
   pub fn next_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
     // if root is none, use self as fallback to return a type-stable Iterator
     let node = self.parent().unwrap_or_else(|| self.clone());
     let mut cursor = node.inner.walk();
     cursor.goto_first_child_for_byte(self.inner.start_byte());
     std::iter::from_fn(move || {
       if cursor.goto_next_sibling() {
         Some(self.root.adopt(cursor.node()))
       } else {
         None
       }
     })
   }
 
+  // wasm32 has wrong goto_first_child_for_byte
+  #[cfg(target_arch = "wasm32")]
+  pub fn next_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
+    let mut node = self.clone();
+    std::iter::from_fn(move || {
+      node.next().map(|n| {
+        node = n.clone();
+        n
+      })
+    })
+  }
+
   #[must_use]
   pub fn prev(&self) -> Option<Node<'r, D>> {
     let inner = self.inner.prev_sibling()?;
     Some(Node {
       inner,
       root: self.root,
     })
   }
 
+  #[cfg(not(target_arch = "wasm32"))]
   pub fn prev_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
     // if root is none, use self as fallback to return a type-stable Iterator
     let node = self.parent().unwrap_or_else(|| self.clone());
     let mut cursor = node.inner.walk();
     cursor.goto_first_child_for_byte(self.inner.start_byte());
     std::iter::from_fn(move || {
       if cursor.goto_previous_sibling() {
         Some(self.root.adopt(cursor.node()))
       } else {
         None
       }
     })
   }
 
+  // wasm32 has wrong goto_first_child_for_byte
+  #[cfg(target_arch = "wasm32")]
+  pub fn prev_all(&self) -> impl Iterator<Item = Node<'r, D>> + '_ {
+    let mut node = self.clone();
+    std::iter::from_fn(move || {
+      node.prev().map(|n| {
+        node = n.clone();
+        n
+      })
+    })
+  }
+
   pub fn dfs<'s>(&'s self) -> Pre<'r, D> {
     Pre::new(self)
   }
 
   #[must_use]
   pub fn find<M: Matcher<D::Lang>>(&self, pat: M) -> Option<NodeMatch<'r, D>> {
     pat.find_node(self.clone())
```

### Comparing `ast_grep_py-0.22.2/crates/core/src/ops.rs` & `ast_grep_py-0.22.3/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/pinned.rs` & `ast_grep_py-0.22.3/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.22.3/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.22.3/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/replacer/template.rs` & `ast_grep_py-0.22.3/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/replacer.rs` & `ast_grep_py-0.22.3/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/source.rs` & `ast_grep_py-0.22.3/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/core/src/traversal.rs` & `ast_grep_py-0.22.3/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/Cargo.toml` & `ast_grep_py-0.22.3/crates/language/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/bash.rs` & `ast_grep_py-0.22.3/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/cpp.rs` & `ast_grep_py-0.22.3/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/csharp.rs` & `ast_grep_py-0.22.3/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/css.rs` & `ast_grep_py-0.22.3/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/elixir.rs` & `ast_grep_py-0.22.3/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/go.rs` & `ast_grep_py-0.22.3/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/haskell.rs` & `ast_grep_py-0.22.3/crates/language/src/haskell.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/html.rs` & `ast_grep_py-0.22.3/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/json.rs` & `ast_grep_py-0.22.3/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/kotlin.rs` & `ast_grep_py-0.22.3/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/lib.rs` & `ast_grep_py-0.22.3/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/lua.rs` & `ast_grep_py-0.22.3/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/parsers.rs` & `ast_grep_py-0.22.3/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/python.rs` & `ast_grep_py-0.22.3/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/ruby.rs` & `ast_grep_py-0.22.3/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/rust.rs` & `ast_grep_py-0.22.3/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/scala.rs` & `ast_grep_py-0.22.3/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/language/src/swift.rs` & `ast_grep_py-0.22.3/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/Cargo.toml` & `ast_grep_py-0.22.3/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/README.md` & `ast_grep_py-0.22.3/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.22.3/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/src/lib.rs` & `ast_grep_py-0.22.3/crates/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.22.3/crates/pyo3/src/py_node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/src/range.rs` & `ast_grep_py-0.22.3/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.22.3/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.22.3/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.22.3/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.22.3/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.22.3/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/Cargo.lock` & `ast_grep_py-0.22.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -140,15 +140,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -156,38 +156,38 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
@@ -210,29 +210,29 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -242,15 +242,15 @@
  "tree-sitter-html",
  "tree-sitter-javascript-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
@@ -308,15 +308,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.22.2"
+version = "0.22.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
```

### Comparing `ast_grep_py-0.22.2/Cargo.toml` & `ast_grep_py-0.22.3/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.22.2"
+version = "0.22.3"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.22.2" }
-ast-grep-config = { path = "crates/config", version = "0.22.2" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.2" }
-ast-grep-language = { path = "crates/language", version = "0.22.2" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.22.2" }
+ast-grep-core = { path = "crates/core", version = "0.22.3" }
+ast-grep-config = { path = "crates/config", version = "0.22.3" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.3" }
+ast-grep-language = { path = "crates/language", version = "0.22.3" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.22.3" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0.200", features = ["derive"] }
 tree-sitter = { version = "0.21.4", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
```

### Comparing `ast_grep_py-0.22.2/pyproject.toml` & `ast_grep_py-0.22.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.22.2"
+version = "0.22.3"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.22.2/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/ast_grep_py/__init__.py` & `ast_grep_py-0.22.3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/README.md` & `ast_grep_py-0.22.3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.2/PKG-INFO` & `ast_grep_py-0.22.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.22.2
+Version: 0.22.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

