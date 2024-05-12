# Comparing `tmp/twiner-0.2.1.tar.gz` & `tmp/twiner-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twiner-0.2.1.tar", max compression
+gzip compressed data, was "twiner-0.3.0.tar", max compression
```

## Comparing `twiner-0.2.1.tar` & `twiner-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-01-31 20:23:18.857000 twiner-0.2.1/LICENSE
--rw-r--r--   0        0        0     5752 2024-02-22 19:32:17.391760 twiner-0.2.1/README.md
--rw-r--r--   0        0        0     1013 2024-02-22 20:02:41.571838 twiner-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-02-22 20:02:55.878736 twiner-0.2.1/twiner/__init__.py
--rw-r--r--   0        0        0    11388 2024-02-10 14:16:03.072000 twiner-0.2.1/twiner/cli.py
--rw-r--r--   0        0        0     1422 2024-02-08 00:09:53.321000 twiner-0.2.1/twiner/config.py
--rw-r--r--   0        0        0      456 2024-02-10 16:00:12.105000 twiner-0.2.1/twiner/notify.py
--rw-r--r--   0        0        0     3301 2024-02-10 13:15:05.951000 twiner-0.2.1/twiner/twitch.py
--rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 twiner-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-31 20:23:18.857000 twiner-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5752 2024-02-22 19:32:17.391760 twiner-0.3.0/README.md
+-rw-r--r--   0        0        0     1013 2024-05-12 23:34:57.344763 twiner-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-02-22 20:08:23.511838 twiner-0.3.0/twiner/__init__.py
+-rw-r--r--   0        0        0    11273 2024-05-12 18:16:12.352203 twiner-0.3.0/twiner/cli.py
+-rw-r--r--   0        0        0     1422 2024-02-08 00:09:53.321000 twiner-0.3.0/twiner/config.py
+-rw-r--r--   0        0        0      456 2024-02-10 16:00:12.105000 twiner-0.3.0/twiner/notify.py
+-rw-r--r--   0        0        0     3301 2024-02-10 13:15:05.951000 twiner-0.3.0/twiner/twitch.py
+-rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 twiner-0.3.0/PKG-INFO
```

### Comparing `twiner-0.2.1/LICENSE` & `twiner-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twiner-0.2.1/README.md` & `twiner-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `twiner-0.2.1/pyproject.toml` & `twiner-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twiner"
-version = "0.2.1"
+version = "0.3.0"
 description = "CLI that helps you with notifications for your favorite streamers on Twitch.tv."
 authors = ["febits <febits@proton.me>"]
 readme = "README.md"
 classifiers = [
   "Environment :: Console",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `twiner-0.2.1/twiner/cli.py` & `twiner-0.3.0/twiner/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,15 @@
                                 else stream_title[:50] + "..."
                             )
                             user.viewer_count = twitch.get_streams_info(
                                 user.username
                             )["viewer_count"]
 
                             console.print(
-                                f'\t[b]{user.username}[/]: "{user.stream_title}" '
-                                f"- {user.viewer_count} viewers"
+                                f'\t[b]{user.username}[/]: "{user.stream_title}" - {user.viewer_count} viewers'
                             )
                             console.print(
                                 f"\t(ready to notify: [b][i]{user.username}[/])\n"
                             )
 
                             send_notify(user, config)
                     else:
@@ -250,22 +249,20 @@
 
                     config.yaml["tonotify"][user] = twitch.get_usericon(
                         config, user
                     )
                     config.write_to_config(config.yaml)
                 else:
                     console.print(
-                        f"\n❌ {user} doesn't exist anymore. Run 'twiner "
-                        f"remove {user}'"
+                        f"\n❌ {user} doesn't exist anymore. Run 'twiner remove {user}'"
                     )
                     raise typer.Exit(1)
 
             console.print(
-                "\n✅ User data was refreshed successfully from "
-                f"{config.path}"
+                f"\n✅ User data was refreshed successfully from {config.path}"
             )
         else:
             console.print("❌ Invalid credentials")
             raise typer.Exit(1)
 
     except FileNotFoundError as exc:
         raise FileNotFoundError("Run 'twiner init' first.") from exc
@@ -337,17 +334,15 @@
 ):
     """Init the config file (it will perform a redefining action through
     the config file, using it exclusively for the initial setup)."""
     config = TwinerConfig(configfile)
 
     if not config.path.exists():
         console.print(
-            f"[b]✅ Config file was successfully created at "
-            f"{config.path}[/]"
+            f"[b]✅ Config file was successfully created at {config.path}[/]"
         )
     else:
         console.print(
-            f"[b]❎ Config file already exists at {config.path} "
-            f"(overwriting current file)[/]"
+            f"[b]❎ Config file already exists at {config.path} (overwriting current file)[/]"
         )
 
     config.write_to_config(config.template)
```

### Comparing `twiner-0.2.1/twiner/config.py` & `twiner-0.3.0/twiner/config.py`

 * *Files identical despite different names*

### Comparing `twiner-0.2.1/twiner/twitch.py` & `twiner-0.3.0/twiner/twitch.py`

 * *Files identical despite different names*

### Comparing `twiner-0.2.1/PKG-INFO` & `twiner-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiner
-Version: 0.2.1
+Version: 0.3.0
 Summary: CLI that helps you with notifications for your favorite streamers on Twitch.tv.
 Author: febits
 Author-email: febits@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

