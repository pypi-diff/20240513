# Comparing `tmp/tcrutils-12.0.157.tar.gz` & `tmp/tcrutils-12.0.158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.157.tar", max compression
+gzip compressed data, was "tcrutils-12.0.158.tar", max compression
```

## Comparing `tcrutils-12.0.157.tar` & `tcrutils-12.0.158.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.157/LICENSE
--rw-r--r--   0        0        0      586 2024-05-12 21:19:09.621037 tcrutils-12.0.157/pyproject.toml
--rw-r--r--   0        0        0     1942 2024-05-12 19:30:06.391823 tcrutils-12.0.157/README.md
--rw-r--r--   0        0        0     4819 2024-05-11 21:17:23.617418 tcrutils-12.0.157/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-05-12 21:19:12.260084 tcrutils-12.0.157/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.157/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.157/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.157/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.157/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.157/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.157/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.157/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.157/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.157/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.157/tcrutils/dr/__init__.py
--rw-r--r--   0        0        0     8244 2024-05-11 19:05:09.032438 tcrutils-12.0.157/tcrutils/dr/core.py
--rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.157/tcrutils/dr/error.py
--rw-r--r--   0        0        0     2532 2024-05-12 21:19:02.962945 tcrutils-12.0.157/tcrutils/dr/placeholder_sets.py
--rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.157/tcrutils/dr/placeholders/__init__.py
--rw-r--r--   0        0        0     1574 2024-05-11 21:47:23.390141 tcrutils-12.0.157/tcrutils/dr/placeholders/p_discord.py
--rw-r--r--   0        0        0     4389 2024-05-12 19:28:10.182266 tcrutils-12.0.157/tcrutils/dr/placeholders/p_math.py
--rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.157/tcrutils/dr/placeholders/p_text.py
--rw-r--r--   0        0        0     4537 2024-05-12 18:55:58.211193 tcrutils-12.0.157/tcrutils/dr/util.py
--rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.157/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.157/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.157/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.157/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.157/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.157/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.157/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     4092 2024-05-11 21:11:34.733039 tcrutils-12.0.157/tcrutils/src/tcr_cloud_imports.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.157/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.157/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.157/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.157/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.157/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.157/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.157/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.157/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.157/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.157/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.157/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.157/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.157/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.157/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.157/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.157/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     3264 2024-05-11 21:18:41.050978 tcrutils-12.0.157/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.157/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.157/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.157/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.157/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.157/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.157/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.157/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.157/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.157/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.157/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     3888 2024-05-07 16:07:40.280190 tcrutils-12.0.157/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.157/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.157/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     6883 2024-05-11 21:36:56.860614 tcrutils-12.0.157/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.157/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.157/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.157/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.157/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 tcrutils-12.0.157/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.158/LICENSE
+-rw-r--r--   0        0        0      586 2024-05-12 21:19:46.998196 tcrutils-12.0.158/pyproject.toml
+-rw-r--r--   0        0        0     1942 2024-05-12 19:30:06.391823 tcrutils-12.0.158/README.md
+-rw-r--r--   0        0        0     4756 2024-05-12 21:19:42.809708 tcrutils-12.0.158/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-12 21:19:49.334966 tcrutils-12.0.158/tcrutils/_version.py
+-rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.158/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.158/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.158/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.158/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.158/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.158/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.158/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.158/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.158/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.158/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     8244 2024-05-11 19:05:09.032438 tcrutils-12.0.158/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.158/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     2532 2024-05-12 21:19:02.962945 tcrutils-12.0.158/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.158/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     1574 2024-05-11 21:47:23.390141 tcrutils-12.0.158/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4389 2024-05-12 19:28:10.182266 tcrutils-12.0.158/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.158/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0     4537 2024-05-12 18:55:58.211193 tcrutils-12.0.158/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.158/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.158/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.158/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.158/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.158/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.158/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.158/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4092 2024-05-11 21:11:34.733039 tcrutils-12.0.158/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.158/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.158/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.158/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.158/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.158/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.158/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.158/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.158/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.158/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.158/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.158/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.158/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.158/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.158/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.158/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.158/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3264 2024-05-11 21:18:41.050978 tcrutils-12.0.158/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.158/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.158/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.158/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.158/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.158/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.158/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.158/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.158/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.158/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.158/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     3888 2024-05-07 16:07:40.280190 tcrutils-12.0.158/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.158/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.158/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6883 2024-05-11 21:36:56.860614 tcrutils-12.0.158/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.158/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.158/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.158/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.158/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 tcrutils-12.0.158/PKG-INFO
```

### Comparing `tcrutils-12.0.157/LICENSE` & `tcrutils-12.0.158/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/pyproject.toml` & `tcrutils-12.0.158/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.157"
+version = "12.0.158"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
```

### Comparing `tcrutils-12.0.157/README.md` & `tcrutils-12.0.158/README.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/__init__.py` & `tcrutils-12.0.158/tcrutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from .src.tcr_constants import *
 from .src.tcr_decorator import autorun, convert, copy_kwargs, instance, test, timeit
 from .src.tcr_dev import generate_function_argument_typehints, generate_type_hinter
 from .src.tcr_dict import DotDict, JSDict, JSDotDict, clean_dunder_dict, dict_zip, merge_dicts
 from .src.tcr_dir import dir2, dir3
 from .src.tcr_error import error  # 'tcrerror' in star imports, either in 'tcr.error'/'tcr.tcrerror'
 from .src.tcr_error import error as tcrerror
-from .src.tcr_execute import Execute, MissingPlaceholderError
 from .src.tcr_extract_error import extract_error, extract_traceback
 from .src.tcr_F import F
 from .src.tcr_getch import getch
 from .src.tcr_inject import ErrorCatcher, WarningCatcher
 from .src.tcr_input import insist
 from .src.tcr_inspect import get_file_colon_lineno, get_lineno
 from .src.tcr_int import float2int, hex, recursive_sum
```

### Comparing `tcrutils-12.0.157/tcrutils/discord/__init__.py` & `tcrutils-12.0.158/tcrutils/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.158/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.158/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.158/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.158/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.158/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/core.py` & `tcrutils-12.0.158/tcrutils/dr/core.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/error.py` & `tcrutils-12.0.158/tcrutils/dr/error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/placeholder_sets.py` & `tcrutils-12.0.158/tcrutils/dr/placeholder_sets.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/placeholders/p_discord.py` & `tcrutils-12.0.158/tcrutils/dr/placeholders/p_discord.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/placeholders/p_math.py` & `tcrutils-12.0.158/tcrutils/dr/placeholders/p_math.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/placeholders/p_text.py` & `tcrutils-12.0.158/tcrutils/dr/placeholders/p_text.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/dr/util.py` & `tcrutils-12.0.158/tcrutils/dr/util.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.158/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.158/tcrutils/imgui/tcri_handler.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.158/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_class.py` & `tcrutils-12.0.158/tcrutils/src/tcr_class.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.158/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_cloud_imports.py` & `tcrutils-12.0.158/tcrutils/src/tcr_cloud_imports.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.158/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_console.py` & `tcrutils-12.0.158/tcrutils/src/tcr_console.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.158/tcrutils/src/tcr_decorator.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.158/tcrutils/src/tcr_dev.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.158/tcrutils/src/tcr_dict.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_error.py` & `tcrutils-12.0.158/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.158/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.158/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.158/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_input.py` & `tcrutils-12.0.158/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.158/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_int.py` & `tcrutils-12.0.158/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.158/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_joke.py` & `tcrutils-12.0.158/tcrutils/src/tcr_joke.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_language.py` & `tcrutils-12.0.158/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.158/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.158/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_null.py` & `tcrutils-12.0.158/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.158/tcrutils/src/tcr_overload.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_path.py` & `tcrutils-12.0.158/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_print.py` & `tcrutils-12.0.158/tcrutils/src/tcr_print.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.158/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_run.py` & `tcrutils-12.0.158/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.158/tcrutils/src/tcr_sdb.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_string.py` & `tcrutils-12.0.158/tcrutils/src/tcr_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.158/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_test.py` & `tcrutils-12.0.158/tcrutils/src/tcr_test.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.158/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.158/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/tcrutils/src/tcr_void.py` & `tcrutils-12.0.158/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.157/PKG-INFO` & `tcrutils-12.0.158/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcrutils
-Version: 12.0.157
+Version: 12.0.158
 Summary: Useful stuff for TCR projects!
 License: GPL-3.0
 Author: TheCreatorrrr
 Requires-Python: >=3.11.0,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tcrutils Version: 12.0.157 Summary: Useful stuff
+Metadata-Version: 2.1 Name: tcrutils Version: 12.0.158 Summary: Useful stuff
 for TCR projects! License: GPL-3.0 Author: TheCreatorrrr Requires-Python:
 >=3.11.0,<3.13 Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: attr (>=0.3.2,<0.4.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: colored (>=2.2.4,<3.0.0) Requires-Dist: hikari
 (>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-miru (>=4.0.0,<5.0.0) Requires-
```

