# Comparing `tmp/elm-messenger-0.2.6.tar.gz` & `tmp/elm_messenger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.6.tar", last modified: Sat Jun  3 16:15:26 2023, max compression
+gzip compressed data, was "elm_messenger-0.3.0.tar", last modified: Mon May 13 00:13:27 2024, max compression
```

## Comparing `elm-messenger-0.2.6.tar` & `elm_messenger-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7109 2023-05-31 16:29:21.000000 elm-messenger-0.2.6/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    20016 2023-06-03 16:12:48.000000 elm-messenger-0.2.6/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      798 2023-06-03 16:04:50.000000 elm-messenger-0.2.6/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.6/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-06-03 16:15:26.258000 elm-messenger-0.2.6/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7181 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     8444 2024-05-12 23:36:00.000000 elm_messenger-0.3.0/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/setup.py
```

### Comparing `elm-messenger-0.2.6/PKG-INFO` & `elm_messenger-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.2.6
+Version: 0.3.0
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: typer
 
 # The Messenger Game Framework
 
 Messenger is a *message-oriented* (2D) game framework for Elm based on **[canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)**.
 
 Messenger is **not** an elm package, it is a framework so some code will be generated by script in your project.
 
 ## Games made with Messenger
 
-- [Reweave](https://focs.ji.sjtu.edu.cn/silverfocs/demo/2022/p2team01/)
-- Waiting for your project!
+- [Reweave](https://github.com/linsyking/Reweave)
+- [SilverFOCS Games](https://focs.ji.sjtu.edu.cn/silverfocs/project/2023/p2) (all games in 2023 are powered by Messenger)
 
 I recommend you to play the game Reweave. There are many examples explained with Reweave in the documentation.
 
 > Hints on playing Reweave:
 >
 > You can press \` button to open the console and use some cheat commands:
 >
```

### Comparing `elm-messenger-0.2.6/Readme.md` & `elm_messenger-0.3.0/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 Messenger is a *message-oriented* (2D) game framework for Elm based on **[canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)**.
 
 Messenger is **not** an elm package, it is a framework so some code will be generated by script in your project.
 
 ## Games made with Messenger
 
-- [Reweave](https://focs.ji.sjtu.edu.cn/silverfocs/demo/2022/p2team01/)
-- Waiting for your project!
+- [Reweave](https://github.com/linsyking/Reweave)
+- [SilverFOCS Games](https://focs.ji.sjtu.edu.cn/silverfocs/project/2023/p2) (all games in 2023 are powered by Messenger)
 
 I recommend you to play the game Reweave. There are many examples explained with Reweave in the documentation.
 
 > Hints on playing Reweave:
 >
 > You can press \` button to open the console and use some cheat commands:
 >
```

### Comparing `elm-messenger-0.2.6/elm_messenger.egg-info/PKG-INFO` & `elm_messenger-0.3.0/elm_messenger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.2.6
+Version: 0.3.0
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: typer
 
 # The Messenger Game Framework
 
 Messenger is a *message-oriented* (2D) game framework for Elm based on **[canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)**.
 
 Messenger is **not** an elm package, it is a framework so some code will be generated by script in your project.
 
 ## Games made with Messenger
 
-- [Reweave](https://focs.ji.sjtu.edu.cn/silverfocs/demo/2022/p2team01/)
-- Waiting for your project!
+- [Reweave](https://github.com/linsyking/Reweave)
+- [SilverFOCS Games](https://focs.ji.sjtu.edu.cn/silverfocs/project/2023/p2) (all games in 2023 are powered by Messenger)
 
 I recommend you to play the game Reweave. There are many examples explained with Reweave in the documentation.
 
 > Hints on playing Reweave:
 >
 > You can press \` button to open the console and use some cheat commands:
 >
```

### Comparing `elm-messenger-0.2.6/messengercli/updater.py` & `elm_messenger-0.3.0/messengercli/updater.py`

 * *Files identical despite different names*

