# Comparing `tmp/tg-searcher-0.4.0.tar.gz` & `tmp/tg_searcher-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-searcher-0.4.0.tar", last modified: Wed Feb  1 16:37:29 2023, max compression
+gzip compressed data, was "tg_searcher-0.5.0.tar", last modified: Mon May 13 18:04:43 2024, max compression
```

## Comparing `tg-searcher-0.4.0.tar` & `tg_searcher-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 16:37:29.704068 tg-searcher-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-02-01 16:37:29.704068 tg-searcher-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/__version__
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 16:37:29.704068 tg-searcher-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 16:37:29.704068 tg-searcher-0.4.0/tg_searcher/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/backend_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20633 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/frontend_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-01 16:37:16.000000 tg-searcher-0.4.0/tg_searcher/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 16:37:29.704068 tg-searcher-0.4.0/tg_searcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-01 16:37:29.000000 tg-searcher-0.4.0/tg_searcher.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1063 2024-05-13 18:04:32.157912 tg_searcher-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3225 2024-05-13 18:04:32.157912 tg_searcher-0.5.0/README.md
+-rw-r--r--   0        0        0     1296 2024-05-13 18:04:43.994091 tg_searcher-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/__main__.py
+-rw-r--r--   0        0        0     9659 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/backend_bot.py
+-rw-r--r--   0        0        0     2602 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/common.py
+-rw-r--r--   0        0        0    20648 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/frontend_bot.py
+-rw-r--r--   0        0        0     4932 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/indexer.py
+-rw-r--r--   0        0        0     3113 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/main.py
+-rw-r--r--   0        0        0     2074 2024-05-13 18:04:32.161913 tg_searcher-0.5.0/tg_searcher/session.py
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 tg_searcher-0.5.0/PKG-INFO
```

### Comparing `tg-searcher-0.4.0/LICENSE` & `tg_searcher-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tg-searcher-0.4.0/PKG-INFO` & `tg_searcher-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: tg-searcher
-Version: 0.4.0
+Version: 0.5.0
 Summary: Telegram searcher bot for Chinese
 Home-page: https://github.com/SharzyL/tg_searcher
-Author: Sharzy L
-Author-email: me@sharzy.in
+Author-Email: SharzyL <me@sharzy.in>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Project-URL: Changelog, https://github.com/SharzyL/tg_searcher/blob/master/CHANGELOG.md
+Project-URL: Homepage, https://github.com/SharzyL/tg_searcher
+Project-URL: Repository, https://github.com/SharzyL/tg_searcher.git
+Requires-Python: <4.0,>=3.9
+Requires-Dist: Telethon<2.0.0,>=1.32.0
+Requires-Dist: python-socks<3.0.0,>=2.4.4
+Requires-Dist: cryptg<1.0.0,>=0.4.0
+Requires-Dist: async-timeout<5.0.0,>=4.0.3
+Requires-Dist: jieba>=0.42.1
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: redis>=5.0.3
+Requires-Dist: whoosh>=2.7.4
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # TG Searcher
 
 众所周知，Telegram 的搜索功能较弱，尤其是对于中文等 CJK 语言，由于 Telegram 无法对其进行正确的分词，因此很难搜到想要的内容。本项目实现了一个通用的框架，用户可以对 Telegram 的会话建立索引，通过 bot 来便捷地搜索消息。
 
 它的使用效果见下图：
```

### Comparing `tg-searcher-0.4.0/README.md` & `tg_searcher-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tg-searcher-0.4.0/tg_searcher/backend_bot.py` & `tg_searcher-0.5.0/tg_searcher/backend_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,22 @@
         self.excluded_chats = cfg.excluded_chats
         self.newest_msg: Dict[int, IndexMsg] = dict()
 
     async def start(self):
         self._logger.info(f'Init backend bot')
 
         for chat_id in self.monitored_chats:
-            chat_name = await self.translate_chat_id(chat_id)
-            self._logger.info(f'Ready to monitor "{chat_name}" ({chat_id})')
+            try:
+                chat_name = await self.translate_chat_id(chat_id)
+                self._logger.info(f'Ready to monitor "{chat_name}" ({chat_id})')
+            except Exception as e:
+                self._logger.error(f'exception on get monitored chat (id={chat_id}): {e}')
+                self.monitored_chats.remove(chat_id)
+                self._indexer.ix.delete_by_term('chat_id', chat_id)
+                self._logger.error(f'remove chat (id={chat_id}) from monitor list and clear its index')
 
         self._register_hooks()
 
     def search(self, q: str, in_chats: Optional[List[int]], page_len: int, page_num: int):
         return self._indexer.search(q, in_chats, page_len, page_num)
 
     def rand_msg(self) -> IndexMsg:
@@ -56,34 +62,39 @@
         if chat_id is not None:
             with self._indexer.ix.searcher() as searcher:
                 return not any(True for _ in searcher.document_numbers(chat_id=str(chat_id)))
         else:
             return self._indexer.ix.is_empty()
 
     async def download_history(self, chat_id: int, min_id: int, max_id: int, call_back=None):
-        writer = self._indexer.ix.writer()
         share_id = get_share_id(chat_id)
         self._logger.info(f'Downloading history from {share_id} ({min_id=}, {max_id=})')
         self.monitored_chats.add(share_id)
+        msg_list = []
         async for tg_message in self.session.iter_messages(chat_id, min_id=min_id, max_id=max_id):
             if msg_text := self._extract_text(tg_message):
                 url = f'https://t.me/c/{share_id}/{tg_message.id}'
                 sender = await self._get_sender_name(tg_message)
                 msg = IndexMsg(
                     content=msg_text,
                     url=url,
                     chat_id=chat_id,
                     post_time=datetime.fromtimestamp(tg_message.date.timestamp()),
                     sender=sender,
                 )
-                self._indexer.add_document(msg, writer)
-                self.newest_msg[share_id] = msg
+                msg_list.append(msg)
                 if call_back:
                     await call_back(tg_message.id)
+        self._logger.info(f'fetching history from {share_id} complete, start writing index')
+        writer = self._indexer.ix.writer()
+        for msg in msg_list:
+            self._indexer.add_document(msg, writer)
+            self.newest_msg[share_id] = msg
         writer.commit()
+        self._logger.info(f'write index commit ok')
 
     def clear(self, chat_ids: Optional[List[int]] = None):
         if chat_ids is not None:
             for chat_id in chat_ids:
                 with self._indexer.ix.writer() as w:
                     w.delete_by_term('chat_id', str(chat_id))
             for chat_id in chat_ids:
```

### Comparing `tg-searcher-0.4.0/tg_searcher/common.py` & `tg_searcher-0.5.0/tg_searcher/common.py`

 * *Files identical despite different names*

### Comparing `tg-searcher-0.4.0/tg_searcher/frontend_bot.py` & `tg_searcher-0.5.0/tg_searcher/frontend_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
     async def _search(self, event: events.NewMessage.Event):
         print('start search')
         if self.backend.is_empty():
             await event.reply('当前索引为空，请先 /download_chat 建立索引')
             return
         start_time = time()
         q: str = event.raw_text
-        if q.startswith('/'):
+        if q.startswith('/') or q.startswith('@'):
             first_space = q.find(' ')
             if first_space < 0:
                 first_space = len(q)
             q = q[first_space + 1:]
 
         if len(q) == 0:
             # do not respond to empty query
@@ -424,21 +424,21 @@
                 string_builder.append(f'<b>{chat_title} (<u>{hit.msg.sender}</u>) [{hit.msg.post_time}]</b>\n')
             else:
                 string_builder.append(f'<b>{chat_title} [{hit.msg.post_time}]</b>\n')
             string_builder.append(f'<a href="{hit.msg.url}">{hit.highlighted}</a>\n')
         return ''.join(string_builder)
 
     def _render_respond_buttons(self, result, cur_page_num):
-        former_page, former_text = (None, ' ') \
+        former_page, former_text = ('', ' ') \
             if cur_page_num == 1 \
             else (f'search_page={cur_page_num - 1}', '上一页⬅️')
-        next_page, next_text = (None, ' ') \
+        next_page, next_text = ('', ' ') \
             if result.is_last_page \
             else (f'search_page={cur_page_num + 1}', '➡️下一页')
         total_pages = - (- result.total_results // self._cfg.page_len)  # use floor to simulate ceil function
         return [
             [
                 Button.inline(former_text, former_page),
-                Button.inline(f'{cur_page_num} / {total_pages}', None),
+                Button.inline(f'{cur_page_num} / {total_pages}', ''),
                 Button.inline(next_text, next_page),
             ]
         ]
```

### Comparing `tg-searcher-0.4.0/tg_searcher/indexer.py` & `tg_searcher-0.5.0/tg_searcher/indexer.py`

 * *Files identical despite different names*

### Comparing `tg-searcher-0.4.0/tg_searcher/main.py` & `tg_searcher-0.5.0/tg_searcher/main.py`

 * *Files identical despite different names*

### Comparing `tg-searcher-0.4.0/tg_searcher/session.py` & `tg_searcher-0.5.0/tg_searcher/session.py`

 * *Files identical despite different names*

