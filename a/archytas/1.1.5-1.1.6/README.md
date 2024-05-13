# Comparing `tmp/archytas-1.1.5.tar.gz` & `tmp/archytas-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-1.1.5.tar", max compression
+gzip compressed data, was "archytas-1.1.6.tar", max compression
```

## Comparing `archytas-1.1.5.tar` & `archytas-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2024-02-07 21:40:45.035603 archytas-1.1.5/LICENSE
--rw-r--r--   0        0        0     2088 2024-02-07 21:40:45.035603 archytas-1.1.5/README.md
--rw-r--r--   0        0        0        0 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/__init__.py
--rw-r--r--   0        0        0    14213 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/agent.py
--rw-r--r--   0        0        0    10031 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/demo_tools.py
--rw-r--r--   0        0        0     4257 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/prompt.py
--rw-r--r--   0        0        0     3247 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/python.py
--rw-r--r--   0        0        0    12375 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/react.py
--rw-r--r--   0        0        0     2116 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/repl.py
--rw-r--r--   0        0        0    14435 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/tool_utils.py
--rw-r--r--   0        0        0     4560 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/tools.py
--rw-r--r--   0        0        0     1280 2024-02-07 21:40:45.035603 archytas-1.1.5/archytas/utils.py
--rw-r--r--   0        0        0      817 2024-02-07 21:40:45.063603 archytas-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 archytas-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    32472 2024-05-13 18:12:00.873649 archytas-1.1.6/LICENSE
+-rw-r--r--   0        0        0     2088 2024-05-13 18:12:00.873649 archytas-1.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/__init__.py
+-rw-r--r--   0        0        0    14651 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/agent.py
+-rw-r--r--   0        0        0    10031 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4257 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/prompt.py
+-rw-r--r--   0        0        0     3247 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/python.py
+-rw-r--r--   0        0        0    13221 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/react.py
+-rw-r--r--   0        0        0     2116 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/repl.py
+-rw-r--r--   0        0        0    14435 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4560 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/tools.py
+-rw-r--r--   0        0        0     1280 2024-05-13 18:12:00.873649 archytas-1.1.6/archytas/utils.py
+-rw-r--r--   0        0        0      817 2024-05-13 18:12:00.905649 archytas-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 archytas-1.1.6/PKG-INFO
```

### Comparing `archytas-1.1.5/LICENSE` & `archytas-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/README.md` & `archytas-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/agent.py` & `archytas-1.1.6/archytas/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -282,14 +282,18 @@
         """Send a user query to the agent. Returns the agent's response"""
         return await self.handle_message(Message(role=Role.user, content=message))
 
     async def observe(self, observation: str) -> str:
         """Send a system/tool observation to the agent. Returns the agent's response"""
         return await self.handle_message(Message(role=Role.system, content=observation))
 
+    async def inspect(self, query: str) -> str:
+        """Send one-off system query that is not recorded in history"""
+        return await self.execute([Message(role=Role.system, content=query)])
+
     async def error(self, error: str, drop_error: bool = True) -> str:
         """
         Send an error message to the agent. Returns the agent's response.
 
         Args:
             error (str): The error message to send to the agent.
             drop_error (bool, optional): If True, the error message and LLMs bad input will be dropped from the chat history. Defaults to `True`.
@@ -299,17 +303,17 @@
         # Drop error + LLM's bad input from chat history
         if drop_error:
             del self.messages[-3:-1]
 
         return result
 
     @retry
-    async def execute(self) -> str:
+    async def execute(self, additional_messages: list[Message] = []) -> str:
         with self.spinner():
-            messages = await self.all_messages()
+            messages = (await self.all_messages()) + additional_messages
             if self.verbose:
                 self.debug(event_type="llm_request", content=messages)
             completion = openai.chat.completions.create(
                 model=self.model,
                 messages=messages,
                 temperature=0,
             )
@@ -365,14 +369,18 @@
         """Synchronous wrapper around the asynchronous query method."""
         return asyncio.run(self.query(message))
 
     def observe_sync(self, observation: str) -> str:
         """Synchronous wrapper around the asynchronous observe method."""
         return asyncio.run(self.observe(observation))
 
+    def inspect_sync(self, message: str) -> str:
+        """Synchronous wrapper around the asynchronous inspect method."""
+        return asyncio.run(self.inspect(message))
+
     def error_sync(self, error: str, drop_error: bool = True) -> str:
         """Synchronous wrapper around the asynchronous error method."""
         return asyncio.run(self.error(error, drop_error))
 
     def execute_sync(self) -> str:
         """Synchronous wrapper around the asynchronous execute method."""
         return asyncio.run(self.execute())
```

### Comparing `archytas-1.1.5/archytas/demo_tools.py` & `archytas-1.1.6/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/prompt.py` & `archytas-1.1.6/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/python.py` & `archytas-1.1.6/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/react.py` & `archytas-1.1.6/archytas/react.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,34 @@
         # number of errors and steps during current task
         self.errors = 0
         self.steps = 0
 
         # keep track of the last tool used (for error messages)
         self.last_tool_name = ""
 
+    def update_prompt(self):
+        tool_list = list(self.tools.values())
+        self.prompt = build_prompt(tool_list)
+        self.system_message["content"] = self.prompt
+    
+    def disable(self, *tool_names):
+        if len(tool_names) == 0:
+            return
+        for tool_name in tool_names:
+            if tool_name in self.tools:
+                self.tools.pop(tool_name)
+            elif "." not in tool_name:
+                matches = [name for name in self.tools.keys() if name.endswith(f".{tool_name}")]
+                if len(matches) > 1:
+                    raise ValueError(f"Ambiguous name: Multiple tools called '{tool_name}'")
+                elif len(matches) == 1:
+                    self.tools.pop(matches[0])
+        self.update_prompt()
+                
+
     def thought_callback(self, thought: str, tool_name: str, tool_input: str) -> None:
         if self.verbose:
             # TODO: better coloring
             self.print(
                 f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n"
             )
 
@@ -278,25 +298,25 @@
 
         thought = action["thought"]
         tool = action["tool"]
         tool_input = action["tool_input"]
 
         return thought, tool, tool_input
 
-    def execute(self) -> str:
+    def execute(self, additional_messages: list[Message] = []) -> str:
         """
         Execute the model and return the output (see `Agent.execute()`).
         Keeps track of the number of execute calls, and raises an error if there are too many.
         """
         self.steps += 1
         if self.steps > self.max_react_steps:
             raise FailedTaskError(
                 f"Too many steps ({self.steps} > max_react_steps) during task.\nLast action should have been either final_answer or fail_task. Instead got: {self.last_tool_name}"
             )
-        return super().execute()
+        return super().execute(additional_messages)
 
     def error(self, mesg) -> str:
         """error handling. If too many errors, break the ReAct loop. Otherwise tell the agent, and continue"""
 
         self.errors += 1
         if self.errors >= self.max_errors:
             raise FailedTaskError(f"Too many errors during task. Last error: {mesg}")
```

### Comparing `archytas-1.1.5/archytas/repl.py` & `archytas-1.1.6/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/tool_utils.py` & `archytas-1.1.6/archytas/tool_utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/tools.py` & `archytas-1.1.6/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/archytas/utils.py` & `archytas-1.1.6/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.1.5/pyproject.toml` & `archytas-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "1.1.5"
+version = "1.1.6"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>", "Matthew Printz <matt@jataware.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-1.1.5/PKG-INFO` & `archytas-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 1.1.5
+Version: 1.1.6
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

