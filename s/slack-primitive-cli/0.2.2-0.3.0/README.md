# Comparing `tmp/slack_primitive_cli-0.2.2.tar.gz` & `tmp/slack_primitive_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_primitive_cli-0.2.2.tar", max compression
+gzip compressed data, was "slack_primitive_cli-0.3.0.tar", max compression
```

## Comparing `slack_primitive_cli-0.2.2.tar` & `slack_primitive_cli-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1080 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/LICENSE
--rw-r--r--   0        0        0     6303 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/README.md
--rw-r--r--   0        0        0     1093 2023-05-16 03:50:33.043161 slack_primitive_cli-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       64 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/__init__.py
--rw-r--r--   0        0        0      414 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/__main__.py
--rw-r--r--   0        0        0      131 2023-05-16 03:50:33.047161 slack_primitive_cli-0.2.2/slack_primitive_cli/__version__.py
--rw-r--r--   0        0        0        0 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/__init__.py
--rw-r--r--   0        0        0     4259 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/chat.py
--rw-r--r--   0        0        0     2393 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/files.py
--rw-r--r--   0        0        0        0 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/common/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/common/utils.py
--rw-r--r--   0        0        0     7231 1970-01-01 00:00:00.000000 slack_primitive_cli-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6312 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/README.md
+-rw-r--r--   0        0        0     3625 2024-05-13 05:50:21.746262 slack_primitive_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/__main__.py
+-rw-r--r--   0        0        0      131 2024-05-13 05:50:21.746262 slack_primitive_cli-0.3.0/slack_primitive_cli/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/command/__init__.py
+-rw-r--r--   0        0        0     4498 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/command/chat.py
+-rw-r--r--   0        0        0     2398 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/command/files.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/common/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-13 05:50:08.882134 slack_primitive_cli-0.3.0/slack_primitive_cli/common/utils.py
+-rw-r--r--   0        0        0     7236 1970-01-01 00:00:00.000000 slack_primitive_cli-0.3.0/PKG-INFO
```

### Comparing `slack_primitive_cli-0.2.2/LICENSE` & `slack_primitive_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_primitive_cli-0.2.2/README.md` & `slack_primitive_cli-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # slack-primitive-cli
-[![Build Status](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli)
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/slack-primitive-cli)
 [![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)
 [![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)
 
 `slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.
 Command line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.
 
 
@@ -158,8 +158,8 @@
 ```
 
 
 See [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.
 
 
 # Usage for Developer
-Refer to https://github.com/kurusugawa-computer/slack-primitive-cli/blob/main/README_for_developer.md .
+Refer to https://github.com/kurusugawa-computer/slack-primitive-cli/blob/main/README_for_developer.md .
```

### Comparing `slack_primitive_cli-0.2.2/slack_primitive_cli/command/chat.py` & `slack_primitive_cli-0.3.0/slack_primitive_cli/command/chat.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,23 +4,20 @@
 import slack_sdk
 
 from slack_primitive_cli.common.utils import TOKEN_ENVVAR, TOKEN_HELP_MESSAGE, set_logger
 
 logger = logging.getLogger(__name__)
 
 
-@click.command(
-    name="chat.postMessage", help="Sends a message to a channel. See https://api.slack.com/methods/chat.postMessage "
-)
+@click.command(name="chat.postMessage", help="Sends a message to a channel. See https://api.slack.com/methods/chat.postMessage ")
 @click.option("--token", envvar=TOKEN_ENVVAR, required=True, help=TOKEN_HELP_MESSAGE)
 @click.option(
     "--channel",
     required=True,
-    help="Channel, private group, or IM channel to send message to. "
-    "Can be an encoded ID, or a name. See below for more details.",
+    help="Channel, private group, or IM channel to send message to. " "Can be an encoded ID, or a name. See below for more details.",
 )
 @click.option(
     "--text",
     required=True,
     help="How this field works and whether it is required depends on other fields you use in your API call.",
 )
 @click.option("--as_user", type=bool, help="Pass true to post the message as the authed user, instead of as a bot.")
@@ -38,45 +35,43 @@
 )
 @click.option("--link_names", type=bool, help="Find and link channel names and usernames.")
 @click.option("--mrkdwn", type=bool, help="Disable Slack markup parsing by setting to false.")
 @click.option("--parse", type=bool, help="Change how messages are treated.")
 @click.option(
     "--reply_broadcast",
     type=bool,
-    help="Used in conjunction with thread_ts and indicates "
-    "whether reply should be made visible to everyone in the channel or conversation.",
+    help="Used in conjunction with thread_ts and indicates " "whether reply should be made visible to everyone in the channel or conversation.",
 )
 @click.option(
     "--thread_ts",
-    help="Provide another message's ts value to make this message a reply. "
-    "Avoid using a reply's ts value; use its parent instead.",
+    help="Provide another message's ts value to make this message a reply. " "Avoid using a reply's ts value; use its parent instead.",
 )
 @click.option("--unfurl_links", type=bool, help="Pass true to enable unfurling of primarily text-based content.")
 @click.option("--unfurl_media", type=bool, help="Pass false to disable unfurling of media content.")
 @click.option(
     "--username",
     help="Set your bot's user name. Must be used in conjunction with as_user set to false, otherwise ignored.",
 )
-def postMessage(
+def postMessage(  # noqa: ANN201, PLR0913
     token: str,
     channel: str,
     text: str,
-    as_user,
-    attachments,
-    blocks,
-    icon_emoji,
-    icon_url,
-    link_names,
-    mrkdwn,
-    parse,
-    reply_broadcast,
-    thread_ts,
-    unfurl_links,
-    unfurl_media,
-    username,
+    as_user,  # noqa: ANN001
+    attachments,  # noqa: ANN001
+    blocks,  # noqa: ANN001
+    icon_emoji,  # noqa: ANN001
+    icon_url,  # noqa: ANN001
+    link_names,  # noqa: ANN001
+    mrkdwn,  # noqa: ANN001
+    parse,  # noqa: ANN001
+    reply_broadcast,  # noqa: ANN001
+    thread_ts,  # noqa: ANN001
+    unfurl_links,  # noqa: ANN001
+    unfurl_media,  # noqa: ANN001
+    username,  # noqa: ANN001
 ):
     set_logger()
     client = slack_sdk.WebClient(token=token)
     response = client.chat_postMessage(
         channel=channel,
         text=text,
         as_user=as_user,
@@ -104,13 +99,13 @@
 @click.option(
     "--as_user",
     type=bool,
     help="Pass true to delete the message as the authed user with chat:write:user scope. "
     "Bot users in this context are considered authed users. "
     "If unused or false, the message will be deleted with chat:write:bot scope.",
 )
-def delete(token: str, channel: str, ts: str, as_user):
+def delete(token: str, channel: str, ts: str, as_user):  # noqa: ANN001, ANN201
     set_logger()
     client = slack_sdk.WebClient(token=token)
     response = client.chat_delete(channel=channel, ts=ts, as_user=as_user)
     print(response)
     return response
```

### Comparing `slack_primitive_cli-0.2.2/slack_primitive_cli/command/files.py` & `slack_primitive_cli-0.3.0/slack_primitive_cli/command/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,39 +8,33 @@
 from slack_primitive_cli.common.utils import TOKEN_ENVVAR, TOKEN_HELP_MESSAGE, my_backoff, set_logger
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(name="files.upload", help="Uploads or creates a file. See https://api.slack.com/methods/files.upload ")
 @click.option("--token", envvar=TOKEN_ENVVAR, required=True, help=TOKEN_HELP_MESSAGE)
-@click.option(
-    "--channels", required=True, help="Comma-separated list of channel names or IDs where the file will be shared."
-)
+@click.option("--channel_id", required=True, help="Channel IDs where the file will be shared.")
 @optgroup.group("File contents", cls=RequiredMutuallyExclusiveOptionGroup)
-@optgroup.option(
-    "--file", help="File contents via multipart/form-data. If omitting this parameter, you must submit content."
-)
-@optgroup.option(
-    "--content", help="File contents via a POST variable. If omitting this parameter, you must provide a file."
-)
+@optgroup.option("--file", help="File contents via multipart/form-data. If omitting this parameter, you must submit content.")
+@optgroup.option("--content", help="File contents via a POST variable. If omitting this parameter, you must provide a file.")
 @click.option("--filename", help="Filename of file.")
 @click.option("--filetype", help="A file type identifier. See also https://api.slack.com/types/file#file_types .")
 @click.option("--initial_comment", help="The message text introducing the file in specified channels.")
 @click.option("--thread_ts", help="Provide another message's ts value to upload this file as a reply.")
 @click.option("--title", help="Title of file.")
 @my_backoff
-def upload(token, channels, file, content, filename, filetype, initial_comment, thread_ts, title):
+def upload(token, channel_id, file, content, filename, filetype, initial_comment, thread_ts, title):  # noqa: ANN001, ANN201
     set_logger()
     client = slack_sdk.WebClient(token=token)
 
     if filename is None and file is not None:
         filename = os.path.basename(file)
 
-    response = client.files_upload(
-        channels=channels,
+    response = client.files_upload_v2(
+        channel=channel_id,
         file=file,
         content=content,
         filename=filename,
         filetype=filetype,
         initial_comment=initial_comment,
         thread_ts=thread_ts,
         title=title,
@@ -49,13 +43,13 @@
     return response
 
 
 @click.command(name="files.delete", help="Deletes a file. See https://api.slack.com/methods/files.delete ")
 @click.option("--token", envvar=TOKEN_ENVVAR, required=True, help=TOKEN_HELP_MESSAGE)
 @click.option("--file", required=True, help="ID of file to delete.")
 @my_backoff
-def delete(token, file):
+def delete(token, file):  # noqa: ANN001, ANN201
     set_logger()
     client = slack_sdk.WebClient(token=token)
     response = client.files_delete(file=file)
     print(response)
     return response
```

### Comparing `slack_primitive_cli-0.2.2/slack_primitive_cli/common/utils.py` & `slack_primitive_cli-0.3.0/slack_primitive_cli/common/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import backoff
 from slack_sdk.errors import SlackClientError
 
 TOKEN_ENVVAR = "SLACK_API_TOKEN"
 TOKEN_HELP_MESSAGE = f"Authentication token. If not specified, refer `{TOKEN_ENVVAR}` environment variable."
 
 
-def set_logger():
+def set_logger() -> None:
     logging_formatter = "%(levelname)-8s : %(asctime)s : %(filename)s : %(name)s : %(funcName)s : %(message)s"
     logging.basicConfig(format=logging_formatter)
     logging.getLogger("slack_primitive_cli").setLevel(level=logging.DEBUG)
 
 
-def my_backoff(function):
+def my_backoff(function):  # noqa: ANN001, ANN201
     """
     タイムアウトが発生したときにリトライする. 最大5分間リトライする。
     """
 
     @functools.wraps(function)
-    def wrapped(*args, **kwargs):
-        def fatal_code(e):
+    def wrapped(*args, **kwargs):  # noqa: ANN002, ANN003, ANN202
+        def fatal_code(e):  # noqa: ANN001, ANN202
             if isinstance(e, socket.timeout):
                 return False
             elif isinstance(e, URLError):
                 return False
             else:
                 return True
```

### Comparing `slack_primitive_cli-0.2.2/PKG-INFO` & `slack_primitive_cli-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: slack-primitive-cli
-Version: 0.2.2
+Version: 0.3.0
 Summary: Primitive Slack CLI
 Home-page: https://github.com/kurusugawa-computer/slack-primitive-cli
 License: MIT
 Keywords: slack,cli
 Author: Kurusugawa Computer Inc.
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,15 @@
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-option-group
 Requires-Dist: slack-sdk (>=3,<4)
 Project-URL: Repository, https://github.com/kurusugawa-computer/slack-primitive-cli
 Description-Content-Type: text/markdown
 
 # slack-primitive-cli
-[![Build Status](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli)
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/slack-primitive-cli)
 [![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)
 [![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)
 
 `slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.
 Command line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.
 
 
@@ -184,7 +184,8 @@
 
 
 See [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.
 
 
 # Usage for Developer
 Refer to https://github.com/kurusugawa-computer/slack-primitive-cli/blob/main/README_for_developer.md .
+
```

