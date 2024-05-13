# Comparing `tmp/xminigrid-0.7.1.tar.gz` & `tmp/xminigrid-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xminigrid-0.7.1.tar", last modified: Wed May  1 13:24:58 2024, max compression
+gzip compressed data, was "xminigrid-0.8.0.tar", last modified: Mon May 13 19:04:08 2024, max compression
```

## Comparing `xminigrid-0.7.1.tar` & `xminigrid-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.813810 xminigrid-0.7.1/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    11357 2024-02-01 08:42:11.000000 xminigrid-0.7.1/LICENSE
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-05-01 13:24:58.811986 xminigrid-0.7.1/PKG-INFO
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16538 2024-03-24 10:53:49.000000 xminigrid-0.7.1/README.md
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2346 2024-04-09 13:16:59.000000 xminigrid-0.7.1/pyproject.toml
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)       38 2024-05-01 13:24:58.813856 xminigrid-0.7.1/setup.cfg
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      131 2023-12-01 17:14:46.000000 xminigrid-0.7.1/setup.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.793691 xminigrid-0.7.1/src/
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.799039 xminigrid-0.7.1/src/xminigrid/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7107 2024-04-09 07:56:53.000000 xminigrid-0.7.1/src/xminigrid/__init__.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4447 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/benchmarks.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.803382 xminigrid-0.7.1/src/xminigrid/core/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4638 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/core/actions.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2597 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/constants.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    13372 2024-04-15 15:41:50.000000 xminigrid-0.7.1/src/xminigrid/core/goals.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7006 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/grid.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5144 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/observation.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16622 2024-04-30 14:39:53.000000 xminigrid-0.7.1/src/xminigrid/core/rules.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4233 2024-03-02 10:45:31.000000 xminigrid-0.7.1/src/xminigrid/environment.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.804715 xminigrid-0.7.1/src/xminigrid/envs/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      641 2023-12-01 17:14:47.000000 xminigrid-0.7.1/src/xminigrid/envs/__init__.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.809209 xminigrid-0.7.1/src/xminigrid/envs/minigrid/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3184 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/blockedunlockpickup.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2443 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/doorkey.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2593 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/empty.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2303 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/fourrooms.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4712 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/lockedroom.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5370 2024-04-30 14:39:53.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/memory.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3209 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/playground.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2433 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlock.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2854 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlockpickup.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7729 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/envs/xland.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3757 2024-02-07 15:00:54.000000 xminigrid-0.7.1/src/xminigrid/envs/xland_tmp.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.809530 xminigrid-0.7.1/src/xminigrid/experimental/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3701 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/experimental/img_obs.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7130 2024-04-16 13:33:53.000000 xminigrid-0.7.1/src/xminigrid/manual_control.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1785 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/registration.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.810554 xminigrid-0.7.1/src/xminigrid/rendering/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     9278 2024-03-28 10:48:43.000000 xminigrid-0.7.1/src/xminigrid/rendering/rgb_render.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5206 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/rendering/text_render.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3597 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/rendering/utils.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1633 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/types.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2677 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/wrappers.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.810952 xminigrid-0.7.1/src/xminigrid.egg-info/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/PKG-INFO
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1209 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/SOURCES.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)        1 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/dependency_links.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      260 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/requires.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)       10 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/top_level.txt
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.231703 xminigrid-0.8.0/
+-rw-r--r--   0 nikulin    (501) staff       (20)    11357 2024-02-01 08:42:11.000000 xminigrid-0.8.0/LICENSE
+-rw-r--r--   0 nikulin    (501) staff       (20)    31136 2024-05-13 19:04:08.231503 xminigrid-0.8.0/PKG-INFO
+-rw-r--r--   0 nikulin    (501) staff       (20)    16538 2024-03-24 10:53:49.000000 xminigrid-0.8.0/README.md
+-rw-r--r--   0 nikulin    (501) staff       (20)     2346 2024-04-09 13:16:59.000000 xminigrid-0.8.0/pyproject.toml
+-rw-r--r--   0 nikulin    (501) staff       (20)       38 2024-05-13 19:04:08.231742 xminigrid-0.8.0/setup.cfg
+-rw-r--r--   0 nikulin    (501) staff       (20)      131 2023-12-01 17:14:46.000000 xminigrid-0.8.0/setup.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.221975 xminigrid-0.8.0/src/
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.224361 xminigrid-0.8.0/src/xminigrid/
+-rw-r--r--   0 nikulin    (501) staff       (20)     8007 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/__init__.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     4447 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/benchmarks.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.226535 xminigrid-0.8.0/src/xminigrid/core/
+-rw-r--r--   0 nikulin    (501) staff       (20)     4638 2024-02-13 10:01:27.000000 xminigrid-0.8.0/src/xminigrid/core/actions.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2597 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/core/constants.py
+-rw-r--r--   0 nikulin    (501) staff       (20)    13372 2024-05-02 20:17:55.000000 xminigrid-0.8.0/src/xminigrid/core/goals.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     7006 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/core/grid.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     5144 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/core/observation.py
+-rw-r--r--   0 nikulin    (501) staff       (20)    16622 2024-05-02 20:17:55.000000 xminigrid-0.8.0/src/xminigrid/core/rules.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     4186 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/environment.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.227429 xminigrid-0.8.0/src/xminigrid/envs/
+-rw-r--r--   0 nikulin    (501) staff       (20)      641 2023-12-01 17:14:47.000000 xminigrid-0.8.0/src/xminigrid/envs/__init__.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.229739 xminigrid-0.8.0/src/xminigrid/envs/minigrid/
+-rw-r--r--   0 nikulin    (501) staff       (20)     3220 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/blockedunlockpickup.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2479 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/doorkey.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2665 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/empty.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2261 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/fourrooms.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     4748 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/lockedroom.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     5392 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/memory.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     3325 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/playground.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2469 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/unlock.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2890 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/minigrid/unlockpickup.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     7773 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/envs/xland.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     3757 2024-02-07 15:00:54.000000 xminigrid-0.8.0/src/xminigrid/envs/xland_tmp.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.229874 xminigrid-0.8.0/src/xminigrid/experimental/
+-rw-r--r--   0 nikulin    (501) staff       (20)     3701 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/experimental/img_obs.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     7130 2024-05-02 20:17:55.000000 xminigrid-0.8.0/src/xminigrid/manual_control.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     1785 2024-02-13 10:01:27.000000 xminigrid-0.8.0/src/xminigrid/registration.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.230584 xminigrid-0.8.0/src/xminigrid/rendering/
+-rw-r--r--   0 nikulin    (501) staff       (20)     9278 2024-03-28 10:48:43.000000 xminigrid-0.8.0/src/xminigrid/rendering/rgb_render.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     5206 2024-03-24 10:53:49.000000 xminigrid-0.8.0/src/xminigrid/rendering/text_render.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     3597 2024-02-13 10:01:27.000000 xminigrid-0.8.0/src/xminigrid/rendering/utils.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     1633 2024-02-13 10:01:27.000000 xminigrid-0.8.0/src/xminigrid/types.py
+-rw-r--r--   0 nikulin    (501) staff       (20)     2579 2024-05-13 08:31:12.000000 xminigrid-0.8.0/src/xminigrid/wrappers.py
+drwxr-xr-x   0 nikulin    (501) staff       (20)        0 2024-05-13 19:04:08.230831 xminigrid-0.8.0/src/xminigrid.egg-info/
+-rw-r--r--   0 nikulin    (501) staff       (20)    31136 2024-05-13 19:04:08.000000 xminigrid-0.8.0/src/xminigrid.egg-info/PKG-INFO
+-rw-r--r--   0 nikulin    (501) staff       (20)     1209 2024-05-13 19:04:08.000000 xminigrid-0.8.0/src/xminigrid.egg-info/SOURCES.txt
+-rw-r--r--   0 nikulin    (501) staff       (20)        1 2024-05-13 19:04:08.000000 xminigrid-0.8.0/src/xminigrid.egg-info/dependency_links.txt
+-rw-r--r--   0 nikulin    (501) staff       (20)      260 2024-05-13 19:04:08.000000 xminigrid-0.8.0/src/xminigrid.egg-info/requires.txt
+-rw-r--r--   0 nikulin    (501) staff       (20)       10 2024-05-13 19:04:08.000000 xminigrid-0.8.0/src/xminigrid.egg-info/top_level.txt
```

### Comparing `xminigrid-0.7.1/LICENSE` & `xminigrid-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/PKG-INFO` & `xminigrid-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminigrid
-Version: 0.7.1
+Version: 0.8.0
 Summary: JAX-accelerated meta-reinforcement learning environments inspired by XLand and MiniGrid
 Author-email: Alexander Nikulin <a.p.nikulin@tinkoff.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xminigrid-0.7.1/README.md` & `xminigrid-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/pyproject.toml` & `xminigrid-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/__init__.py` & `xminigrid-0.8.0/src/xminigrid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .benchmarks import load_benchmark, registered_benchmarks
 from .registration import make, register, registered_environments
 
 # TODO: add __all__
-__version__ = "0.7.1"
+__version__ = "0.8.0"
 
 # ---------- XLand-MiniGrid environments ----------
 
 # WARN: TMP, only for FPS measurements
 # register(
 #     id="MiniGrid-1Rules",
 #     entry_point="xminigrid.envs.xland_tmp:XLandMiniGrid",
@@ -87,22 +87,38 @@
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R1",
     height=9,
     width=9,
 )
 
 register(
+    id="XLand-MiniGrid-R1-11x11",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R1",
+    height=11,
+    width=11,
+)
+
+register(
     id="XLand-MiniGrid-R1-13x13",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R1",
     height=13,
     width=13,
 )
 
 register(
+    id="XLand-MiniGrid-R1-15x15",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R1",
+    height=15,
+    width=15,
+)
+
+register(
     id="XLand-MiniGrid-R1-17x17",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R1",
     height=17,
     width=17,
 )
 
@@ -112,22 +128,38 @@
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R2",
     height=9,
     width=9,
 )
 
 register(
+    id="XLand-MiniGrid-R2-11x11",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R2",
+    height=11,
+    width=11,
+)
+
+register(
     id="XLand-MiniGrid-R2-13x13",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R2",
     height=13,
     width=13,
 )
 
 register(
+    id="XLand-MiniGrid-R2-15x15",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R2",
+    height=15,
+    width=15,
+)
+
+register(
     id="XLand-MiniGrid-R2-17x17",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R2",
     height=17,
     width=17,
 )
 
@@ -137,22 +169,38 @@
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R4",
     height=9,
     width=9,
 )
 
 register(
+    id="XLand-MiniGrid-R4-11x11",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R4",
+    height=11,
+    width=11,
+)
+
+register(
     id="XLand-MiniGrid-R4-13x13",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R4",
     height=13,
     width=13,
 )
 
 register(
+    id="XLand-MiniGrid-R4-15x15",
+    entry_point="xminigrid.envs.xland:XLandMiniGrid",
+    grid_type="R4",
+    height=15,
+    width=15,
+)
+
+register(
     id="XLand-MiniGrid-R4-17x17",
     entry_point="xminigrid.envs.xland:XLandMiniGrid",
     grid_type="R4",
     height=17,
     width=17,
 )
```

### Comparing `xminigrid-0.7.1/src/xminigrid/benchmarks.py` & `xminigrid-0.8.0/src/xminigrid/benchmarks.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/actions.py` & `xminigrid-0.8.0/src/xminigrid/core/actions.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/constants.py` & `xminigrid-0.8.0/src/xminigrid/core/constants.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/goals.py` & `xminigrid-0.8.0/src/xminigrid/core/goals.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/grid.py` & `xminigrid-0.8.0/src/xminigrid/core/grid.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/observation.py` & `xminigrid-0.8.0/src/xminigrid/core/observation.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/core/rules.py` & `xminigrid-0.8.0/src/xminigrid/core/rules.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/environment.py` & `xminigrid-0.8.0/src/xminigrid/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import abc
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, Optional, TypeVar
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from flax import struct
 
 from .core.actions import take_action
@@ -22,14 +22,15 @@
     # WARN: pytree_node=False, so you CAN NOT vmap on them!
     # You can add pytree node params, but be careful and
     # test that your code will work under jit.
     # Spoiler: probably it will not :(
     height: int = struct.field(pytree_node=False, default=9)
     width: int = struct.field(pytree_node=False, default=9)
     view_size: int = struct.field(pytree_node=False, default=7)
+    max_steps: Optional[None] = struct.field(pytree_node=False, default=None)
     render_mode: str = struct.field(pytree_node=False, default="rgb_array")
 
 
 EnvParamsT = TypeVar("EnvParamsT", bound="EnvParams")
 
 
 class Environment(abc.ABC, Generic[EnvParamsT, EnvCarryT]):
@@ -39,18 +40,14 @@
 
     def num_actions(self, params: EnvParamsT) -> int:
         return int(NUM_ACTIONS)
 
     def observation_shape(self, params: EnvParamsT) -> tuple[int, int, int]:
         return params.view_size, params.view_size, NUM_LAYERS
 
-    # TODO: NOT sure that this should be hardcoded like that...
-    def time_limit(self, params: EnvParamsT) -> int:
-        return 3 * params.height * params.width
-
     @abc.abstractmethod
     def _generate_problem(self, params: EnvParamsT, key: jax.Array) -> State[EnvCarryT]:
         ...
 
     def reset(self, params: EnvParamsT, key: jax.Array) -> TimeStep[EnvCarryT]:
         state = self._generate_problem(params, key)
         timestep = TimeStep(
@@ -72,17 +69,19 @@
             agent=new_agent,
             step_num=timestep.state.step_num + 1,
         )
         new_observation = transparent_field_of_view(new_state.grid, new_state.agent, params.view_size, params.view_size)
 
         # checking for termination or truncation, choosing step type
         terminated = check_goal(new_state.goal_encoding, new_state.grid, new_state.agent, action, changed_position)
-        truncated = jnp.equal(new_state.step_num, self.time_limit(params))
 
-        reward = jax.lax.select(terminated, 1.0 - 0.9 * (new_state.step_num / self.time_limit(params)), 0.0)
+        assert params.max_steps is not None
+        truncated = jnp.equal(new_state.step_num, params.max_steps)
+
+        reward = jax.lax.select(terminated, 1.0 - 0.9 * (new_state.step_num / params.max_steps), 0.0)
 
         step_type = jax.lax.select(terminated | truncated, StepType.LAST, StepType.MID)
         discount = jax.lax.select(terminated, jnp.asarray(0.0), jnp.asarray(1.0))
 
         timestep = TimeStep(
             state=new_state,
             step_type=step_type,
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/__init__.py` & `xminigrid-0.8.0/src/xminigrid/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/blockedunlockpickup.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/blockedunlockpickup.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,20 +31,21 @@
     )
 )
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class BlockedUnlockPickUp(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=6, width=11)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=6, width=11)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 16 * params.height**2
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=16 * params.height**2)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, _key = jax.random.split(key)
         keys = jax.random.split(_key, num=7)
 
         pickup_obj, block_obj = jax.random.choice(keys[0], _allowed_entities, shape=(2,))
         door_color, pickup_obj_color, block_obj_color = jax.random.choice(keys[1], _allowed_colors, shape=(3,))
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/doorkey.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/doorkey.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 
 _goal_encoding = AgentOnTileGoal(tile=TILES_REGISTRY[Tiles.GOAL, Colors.GREEN]).encode()
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class DoorKey(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=5, width=5)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=5, width=5)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 10 * (params.height * params.width)
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=10 * (params.height * params.width))
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, _key = jax.random.split(key)
         keys = jax.random.split(_key, num=4)
 
         wall_pos = jax.random.randint(keys[0], shape=(), minval=2, maxval=params.width - 2)
         door_pos = jax.random.randint(keys[1], shape=(), minval=1, maxval=params.width - 2)
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/empty.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/empty.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # goals and rules are hardcoded for minigrid envs
 _goal_encoding = AgentOnTileGoal(tile=TILES_REGISTRY[Tiles.GOAL, Colors.GREEN]).encode()
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class Empty(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=9, width=9)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=9, width=9)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 4 * (params.height * params.width)
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=4 * (params.height * params.width))
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         grid = room(params.height, params.width)
 
         grid = grid.at[params.height - 2, params.width - 2].set(TILES_REGISTRY[Tiles.GOAL, Colors.GREEN])
         agent = AgentState(position=jnp.array((1, 1)), direction=jnp.asarray(1))
 
@@ -40,20 +41,21 @@
             carry=EnvCarry(),
         )
         return state
 
 
 class EmptyRandom(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=9, width=9)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=9, width=9)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 4 * (params.height * params.width)
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=4 * (params.height * params.width))
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, pos_key, dir_key = jax.random.split(key, num=3)
 
         grid = room(params.height, params.width)
         grid = grid.at[params.height - 2, params.width - 2].set(TILES_REGISTRY[Tiles.GOAL, Colors.GREEN])
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/fourrooms.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/fourrooms.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # goals and rules are hardcoded for minigrid envs
 _goal_encoding = AgentOnTileGoal(tile=TILES_REGISTRY[Tiles.GOAL, Colors.GREEN]).encode()
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class FourRooms(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=19, width=19)
-        default_params = default_params.replace(**kwargs)
-        return default_params
-
-    def time_limit(self, params: EnvParams) -> int:
-        # TODO: this is hardcoded and thus problematic. Move it to EnvParams?
-        return 100
+        params = EnvParams(height=19, width=19)
+        params = params.replace(**kwargs)
+
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=100)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, *keys = jax.random.split(key, num=4)
 
         grid = four_rooms(params.height, params.width)
 
         black_floor = TILES_REGISTRY[Tiles.FLOOR, Colors.BLACK]
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/lockedroom.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/lockedroom.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,21 @@
         Colors.RED,
     )
 )
 
 
 class LockedRoom(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=19, width=19)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=19, width=19)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 10 * params.height
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=10 * params.height)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, rooms_key, colors_key, objects_key, coords_key, agent_pos_key, agent_dir_key = jax.random.split(key, num=7)
 
         # set up rooms
         grid = room(params.height, params.width)
         grid = vertical_line(grid, params.width // 2 - 2, 0, params.height, _wall_tile)
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/memory.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,20 +35,21 @@
     success_pos: jax.Array
     failure_pos: jax.Array
 
 
 # TODO: Random corridor length is a bit problematic due to the dynamic slicing.
 class Memory(Environment[EnvParams, MemoryEnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=7, width=13, view_size=3)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=7, width=13, view_size=3)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 5 * params.width**2
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=5 * params.width**2)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[MemoryEnvCarry]:
         key, corridor_key, agent_key, mem_key, place_key = jax.random.split(key, num=5)
 
         corridor_length = params.width - 6
         corridor_end = 4 + corridor_length
 
@@ -111,22 +112,22 @@
         # disabling pick_up action
         action = jax.lax.select(jnp.equal(action, 3), jnp.asarray(5, dtype=jnp.uint8), action)
         new_grid, new_agent, _ = take_action(timestep.state.grid, timestep.state.agent, action)
 
         new_state = timestep.state.replace(grid=new_grid, agent=new_agent, step_num=timestep.state.step_num + 1)
         new_observation = transparent_field_of_view(new_state.grid, new_state.agent, params.view_size, params.view_size)
 
-        truncated = new_state.step_num == self.time_limit(params)
+        truncated = new_state.step_num == params.max_steps
         terminated = jnp.logical_or(
             jnp.array_equal(new_agent.position, new_state.carry.success_pos),
             jnp.array_equal(new_agent.position, new_state.carry.failure_pos),
         )
         reward = jax.lax.select(
             jnp.array_equal(new_agent.position, new_state.carry.success_pos),
-            1.0 - 0.9 * (new_state.step_num / self.time_limit(params)),
+            1.0 - 0.9 * (new_state.step_num / params.max_steps),
             0.0,
         )
         step_type = jax.lax.select(terminated | truncated, StepType.LAST, StepType.MID)
         discount = jax.lax.select(terminated, jnp.asarray(0.0), jnp.asarray(1.0))
 
         timestep = TimeStep(
             state=new_state,
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/playground.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/playground.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,21 @@
 
 class PlaygroundEnvParams(EnvParams):
     num_objects: int = struct.field(pytree_node=False, default=12)
 
 
 class Playground(Environment[PlaygroundEnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> PlaygroundEnvParams:
-        return PlaygroundEnvParams(height=19, width=19).replace(**kwargs)
+        params = PlaygroundEnvParams(height=19, width=19)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 512
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=512)
+        return params
 
     def _generate_problem(self, params: PlaygroundEnvParams, key: jax.Array) -> State[EnvCarry]:
         key, *keys = jax.random.split(key, num=6)
 
         grid = nine_rooms(params.height, params.width)
         roomW, roomH = params.width // 3, params.height // 3
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlock.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/unlock.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     )
 )
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class Unlock(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=6, width=11)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=6, width=11)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 8 * params.height**2
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=8 * params.height**2)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, *keys = jax.random.split(key, num=5)
 
         color = jax.random.choice(keys[0], _allowed_colors)
         door_pos = jax.random.randint(keys[1], shape=(), minval=1, maxval=params.height - 1)
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlockpickup.py` & `xminigrid-0.8.0/src/xminigrid/envs/minigrid/unlockpickup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,21 @@
     )
 )
 _rule_encoding = EmptyRule().encode()[None, ...]
 
 
 class UnlockPickUp(Environment[EnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> EnvParams:
-        default_params = EnvParams(height=6, width=11)
-        default_params = default_params.replace(**kwargs)
-        return default_params
+        params = EnvParams(height=6, width=11)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: EnvParams) -> int:
-        return 8 * params.height**2
+        if params.max_steps is None:
+            # formula directly taken from MiniGrid
+            params = params.replace(max_steps=8 * params.height**2)
+        return params
 
     def _generate_problem(self, params: EnvParams, key: jax.Array) -> State[EnvCarry]:
         key, *keys = jax.random.split(key, num=7)
 
         obj = jax.random.choice(keys[0], _allowed_entities)
         door_color, obj_color = jax.random.choice(keys[1], _allowed_colors, shape=(2,))
         door_pos = jax.random.randint(keys[2], shape=(), minval=1, maxval=params.height - 1)
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/xland.py` & `xminigrid-0.8.0/src/xminigrid/envs/xland.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,22 +140,23 @@
     ruleset: RuleSet = struct.field(pytree_node=True, default=_empty_ruleset)
     # experimental (can not vmap on it)
     grid_type: int = struct.field(pytree_node=False, default="1R")
 
 
 class XLandMiniGrid(Environment[XLandEnvParams, EnvCarry]):
     def default_params(self, **kwargs) -> XLandEnvParams:
-        default_params = XLandEnvParams(view_size=5)
-        return default_params.replace(**kwargs)
+        params = XLandEnvParams(view_size=5)
+        params = params.replace(**kwargs)
 
-    def time_limit(self, params: XLandEnvParams) -> int:
-        # this is just a heuristic to prevent brute force in one episode,
-        # agent need to remember what he tried in previous episodes.
-        # If this is too small, change it or increase number of trials (these are not equivalent).
-        return 3 * (params.height * params.width)
+        if params.max_steps is None:
+            # this is just a heuristic to prevent brute force in one episode,
+            # so that agent need to remember what he tried in previous episodes.
+            # If this is too small, change it or increase number of trials (NB: these are not equivalent).
+            params = params.replace(max_steps=3 * (params.height * params.width))
+        return params
 
     def _generate_problem(self, params: XLandEnvParams, key: jax.Array) -> State[EnvCarry]:
         # WARN: we can make this compatible with jit (to vmap on different layouts during training),
         # but it will probably be very costly, as lax.switch will generate all layouts during reset under vmap
         # TODO: experiment with this under jit, does it possible to make it jit-compatible without overhead?
         if params.grid_type == "R1":
             key, grid = generate_room(key, params.height, params.width)
```

### Comparing `xminigrid-0.7.1/src/xminigrid/envs/xland_tmp.py` & `xminigrid-0.8.0/src/xminigrid/envs/xland_tmp.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/experimental/img_obs.py` & `xminigrid-0.8.0/src/xminigrid/experimental/img_obs.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/manual_control.py` & `xminigrid-0.8.0/src/xminigrid/manual_control.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/registration.py` & `xminigrid-0.8.0/src/xminigrid/registration.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/rendering/rgb_render.py` & `xminigrid-0.8.0/src/xminigrid/rendering/rgb_render.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/rendering/text_render.py` & `xminigrid-0.8.0/src/xminigrid/rendering/text_render.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/rendering/utils.py` & `xminigrid-0.8.0/src/xminigrid/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/types.py` & `xminigrid-0.8.0/src/xminigrid/types.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.1/src/xminigrid/wrappers.py` & `xminigrid-0.8.0/src/xminigrid/wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
     def num_actions(self, params: EnvParamsT) -> int:
         return self._env.num_actions(params)
 
     def observation_shape(self, params: EnvParamsT) -> tuple[int, int, int]:
         return self._env.observation_shape(params)
 
-    def time_limit(self, params: EnvParamsT) -> int:
-        return self._env.time_limit(params)
-
     def _generate_problem(self, params: EnvParamsT, key: jax.Array) -> State[EnvCarryT]:
         return self._env._generate_problem(params, key)
 
     def reset(self, params: EnvParamsT, key: jax.Array) -> TimeStep[EnvCarryT]:
         return self._env.reset(params, key)
 
     def step(self, params: EnvParamsT, timestep: TimeStep[EnvCarryT], action: IntOrArray) -> TimeStep[EnvCarryT]:
```

### Comparing `xminigrid-0.7.1/src/xminigrid.egg-info/PKG-INFO` & `xminigrid-0.8.0/src/xminigrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminigrid
-Version: 0.7.1
+Version: 0.8.0
 Summary: JAX-accelerated meta-reinforcement learning environments inspired by XLand and MiniGrid
 Author-email: Alexander Nikulin <a.p.nikulin@tinkoff.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xminigrid-0.7.1/src/xminigrid.egg-info/SOURCES.txt` & `xminigrid-0.8.0/src/xminigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

