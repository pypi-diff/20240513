# Comparing `tmp/wgpu-0.9.4.tar.gz` & `tmp/wgpu-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgpu-0.9.4.tar", last modified: Thu Feb 23 10:56:24 2023, max compression
+gzip compressed data, was "wgpu-0.9.5.tar", last modified: Mon Oct  2 14:45:57 2023, max compression
```

## Comparing `wgpu-0.9.4.tar` & `wgpu-0.9.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.669783 wgpu-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-23 10:56:00.000000 wgpu-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-02-23 10:56:24.669783 wgpu-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-02-23 10:56:00.000000 wgpu-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-23 10:56:00.000000 wgpu-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-23 10:56:24.669783 wgpu-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-23 10:56:00.000000 wgpu-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.661783 wgpu-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_gui_auto_offscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_gui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_gui_glfw.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_rs_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_rs_compute_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_rs_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_rs_render_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_util_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/test_util_shadertoy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-02-23 10:56:00.000000 wgpu-0.9.4/tests/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.665783 wgpu-0.9.4/wgpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.665783 wgpu-0.9.4/wgpu/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/__pyinstaller/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/__pyinstaller/hook-wgpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/__pyinstaller/test_wgpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/_coreutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.665783 wgpu-0.9.4/wgpu/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/js.py
--rw-r--r--   0 runner    (1001) docker     (123)   110083 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/rs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/rs_ffi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/rs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/rs_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/backends/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)    72073 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.669783 wgpu-0.9.4/wgpu/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/_offscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/glfw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/offscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/gui/wx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.669783 wgpu-0.9.4/wgpu/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79029 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/resources/webgpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/resources/webgpu.idl
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/resources/wgpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.669783 wgpu-0.9.4/wgpu/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/utils/_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/utils/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-02-23 10:56:00.000000 wgpu-0.9.4/wgpu/utils/shadertoy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:56:24.665783 wgpu-0.9.4/wgpu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-23 10:56:24.000000 wgpu-0.9.4/wgpu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.352437 wgpu-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-10-02 14:45:35.000000 wgpu-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-02 14:45:57.352437 wgpu-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2023-10-02 14:45:35.000000 wgpu-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-10-02 14:45:35.000000 wgpu-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-10-02 14:45:57.352437 wgpu-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-10-02 14:45:35.000000 wgpu-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.348437 wgpu-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_gui_auto_offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_gui_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_gui_glfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28489 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_rs_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_rs_compute_tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19393 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_rs_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_rs_render_tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_util_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/test_util_shadertoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-10-02 14:45:35.000000 wgpu-0.9.5/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.348437 wgpu-0.9.5/wgpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.348437 wgpu-0.9.5/wgpu/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/__pyinstaller/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/__pyinstaller/hook-wgpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/__pyinstaller/test_wgpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/_coreutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.348437 wgpu-0.9.5/wgpu/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109622 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/rs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/rs_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/rs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/rs_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/backends/vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72073 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.352437 wgpu-0.9.5/wgpu/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/_offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/glfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14069 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/gui/wx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.352437 wgpu-0.9.5/wgpu/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79029 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/resources/webgpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36033 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/resources/webgpu.idl
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/resources/wgpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22704 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.352437 wgpu-0.9.5/wgpu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/utils/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/utils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2023-10-02 14:45:35.000000 wgpu-0.9.5/wgpu/utils/shadertoy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:45:57.348437 wgpu-0.9.5/wgpu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-02 14:45:57.000000 wgpu-0.9.5/wgpu.egg-info/top_level.txt
```

### Comparing `wgpu-0.9.4/LICENSE` & `wgpu-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/PKG-INFO` & `wgpu-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,9 @@
-Metadata-Version: 2.1
-Name: wgpu
-Version: 0.9.4
-Summary: Next generation GPU API for Python
-Home-page: https://github.com/pygfx/wgpu-py
-Author: Almar Klein
-Author-email: almar.klein@gmail.com
-License: BSD 2-Clause
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: jupyter
-Provides-Extra: glfw
-Provides-Extra: docs
-License-File: LICENSE
-
 [![CI](https://github.com/pygfx/wgpu-py/workflows/CI/badge.svg)](https://github.com/pygfx/wgpu-py/actions)
-[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=latest)](https://wgpu-py.readthedocs.io)
+[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=stable)](https://wgpu-py.readthedocs.io)
 [![PyPI version](https://badge.fury.io/py/wgpu.svg)](https://badge.fury.io/py/wgpu)
 
 # wgpu-py
 
 A Python implementation of WebGPU - the next generation GPU API.
 
 <img width=300 src='https://raw.githubusercontent.com/pygfx/wgpu-py/main/examples/screenshots/cube.png' />
```

### Comparing `wgpu-0.9.4/README.md` & `wgpu-0.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,30 @@
+Metadata-Version: 2.1
+Name: wgpu
+Version: 0.9.5
+Summary: Next generation GPU API for Python
+Home-page: https://github.com/pygfx/wgpu-py
+Author: Almar Klein
+Author-email: almar.klein@gmail.com
+License: BSD 2-Clause
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cffi>=1.15.0rc2
+Requires-Dist: rubicon-objc>=0.4.1; sys_platform == "darwin"
+Provides-Extra: jupyter
+Requires-Dist: jupyter_rfb>=0.3.1; extra == "jupyter"
+Provides-Extra: glfw
+Requires-Dist: glfw>=1.9; extra == "glfw"
+Provides-Extra: docs
+Requires-Dist: sphinx>7.2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+
 [![CI](https://github.com/pygfx/wgpu-py/workflows/CI/badge.svg)](https://github.com/pygfx/wgpu-py/actions)
-[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=latest)](https://wgpu-py.readthedocs.io)
+[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=stable)](https://wgpu-py.readthedocs.io)
 [![PyPI version](https://badge.fury.io/py/wgpu.svg)](https://badge.fury.io/py/wgpu)
 
 # wgpu-py
 
 A Python implementation of WebGPU - the next generation GPU API.
 
 <img width=300 src='https://raw.githubusercontent.com/pygfx/wgpu-py/main/examples/screenshots/cube.png' />
```

### Comparing `wgpu-0.9.4/pyproject.toml` & `wgpu-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/setup.cfg` & `wgpu-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/setup.py` & `wgpu-0.9.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 else:
     pass  # don't include binaries; user will have to arrange for the lib
 
 runtime_deps = ["cffi>=1.15.0rc2", "rubicon-objc>=0.4.1; sys_platform == 'darwin'"]
 extra_deps = {
     "jupyter": ["jupyter_rfb>=0.3.1"],
     "glfw": ["glfw>=1.9"],
-    "docs": ["sphinx"],
+    "docs": ["sphinx>7.2", "sphinx_rtd_theme"],
 }
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=["codegen", "codegen.*", "tests", "tests.*", "examples", "examples.*"]
```

### Comparing `wgpu-0.9.4/tests/test_api.py` & `wgpu-0.9.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_gui_auto_offscreen.py` & `wgpu-0.9.5/tests/test_gui_auto_offscreen.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_gui_base.py` & `wgpu-0.9.5/tests/test_gui_base.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_gui_glfw.py` & `wgpu-0.9.5/tests/test_gui_glfw.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_rs_basics.py` & `wgpu-0.9.5/tests/test_rs_basics.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_rs_compute_tex.py` & `wgpu-0.9.5/tests/test_rs_compute_tex.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,15 +480,15 @@
     texture_view2 = texture2.create_view()
 
     # Create buffer that we need to upload the data
     buffer_usage = wgpu.BufferUsage.COPY_SRC | wgpu.BufferUsage.COPY_DST
     buffer = device.create_buffer_with_data(data=data1, usage=buffer_usage)
     assert buffer.usage == buffer_usage
 
-    texture_sample_type = "float"
+    texture_sample_type = "unfilterable-float"
     if "uint" in texture_format:
         texture_sample_type = "uint"
     elif "sint" in texture_format:
         texture_sample_type = "sint"
 
     # Define bindings
     # One can see here why we need 2 textures: one is readonly, one writeonly
```

### Comparing `wgpu-0.9.4/tests/test_rs_render.py` & `wgpu-0.9.5/tests/test_rs_render.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_rs_render_tex.py` & `wgpu-0.9.5/tests/test_rs_render_tex.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,31 +475,35 @@
     texture_view = texture.create_view(
         format=texture_format,
         dimension=wgpu.TextureDimension.d2,
     )
 
     sampler = device.create_sampler(mag_filter="nearest", min_filter="nearest")
 
+    # Default sampler type.
+    # Note that integer texture types cannot even use a sampler.
+    sampler_type = wgpu.SamplerBindingType.filtering
+
     # Determine texture component type from the format
-    if texture_format.endswith(("norm", "float")):
+    if texture_format.endswith("norm"):
+        # We can use a filtering sampler
         texture_sample_type = wgpu.TextureSampleType.float
+    elif texture_format.endswith("float"):
+        # On Vanilla wgpu, float32 textures cannot use a filtering
+        # (interpolating) texture, (need to enable a feature for that).
+        # Without it, we need to use a non-filterin sampler.
+        texture_sample_type = wgpu.TextureSampleType.unfilterable_float
+        sampler_type = wgpu.SamplerBindingType.non_filtering
     elif "uint" in texture_format:
+        # Cannot even use a sampler (use textureLoad instwad of textureSample)
         texture_sample_type = wgpu.TextureSampleType.uint
     else:
+        # Dito
         texture_sample_type = wgpu.TextureSampleType.sint
 
-    # Determine sampler type.
-    # Note that integer texture types cannot even use a sampler.
-    sampler_type = wgpu.SamplerBindingType.filtering
-    # On Vanilla wgpu, float32 textures cannot use a filtering
-    # (interpolating) texture, but we request a feature so that we can.
-    # if "32float" in texture_format:
-    #     sampler_type = wgpu.SamplerBindingType.non_filtering
-    #     texture_sample_type = wgpu.TextureSampleType.unfilterable_float
-
     # Bindings and layout
     bindings = [
         {"binding": 0, "resource": texture_view},
         {"binding": 1, "resource": sampler},
     ]
     binding_layouts = [
         {
```

### Comparing `wgpu-0.9.4/tests/test_util_compute.py` & `wgpu-0.9.5/tests/test_util_compute.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/test_util_shadertoy.py` & `wgpu-0.9.5/tests/test_util_shadertoy.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/tests/testutils.py` & `wgpu-0.9.5/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/__init__.py` & `wgpu-0.9.5/wgpu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ._coreutils import logger  # noqa: F401,F403
 from .flags import *  # noqa: F401,F403
 from .enums import *  # noqa: F401,F403
 from .base import *  # noqa: F401,F403
 from .gui import WgpuCanvasInterface  # noqa: F401,F403
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 version_info = tuple(map(int, __version__.split(".")))
 
 
 def _register_backend(cls):
     """Backends call this to acticate themselves."""
     GPU = cls  # noqa: N806
     if not (
```

### Comparing `wgpu-0.9.4/wgpu/_coreutils.py` & `wgpu-0.9.5/wgpu/_coreutils.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/backends/js.py` & `wgpu-0.9.5/wgpu/backends/js.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/backends/rs.py` & `wgpu-0.9.5/wgpu/backends/rs.py`

 * *Files 1% similar despite different names*

```diff
@@ -658,24 +658,14 @@
                 i1 = enummap.get(f"FeatureName.{f}", None)
                 i2 = getattr(lib, f"WGPUNativeFeature_{f.upper()}", None)
                 i = i2 if i1 is None else i1
                 if i is None:
                     raise KeyError(f"Unknown feature: '{f}'")
                 c_features.add(i)
 
-        # Vanilla WGPU does not support interpolating samplers for float32 textures,
-        # which is sad for scientific data in particular. We can enable it
-        # (on the hardware were wgpu-py likely runs) using the feature:
-        # WGPUNativeFeature_TEXTURE_ADAPTER_SPECIFIC_FORMAT_FEATURES
-
-        builtin_features = [
-            lib.WGPUNativeFeature_TEXTURE_ADAPTER_SPECIFIC_FORMAT_FEATURES
-        ]
-        c_features.update(builtin_features)
-
         c_features = sorted(c_features)  # makes it a list
 
         # ----- Set limits
 
         # H: nextInChain: WGPUChainedStruct *, limits: WGPULimits
         c_required_limits = new_struct_p(
             "WGPURequiredLimits *",
```

### Comparing `wgpu-0.9.4/wgpu/backends/rs_ffi.py` & `wgpu-0.9.5/wgpu/backends/rs_ffi.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/backends/rs_helpers.py` & `wgpu-0.9.5/wgpu/backends/rs_helpers.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/backends/rs_mappings.py` & `wgpu-0.9.5/wgpu/backends/rs_mappings.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/base.py` & `wgpu-0.9.5/wgpu/base.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/enums.py` & `wgpu-0.9.5/wgpu/enums.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/flags.py` & `wgpu-0.9.5/wgpu/flags.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/_offscreen.py` & `wgpu-0.9.5/wgpu/gui/_offscreen.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/auto.py` & `wgpu-0.9.5/wgpu/gui/auto.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/base.py` & `wgpu-0.9.5/wgpu/gui/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 
     def handle_event(self, event):
         """Handle an incoming event.
 
         Subclasses can overload this method. Events include widget
         resize, mouse/touch interaction, key events, and more. An event
         is a dict with at least the key event_type. For details, see
-        https://jupyter-rfb.readthedocs.io/en/latest/events.html
+        https://jupyter-rfb.readthedocs.io/en/stable/events.html
 
         The default implementation dispatches the event to the
         registered event handlers.
         """
         # Collect callbacks
         event_type = event.get("event_type")
         callbacks = self._event_handlers[event_type] | self._event_handlers["*"]
@@ -305,15 +305,15 @@
 
         Arguments:
             callback (callable): The event handler. Must accept a
                 single event argument.
             *types (list of strings): A list of event types.
 
         For the available events, see
-        https://jupyter-rfb.readthedocs.io/en/latest/events.html
+        https://jupyter-rfb.readthedocs.io/en/stable/events.html
 
         Can also be used as a decorator.
 
         Example:
 
         .. code-block:: py
```

### Comparing `wgpu-0.9.4/wgpu/gui/glfw.py` & `wgpu-0.9.5/wgpu/gui/glfw.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/jupyter.py` & `wgpu-0.9.5/wgpu/gui/jupyter.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/offscreen.py` & `wgpu-0.9.5/wgpu/gui/offscreen.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/gui/qt.py` & `wgpu-0.9.5/wgpu/gui/qt.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,24 @@
         break
 else:
     raise ImportError(
         "Before importing wgpu.gui.qt, import one of PySide6/PySide2/PyQt6/PyQt5 to select a Qt toolkit."
     )
 
 
+# Get version
+if libname.startswith("PySide"):
+    qt_version_info = QtCore.__version_info__
+else:
+    try:
+        qt_version_info = tuple(int(i) for i in QtCore.QT_VERSION_STR.split(".")[:3])
+    except Exception:  # Failsafe
+        qt_version_info = (0, 0, 0)
+
+
 BUTTON_MAP = {
     QtCore.Qt.MouseButton.LeftButton: 1,  # == MOUSE_BUTTON_LEFT
     QtCore.Qt.MouseButton.RightButton: 2,  # == MOUSE_BUTTON_RIGHT
     QtCore.Qt.MouseButton.MiddleButton: 3,  # == MOUSE_BUTTON_MIDDLE
     QtCore.Qt.MouseButton.BackButton: 4,
     QtCore.Qt.MouseButton.ForwardButton: 5,
     QtCore.Qt.MouseButton.TaskButton: 6,
@@ -94,26 +104,23 @@
 # is_wayland = "wayland" in os.getenv("XDG_SESSION_TYPE", "").lower()
 # if is_wayland:
 #     os.environ["QT_QPA_PLATFORM"] = "wayland"
 
 
 def enable_hidpi():
     """Enable high-res displays."""
-    try:
-        set_dpi_aware = QtCore.__version_info__ < (6, 4)
-    except Exception:
-        set_dpi_aware = True
-    try:
-        # See https://github.com/pyzo/pyzo/pull/700 why we seem to need both
-        # See https://github.com/pygfx/pygfx/issues/368 for high Qt versions
-        if set_dpi_aware:
+    set_dpi_aware = qt_version_info < (6, 4)  # Pyside
+    if set_dpi_aware:
+        try:
+            # See https://github.com/pyzo/pyzo/pull/700 why we seem to need both
+            # See https://github.com/pygfx/pygfx/issues/368 for high Qt versions
             ctypes.windll.shcore.SetProcessDpiAwareness(1)  # global dpi aware
             ctypes.windll.shcore.SetProcessDpiAwareness(2)  # per-monitor dpi aware
-    except Exception:
-        pass  # fail on non-windows
+        except Exception:
+            pass  # fail on non-windows
     try:
         QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)
     except Exception:
         pass  # fail on older Qt's
 
 
 # If you import this module, you want to use wgpu in a way that does not suck
```

### Comparing `wgpu-0.9.4/wgpu/gui/wx.py` & `wgpu-0.9.5/wgpu/gui/wx.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/resources/webgpu.h` & `wgpu-0.9.5/wgpu/resources/webgpu.h`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/resources/webgpu.idl` & `wgpu-0.9.5/wgpu/resources/webgpu.idl`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/resources/wgpu.h` & `wgpu-0.9.5/wgpu/resources/wgpu.h`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/structs.py` & `wgpu-0.9.5/wgpu/structs.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/utils/__init__.py` & `wgpu-0.9.5/wgpu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/utils/_compute.py` & `wgpu-0.9.5/wgpu/utils/_compute.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/utils/_device.py` & `wgpu-0.9.5/wgpu/utils/_device.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu/utils/shadertoy.py` & `wgpu-0.9.5/wgpu/utils/shadertoy.py`

 * *Files identical despite different names*

### Comparing `wgpu-0.9.4/wgpu.egg-info/PKG-INFO` & `wgpu-0.9.5/wgpu.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: wgpu
-Version: 0.9.4
+Version: 0.9.5
 Summary: Next generation GPU API for Python
 Home-page: https://github.com/pygfx/wgpu-py
 Author: Almar Klein
 Author-email: almar.klein@gmail.com
 License: BSD 2-Clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cffi>=1.15.0rc2
+Requires-Dist: rubicon-objc>=0.4.1; sys_platform == "darwin"
 Provides-Extra: jupyter
+Requires-Dist: jupyter_rfb>=0.3.1; extra == "jupyter"
 Provides-Extra: glfw
+Requires-Dist: glfw>=1.9; extra == "glfw"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx>7.2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 [![CI](https://github.com/pygfx/wgpu-py/workflows/CI/badge.svg)](https://github.com/pygfx/wgpu-py/actions)
-[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=latest)](https://wgpu-py.readthedocs.io)
+[![Documentation Status](https://readthedocs.org/projects/wgpu-py/badge/?version=stable)](https://wgpu-py.readthedocs.io)
 [![PyPI version](https://badge.fury.io/py/wgpu.svg)](https://badge.fury.io/py/wgpu)
 
 # wgpu-py
 
 A Python implementation of WebGPU - the next generation GPU API.
 
 <img width=300 src='https://raw.githubusercontent.com/pygfx/wgpu-py/main/examples/screenshots/cube.png' />
```

### Comparing `wgpu-0.9.4/wgpu.egg-info/SOURCES.txt` & `wgpu-0.9.5/wgpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

