# Comparing `tmp/accesskit-0.3.1.tar.gz` & `tmp/accesskit-0.3.2.tar.gz`

## Comparing `accesskit-0.3.1.tar` & `accesskit-0.3.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0     1001      127     1294 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127    11518 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/README.md
--rw-r--r--   0     1001      127     6935 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    13572 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6053 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      945 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     1459 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     8048 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1389 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      670 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     3370 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    12747 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     3414 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      541 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1036 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      334 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      753 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    39324 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    13107 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     1157 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/util.rs
--rw-r--r--   0     1001      127      705 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/Cargo.toml
--rw-r--r--   0     1001      127    15163 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/README.md
--rw-r--r--   0     1001      127    22792 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/src/geometry.rs
--rw-r--r--   0     1001      127    78839 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/src/lib.rs
--rw-r--r--   0     1001      127      942 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    15511 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/README.md
--rw-r--r--   0     1001      127     9554 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2731 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     9063 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      334 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      557 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    33624 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3146 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9523 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2819 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      956 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    25830 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/README.md
--rw-r--r--   0     1001      127    11651 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    15926 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1850 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      403 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127      482 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    38489 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6179 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11438 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     6937 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     3536 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19711 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/util.rs
--rw-r--r--   0     1001      127      406 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/Cargo.toml
--rw-r--r--   0     1001      127    18087 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/README.md
--rw-r--r--   0     1001      127     1262 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/filters.rs
--rw-r--r--   0     1001      127    24021 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     6115 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/lib.rs
--rw-r--r--   0     1001      127    33886 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/node.rs
--rw-r--r--   0     1001      127    64423 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/text.rs
--rw-r--r--   0     1001      127    27978 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/tree.rs
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.1/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     5346 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     6979 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    24191 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2818 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     7316 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1506 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4126 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    73407 2024-05-11 16:09:37.000000 accesskit-0.3.1/Cargo.lock
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-05-11 16:09:37.000000 accesskit-0.3.1/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.1/PKG-INFO
+-rw-r--r--   0     1001      127     1294 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    11644 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    13572 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6053 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      945 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     1459 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8048 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1389 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      942 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    16025 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9554 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2731 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     8399 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      282 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      557 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    32713 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3146 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9523 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2819 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/util.rs
+-rw-r--r--   0     1001      127      705 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/Cargo.toml
+-rw-r--r--   0     1001      127    15163 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/src/geometry.rs
+-rw-r--r--   0     1001      127    78839 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/src/lib.rs
+-rw-r--r--   0     1001      127      956 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    26348 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11651 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    15277 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1850 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      356 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    36973 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6937 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3536 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19711 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6500 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/util.rs
+-rw-r--r--   0     1001      127      435 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    18903 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/README.md
+-rw-r--r--   0     1001      127      958 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    25410 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     6057 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    31830 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/node.rs
+-rw-r--r--   0     1001      127    64423 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/text.rs
+-rw-r--r--   0     1001      127    25493 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/tree.rs
+-rw-r--r--   0     1001      127      670 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     4126 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    12926 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      541 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1036 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      282 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      753 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    37868 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    13107 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     1157 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/util.rs
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.2/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     5568 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     6979 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24191 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2818 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    75008 2024-05-13 21:02:49.000000 accesskit-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-05-13 21:02:49.000000 accesskit-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.2/PKG-INFO
```

### Comparing `accesskit-0.3.1/platforms/unix/Cargo.toml` & `accesskit-0.3.2/platforms/unix/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.9.1"
+version = "0.9.2"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -14,15 +14,15 @@
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_atspi_common = { version = "0.4.1", path = "../atspi-common" }
+accesskit_atspi_common = { version = "0.4.2", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
 async-channel = { version = "2.1.1", optional = true }
```

### Comparing `accesskit-0.3.1/platforms/unix/CHANGELOG.md` & `accesskit-0.3.2/platforms/unix/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,18 @@
   * dependencies
     * accesskit_atspi_common bumped from 0.1.2 to 0.2.0
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.4.0 to 0.4.1
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_atspi_common bumped from 0.4.1 to 0.4.2
+
 ## [0.9.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.8.0...accesskit_unix-v0.9.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Force a semver-breaking release ([#398](https://github.com/AccessKit/accesskit/issues/398))
```

### Comparing `accesskit-0.3.1/platforms/unix/src/adapter.rs` & `accesskit-0.3.2/platforms/unix/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/bus.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/bus.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.3.2/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/context.rs` & `accesskit-0.3.2/platforms/unix/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/executor.rs` & `accesskit-0.3.2/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/lib.rs` & `accesskit-0.3.2/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/unix/src/util.rs` & `accesskit-0.3.2/platforms/unix/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/Cargo.toml` & `accesskit-0.3.2/platforms/atspi-common/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.4.1"
+version = "0.4.2"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
+accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
```

### Comparing `accesskit-0.3.1/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.3.2/platforms/atspi-common/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,29 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.4.2](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.4.1...accesskit_atspi_common-v0.4.2) (2024-05-13)
+
+
+### Bug Fixes
+
+* Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
+* Return to handling focus events directly, after generic node changes ([#409](https://github.com/AccessKit/accesskit/issues/409)) ([cd2e35e](https://github.com/AccessKit/accesskit/commit/cd2e35e43817405199ae6acd64ef90aee445be0b))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.1 to 0.20.0
+
 ## [0.4.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.3.0...accesskit_atspi_common-v0.4.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
 * Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
```

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/adapter.rs` & `accesskit-0.3.2/platforms/atspi-common/src/adapter.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{ActionHandler, NodeId, Role, TreeUpdate};
-use accesskit_consumer::{DetachedNode, FilterResult, Node, Tree, TreeChangeHandler, TreeState};
+use accesskit_consumer::{FilterResult, Node, Tree, TreeChangeHandler, TreeState};
 use atspi_common::{InterfaceSet, Live, State};
 use std::sync::{
     atomic::{AtomicUsize, Ordering},
     Arc, RwLock,
 };
 
 use crate::{
     context::{ActionHandlerNoMut, ActionHandlerWrapper, AppContext, Context},
-    filters::{filter, filter_detached},
+    filters::filter,
     node::{NodeIdOrRoot, NodeWrapper, PlatformNode, PlatformRoot},
     util::WindowBounds,
     AdapterCallback, Event, ObjectEvent, WindowEvent,
 };
 
 struct AdapterChangeHandler<'a> {
     adapter: &'a Adapter,
 }
 
 impl AdapterChangeHandler<'_> {
     fn add_node(&mut self, node: &Node) {
         let role = node.role();
         let is_root = node.is_root();
-        let node = NodeWrapper::Node(node);
+        let node = NodeWrapper(node);
         let interfaces = node.interfaces();
         self.adapter.register_interfaces(node.id(), interfaces);
         if is_root && role == Role::Window {
             let adapter_index = self
                 .adapter
                 .context
                 .read_app_context()
@@ -45,18 +45,18 @@
             if let Some(name) = node.name() {
                 self.adapter
                     .emit_object_event(node.id(), ObjectEvent::Announcement(name, live));
             }
         }
     }
 
-    fn remove_node(&mut self, node: &DetachedNode) {
+    fn remove_node(&mut self, node: &Node) {
         let role = node.role();
         let is_root = node.is_root();
-        let node = NodeWrapper::DetachedNode(node);
+        let node = NodeWrapper(node);
         if is_root && role == Role::Window {
             self.adapter.window_destroyed(node.id());
         }
         self.adapter
             .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Defunct, true));
         self.adapter
             .unregister_interfaces(node.id(), node.interfaces());
@@ -66,57 +66,60 @@
 impl TreeChangeHandler for AdapterChangeHandler<'_> {
     fn node_added(&mut self, node: &Node) {
         if filter(node) == FilterResult::Include {
             self.add_node(node);
         }
     }
 
-    fn node_updated(&mut self, old_node: &DetachedNode, new_node: &Node) {
-        let filter_old = filter_detached(old_node);
+    fn node_updated(&mut self, old_node: &Node, new_node: &Node) {
+        let filter_old = filter(old_node);
         let filter_new = filter(new_node);
         if filter_new != filter_old {
             if filter_new == FilterResult::Include {
                 self.add_node(new_node);
             } else if filter_old == FilterResult::Include {
                 self.remove_node(old_node);
             }
         } else if filter_new == FilterResult::Include {
-            let old_wrapper = NodeWrapper::DetachedNode(old_node);
-            let new_wrapper = NodeWrapper::Node(new_node);
+            let old_wrapper = NodeWrapper(old_node);
+            let new_wrapper = NodeWrapper(new_node);
             let old_interfaces = old_wrapper.interfaces();
             let new_interfaces = new_wrapper.interfaces();
             let kept_interfaces = old_interfaces & new_interfaces;
             self.adapter
                 .unregister_interfaces(new_wrapper.id(), old_interfaces ^ kept_interfaces);
             self.adapter
                 .register_interfaces(new_node.id(), new_interfaces ^ kept_interfaces);
             let bounds = *self.adapter.context.read_root_window_bounds();
             new_wrapper.notify_changes(&bounds, self.adapter, &old_wrapper);
         }
     }
 
-    fn focus_moved(
-        &mut self,
-        old_node: Option<&DetachedNode>,
-        new_node: Option<&Node>,
-        current_state: &TreeState,
-    ) {
-        if let Some(root_window) = root_window(current_state) {
-            if old_node.is_none() && new_node.is_some() {
-                self.adapter
-                    .window_activated(&NodeWrapper::Node(&root_window));
-            } else if old_node.is_some() && new_node.is_none() {
-                self.adapter
-                    .window_deactivated(&NodeWrapper::Node(&root_window));
+    fn focus_moved(&mut self, old_node: Option<&Node>, new_node: Option<&Node>) {
+        if let (None, Some(new_node)) = (old_node, new_node) {
+            if let Some(root_window) = root_window(new_node.tree_state) {
+                self.adapter.window_activated(&NodeWrapper(&root_window));
             }
+        } else if let (Some(old_node), None) = (old_node, new_node) {
+            if let Some(root_window) = root_window(old_node.tree_state) {
+                self.adapter.window_deactivated(&NodeWrapper(&root_window));
+            }
+        }
+        if let Some(node) = new_node {
+            self.adapter
+                .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Focused, true));
+        }
+        if let Some(node) = old_node {
+            self.adapter
+                .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Focused, false));
         }
     }
 
-    fn node_removed(&mut self, node: &DetachedNode, _: &TreeState) {
-        if filter_detached(node) == FilterResult::Include {
+    fn node_removed(&mut self, node: &Node) {
+        if filter(node) == FilterResult::Include {
             self.remove_node(node);
         }
     }
 }
 
 static NEXT_ADAPTER_ID: AtomicUsize = AtomicUsize::new(0);
 
@@ -200,15 +203,15 @@
         adapter
     }
 
     fn register_tree(&self) {
         fn add_children(node: Node<'_>, to_add: &mut Vec<(NodeId, InterfaceSet)>) {
             for child in node.filtered_children(&filter) {
                 let child_id = child.id();
-                let wrapper = NodeWrapper::Node(&child);
+                let wrapper = NodeWrapper(&child);
                 let interfaces = wrapper.interfaces();
                 to_add.push((child_id, interfaces));
                 add_children(child, to_add);
             }
         }
 
         let mut objects_to_add = Vec::new();
@@ -219,15 +222,15 @@
             let mut app_context = self.context.write_app_context();
             app_context.name = tree_state.app_name();
             app_context.toolkit_name = tree_state.toolkit_name();
             app_context.toolkit_version = tree_state.toolkit_version();
             let adapter_index = app_context.adapter_index(self.id).unwrap();
             let root = tree_state.root();
             let root_id = root.id();
-            let wrapper = NodeWrapper::Node(&root);
+            let wrapper = NodeWrapper(&root);
             objects_to_add.push((root_id, wrapper.interfaces()));
             add_children(root, &mut objects_to_add);
             (adapter_index, root_id)
         };
 
         for (id, interfaces) in objects_to_add {
             self.register_interfaces(id, interfaces);
```

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/callback.rs` & `accesskit-0.3.2/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/context.rs` & `accesskit-0.3.2/platforms/atspi-common/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/error.rs` & `accesskit-0.3.2/platforms/atspi-common/src/error.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/events.rs` & `accesskit-0.3.2/platforms/atspi-common/src/events.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/lib.rs` & `accesskit-0.3.2/platforms/atspi-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/node.rs` & `accesskit-0.3.2/platforms/atspi-common/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,104 +8,85 @@
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 use accesskit::{
     Action, ActionData, ActionRequest, Affine, DefaultActionVerb, Live, NodeId, Point, Rect, Role,
     Toggled,
 };
-use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState, TreeState};
+use accesskit_consumer::{FilterResult, Node, TreeState};
 use atspi_common::{
     CoordType, Interface, InterfaceSet, Layer, Live as AtspiLive, Role as AtspiRole, State,
     StateSet,
 };
 use std::{
     hash::{Hash, Hasher},
     iter::FusedIterator,
     sync::{Arc, RwLock, RwLockReadGuard, Weak},
 };
 
 use crate::{
     adapter::Adapter,
     context::{AppContext, Context},
-    filters::{filter, filter_detached},
+    filters::filter,
     util::WindowBounds,
     Action as AtspiAction, Error, ObjectEvent, Property, Rect as AtspiRect, Result,
 };
 
-pub(crate) enum NodeWrapper<'a> {
-    Node(&'a Node<'a>),
-    DetachedNode(&'a DetachedNode),
-}
+pub(crate) struct NodeWrapper<'a>(pub(crate) &'a Node<'a>);
 
 impl<'a> NodeWrapper<'a> {
-    fn node_state(&self) -> &NodeState {
-        match self {
-            Self::Node(node) => node.state(),
-            Self::DetachedNode(node) => node.state(),
-        }
-    }
-
     pub(crate) fn name(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.name(),
-            Self::DetachedNode(node) => node.name(),
-        }
+        self.0.name()
     }
 
     pub(crate) fn description(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.description(),
-            Self::DetachedNode(node) => node.description(),
-        }
+        self.0.description()
     }
 
     pub(crate) fn parent_id(&self) -> Option<NodeId> {
-        self.node_state().parent_id()
+        self.0.parent_id()
     }
 
     pub(crate) fn id(&self) -> NodeId {
-        self.node_state().id()
+        self.0.id()
     }
 
     fn child_ids(
         &self,
     ) -> impl DoubleEndedIterator<Item = NodeId>
            + ExactSizeIterator<Item = NodeId>
            + FusedIterator<Item = NodeId>
            + '_ {
-        self.node_state().child_ids()
+        self.0.child_ids()
     }
 
     fn filtered_child_ids(
         &self,
     ) -> impl DoubleEndedIterator<Item = NodeId> + FusedIterator<Item = NodeId> + '_ {
-        match self {
-            Self::Node(node) => node.filtered_children(&filter).map(|child| child.id()),
-            _ => unreachable!(),
-        }
+        self.0.filtered_children(&filter).map(|child| child.id())
     }
 
     pub(crate) fn role(&self) -> AtspiRole {
-        if self.node_state().has_role_description() {
+        if self.0.has_role_description() {
             return AtspiRole::Extended;
         }
 
-        match self.node_state().role() {
+        match self.0.role() {
             Role::Alert => AtspiRole::Notification,
             Role::AlertDialog => AtspiRole::Alert,
             Role::Comment | Role::Suggestion => AtspiRole::Section,
             // TODO: See how to represent ARIA role="application"
             Role::Application => AtspiRole::Embedded,
             Role::Article => AtspiRole::Article,
             Role::Audio => AtspiRole::Audio,
             Role::Banner | Role::Header => AtspiRole::Landmark,
             Role::Blockquote => AtspiRole::BlockQuote,
             Role::Caret => AtspiRole::Unknown,
             Role::Button => {
-                if self.node_state().toggled().is_some() {
+                if self.0.toggled().is_some() {
                     AtspiRole::ToggleButton
                 } else {
                     AtspiRole::PushButton
                 }
             }
             Role::DefaultButton => AtspiRole::PushButton,
             Role::Canvas => AtspiRole::Canvas,
@@ -205,15 +186,14 @@
             // expose their descendants, and the descendants should be ignored. This
             // is because the alternative text depends on the counter style and can
             // be different from the actual (visual) marker text, and hence,
             // inconsistent with the descendants. We treat a list marker as non-text
             // only if it still has non-ignored descendants, which happens only when =>
             // - The list marker itself is ignored but the descendants are not
             // - Or the list marker contains images
-            // TODO: How to check for unignored children when the node is detached?
             Role::ListMarker => AtspiRole::Static,
             Role::Log => AtspiRole::Log,
             Role::Main => AtspiRole::Landmark,
             Role::Mark => AtspiRole::Static,
             Role::Math => AtspiRole::Math,
             Role::Marquee => AtspiRole::Marquee,
             Role::Menu | Role::MenuListPopup => AtspiRole::Menu,
@@ -297,35 +277,29 @@
             Role::Unknown => AtspiRole::Unknown,
             Role::ImeCandidate | Role::Keyboard => AtspiRole::RedundantObject,
             Role::Terminal => AtspiRole::Terminal,
         }
     }
 
     fn is_focused(&self) -> bool {
-        match self {
-            Self::Node(node) => node.is_focused(),
-            Self::DetachedNode(node) => node.is_focused(),
-        }
+        self.0.is_focused()
     }
 
     pub(crate) fn state(&self, is_window_focused: bool) -> StateSet {
-        let state = self.node_state();
+        let state = self.0;
         let atspi_role = self.role();
         let mut atspi_state = StateSet::empty();
         if state.parent_id().is_none() && state.role() == Role::Window && is_window_focused {
             atspi_state.insert(State::Active);
         }
         // TODO: Focus and selection.
         if state.is_focusable() {
             atspi_state.insert(State::Focusable);
         }
-        let filter_result = match self {
-            Self::Node(node) => filter(node),
-            Self::DetachedNode(node) => filter_detached(node),
-        };
+        let filter_result = filter(self.0);
         if filter_result == FilterResult::Include {
             atspi_state.insert(State::Visible | State::Showing);
         }
         if atspi_role != AtspiRole::ToggleButton && state.toggled().is_some() {
             atspi_state.insert(State::Checkable);
         }
         if let Some(selected) = state.is_selected() {
@@ -369,26 +343,23 @@
             atspi_state.insert(State::Focused);
         }
 
         atspi_state
     }
 
     fn is_root(&self) -> bool {
-        match self {
-            Self::Node(node) => node.is_root(),
-            Self::DetachedNode(node) => node.is_root(),
-        }
+        self.0.is_root()
     }
 
     fn supports_action(&self) -> bool {
-        self.node_state().default_action_verb().is_some()
+        self.0.default_action_verb().is_some()
     }
 
     fn supports_component(&self) -> bool {
-        self.node_state().raw_bounds().is_some() || self.is_root()
+        self.0.raw_bounds().is_some() || self.is_root()
     }
 
     fn supports_value(&self) -> bool {
         self.current_value().is_some()
     }
 
     pub(crate) fn interfaces(&self) -> InterfaceSet {
@@ -402,37 +373,34 @@
         if self.supports_value() {
             interfaces.insert(Interface::Value);
         }
         interfaces
     }
 
     pub(crate) fn live(&self) -> AtspiLive {
-        let live = match self {
-            Self::Node(node) => node.live(),
-            Self::DetachedNode(node) => node.live(),
-        };
+        let live = self.0.live();
         match live {
             Live::Off => AtspiLive::None,
             Live::Polite => AtspiLive::Polite,
             Live::Assertive => AtspiLive::Assertive,
         }
     }
 
     fn n_actions(&self) -> i32 {
-        match self.node_state().default_action_verb() {
+        match self.0.default_action_verb() {
             Some(_) => 1,
             None => 0,
         }
     }
 
     fn get_action_name(&self, index: i32) -> String {
         if index != 0 {
             return String::new();
         }
-        String::from(match self.node_state().default_action_verb() {
+        String::from(match self.0.default_action_verb() {
             Some(DefaultActionVerb::Click) => "click",
             Some(DefaultActionVerb::Focus) => "focus",
             Some(DefaultActionVerb::Check) => "check",
             Some(DefaultActionVerb::Uncheck) => "uncheck",
             Some(DefaultActionVerb::ClickAncestor) => "clickAncestor",
             Some(DefaultActionVerb::Jump) => "jump",
             Some(DefaultActionVerb::Open) => "open",
@@ -440,41 +408,38 @@
             Some(DefaultActionVerb::Select) => "select",
             Some(DefaultActionVerb::Unselect) => "unselect",
             None => "",
         })
     }
 
     fn raw_bounds_and_transform(&self) -> (Option<Rect>, Affine) {
-        let state = self.node_state();
+        let state = self.0;
         (state.raw_bounds(), state.direct_transform())
     }
 
     fn extents(&self, window_bounds: &WindowBounds) -> AtspiRect {
         if self.is_root() {
             return window_bounds.outer.into();
         }
-        match self {
-            Self::Node(node) => node.bounding_box().map_or_else(
-                || AtspiRect::INVALID,
-                |bounds| {
-                    let window_top_left = window_bounds.inner.origin();
-                    let node_origin = bounds.origin();
-                    let new_origin = Point::new(
-                        window_top_left.x + node_origin.x,
-                        window_top_left.y + node_origin.y,
-                    );
-                    bounds.with_origin(new_origin).into()
-                },
-            ),
-            _ => unreachable!(),
-        }
+        self.0.bounding_box().map_or_else(
+            || AtspiRect::INVALID,
+            |bounds| {
+                let window_top_left = window_bounds.inner.origin();
+                let node_origin = bounds.origin();
+                let new_origin = Point::new(
+                    window_top_left.x + node_origin.x,
+                    window_top_left.y + node_origin.y,
+                );
+                bounds.with_origin(new_origin).into()
+            },
+        )
     }
 
     fn current_value(&self) -> Option<f64> {
-        self.node_state().numeric_value()
+        self.0.numeric_value()
     }
 
     pub(crate) fn notify_changes(
         &self,
         window_bounds: &WindowBounds,
         adapter: &Adapter,
         old: &NodeWrapper<'_>,
@@ -486,14 +451,18 @@
     }
 
     fn notify_state_changes(&self, adapter: &Adapter, old: &NodeWrapper<'_>) {
         let old_state = old.state(true);
         let new_state = self.state(true);
         let changed_states = old_state ^ new_state;
         for state in changed_states.iter() {
+            if state == State::Focused {
+                // This is handled specially in `focus_moved`.
+                continue;
+            }
             adapter.emit_object_event(
                 self.id(),
                 ObjectEvent::StateChanged(state, new_state.contains(state)),
             );
         }
     }
 
@@ -518,19 +487,16 @@
                 ObjectEvent::PropertyChanged(Property::Description(
                     description.unwrap_or_default(),
                 )),
             );
         }
         let parent_id = self.parent_id();
         if parent_id != old.parent_id() {
-            let node = match self {
-                NodeWrapper::Node(node) => node,
-                _ => unreachable!(),
-            };
-            let parent = node
+            let parent = self
+                .0
                 .filtered_parent(&filter)
                 .map_or(NodeIdOrRoot::Root, |node| NodeIdOrRoot::Node(node.id()));
             adapter.emit_object_event(
                 self.id(),
                 ObjectEvent::PropertyChanged(Property::Parent(parent)),
             );
         }
@@ -662,22 +628,22 @@
         } else {
             Err(Error::Defunct)
         }
     }
 
     pub fn name(&self) -> Result<String> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.name().unwrap_or_default())
         })
     }
 
     pub fn description(&self) -> Result<String> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.description().unwrap_or_default())
         })
     }
 
     pub fn relative(&self, id: NodeId) -> Self {
         Self {
             context: self.context.clone(),
@@ -752,76 +718,76 @@
             i32::try_from(node.preceding_filtered_siblings(&filter).count())
                 .map_err(|_| Error::IndexOutOfRange)
         })
     }
 
     pub fn role(&self) -> Result<AtspiRole> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.role())
         })
     }
 
     pub fn localized_role_name(&self) -> Result<String> {
-        self.resolve(|node| Ok(node.state().role_description().unwrap_or_default()))
+        self.resolve(|node| Ok(node.role_description().unwrap_or_default()))
     }
 
     pub fn state(&self) -> StateSet {
         self.resolve_with_context(|node, context| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.state(context.read_tree().state().focus_id().is_some()))
         })
         .unwrap_or(State::Defunct.into())
     }
 
     pub fn supports_action(&self) -> Result<bool> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_action())
         })
     }
 
     pub fn supports_component(&self) -> Result<bool> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_component())
         })
     }
 
     pub fn supports_value(&self) -> Result<bool> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_value())
         })
     }
 
     pub fn interfaces(&self) -> Result<InterfaceSet> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.interfaces())
         })
     }
 
     pub fn n_actions(&self) -> Result<i32> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.n_actions())
         })
     }
 
     pub fn action_name(&self, index: i32) -> Result<String> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.get_action_name(index))
         })
     }
 
     pub fn actions(&self) -> Result<Vec<AtspiAction>> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             let n_actions = wrapper.n_actions() as usize;
             let mut actions = Vec::with_capacity(n_actions);
             for i in 0..n_actions {
                 actions.push(AtspiAction {
                     localized_name: wrapper.get_action_name(i as i32),
                     description: "".into(),
                     key_binding: "".into(),
@@ -903,15 +869,15 @@
                 _ => Err(Error::UnsupportedInterface),
             }
         })
     }
 
     pub fn layer(&self) -> Result<Layer> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             if wrapper.role() == AtspiRole::Window {
                 Ok(Layer::Window)
             } else {
                 Ok(Layer::Widget)
             }
         })
     }
@@ -937,28 +903,28 @@
                 data: Some(ActionData::ScrollToPoint(point)),
             }
         })?;
         Ok(true)
     }
 
     pub fn minimum_value(&self) -> Result<f64> {
-        self.resolve(|node| Ok(node.state().min_numeric_value().unwrap_or(f64::MIN)))
+        self.resolve(|node| Ok(node.min_numeric_value().unwrap_or(f64::MIN)))
     }
 
     pub fn maximum_value(&self) -> Result<f64> {
-        self.resolve(|node| Ok(node.state().max_numeric_value().unwrap_or(f64::MAX)))
+        self.resolve(|node| Ok(node.max_numeric_value().unwrap_or(f64::MAX)))
     }
 
     pub fn minimum_increment(&self) -> Result<f64> {
-        self.resolve(|node| Ok(node.state().numeric_value_step().unwrap_or(0.0)))
+        self.resolve(|node| Ok(node.numeric_value_step().unwrap_or(0.0)))
     }
 
     pub fn current_value(&self) -> Result<f64> {
         self.resolve(|node| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             Ok(wrapper.current_value().unwrap_or(0.0))
         })
     }
 
     pub fn set_current_value(&self, value: f64) -> Result<()> {
         self.do_action_internal(|_, _| ActionRequest {
             action: Action::SetValue,
```

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/rect.rs` & `accesskit-0.3.2/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/simplified.rs` & `accesskit-0.3.2/platforms/atspi-common/src/simplified.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/atspi-common/src/util.rs` & `accesskit-0.3.2/platforms/atspi-common/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/common/Cargo.toml` & `accesskit-0.3.2/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/common/CHANGELOG.md` & `accesskit-0.3.2/common/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/common/README.md` & `accesskit-0.3.2/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/common/src/geometry.rs` & `accesskit-0.3.2/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/common/src/lib.rs` & `accesskit-0.3.2/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/Cargo.toml` & `accesskit-0.3.2/platforms/macos/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_macos"
-version = "0.13.1"
+version = "0.13.2"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: macOS adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -12,15 +12,15 @@
 rust-version.workspace = true
 
 [package.metadata.docs.rs]
 default-target = "x86_64-apple-darwin"
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
+accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
 once_cell = "1.13.0"
 objc2 = "0.5.1"
 objc2-foundation = { version = "0.2.0", features = [
     "NSArray",
     "NSDictionary",
     "NSValue",
     "NSThread",
```

### Comparing `accesskit-0.3.1/platforms/macos/CHANGELOG.md` & `accesskit-0.3.2/platforms/macos/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,28 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.13.2](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.13.1...accesskit_macos-v0.13.2) (2024-05-13)
+
+
+### Bug Fixes
+
+* Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.1 to 0.20.0
+
 ## [0.13.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.12.0...accesskit_macos-v0.13.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
 * Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
```

### Comparing `accesskit-0.3.1/platforms/macos/src/adapter.rs` & `accesskit-0.3.2/platforms/macos/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/src/context.rs` & `accesskit-0.3.2/platforms/macos/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/src/event.rs` & `accesskit-0.3.2/platforms/macos/src/event.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{Live, NodeId, Role};
-use accesskit_consumer::{DetachedNode, FilterResult, Node, TreeChangeHandler, TreeState};
+use accesskit_consumer::{FilterResult, Node, TreeChangeHandler};
 use objc2::runtime::{AnyObject, ProtocolObject};
 use objc2_app_kit::*;
 use objc2_foundation::{NSMutableDictionary, NSNumber, NSString};
 use std::{collections::HashSet, rc::Rc};
 
-use crate::{
-    context::Context,
-    filters::{filter, filter_detached},
-    node::NodeWrapper,
-};
+use crate::{context::Context, filters::filter, node::NodeWrapper};
 
 // This type is designed to be safe to create on a non-main thread
 // and send to the main thread. This ability isn't yet used though.
 pub(crate) enum QueuedEvent {
     Generic {
         node_id: NodeId,
         notification: &'static NSAccessibilityNotificationName,
@@ -180,53 +176,38 @@
         if node.role() != Role::InlineTextBox {
             return;
         }
         if let Some(node) = node.filtered_parent(&filter) {
             self.insert_text_change_if_needed_parent(node);
         }
     }
-
-    fn insert_text_change_if_needed_for_removed_node(
-        &mut self,
-        node: &DetachedNode,
-        current_state: &TreeState,
-    ) {
-        if node.role() != Role::InlineTextBox {
-            return;
-        }
-        if let Some(id) = node.parent_id() {
-            if let Some(node) = current_state.node_by_id(id) {
-                self.insert_text_change_if_needed_parent(node);
-            }
-        }
-    }
 }
 
 impl TreeChangeHandler for EventGenerator {
     fn node_added(&mut self, node: &Node) {
         self.insert_text_change_if_needed(node);
         if filter(node) != FilterResult::Include {
             return;
         }
         if node.name().is_some() && node.live() != Live::Off {
             self.events
                 .push(QueuedEvent::live_region_announcement(node));
         }
     }
 
-    fn node_updated(&mut self, old_node: &DetachedNode, new_node: &Node) {
+    fn node_updated(&mut self, old_node: &Node, new_node: &Node) {
         if old_node.raw_value() != new_node.raw_value() {
             self.insert_text_change_if_needed(new_node);
         }
         if filter(new_node) != FilterResult::Include {
             return;
         }
         let node_id = new_node.id();
-        let old_wrapper = NodeWrapper::DetachedNode(old_node);
-        let new_wrapper = NodeWrapper::Node(new_node);
+        let old_wrapper = NodeWrapper(old_node);
+        let new_wrapper = NodeWrapper(new_node);
         if old_wrapper.title() != new_wrapper.title() {
             self.events.push(QueuedEvent::Generic {
                 node_id,
                 notification: unsafe { NSAccessibilityTitleChangedNotification },
             });
         }
         if old_wrapper.value() != new_wrapper.value() {
@@ -244,33 +225,28 @@
                 notification: unsafe { NSAccessibilitySelectedTextChangedNotification },
             });
         }
         if new_node.name().is_some()
             && new_node.live() != Live::Off
             && (new_node.name() != old_node.name()
                 || new_node.live() != old_node.live()
-                || filter_detached(old_node) != FilterResult::Include)
+                || filter(old_node) != FilterResult::Include)
         {
             self.events
                 .push(QueuedEvent::live_region_announcement(new_node));
         }
     }
 
-    fn focus_moved(
-        &mut self,
-        _old_node: Option<&DetachedNode>,
-        new_node: Option<&Node>,
-        _current_state: &TreeState,
-    ) {
+    fn focus_moved(&mut self, _old_node: Option<&Node>, new_node: Option<&Node>) {
         if let Some(new_node) = new_node {
             if filter(new_node) != FilterResult::Include {
                 return;
             }
             self.events.push(focus_event(new_node.id()));
         }
     }
 
-    fn node_removed(&mut self, node: &DetachedNode, current_state: &TreeState) {
-        self.insert_text_change_if_needed_for_removed_node(node, current_state);
+    fn node_removed(&mut self, node: &Node) {
+        self.insert_text_change_if_needed(node);
         self.events.push(QueuedEvent::NodeDestroyed(node.id()));
     }
 }
```

### Comparing `accesskit-0.3.1/platforms/macos/src/lib.rs` & `accesskit-0.3.2/platforms/macos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/src/node.rs` & `accesskit-0.3.2/platforms/macos/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 // Copyright 2018 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
 use accesskit::{Action, ActionData, ActionRequest, NodeId, Role, TextSelection, Toggled};
-use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState};
+use accesskit_consumer::{FilterResult, Node};
 use objc2::{
     declare_class, msg_send_id,
     mutability::InteriorMutable,
     rc::Id,
     runtime::{AnyObject, Sel},
     sel, ClassType, DeclaredClass,
 };
@@ -24,16 +24,16 @@
     ns_string, NSArray, NSCopying, NSInteger, NSNumber, NSObject, NSPoint, NSRange, NSRect,
     NSString,
 };
 use std::rc::{Rc, Weak};
 
 use crate::{context::Context, filters::filter, util::*};
 
-fn ns_role(node_state: &NodeState) -> &'static NSAccessibilityRole {
-    let role = node_state.role();
+fn ns_role(node: &Node) -> &'static NSAccessibilityRole {
+    let role = node.role();
     // TODO: Handle special cases.
     unsafe {
         match role {
             Role::Unknown => NSAccessibilityUnknownRole,
             Role::InlineTextBox => NSAccessibilityUnknownRole,
             Role::Cell => NSAccessibilityCellRole,
             Role::StaticText => NSAccessibilityStaticTextRole,
@@ -54,15 +54,15 @@
             | Role::SearchInput
             | Role::EmailInput
             | Role::NumberInput
             | Role::PasswordInput
             | Role::PhoneNumberInput
             | Role::UrlInput => NSAccessibilityTextFieldRole,
             Role::Button => {
-                if node_state.toggled().is_some() {
+                if node.toggled().is_some() {
                     NSAccessibilityCheckBoxRole
                 } else {
                     NSAccessibilityButtonRole
                 }
             }
             Role::DefaultButton => NSAccessibilityButtonRole,
             Role::Pane => NSAccessibilityUnknownRole,
@@ -237,75 +237,53 @@
 #[derive(PartialEq)]
 pub(crate) enum Value {
     Bool(bool),
     Number(f64),
     String(String),
 }
 
-pub(crate) enum NodeWrapper<'a> {
-    Node(&'a Node<'a>),
-    DetachedNode(&'a DetachedNode),
-}
+pub(crate) struct NodeWrapper<'a>(pub(crate) &'a Node<'a>);
 
 impl<'a> NodeWrapper<'a> {
-    fn node_state(&self) -> &'a NodeState {
-        match self {
-            Self::Node(node) => node.state(),
-            Self::DetachedNode(node) => node.state(),
-        }
-    }
-
     fn is_root(&self) -> bool {
-        match self {
-            Self::Node(node) => node.is_root(),
-            Self::DetachedNode(node) => node.is_root(),
-        }
+        self.0.is_root()
     }
 
     fn name(&self) -> Option<String> {
-        if self.is_root() && self.node_state().role() == Role::Window {
+        if self.is_root() && self.0.role() == Role::Window {
             // If the group element that we expose for the top-level window
             // includes a title, VoiceOver behavior is broken.
             return None;
         }
-        match self {
-            Self::Node(node) => node.name(),
-            Self::DetachedNode(node) => node.name(),
-        }
+        self.0.name()
     }
 
     fn node_value(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.value(),
-            Self::DetachedNode(node) => node.value(),
-        }
+        self.0.value()
     }
 
     // TODO: implement proper logic for title and value;
     // see Chromium's content/browser/accessibility/browser_accessibility_cocoa.mm
     // and figure out how this is different in the macOS 10.10+ protocol
 
     pub(crate) fn title(&self) -> Option<String> {
-        let state = self.node_state();
+        let state = self.0;
         if state.role() == Role::StaticText && state.raw_value().is_none() {
             // In this case, macOS wants the text to be the value, not title.
             return None;
         }
         self.name()
     }
 
     pub(crate) fn description(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.description(),
-            Self::DetachedNode(node) => node.description(),
-        }
+        self.0.description()
     }
 
     pub(crate) fn value(&self) -> Option<Value> {
-        let state = self.node_state();
+        let state = self.0;
         if let Some(toggled) = state.toggled() {
             return Some(Value::Bool(toggled != Toggled::False));
         }
         if let Some(value) = self.node_value() {
             return Some(Value::String(value));
         }
         if let Some(value) = state.numeric_value() {
@@ -316,22 +294,19 @@
                 return Some(Value::String(name));
             }
         }
         None
     }
 
     pub(crate) fn supports_text_ranges(&self) -> bool {
-        match self {
-            Self::Node(node) => node.supports_text_ranges(),
-            Self::DetachedNode(node) => node.supports_text_ranges(),
-        }
+        self.0.supports_text_ranges()
     }
 
     pub(crate) fn raw_text_selection(&self) -> Option<&TextSelection> {
-        self.node_state().raw_text_selection()
+        self.0.raw_text_selection()
     }
 }
 
 pub(crate) struct PlatformNodeIvars {
     context: Weak<Context>,
     node_id: NodeId,
 }
@@ -399,15 +374,15 @@
                 )
             })
             .unwrap_or(NSRect::ZERO)
         }
 
         #[method_id(accessibilityRole)]
         fn role(&self) -> Id<NSAccessibilityRole> {
-            self.resolve(|node| ns_role(node.state()))
+            self.resolve(ns_role)
                 .unwrap_or(unsafe { NSAccessibilityUnknownRole })
                 .copy()
         }
 
         #[method_id(accessibilityRoleDescription)]
         fn role_description(&self) -> Option<Id<NSString>> {
             self.resolve(|node| {
@@ -419,33 +394,33 @@
             })
             .flatten()
         }
 
         #[method_id(accessibilityTitle)]
         fn title(&self) -> Option<Id<NSString>> {
             self.resolve(|node| {
-                let wrapper = NodeWrapper::Node(node);
+                let wrapper = NodeWrapper(node);
                 wrapper.title().map(|title| NSString::from_str(&title))
             })
             .flatten()
         }
 
         #[method_id(accessibilityHelp)]
         fn description(&self) -> Option<Id<NSString>> {
             self.resolve(|node| {
-                let wrapper = NodeWrapper::Node(node);
+                let wrapper = NodeWrapper(node);
                 wrapper.description().map(|description| NSString::from_str(&description))
             })
             .flatten()
         }
 
         #[method_id(accessibilityValue)]
         fn value(&self) -> Option<Id<NSObject>> {
             self.resolve(|node| {
-                let wrapper = NodeWrapper::Node(node);
+                let wrapper = NodeWrapper(node);
                 wrapper.value().map(|value| match value {
                     Value::Bool(value) => {
                         Id::into_super(Id::into_super(NSNumber::new_bool(value)))
                     }
                     Value::Number(value) => {
                         Id::into_super(Id::into_super(NSNumber::new_f64(value)))
                     }
```

### Comparing `accesskit-0.3.1/platforms/macos/src/patch.rs` & `accesskit-0.3.2/platforms/macos/src/patch.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/src/subclass.rs` & `accesskit-0.3.2/platforms/macos/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/macos/src/util.rs` & `accesskit-0.3.2/platforms/macos/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/Cargo.toml` & `accesskit-0.3.2/platforms/windows/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.18.1"
+version = "0.18.2"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
+accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
```

### Comparing `accesskit-0.3.1/platforms/windows/CHANGELOG.md` & `accesskit-0.3.2/platforms/windows/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,28 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.18.2](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.1...accesskit_windows-v0.18.2) (2024-05-13)
+
+
+### Bug Fixes
+
+* Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.1 to 0.20.0
+
 ## [0.18.1](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.0...accesskit_windows-v0.18.1) (2024-05-11)
 
 
 ### Bug Fixes
 
 * Make the transition from placeholder to real tree more robust ([#405](https://github.com/AccessKit/accesskit/issues/405)) ([928e11d](https://github.com/AccessKit/accesskit/commit/928e11d00e7c60b3cafcc0ac623f6377b36f7ea7))
```

### Comparing `accesskit-0.3.1/platforms/windows/examples/hello_world.rs` & `accesskit-0.3.2/platforms/windows/examples/hello_world.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/adapter.rs` & `accesskit-0.3.2/platforms/windows/src/adapter.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
     ActionHandler, ActivationHandler, Live, NodeBuilder, NodeId, Role, Tree as TreeData, TreeUpdate,
 };
-use accesskit_consumer::{DetachedNode, FilterResult, Node, Tree, TreeChangeHandler, TreeState};
+use accesskit_consumer::{FilterResult, Node, Tree, TreeChangeHandler};
 use std::{
     collections::HashSet,
     sync::{atomic::Ordering, Arc},
 };
 use windows::Win32::{
     Foundation::*,
     UI::{Accessibility::*, WindowsAndMessaging::*},
 };
 
 use crate::{
     context::{ActionHandlerNoMut, ActionHandlerWrapper, Context},
-    filters::{filter, filter_detached},
+    filters::filter,
     node::{NodeWrapper, PlatformNode},
     util::QueuedEvent,
 };
 
 fn focus_event(context: &Arc<Context>, node_id: NodeId) -> QueuedEvent {
     let platform_node = PlatformNode::new(context, node_id);
     let element: IRawElementProviderSimple = platform_node.into();
@@ -76,29 +76,14 @@
         if node.role() != Role::InlineTextBox {
             return;
         }
         if let Some(node) = node.filtered_parent(&filter) {
             self.insert_text_change_if_needed_parent(node);
         }
     }
-
-    fn insert_text_change_if_needed_for_removed_node(
-        &mut self,
-        node: &DetachedNode,
-        current_state: &TreeState,
-    ) {
-        if node.role() != Role::InlineTextBox {
-            return;
-        }
-        if let Some(id) = node.parent_id() {
-            if let Some(node) = current_state.node_by_id(id) {
-                self.insert_text_change_if_needed_parent(node);
-            }
-        }
-    }
 }
 
 impl TreeChangeHandler for AdapterChangeHandler<'_> {
     fn node_added(&mut self, node: &Node) {
         self.insert_text_change_if_needed(node);
         if filter(node) != FilterResult::Include {
             return;
@@ -109,52 +94,47 @@
             self.queue.push(QueuedEvent::Simple {
                 element,
                 event_id: UIA_LiveRegionChangedEventId,
             });
         }
     }
 
-    fn node_updated(&mut self, old_node: &DetachedNode, new_node: &Node) {
+    fn node_updated(&mut self, old_node: &Node, new_node: &Node) {
         if old_node.raw_value() != new_node.raw_value() {
             self.insert_text_change_if_needed(new_node);
         }
         if filter(new_node) != FilterResult::Include {
             return;
         }
         let platform_node = PlatformNode::new(self.context, new_node.id());
         let element: IRawElementProviderSimple = platform_node.into();
-        let old_wrapper = NodeWrapper::DetachedNode(old_node);
-        let new_wrapper = NodeWrapper::Node(new_node);
+        let old_wrapper = NodeWrapper(old_node);
+        let new_wrapper = NodeWrapper(new_node);
         new_wrapper.enqueue_property_changes(&mut self.queue, &element, &old_wrapper);
         if new_node.name().is_some()
             && new_node.live() != Live::Off
             && (new_node.name() != old_node.name()
                 || new_node.live() != old_node.live()
-                || filter_detached(old_node) != FilterResult::Include)
+                || filter(old_node) != FilterResult::Include)
         {
             self.queue.push(QueuedEvent::Simple {
                 element,
                 event_id: UIA_LiveRegionChangedEventId,
             });
         }
     }
 
-    fn focus_moved(
-        &mut self,
-        _old_node: Option<&DetachedNode>,
-        new_node: Option<&Node>,
-        _current_state: &TreeState,
-    ) {
+    fn focus_moved(&mut self, _old_node: Option<&Node>, new_node: Option<&Node>) {
         if let Some(new_node) = new_node {
             self.queue.push(focus_event(self.context, new_node.id()));
         }
     }
 
-    fn node_removed(&mut self, node: &DetachedNode, current_state: &TreeState) {
-        self.insert_text_change_if_needed_for_removed_node(node, current_state);
+    fn node_removed(&mut self, node: &Node) {
+        self.insert_text_change_if_needed(node);
     }
 
     // TODO: handle other events (#20)
 }
 
 const PLACEHOLDER_ROOT_ID: NodeId = NodeId(0);
```

### Comparing `accesskit-0.3.1/platforms/windows/src/context.rs` & `accesskit-0.3.2/platforms/windows/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/node.rs` & `accesskit-0.3.2/platforms/windows/src/node.rs`

 * *Files 17% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
 use accesskit::{
     Action, ActionData, ActionRequest, Live, NodeId, NodeIdContent, Point, Role, Toggled,
 };
-use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState, TreeState};
+use accesskit_consumer::{FilterResult, Node, TreeState};
 use paste::paste;
 use std::sync::{atomic::Ordering, Arc, Weak};
 use windows::{
     core::*,
     Win32::{Foundation::*, System::Com::*, UI::Accessibility::*},
 };
 
 use crate::{
     context::Context,
-    filters::{filter, filter_detached, filter_with_root_exception},
+    filters::{filter, filter_with_root_exception},
     text::PlatformRange as PlatformTextRange,
     util::*,
 };
 
 const RUNTIME_ID_SIZE: usize = 3;
 
 fn runtime_id_from_node_id(id: NodeId) -> [i32; RUNTIME_ID_SIZE] {
@@ -36,29 +36,19 @@
     [
         UiaAppendRuntimeId as _,
         ((id >> 32) & 0xFFFFFFFF) as _,
         (id & 0xFFFFFFFF) as _,
     ]
 }
 
-pub(crate) enum NodeWrapper<'a> {
-    Node(&'a Node<'a>),
-    DetachedNode(&'a DetachedNode),
-}
+pub(crate) struct NodeWrapper<'a>(pub(crate) &'a Node<'a>);
 
 impl<'a> NodeWrapper<'a> {
-    fn node_state(&self) -> &'a NodeState {
-        match self {
-            Self::Node(node) => node.state(),
-            Self::DetachedNode(node) => node.state(),
-        }
-    }
-
     fn control_type(&self) -> UIA_CONTROLTYPE_ID {
-        let role = self.node_state().role();
+        let role = self.0.role();
         // TODO: Handle special cases. (#14)
         match role {
             Role::Unknown => UIA_CustomControlTypeId,
             Role::InlineTextBox => UIA_CustomControlTypeId,
             Role::Cell => UIA_DataItemControlTypeId,
             Role::StaticText => UIA_TextControlTypeId,
             Role::Image => UIA_ImageControlTypeId,
@@ -260,171 +250,143 @@
             Role::DocTip => UIA_GroupControlTypeId,
             Role::DocToc => UIA_GroupControlTypeId,
             Role::ListGrid => UIA_DataGridControlTypeId,
         }
     }
 
     fn localized_control_type(&self) -> Option<String> {
-        self.node_state().role_description()
+        self.0.role_description()
     }
 
     fn name(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.name(),
-            Self::DetachedNode(node) => node.name(),
-        }
+        self.0.name()
     }
 
     fn description(&self) -> Option<String> {
-        match self {
-            Self::Node(node) => node.description(),
-            Self::DetachedNode(node) => node.description(),
-        }
+        self.0.description()
     }
 
     fn is_content_element(&self) -> bool {
-        let result = match self {
-            Self::Node(node) => filter(node),
-            Self::DetachedNode(node) => filter_detached(node),
-        };
-        result == FilterResult::Include
+        filter(self.0) == FilterResult::Include
     }
 
     fn is_enabled(&self) -> bool {
-        !self.node_state().is_disabled()
+        !self.0.is_disabled()
     }
 
     fn is_focusable(&self) -> bool {
-        self.node_state().is_focusable()
+        self.0.is_focusable()
     }
 
     fn is_focused(&self) -> bool {
-        match self {
-            Self::Node(node) => node.is_focused(),
-            Self::DetachedNode(node) => node.is_focused(),
-        }
+        self.0.is_focused()
     }
 
     fn live_setting(&self) -> LiveSetting {
-        let live = match self {
-            Self::Node(node) => node.live(),
-            Self::DetachedNode(node) => node.live(),
-        };
+        let live = self.0.live();
         match live {
             Live::Off => Off,
             Live::Polite => Polite,
             Live::Assertive => Assertive,
         }
     }
 
     fn class_name(&self) -> Option<&str> {
-        self.node_state().class_name()
+        self.0.class_name()
     }
 
     fn is_toggle_pattern_supported(&self) -> bool {
-        self.node_state().toggled().is_some() && !self.is_selection_item_pattern_supported()
+        self.0.toggled().is_some() && !self.is_selection_item_pattern_supported()
     }
 
     fn toggle_state(&self) -> ToggleState {
-        match self.node_state().toggled().unwrap() {
+        match self.0.toggled().unwrap() {
             Toggled::False => ToggleState_Off,
             Toggled::True => ToggleState_On,
             Toggled::Mixed => ToggleState_Indeterminate,
         }
     }
 
     fn is_invoke_pattern_supported(&self) -> bool {
-        self.node_state().is_invocable()
+        self.0.is_invocable()
     }
 
     fn is_value_pattern_supported(&self) -> bool {
-        match self {
-            Self::Node(node) => node.has_value(),
-            Self::DetachedNode(node) => node.has_value(),
-        }
+        self.0.has_value()
     }
 
     fn is_range_value_pattern_supported(&self) -> bool {
-        self.node_state().numeric_value().is_some()
+        self.0.numeric_value().is_some()
     }
 
     fn value(&self) -> String {
-        match self {
-            Self::Node(node) => node.value().unwrap(),
-            Self::DetachedNode(node) => node.value().unwrap(),
-        }
+        self.0.value().unwrap()
     }
 
     fn is_read_only(&self) -> bool {
-        self.node_state().is_read_only()
+        self.0.is_read_only()
     }
 
     fn numeric_value(&self) -> f64 {
-        self.node_state().numeric_value().unwrap()
+        self.0.numeric_value().unwrap()
     }
 
     fn min_numeric_value(&self) -> f64 {
-        self.node_state().min_numeric_value().unwrap_or(0.0)
+        self.0.min_numeric_value().unwrap_or(0.0)
     }
 
     fn max_numeric_value(&self) -> f64 {
-        self.node_state().max_numeric_value().unwrap_or(0.0)
+        self.0.max_numeric_value().unwrap_or(0.0)
     }
 
     fn numeric_value_step(&self) -> f64 {
-        self.node_state().numeric_value_step().unwrap_or(0.0)
+        self.0.numeric_value_step().unwrap_or(0.0)
     }
 
     fn numeric_value_jump(&self) -> f64 {
-        self.node_state()
+        self.0
             .numeric_value_jump()
             .unwrap_or_else(|| self.numeric_value_step())
     }
 
     fn is_selection_item_pattern_supported(&self) -> bool {
-        match self.node_state().role() {
+        match self.0.role() {
             // TODO: tables (#29)
             // https://www.w3.org/TR/core-aam-1.1/#mapping_state-property_table
             // SelectionItem.IsSelected is exposed when aria-checked is True or
             // False, for 'radio' and 'menuitemradio' roles.
-            Role::RadioButton | Role::MenuItemRadio => matches!(
-                self.node_state().toggled(),
-                Some(Toggled::True | Toggled::False)
-            ),
+            Role::RadioButton | Role::MenuItemRadio => {
+                matches!(self.0.toggled(), Some(Toggled::True | Toggled::False))
+            }
             // https://www.w3.org/TR/wai-aria-1.1/#aria-selected
             // SelectionItem.IsSelected is exposed when aria-select is True or False.
             Role::ListBoxOption
             | Role::ListItem
             | Role::MenuListOption
             | Role::Tab
-            | Role::TreeItem => self.node_state().is_selected().is_some(),
+            | Role::TreeItem => self.0.is_selected().is_some(),
             _ => false,
         }
     }
 
     fn is_selected(&self) -> bool {
-        match self.node_state().role() {
+        match self.0.role() {
             // https://www.w3.org/TR/core-aam-1.1/#mapping_state-property_table
             // SelectionItem.IsSelected is set according to the True or False
             // value of aria-checked for 'radio' and 'menuitemradio' roles.
-            Role::RadioButton | Role::MenuItemRadio => {
-                self.node_state().toggled() == Some(Toggled::True)
-            }
+            Role::RadioButton | Role::MenuItemRadio => self.0.toggled() == Some(Toggled::True),
             // https://www.w3.org/TR/wai-aria-1.1/#aria-selected
             // SelectionItem.IsSelected is set according to the True or False
             // value of aria-selected.
-            _ => self.node_state().is_selected().unwrap_or(false),
+            _ => self.0.is_selected().unwrap_or(false),
         }
     }
 
     fn is_text_pattern_supported(&self) -> bool {
-        match self {
-            Self::Node(node) => node.supports_text_ranges(),
-            Self::DetachedNode(node) => node.supports_text_ranges(),
-        }
+        self.0.supports_text_ranges()
     }
 
     pub(crate) fn enqueue_property_changes(
         &self,
         queue: &mut Vec<QueuedEvent>,
         element: &IRawElementProviderSimple,
         old: &NodeWrapper,
@@ -447,15 +409,15 @@
             queue.push(QueuedEvent::Simple {
                 element: element.clone(),
                 event_id: UIA_SelectionItem_ElementSelectedEventId,
             });
         }
         if self.is_text_pattern_supported()
             && old.is_text_pattern_supported()
-            && self.node_state().raw_text_selection() != old.node_state().raw_text_selection()
+            && self.0.raw_text_selection() != old.0.raw_text_selection()
         {
             queue.push(QueuedEvent::Simple {
                 element: element.clone(),
                 event_id: UIA_Text_TextSelectionChangedEventId,
             });
         }
     }
@@ -642,15 +604,15 @@
 
     fn GetPatternProvider(&self, pattern_id: UIA_PATTERN_ID) -> Result<IUnknown> {
         self.pattern_provider(pattern_id)
     }
 
     fn GetPropertyValue(&self, property_id: UIA_PROPERTY_ID) -> Result<VARIANT> {
         self.resolve_with_tree_state_and_context(|node, state, context| {
-            let wrapper = NodeWrapper::Node(&node);
+            let wrapper = NodeWrapper(&node);
             let mut result = wrapper.get_property_value(property_id);
             if result.is_empty() {
                 if node.is_root() {
                     match property_id {
                         UIA_NamePropertyId => {
                             result = window_title(context.hwnd).into();
                         }
@@ -826,15 +788,15 @@
         $(($base_property_id:ident, $getter:ident, $com_type:ident)),*
     ), (
         $($extra_trait_method:item),*
     ))),+) => {
         impl PlatformNode {
             fn pattern_provider(&self, pattern_id: UIA_PATTERN_ID) -> Result<IUnknown> {
                 self.resolve(|node| {
-                    let wrapper = NodeWrapper::Node(&node);
+                    let wrapper = NodeWrapper(&node);
                     match pattern_id {
                         $(paste! { [< UIA_ $base_pattern_id PatternId>] } => {
                             if wrapper.$is_supported() {
                                 // SAFETY: We know we're running inside a full COM implementation.
                                 let intermediate: paste! { [< I $base_pattern_id Provider>] } =
                                     unsafe { self.cast() }?;
                                 return intermediate.cast();
@@ -871,15 +833,15 @@
             }
         }
         paste! {
             $(#[allow(non_snake_case)]
             impl [< I $base_pattern_id Provider_Impl>] for PlatformNode {
                 $(fn $base_property_id(&self) -> Result<$com_type> {
                     self.resolve(|node| {
-                        let wrapper = NodeWrapper::Node(&node);
+                        let wrapper = NodeWrapper(&node);
                         Ok(wrapper.$getter().into())
                     })
                 })*
                 $($extra_trait_method)*
             })*
         }
     };
```

### Comparing `accesskit-0.3.1/platforms/windows/src/subclass.rs` & `accesskit-0.3.2/platforms/windows/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/tests/mod.rs` & `accesskit-0.3.2/platforms/windows/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/tests/simple.rs` & `accesskit-0.3.2/platforms/windows/src/tests/simple.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.3.2/platforms/windows/src/tests/subclassed.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/text.rs` & `accesskit-0.3.2/platforms/windows/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/platforms/windows/src/util.rs` & `accesskit-0.3.2/platforms/windows/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/consumer/CHANGELOG.md` & `accesskit-0.3.2/consumer/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,30 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.20.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.19.1...accesskit_consumer-v0.20.0) (2024-05-13)
+
+
+### ⚠ BREAKING CHANGES
+
+* Restore full copy-on-write tree snapshots, now using `immutable-chunkmap` ([#365](https://github.com/AccessKit/accesskit/issues/365))
+
+### Bug Fixes
+
+* Fix the filtered sibling iterators to use the filtered parent to find the back node ([#408](https://github.com/AccessKit/accesskit/issues/408)) ([2f8155c](https://github.com/AccessKit/accesskit/commit/2f8155ca260d7e50de5de502744b420769875e83))
+
+
+### Code Refactoring
+
+* Restore full copy-on-write tree snapshots, now using `immutable-chunkmap` ([#365](https://github.com/AccessKit/accesskit/issues/365)) ([441bf5f](https://github.com/AccessKit/accesskit/commit/441bf5ff77d1785dfea228de9109aceff4773da1))
+
 ## [0.19.1](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.19.0...accesskit_consumer-v0.19.1) (2024-05-11)
 
 
 ### Bug Fixes
 
 * Improve panic messages ([#401](https://github.com/AccessKit/accesskit/issues/401)) ([e6ce021](https://github.com/AccessKit/accesskit/commit/e6ce021b3b172f5ea7ee31496c9afaf66b1871f2))
```

### Comparing `accesskit-0.3.1/consumer/src/iterators.rs` & `accesskit-0.3.2/consumer/src/iterators.rs`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
     front: Option<Node<'a>>,
 }
 
 impl<'a, Filter: Fn(&Node) -> FilterResult> FollowingFilteredSiblings<'a, Filter> {
     pub(crate) fn new(node: Node<'a>, filter: Filter) -> Self {
         let front = next_filtered_sibling(Some(node), &filter);
         let back = node
-            .parent()
+            .filtered_parent(&filter)
             .and_then(|parent| parent.last_filtered_child(&filter));
         Self {
             filter,
             back,
             done: back.is_none() || front.is_none(),
             front,
         }
@@ -326,15 +326,15 @@
     front: Option<Node<'a>>,
 }
 
 impl<'a, Filter: Fn(&Node) -> FilterResult> PrecedingFilteredSiblings<'a, Filter> {
     pub(crate) fn new(node: Node<'a>, filter: Filter) -> Self {
         let front = previous_filtered_sibling(Some(node), &filter);
         let back = node
-            .parent()
+            .filtered_parent(&filter)
             .and_then(|parent| parent.first_filtered_child(&filter));
         Self {
             filter,
             back,
             done: back.is_none() || front.is_none(),
             front,
         }
@@ -637,14 +637,23 @@
             tree.state()
                 .node_by_id(PARAGRAPH_0_ID)
                 .unwrap()
                 .following_filtered_siblings(test_tree_filter)
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
+        assert_eq!(
+            [BUTTON_3_2_ID],
+            tree.state()
+                .node_by_id(STATIC_TEXT_3_1_0_ID)
+                .unwrap()
+                .following_filtered_siblings(test_tree_filter)
+                .map(|node| node.id())
+                .collect::<Vec<NodeId>>()[..]
+        );
         assert!(tree
             .state()
             .node_by_id(PARAGRAPH_3_IGNORED_ID)
             .unwrap()
             .following_filtered_siblings(test_tree_filter)
             .next()
             .is_none());
@@ -670,14 +679,24 @@
                 .node_by_id(PARAGRAPH_0_ID)
                 .unwrap()
                 .following_filtered_siblings(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
+        assert_eq!(
+            [BUTTON_3_2_ID,],
+            tree.state()
+                .node_by_id(STATIC_TEXT_3_1_0_ID)
+                .unwrap()
+                .following_filtered_siblings(test_tree_filter)
+                .rev()
+                .map(|node| node.id())
+                .collect::<Vec<NodeId>>()[..]
+        );
         assert!(tree
             .state()
             .node_by_id(PARAGRAPH_3_IGNORED_ID)
             .unwrap()
             .following_filtered_siblings(test_tree_filter)
             .next_back()
             .is_none());
@@ -697,14 +716,23 @@
             tree.state()
                 .node_by_id(PARAGRAPH_3_IGNORED_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
+        assert_eq!(
+            [PARAGRAPH_2_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_0_ID],
+            tree.state()
+                .node_by_id(STATIC_TEXT_3_1_0_ID)
+                .unwrap()
+                .preceding_filtered_siblings(test_tree_filter)
+                .map(|node| node.id())
+                .collect::<Vec<NodeId>>()[..]
+        );
         assert!(tree
             .state()
             .node_by_id(PARAGRAPH_0_ID)
             .unwrap()
             .preceding_filtered_siblings(test_tree_filter)
             .next()
             .is_none());
@@ -725,14 +753,24 @@
                 .node_by_id(PARAGRAPH_3_IGNORED_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
+        assert_eq!(
+            [PARAGRAPH_0_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_2_ID],
+            tree.state()
+                .node_by_id(STATIC_TEXT_3_1_0_ID)
+                .unwrap()
+                .preceding_filtered_siblings(test_tree_filter)
+                .rev()
+                .map(|node| node.id())
+                .collect::<Vec<NodeId>>()[..]
+        );
         assert!(tree
             .state()
             .node_by_id(PARAGRAPH_0_ID)
             .unwrap()
             .preceding_filtered_siblings(test_tree_filter)
             .next_back()
             .is_none());
```

### Comparing `accesskit-0.3.1/consumer/src/lib.rs` & `accesskit-0.3.2/consumer/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 pub(crate) mod tree;
 pub use tree::{ChangeHandler as TreeChangeHandler, State as TreeState, Tree};
 
 pub(crate) mod node;
-pub use node::{DetachedNode, Node, NodeState};
+pub use node::Node;
 
 pub(crate) mod filters;
-pub use filters::{
-    common_filter, common_filter_detached, common_filter_with_root_exception, FilterResult,
-};
+pub use filters::{common_filter, common_filter_with_root_exception, FilterResult};
 
 pub(crate) mod iterators;
 
 pub(crate) mod text;
 pub use text::{
     AttributeValue as TextAttributeValue, Position as TextPosition, Range as TextRange,
     WeakRange as WeakTextRange,
```

### Comparing `accesskit-0.3.1/consumer/src/node.rs` & `accesskit-0.3.2/consumer/src/node.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 // the LICENSE-MIT file), at your option.
 
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2021 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
-use std::{iter::FusedIterator, ops::Deref, sync::Arc};
+use std::{iter::FusedIterator, sync::Arc};
 
 use accesskit::{
     Action, Affine, DefaultActionVerb, Live, Node as NodeData, NodeId, Point, Rect, Role,
     TextSelection, Toggled,
 };
 
 use crate::filters::FilterResult;
@@ -22,74 +22,52 @@
 };
 use crate::tree::State as TreeState;
 
 #[derive(Clone, Copy, PartialEq, Eq)]
 pub(crate) struct ParentAndIndex(pub(crate) NodeId, pub(crate) usize);
 
 #[derive(Clone)]
-pub struct NodeState {
-    pub(crate) id: NodeId,
+pub(crate) struct NodeState {
     pub(crate) parent_and_index: Option<ParentAndIndex>,
     pub(crate) data: Arc<NodeData>,
 }
 
 #[derive(Copy, Clone)]
 pub struct Node<'a> {
     pub tree_state: &'a TreeState,
+    pub(crate) id: NodeId,
     pub(crate) state: &'a NodeState,
 }
 
-impl NodeState {
-    pub(crate) fn data(&self) -> &NodeData {
-        &self.data
-    }
-}
-
 impl<'a> Node<'a> {
-    pub fn detached(&self) -> DetachedNode {
-        DetachedNode {
-            state: self.state.clone(),
-            is_focused: self.is_focused(),
-            is_root: self.is_root(),
-            name: self.name(),
-            description: self.description(),
-            value: self.value(),
-            live: self.live(),
-            supports_text_ranges: self.supports_text_ranges(),
-        }
+    pub(crate) fn data(&self) -> &NodeData {
+        &self.state.data
     }
 
     pub fn is_focused(&self) -> bool {
         self.tree_state.focus_id() == Some(self.id())
     }
-}
 
-impl NodeState {
     pub fn is_focusable(&self) -> bool {
         self.supports_action(Action::Focus)
     }
-}
 
-impl<'a> Node<'a> {
     pub fn is_root(&self) -> bool {
         // Don't check for absence of a parent node, in case a non-root node
         // somehow gets detached from the tree.
         self.id() == self.tree_state.root_id()
     }
-}
 
-impl NodeState {
     pub fn parent_id(&self) -> Option<NodeId> {
-        self.parent_and_index
+        self.state
+            .parent_and_index
             .as_ref()
             .map(|ParentAndIndex(id, _)| *id)
     }
-}
 
-impl<'a> Node<'a> {
     pub fn parent(&self) -> Option<Node<'a>> {
         self.parent_id()
             .map(|id| self.tree_state.node_by_id(id).unwrap())
     }
 
     pub fn filtered_parent(&self, filter: &impl Fn(&Node) -> FilterResult) -> Option<Node<'a>> {
         self.parent().and_then(move |parent| {
@@ -105,39 +83,36 @@
         self.state
             .parent_and_index
             .as_ref()
             .map(|ParentAndIndex(parent, index)| {
                 (self.tree_state.node_by_id(*parent).unwrap(), *index)
             })
     }
-}
 
-impl NodeState {
     pub fn child_ids(
         &self,
     ) -> impl DoubleEndedIterator<Item = NodeId>
            + ExactSizeIterator<Item = NodeId>
            + FusedIterator<Item = NodeId>
            + '_ {
-        let data = &self.data;
+        let data = &self.state.data;
         data.children().iter().copied()
     }
-}
 
-impl<'a> Node<'a> {
     pub fn children(
         &self,
     ) -> impl DoubleEndedIterator<Item = Node<'a>>
            + ExactSizeIterator<Item = Node<'a>>
            + FusedIterator<Item = Node<'a>>
            + 'a {
         let state = self.tree_state;
-        self.state
-            .child_ids()
-            .map(move |id| state.node_by_id(id).unwrap())
+        let data = &self.state.data;
+        data.children()
+            .iter()
+            .map(move |id| state.node_by_id(*id).unwrap())
     }
 
     pub fn filtered_children(
         &self,
         filter: impl Fn(&Node) -> FilterResult + 'a,
     ) -> impl DoubleEndedIterator<Item = Node<'a>> + FusedIterator<Item = Node<'a>> + 'a {
         FilteredChildren::new(*self, filter)
@@ -240,27 +215,23 @@
             return true;
         }
         if let Some(parent) = self.parent() {
             return parent.is_descendant_of(ancestor);
         }
         false
     }
-}
 
-impl NodeState {
     /// Returns the transform defined directly on this node, or the identity
     /// transform, without taking into account transforms on ancestors.
     pub fn direct_transform(&self) -> Affine {
         self.data()
             .transform()
             .map_or(Affine::IDENTITY, |value| *value)
     }
-}
 
-impl<'a> Node<'a> {
     /// Returns the combined affine transform of this node and its ancestors,
     /// up to and including the root of this node's tree.
     pub fn transform(&self) -> Affine {
         self.parent()
             .map_or(Affine::IDENTITY, |parent| parent.transform())
             * self.direct_transform()
     }
@@ -273,39 +244,33 @@
                 parent.relative_transform(stop_at)
             }
         } else {
             Affine::IDENTITY
         };
         parent_transform * self.direct_transform()
     }
-}
 
-impl NodeState {
     pub fn raw_bounds(&self) -> Option<Rect> {
         self.data().bounds()
     }
-}
 
-impl<'a> Node<'a> {
     pub fn has_bounds(&self) -> bool {
-        self.state.raw_bounds().is_some()
+        self.raw_bounds().is_some()
     }
 
     /// Returns the node's transformed bounding box relative to the tree's
     /// container (e.g. window).
     pub fn bounding_box(&self) -> Option<Rect> {
-        self.state
-            .raw_bounds()
+        self.raw_bounds()
             .as_ref()
             .map(|rect| self.transform().transform_rect_bbox(*rect))
     }
 
     pub(crate) fn bounding_box_in_coordinate_space(&self, other: &Node) -> Option<Rect> {
-        self.state
-            .raw_bounds()
+        self.raw_bounds()
             .as_ref()
             .map(|rect| self.relative_transform(other).transform_rect_bbox(*rect))
     }
 
     pub(crate) fn hit_test(
         &self,
         point: Point,
@@ -321,15 +286,15 @@
             let point = child.direct_transform().inverse() * point;
             if let Some(result) = child.hit_test(point, filter) {
                 return Some(result);
             }
         }
 
         if filter_result == FilterResult::Include {
-            if let Some(rect) = &self.state.raw_bounds() {
+            if let Some(rect) = &self.raw_bounds() {
                 if rect.contains(point) {
                     return Some((*self, point));
                 }
             }
         }
 
         None
@@ -340,17 +305,15 @@
     pub fn node_at_point(
         &self,
         point: Point,
         filter: &impl Fn(&Node) -> FilterResult,
     ) -> Option<Node<'a>> {
         self.hit_test(point, filter).map(|(node, _)| node)
     }
-}
 
-impl NodeState {
     pub fn id(&self) -> NodeId {
         self.id
     }
 
     pub fn role(&self) -> Role {
         self.data().role()
     }
@@ -557,17 +520,15 @@
             None
         }
     }
 
     pub fn has_value(&self) -> bool {
         self.data().value().is_some() || (self.supports_text_ranges() && !self.is_multiline())
     }
-}
 
-impl NodeState {
     pub fn is_read_only_supported(&self) -> bool {
         self.is_text_input()
             || matches!(
                 self.role(),
                 Role::CheckBox
                     | Role::ColorWell
                     | Role::ComboBox
@@ -602,25 +563,21 @@
                 | Role::RootWebArea
                 | Role::Term
                 | Role::Timer
                 | Role::Toolbar
                 | Role::Tooltip
         )
     }
-}
 
-impl<'a> Node<'a> {
     pub fn live(&self) -> Live {
         self.data()
             .live()
             .unwrap_or_else(|| self.parent().map_or(Live::Off, |parent| parent.live()))
     }
-}
 
-impl NodeState {
     pub fn is_selected(&self) -> Option<bool> {
         self.data().is_selected()
     }
 
     pub fn raw_text_selection(&self) -> Option<&TextSelection> {
         self.data().text_selection()
     }
@@ -628,17 +585,15 @@
     pub fn raw_value(&self) -> Option<&str> {
         self.data().value()
     }
 
     pub fn class_name(&self) -> Option<&str> {
         self.data().class_name()
     }
-}
 
-impl<'a> Node<'a> {
     pub fn index_path(&self) -> Vec<usize> {
         self.relative_index_path(self.tree_state.root_id())
     }
 
     pub fn relative_index_path(&self, ancestor_id: NodeId) -> Vec<usize> {
         let mut result = Vec::new();
         let mut current = *self;
@@ -682,84 +637,14 @@
                 if let Some(descendant) = child.last_filtered_child(filter) {
                     return Some(descendant);
                 }
             }
         }
         None
     }
-
-    pub fn state(&self) -> &'a NodeState {
-        self.state
-    }
-}
-
-impl<'a> Deref for Node<'a> {
-    type Target = NodeState;
-
-    fn deref(&self) -> &NodeState {
-        self.state
-    }
-}
-
-#[derive(Clone)]
-pub struct DetachedNode {
-    pub(crate) state: NodeState,
-    pub(crate) is_focused: bool,
-    pub(crate) is_root: bool,
-    pub(crate) name: Option<String>,
-    pub(crate) description: Option<String>,
-    pub(crate) value: Option<String>,
-    pub(crate) live: Live,
-    pub(crate) supports_text_ranges: bool,
-}
-
-impl DetachedNode {
-    pub fn is_focused(&self) -> bool {
-        self.is_focused
-    }
-
-    pub fn is_root(&self) -> bool {
-        self.is_root
-    }
-
-    pub fn name(&self) -> Option<String> {
-        self.name.clone()
-    }
-
-    pub fn description(&self) -> Option<String> {
-        self.description.clone()
-    }
-
-    pub fn value(&self) -> Option<String> {
-        self.value.clone()
-    }
-
-    pub fn has_value(&self) -> bool {
-        self.value.is_some()
-    }
-
-    pub fn live(&self) -> Live {
-        self.live
-    }
-
-    pub fn supports_text_ranges(&self) -> bool {
-        self.supports_text_ranges
-    }
-
-    pub fn state(&self) -> &NodeState {
-        &self.state
-    }
-}
-
-impl Deref for DetachedNode {
-    type Target = NodeState;
-
-    fn deref(&self) -> &NodeState {
-        &self.state
-    }
 }
 
 #[cfg(test)]
 mod tests {
     use accesskit::{NodeBuilder, NodeId, Point, Rect, Role, Tree, TreeUpdate};
 
     use crate::tests::*;
```

### Comparing `accesskit-0.3.1/consumer/src/text.rs` & `accesskit-0.3.2/consumer/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/consumer/src/tree.rs` & `accesskit-0.3.2/consumer/src/tree.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,96 +1,87 @@
 // Copyright 2021 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use accesskit::{Live, Node as NodeData, NodeId, Tree as TreeData, TreeUpdate};
+use accesskit::{Node as NodeData, NodeId, Tree as TreeData, TreeUpdate};
+use immutable_chunkmap::map::MapM as ChunkMap;
 use std::{
     collections::{HashMap, HashSet},
     sync::Arc,
 };
 
-use crate::node::{DetachedNode, Node, NodeState, ParentAndIndex};
+use crate::node::{Node, NodeState, ParentAndIndex};
 
 #[derive(Clone)]
 pub struct State {
-    pub(crate) nodes: HashMap<NodeId, NodeState>,
+    pub(crate) nodes: ChunkMap<NodeId, NodeState>,
     pub(crate) data: TreeData,
     focus: NodeId,
     is_host_focused: bool,
 }
 
-struct InternalFocusChange {
-    old_focus: Option<DetachedNode>,
-    new_focus_old_node: Option<DetachedNode>,
-}
-
 #[derive(Default)]
 struct InternalChanges {
     added_node_ids: HashSet<NodeId>,
-    updated_nodes: HashMap<NodeId, DetachedNode>,
-    focus_change: Option<InternalFocusChange>,
-    removed_nodes: HashMap<NodeId, DetachedNode>,
+    updated_node_ids: HashSet<NodeId>,
+    removed_node_ids: HashSet<NodeId>,
 }
 
 impl State {
     fn validate_global(&self) {
-        if !self.nodes.contains_key(&self.data.root) {
+        if self.nodes.get_key(&self.data.root).is_none() {
             panic!("Root id #{} is not in the node list", self.data.root.0);
         }
-        if !self.nodes.contains_key(&self.focus) {
+        if self.nodes.get_key(&self.focus).is_none() {
             panic!("Focused id #{} is not in the node list", self.focus.0);
         }
     }
 
     fn update(
         &mut self,
         update: TreeUpdate,
         is_host_focused: bool,
         mut changes: Option<&mut InternalChanges>,
     ) {
-        // First, if we're collecting changes, get the accurate state
-        // of any updated nodes.
+        // First, if we're collecting changes, collect the IDS of any nodes
+        // in the update that were in the previous state.
         if let Some(changes) = &mut changes {
             for (node_id, _) in &update.nodes {
-                if let Some(old_node) = self.node_by_id(*node_id) {
-                    let old_node = old_node.detached();
-                    changes.updated_nodes.insert(*node_id, old_node);
+                if self.nodes.get(node_id).is_some() {
+                    changes.updated_node_ids.insert(*node_id);
                 }
             }
         }
 
         let mut orphans = HashSet::new();
-        let old_focus_id = self.is_host_focused.then_some(self.focus);
-        let old_root_id = self.data.root;
 
         if let Some(tree) = update.tree {
             if tree.root != self.data.root {
                 orphans.insert(self.data.root);
             }
             self.data = tree;
         }
 
         let root = self.data.root;
         let mut pending_nodes: HashMap<NodeId, _> = HashMap::new();
         let mut pending_children = HashMap::new();
 
         fn add_node(
-            nodes: &mut HashMap<NodeId, NodeState>,
+            nodes: &mut ChunkMap<NodeId, NodeState>,
             changes: &mut Option<&mut InternalChanges>,
             parent_and_index: Option<ParentAndIndex>,
             id: NodeId,
             data: NodeData,
         ) {
             let state = NodeState {
-                id,
                 parent_and_index,
                 data: Arc::new(data),
             };
-            nodes.insert(id, state);
+            nodes.insert_cow(id, state);
             if let Some(changes) = changes {
                 changes.added_node_ids.insert(id);
             }
         }
 
         for (node_id, node_data) in update.nodes {
             orphans.remove(&node_id);
@@ -101,15 +92,15 @@
                     panic!(
                         "Node #{} of TreeUpdate includes duplicate child #{};",
                         node_id.0, child_id.0
                     );
                 }
                 orphans.remove(child_id);
                 let parent_and_index = ParentAndIndex(node_id, child_index);
-                if let Some(child_state) = self.nodes.get_mut(child_id) {
+                if let Some(child_state) = self.nodes.get_mut_cow(child_id) {
                     if child_state.parent_and_index != Some(parent_and_index) {
                         child_state.parent_and_index = Some(parent_and_index);
                     }
                 } else if let Some(child_data) = pending_nodes.remove(child_id) {
                     add_node(
                         &mut self.nodes,
                         &mut changes,
@@ -119,15 +110,15 @@
                     );
                 } else {
                     pending_children.insert(*child_id, parent_and_index);
                 }
                 seen_child_ids.insert(child_id);
             }
 
-            if let Some(node_state) = self.nodes.get_mut(&node_id) {
+            if let Some(node_state) = self.nodes.get_mut_cow(&node_id) {
                 if node_id == root {
                     node_state.parent_and_index = None;
                 }
                 for child_id in node_state.data.children().iter() {
                     if !seen_child_ids.contains(child_id) {
                         orphans.insert(*child_id);
                     }
@@ -151,37 +142,22 @@
         if !pending_nodes.is_empty() {
             panic!("TreeUpdate includes {} nodes which are neither in the current tree nor a child of another node from the update: {}", pending_nodes.len(), short_node_list(pending_nodes.keys()));
         }
         if !pending_children.is_empty() {
             panic!("TreeUpdate's nodes include {} children ids which are neither in the current tree nor the id of another node from the update: {}", pending_children.len(), short_node_list(pending_children.keys()));
         }
 
-        if update.focus != self.focus || is_host_focused != self.is_host_focused {
-            let old_focus = old_focus_id.map(|id| self.node_by_id(id).unwrap().detached());
-            let new_focus = is_host_focused.then_some(update.focus);
-            if let Some(changes) = &mut changes {
-                changes.focus_change = Some(InternalFocusChange {
-                    old_focus,
-                    new_focus_old_node: new_focus
-                        .and_then(|id| {
-                            (!changes.updated_nodes.contains_key(&id))
-                                .then(|| self.node_by_id(id).map(|node| node.detached()))
-                        })
-                        .flatten(),
-                });
-            }
-            self.focus = update.focus;
-            self.is_host_focused = is_host_focused;
-        }
+        self.focus = update.focus;
+        self.is_host_focused = is_host_focused;
 
         if !orphans.is_empty() {
             let mut to_remove = HashSet::new();
 
             fn traverse_orphan(
-                nodes: &HashMap<NodeId, NodeState>,
+                nodes: &ChunkMap<NodeId, NodeState>,
                 to_remove: &mut HashSet<NodeId>,
                 id: NodeId,
             ) {
                 to_remove.insert(id);
                 let node = nodes.get(&id).unwrap();
                 for child_id in node.data.children().iter() {
                     traverse_orphan(nodes, to_remove, *child_id);
@@ -189,27 +165,17 @@
             }
 
             for id in orphans {
                 traverse_orphan(&self.nodes, &mut to_remove, id);
             }
 
             for id in to_remove {
-                if let Some(old_node_state) = self.nodes.remove(&id) {
+                if self.nodes.remove_cow(&id).is_some() {
                     if let Some(changes) = &mut changes {
-                        let old_node = DetachedNode {
-                            state: old_node_state,
-                            is_focused: old_focus_id == Some(id),
-                            is_root: old_root_id == id,
-                            name: None,
-                            description: None,
-                            value: None,
-                            live: Live::Off,
-                            supports_text_ranges: false,
-                        };
-                        changes.removed_nodes.insert(id, old_node);
+                        changes.removed_node_ids.insert(id);
                     }
                 }
             }
         }
 
         self.validate_global();
     }
@@ -246,20 +212,21 @@
             nodes,
             tree: Some(self.data.clone()),
             focus: self.focus,
         }
     }
 
     pub fn has_node(&self, id: NodeId) -> bool {
-        self.nodes.contains_key(&id)
+        self.nodes.get(&id).is_some()
     }
 
     pub fn node_by_id(&self, id: NodeId) -> Option<Node<'_>> {
         self.nodes.get(&id).map(|node_state| Node {
             tree_state: self,
+            id,
             state: node_state,
         })
     }
 
     pub fn root_id(&self) -> NodeId {
         self.data.root
     }
@@ -291,42 +258,30 @@
     pub fn toolkit_version(&self) -> Option<String> {
         self.data.toolkit_version.clone()
     }
 }
 
 pub trait ChangeHandler {
     fn node_added(&mut self, node: &Node);
-    fn node_updated(&mut self, old_node: &DetachedNode, new_node: &Node);
-    fn focus_moved(
-        &mut self,
-        old_node: Option<&DetachedNode>,
-        new_node: Option<&Node>,
-        current_state: &State,
-    );
-    /// The tree update process doesn't currently collect all possible information
-    /// about removed nodes. The following methods don't accurately reflect
-    /// the full state of the old node:
-    ///
-    /// * [`DetachedNode::name`]
-    /// * [`DetachedNode::live`]
-    /// * [`DetachedNode::supports_text_ranges`]
-    fn node_removed(&mut self, node: &DetachedNode, current_state: &State);
+    fn node_updated(&mut self, old_node: &Node, new_node: &Node);
+    fn focus_moved(&mut self, old_node: Option<&Node>, new_node: Option<&Node>);
+    fn node_removed(&mut self, node: &Node);
 }
 
 pub struct Tree {
     state: State,
 }
 
 impl Tree {
     pub fn new(mut initial_state: TreeUpdate, is_host_focused: bool) -> Self {
         let Some(tree) = initial_state.tree.take() else {
             panic!("Tried to initialize the accessibility tree without a root tree. TreeUpdate::tree must be Some.");
         };
         let mut state = State {
-            nodes: HashMap::new(),
+            nodes: ChunkMap::new(),
             data: tree,
             focus: initial_state.focus,
             is_host_focused,
         };
         state.update(initial_state, is_host_focused, None);
         Self { state }
     }
@@ -337,72 +292,78 @@
 
     pub fn update_and_process_changes(
         &mut self,
         update: TreeUpdate,
         handler: &mut impl ChangeHandler,
     ) {
         let mut changes = InternalChanges::default();
+        let old_state = self.state.clone();
         self.state
             .update(update, self.state.is_host_focused, Some(&mut changes));
-        self.process_changes(changes, handler);
+        self.process_changes(old_state, changes, handler);
     }
 
     pub fn update_host_focus_state(&mut self, is_host_focused: bool) {
         self.state.update_host_focus_state(is_host_focused, None);
     }
 
     pub fn update_host_focus_state_and_process_changes(
         &mut self,
         is_host_focused: bool,
         handler: &mut impl ChangeHandler,
     ) {
         let mut changes = InternalChanges::default();
+        let old_state = self.state.clone();
         self.state
             .update_host_focus_state(is_host_focused, Some(&mut changes));
-        self.process_changes(changes, handler);
+        self.process_changes(old_state, changes, handler);
     }
 
-    fn process_changes(&self, changes: InternalChanges, handler: &mut impl ChangeHandler) {
+    fn process_changes(
+        &self,
+        old_state: State,
+        changes: InternalChanges,
+        handler: &mut impl ChangeHandler,
+    ) {
         for id in &changes.added_node_ids {
             let node = self.state.node_by_id(*id).unwrap();
             handler.node_added(&node);
         }
-        for (id, old_node) in &changes.updated_nodes {
+        for id in &changes.updated_node_ids {
+            let old_node = old_state.node_by_id(*id).unwrap();
             let new_node = self.state.node_by_id(*id).unwrap();
-            handler.node_updated(old_node, &new_node);
+            handler.node_updated(&old_node, &new_node);
         }
-        if let Some(focus_change) = changes.focus_change {
-            if let Some(old_node) = &focus_change.old_focus {
+        if old_state.focus_id() != self.state.focus_id() {
+            let old_node = old_state.focus();
+            if let Some(old_node) = &old_node {
                 let id = old_node.id();
-                if !changes.updated_nodes.contains_key(&id)
-                    && !changes.removed_nodes.contains_key(&id)
+                if !changes.updated_node_ids.contains(&id)
+                    && !changes.removed_node_ids.contains(&id)
                 {
                     if let Some(old_node_new_version) = self.state.node_by_id(id) {
                         handler.node_updated(old_node, &old_node_new_version);
                     }
                 }
             }
             let new_node = self.state.focus();
-            if let Some(new_node) = new_node {
+            if let Some(new_node) = &new_node {
                 let id = new_node.id();
-                if !changes.added_node_ids.contains(&id) && !changes.updated_nodes.contains_key(&id)
+                if !changes.added_node_ids.contains(&id) && !changes.updated_node_ids.contains(&id)
                 {
-                    if let Some(new_node_old_version) = focus_change.new_focus_old_node {
-                        handler.node_updated(&new_node_old_version, &new_node);
+                    if let Some(new_node_old_version) = old_state.node_by_id(id) {
+                        handler.node_updated(&new_node_old_version, new_node);
                     }
                 }
             }
-            handler.focus_moved(
-                focus_change.old_focus.as_ref(),
-                new_node.as_ref(),
-                &self.state,
-            );
+            handler.focus_moved(old_node.as_ref(), new_node.as_ref());
         }
-        for node in changes.removed_nodes.values() {
-            handler.node_removed(node, &self.state);
+        for id in &changes.removed_node_ids {
+            let node = old_state.node_by_id(*id).unwrap();
+            handler.node_removed(&node);
         }
     }
 
     pub fn state(&self) -> &State {
         &self.state
     }
 }
@@ -506,37 +467,32 @@
             fn node_added(&mut self, node: &crate::Node) {
                 if node.id() == NodeId(1) {
                     self.got_new_child_node = true;
                     return;
                 }
                 unexpected_change();
             }
-            fn node_updated(&mut self, old_node: &crate::DetachedNode, new_node: &crate::Node) {
+            fn node_updated(&mut self, old_node: &crate::Node, new_node: &crate::Node) {
                 if new_node.id() == NodeId(0)
                     && old_node.data().children().is_empty()
                     && new_node.data().children() == [NodeId(1)]
                 {
                     self.got_updated_root_node = true;
                     return;
                 }
                 unexpected_change();
             }
             fn focus_moved(
                 &mut self,
-                _old_node: Option<&crate::DetachedNode>,
+                _old_node: Option<&crate::Node>,
                 _new_node: Option<&crate::Node>,
-                _current_state: &crate::TreeState,
             ) {
                 unexpected_change();
             }
-            fn node_removed(
-                &mut self,
-                _node: &crate::DetachedNode,
-                _current_state: &crate::TreeState,
-            ) {
+            fn node_removed(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
         }
         let mut handler = Handler {
             got_new_child_node: false,
             got_updated_root_node: false,
         };
@@ -581,37 +537,32 @@
         fn unexpected_change() {
             panic!("expected only removed child node and updated root node");
         }
         impl super::ChangeHandler for Handler {
             fn node_added(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
-            fn node_updated(&mut self, old_node: &crate::DetachedNode, new_node: &crate::Node) {
+            fn node_updated(&mut self, old_node: &crate::Node, new_node: &crate::Node) {
                 if new_node.id() == NodeId(0)
                     && old_node.data().children() == [NodeId(1)]
                     && new_node.data().children().is_empty()
                 {
                     self.got_updated_root_node = true;
                     return;
                 }
                 unexpected_change();
             }
             fn focus_moved(
                 &mut self,
-                _old_node: Option<&crate::DetachedNode>,
+                _old_node: Option<&crate::Node>,
                 _new_node: Option<&crate::Node>,
-                _current_state: &crate::TreeState,
             ) {
                 unexpected_change();
             }
-            fn node_removed(
-                &mut self,
-                node: &crate::DetachedNode,
-                _current_state: &crate::TreeState,
-            ) {
+            fn node_removed(&mut self, node: &crate::Node) {
                 if node.id() == NodeId(1) {
                     self.got_removed_child_node = true;
                     return;
                 }
                 unexpected_change();
             }
         }
@@ -656,15 +607,15 @@
         fn unexpected_change() {
             panic!("expected only focus change");
         }
         impl super::ChangeHandler for Handler {
             fn node_added(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
-            fn node_updated(&mut self, old_node: &crate::DetachedNode, new_node: &crate::Node) {
+            fn node_updated(&mut self, old_node: &crate::Node, new_node: &crate::Node) {
                 if old_node.id() == NodeId(1)
                     && new_node.id() == NodeId(1)
                     && old_node.is_focused()
                     && !new_node.is_focused()
                 {
                     self.got_old_focus_node_update = true;
                     return;
@@ -677,31 +628,26 @@
                     self.got_new_focus_node_update = true;
                     return;
                 }
                 unexpected_change();
             }
             fn focus_moved(
                 &mut self,
-                old_node: Option<&crate::DetachedNode>,
+                old_node: Option<&crate::Node>,
                 new_node: Option<&crate::Node>,
-                _current_state: &crate::TreeState,
             ) {
                 if let (Some(old_node), Some(new_node)) = (old_node, new_node) {
                     if old_node.id() == NodeId(1) && new_node.id() == NodeId(2) {
                         self.got_focus_change = true;
                         return;
                     }
                 }
                 unexpected_change();
             }
-            fn node_removed(
-                &mut self,
-                _node: &crate::DetachedNode,
-                _current_state: &crate::TreeState,
-            ) {
+            fn node_removed(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
         }
         let mut handler = Handler {
             got_old_focus_node_update: false,
             got_new_focus_node_update: false,
             got_focus_change: false,
@@ -753,37 +699,32 @@
         fn unexpected_change() {
             panic!("expected only updated child node");
         }
         impl super::ChangeHandler for Handler {
             fn node_added(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
-            fn node_updated(&mut self, old_node: &crate::DetachedNode, new_node: &crate::Node) {
+            fn node_updated(&mut self, old_node: &crate::Node, new_node: &crate::Node) {
                 if new_node.id() == NodeId(1)
                     && old_node.name() == Some("foo".into())
                     && new_node.name() == Some("bar".into())
                 {
                     self.got_updated_child_node = true;
                     return;
                 }
                 unexpected_change();
             }
             fn focus_moved(
                 &mut self,
-                _old_node: Option<&crate::DetachedNode>,
+                _old_node: Option<&crate::Node>,
                 _new_node: Option<&crate::Node>,
-                _current_state: &crate::TreeState,
             ) {
                 unexpected_change();
             }
-            fn node_removed(
-                &mut self,
-                _node: &crate::DetachedNode,
-                _current_state: &crate::TreeState,
-            ) {
+            fn node_removed(&mut self, _node: &crate::Node) {
                 unexpected_change();
             }
         }
         let mut handler = Handler {
             got_updated_child_node: false,
         };
         tree.update_and_process_changes(second_update, &mut handler);
```

### Comparing `accesskit-0.3.1/bindings/python/Cargo.toml` & `accesskit-0.3.2/bindings/python/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.3.1"
+version = "0.3.2"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -17,14 +17,14 @@
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.18.1", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.18.2", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.13.1", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.13.2", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.9.1", path = "../../platforms/unix" }
+accesskit_unix = { version = "0.9.2", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.3.1/bindings/python/CHANGELOG.md` & `accesskit-0.3.2/bindings/python/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,20 @@
   * dependencies
     * accesskit_unix bumped from 0.7.4 to 0.7.5
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_windows bumped from 0.16.3 to 0.16.4
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_windows bumped from 0.18.1 to 0.18.2
+    * accesskit_macos bumped from 0.13.1 to 0.13.2
+    * accesskit_unix bumped from 0.9.1 to 0.9.2
+
 ## [0.3.1](https://github.com/AccessKit/accesskit/compare/accesskit_python-v0.3.0...accesskit_python-v0.3.1) (2024-05-11)
 
 
 ### Bug Fixes
 
 * Fix dead code warning on Unix platforms ([#403](https://github.com/AccessKit/accesskit/issues/403)) ([09d9157](https://github.com/AccessKit/accesskit/commit/09d91577dd88743e379a1fdea34b25a94726d0fb))
```

### Comparing `accesskit-0.3.1/bindings/python/README.md` & `accesskit-0.3.2/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/examples/pygame/.gitignore` & `accesskit-0.3.2/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.3.2/bindings/python/examples/pygame/hello_world.py`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/common.rs` & `accesskit-0.3.2/bindings/python/src/common.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/geometry.rs` & `accesskit-0.3.2/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/lib.rs` & `accesskit-0.3.2/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/macos.rs` & `accesskit-0.3.2/bindings/python/src/macos.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/unix.rs` & `accesskit-0.3.2/bindings/python/src/unix.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/bindings/python/src/windows.rs` & `accesskit-0.3.2/bindings/python/src/windows.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/Cargo.lock` & `accesskit-0.3.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -26,68 +26,69 @@
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.10.0"
+version = "0.10.1"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.19.1"
+version = "0.20.0"
 dependencies = [
  "accesskit",
+ "immutable-chunkmap",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.13.1"
+version = "0.13.2"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "objc2",
  "objc2-app-kit",
  "objc2-foundation",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
@@ -97,29 +98,29 @@
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.18.1"
+version = "0.18.2"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.20.1"
+version = "0.20.2"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
@@ -427,14 +428,26 @@
 [[package]]
 name = "bitflags"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
@@ -662,15 +675,15 @@
 
 [[package]]
 name = "dlib"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
 dependencies = [
- "libloading 0.7.4",
+ "libloading",
 ]
 
 [[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
@@ -826,14 +839,20 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "futures-core"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
 
 [[package]]
 name = "futures-io"
@@ -954,14 +973,25 @@
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "immutable-chunkmap"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "374b75d1b5a9df2c4d9392f21a9e821113543ffc49571b3428d8e161802f8cc7"
+dependencies = [
+ "arrayvec",
+ "packed_struct",
+ "packed_struct_codegen",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -1049,24 +1079,14 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libloading"
-version = "0.7.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
-dependencies = [
- "cfg-if",
- "winapi",
-]
-
-[[package]]
-name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
  "windows-targets 0.52.3",
 ]
@@ -1349,14 +1369,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e25e9fb15717794fae58ab55c26e044103aad13186fbb625893f9a3bbcc24228"
 dependencies = [
  "ttf-parser",
 ]
 
 [[package]]
+name = "packed_struct"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "36b29691432cc9eff8b282278473b63df73bea49bc3ec5e67f31a3ae9c3ec190"
+dependencies = [
+ "bitvec",
+ "packed_struct_codegen",
+]
+
+[[package]]
+name = "packed_struct_codegen"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cd6706dfe50d53e0f6aa09e12c034c44faacd23e966ae5a209e8bdb8f179f98"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "parking"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
 
 [[package]]
 name = "parking_lot"
@@ -1563,14 +1604,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -1946,14 +1993,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "tempfile"
@@ -2718,14 +2771,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "wyz"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
+
+[[package]]
 name = "x11-dl"
 version = "2.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38735924fedd5314a6e548792904ed8c6de6636285cb9fec04d5b1db85c1516f"
 dependencies = [
  "libc",
  "once_cell",
@@ -2737,15 +2799,15 @@
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
 dependencies = [
  "as-raw-xcb-connection",
  "gethostname",
  "libc",
- "libloading 0.8.3",
+ "libloading",
  "once_cell",
  "rustix 0.38.21",
  "x11rb-protocol",
 ]
 
 [[package]]
 name = "x11rb-protocol"
```

### Comparing `accesskit-0.3.1/pyproject.toml` & `accesskit-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/LICENSE-APACHE` & `accesskit-0.3.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/LICENSE-MIT` & `accesskit-0.3.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/LICENSE.chromium` & `accesskit-0.3.2/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.1/PKG-INFO` & `accesskit-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

