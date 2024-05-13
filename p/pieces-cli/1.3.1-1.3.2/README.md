# Comparing `tmp/pieces_cli-1.3.1.tar.gz` & `tmp/pieces_cli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pieces_cli-1.3.1.tar", max compression
+gzip compressed data, was "pieces_cli-1.3.2.tar", max compression
```

## Comparing `pieces_cli-1.3.1.tar` & `pieces_cli-1.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-05-10 19:11:21.427120 pieces_cli-1.3.1/LICENSE
--rw-r--r--   0        0        0     9444 2024-05-10 19:11:21.427336 pieces_cli-1.3.1/README.md
--rw-r--r--   0        0        0      908 2024-05-10 19:11:50.911204 pieces_cli-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      261 2024-05-10 19:11:21.427853 pieces_cli-1.3.1/src/pieces/__init__.py
--rw-r--r--   0        0        0      215 2024-05-10 19:11:21.427957 pieces_cli-1.3.1/src/pieces/__main__.py
--rw-r--r--   0        0        0     7029 2024-05-10 19:11:21.428068 pieces_cli-1.3.1/src/pieces/app.py
--rw-r--r--   0        0        0      128 2024-05-10 19:11:21.428210 pieces_cli-1.3.1/src/pieces/assets/__init__.py
--rw-r--r--   0        0        0     7860 2024-05-10 19:11:21.428355 pieces_cli-1.3.1/src/pieces/assets/assets_api.py
--rw-r--r--   0        0        0     5177 2024-05-10 19:11:21.428479 pieces_cli-1.3.1/src/pieces/assets/assets_command.py
--rw-r--r--   0        0        0     2036 2024-05-10 19:11:21.428598 pieces_cli-1.3.1/src/pieces/assets/assets_identifiers_ws.py
--rw-r--r--   0        0        0       34 2024-05-10 19:11:21.428743 pieces_cli-1.3.1/src/pieces/autocommit/__init__.py
--rw-r--r--   0        0        0     9766 2024-05-10 19:11:21.428861 pieces_cli-1.3.1/src/pieces/autocommit/autocommit.py
--rw-r--r--   0        0        0     1452 2024-05-10 19:11:21.428979 pieces_cli-1.3.1/src/pieces/autocommit/git_api.py
--rw-r--r--   0        0        0      354 2024-05-10 19:11:21.429123 pieces_cli-1.3.1/src/pieces/commands/__init__.py
--rw-r--r--   0        0        0      863 2024-05-10 19:11:21.429270 pieces_cli-1.3.1/src/pieces/commands/change_model.py
--rw-r--r--   0        0        0     4121 2024-05-10 19:11:21.429457 pieces_cli-1.3.1/src/pieces/commands/cli_loop.py
--rw-r--r--   0        0        0     5876 2024-05-10 19:11:21.429621 pieces_cli-1.3.1/src/pieces/commands/extensions.json
--rw-r--r--   0        0        0     2890 2024-05-10 19:11:21.429758 pieces_cli-1.3.1/src/pieces/commands/list_command.py
--rw-r--r--   0        0        0     2622 2024-05-10 19:11:21.429903 pieces_cli-1.3.1/src/pieces/commands/search_command.py
--rw-r--r--   0        0        0      213 2024-05-10 19:11:21.430023 pieces_cli-1.3.1/src/pieces/commands/signout_command.py
--rw-r--r--   0        0        0      257 2024-05-10 19:11:21.430134 pieces_cli-1.3.1/src/pieces/commands/version_command.py
--rw-r--r--   0        0        0       96 2024-05-10 19:11:21.430251 pieces_cli-1.3.1/src/pieces/copilot/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-10 19:11:21.430357 pieces_cli-1.3.1/src/pieces/copilot/ask_command.py
--rw-r--r--   0        0        0     5876 2024-05-10 19:11:21.430506 pieces_cli-1.3.1/src/pieces/copilot/conversations.py
--rw-r--r--   0        0        0     4703 2024-05-10 19:11:21.430629 pieces_cli-1.3.1/src/pieces/copilot/pieces_ask_websocket.py
--rw-r--r--   0        0        0     5693 2024-05-10 19:11:21.430770 pieces_cli-1.3.1/src/pieces/gui.py
--rw-r--r--   0        0        0     2906 2024-05-10 19:11:21.430916 pieces_cli-1.3.1/src/pieces/pieces_argparser.py
--rw-r--r--   0        0        0     6247 2024-05-10 19:11:21.431078 pieces_cli-1.3.1/src/pieces/settings.py
--rw-r--r--   0        0        0     1364 2024-05-10 19:11:21.431243 pieces_cli-1.3.1/src/pieces/utils.py
--rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pieces_cli-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-13 18:10:00.328960 pieces_cli-1.3.2/LICENSE
+-rw-r--r--   0        0        0     9610 2024-05-13 18:10:00.329139 pieces_cli-1.3.2/README.md
+-rw-r--r--   0        0        0      908 2024-05-13 18:10:25.193257 pieces_cli-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      261 2024-05-13 18:10:00.329622 pieces_cli-1.3.2/src/pieces/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-13 18:10:00.329738 pieces_cli-1.3.2/src/pieces/__main__.py
+-rw-r--r--   0        0        0     7029 2024-05-13 18:10:00.329863 pieces_cli-1.3.2/src/pieces/app.py
+-rw-r--r--   0        0        0      128 2024-05-13 18:10:00.329995 pieces_cli-1.3.2/src/pieces/assets/__init__.py
+-rw-r--r--   0        0        0     7818 2024-05-13 18:10:00.330137 pieces_cli-1.3.2/src/pieces/assets/assets_api.py
+-rw-r--r--   0        0        0     5177 2024-05-13 18:10:00.330248 pieces_cli-1.3.2/src/pieces/assets/assets_command.py
+-rw-r--r--   0        0        0     1795 2024-05-13 18:10:00.330360 pieces_cli-1.3.2/src/pieces/assets/assets_identifiers_ws.py
+-rw-r--r--   0        0        0       34 2024-05-13 18:10:00.330497 pieces_cli-1.3.2/src/pieces/autocommit/__init__.py
+-rw-r--r--   0        0        0     9766 2024-05-13 18:10:00.330643 pieces_cli-1.3.2/src/pieces/autocommit/autocommit.py
+-rw-r--r--   0        0        0     1452 2024-05-13 18:10:00.330746 pieces_cli-1.3.2/src/pieces/autocommit/git_api.py
+-rw-r--r--   0        0        0      354 2024-05-13 18:10:00.330868 pieces_cli-1.3.2/src/pieces/commands/__init__.py
+-rw-r--r--   0        0        0      863 2024-05-13 18:10:00.331009 pieces_cli-1.3.2/src/pieces/commands/change_model.py
+-rw-r--r--   0        0        0     4121 2024-05-13 18:10:00.331123 pieces_cli-1.3.2/src/pieces/commands/cli_loop.py
+-rw-r--r--   0        0        0     5876 2024-05-13 18:10:00.331235 pieces_cli-1.3.2/src/pieces/commands/extensions.json
+-rw-r--r--   0        0        0     2890 2024-05-13 18:10:00.331342 pieces_cli-1.3.2/src/pieces/commands/list_command.py
+-rw-r--r--   0        0        0     2514 2024-05-13 18:10:00.331533 pieces_cli-1.3.2/src/pieces/commands/search_command.py
+-rw-r--r--   0        0        0      213 2024-05-13 18:10:00.331663 pieces_cli-1.3.2/src/pieces/commands/signout_command.py
+-rw-r--r--   0        0        0      257 2024-05-13 18:10:00.331769 pieces_cli-1.3.2/src/pieces/commands/version_command.py
+-rw-r--r--   0        0        0       96 2024-05-13 18:10:00.331932 pieces_cli-1.3.2/src/pieces/copilot/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-13 18:10:00.332069 pieces_cli-1.3.2/src/pieces/copilot/ask_command.py
+-rw-r--r--   0        0        0     5876 2024-05-13 18:10:00.332186 pieces_cli-1.3.2/src/pieces/copilot/conversations.py
+-rw-r--r--   0        0        0     4703 2024-05-13 18:10:00.332287 pieces_cli-1.3.2/src/pieces/copilot/pieces_ask_websocket.py
+-rw-r--r--   0        0        0     5735 2024-05-13 18:10:00.332495 pieces_cli-1.3.2/src/pieces/gui.py
+-rw-r--r--   0        0        0     2906 2024-05-13 18:10:00.332659 pieces_cli-1.3.2/src/pieces/pieces_argparser.py
+-rw-r--r--   0        0        0     6591 2024-05-13 18:10:00.332807 pieces_cli-1.3.2/src/pieces/settings.py
+-rw-r--r--   0        0        0     1529 2024-05-13 18:10:00.332946 pieces_cli-1.3.2/src/pieces/utils.py
+-rw-r--r--   0        0        0    10481 1970-01-01 00:00:00.000000 pieces_cli-1.3.2/PKG-INFO
```

### Comparing `pieces_cli-1.3.1/LICENSE` & `pieces_cli-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/README.md` & `pieces_cli-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 <p align="center"> This is a comprehensive command-line interface (CLI) tool designed to interact seamlessly with Pieces OS. It provides a range of functionalities such as asset management, application interaction, and integration with various Pieces OS features.
 
 </p>
   
 ##### <p align="center"> [Website](https://pieces.app/) • [Pieces OS Documentation](https://docs.pieces.app/) • [Pieces Python CLI Documentation](https://github.com/pieces-app/cli-agent/blob/prod/Documentation.md)
 </p>
-<br>
+
+# Important
+
+Make sure you have [**Pieces OS**](https://docs.pieces.app/installation-getting-started/what-am-i-installing) installed in order to run the Pieces CLI tool.
 
 ### Table of Contents
 - [Operating System Support](#operating-system-support)
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Terminologies](#some-important-terminologies)
 - [Usage](#usage)
```

### Comparing `pieces_cli-1.3.1/pyproject.toml` & `pieces_cli-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
   name = "pieces-cli"
-  version = "1.3.1"
+  version = "1.3.2"
   description = "A powerful cli tool to interact with the pieces os "
   authors = ["Pieces <development@pieces.app>"]
   readme = "README.md"
   homepage = "https://pieces.app"
   keywords = ["copilot", "pieces","ai","snippets"]
   packages = [{ include = "pieces", from = "src" }]
   license = "MIT"
```

### Comparing `pieces_cli-1.3.1/src/pieces/app.py` & `pieces_cli-1.3.2/src/pieces/app.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/assets/assets_api.py` & `pieces_cli-1.3.2/src/pieces/assets/assets_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 				language = original.classification.specific.value
 				
 				if original.fragment:
 					raw = original.fragment.string.raw
 				elif original.file.string:
 					raw = original.file.string.raw
 				elif original.file.bytes:
-					return show_error("Error in the open command","Image is not supported")
+					raw = original.file.bytes.raw
 				
 		return {"name":name,
 				"created_at":created_readable,
 				'updated_at': updated_readable,
 				"type" :type,
 				"language": language,
 				"raw": raw}
```

### Comparing `pieces_cli-1.3.1/src/pieces/assets/assets_command.py` & `pieces_cli-1.3.2/src/pieces/assets/assets_command.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/assets/assets_identifiers_ws.py` & `pieces_cli-1.3.2/src/pieces/assets/assets_identifiers_ws.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,25 +15,19 @@
         self.ws = None
         self.on_message_callback = on_message_callback
 
         # Create a new event loop
         self.loop = asyncio.new_event_loop()
 
         # Run the event loop in a new thread
-        self.thread = threading.Thread(target=self.start_event_loop, args=(self.loop,))
+        self.thread = threading.Thread(target=self.open_websocket)
         self.thread.start()
+    
 
-        # Open the websocket connection
-        asyncio.run_coroutine_threadsafe(self.open_websocket(), self.loop)
-
-    def start_event_loop(self, loop):
-        asyncio.set_event_loop(loop)
-        loop.run_forever()
-
-    async def open_websocket(self):
+    def open_websocket(self):
         """Opens a websocket connection"""
         if self.ws: # connect only once
             return
         self.ws = websocket.WebSocketApp(Settings.ASSETS_IDENTIFIERS_WS_URL,
                                          on_message=self.on_message,
                                          on_error=self.on_error,
                                          on_close=self.on_close)
```

### Comparing `pieces_cli-1.3.1/src/pieces/autocommit/autocommit.py` & `pieces_cli-1.3.2/src/pieces/autocommit/autocommit.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/autocommit/git_api.py` & `pieces_cli-1.3.2/src/pieces/autocommit/git_api.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/commands/change_model.py` & `pieces_cli-1.3.2/src/pieces/commands/change_model.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/commands/cli_loop.py` & `pieces_cli-1.3.2/src/pieces/commands/cli_loop.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/commands/extensions.json` & `pieces_cli-1.3.2/src/pieces/commands/extensions.json`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/commands/list_command.py` & `pieces_cli-1.3.2/src/pieces/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/commands/search_command.py` & `pieces_cli-1.3.2/src/pieces/commands/search_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 from pieces.settings import Settings
 from pieces.gui import show_error, print_asset_details
 from pieces.assets.assets_api import AssetsCommandsApi
 
 
 def search(query, **kwargs):
-    global asset_ids 
-
     search_type = kwargs.get('search_type', 'assets')
 
     # Join the list of strings into a single search phrase
     search_phrase = ' '.join(query)
 
     # Call the API function with the search phrase and type
     query = search_phrase
@@ -40,18 +38,17 @@
         if isinstance(iterable_list, list) and all(hasattr(asset, 'exact') and hasattr(asset, 'identifier') for asset in iterable_list):
             # Extracting suggested and exact IDs
             suggested_ids = [asset.identifier for asset in iterable_list if not asset.exact]
             exact_ids = [asset.identifier for asset in iterable_list if asset.exact]
 
             # Combine and store best and suggested matches in asset_ids
             combined_ids = exact_ids + suggested_ids
-            asset_ids = {index + 1: asset_id for index, asset_id in enumerate(combined_ids)}
 
             # Prepare the combined list of names for printing
-            combined_details = [(asset_id,  AssetsCommandsApi.get_asset_by_id(asset_id)) for asset_id in combined_ids]
+            combined_details = [(asset_id,  AssetsCommandsApi.get_asset_snapshot(asset_id).name) for asset_id in combined_ids]
 
             # Print the combined asset details
             if combined_details:
                 print_asset_details(combined_details, "Asset Matches:", search_type)
             else:
                 print("No matches found.")
         else:
```

### Comparing `pieces_cli-1.3.1/src/pieces/copilot/ask_command.py` & `pieces_cli-1.3.2/src/pieces/copilot/ask_command.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/copilot/conversations.py` & `pieces_cli-1.3.2/src/pieces/copilot/conversations.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/copilot/pieces_ask_websocket.py` & `pieces_cli-1.3.2/src/pieces/copilot/pieces_ask_websocket.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/gui.py` & `pieces_cli-1.3.2/src/pieces/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     print("############################")
     print()
 
 def server_startup_failed():
     print()
     print("############################")
     print()
-    print("Please start your Pieces OS Server")
+    print("Please make sure Pieces OS is running and up-to-date")
     print()
-    print("Or to install pieces OS: ")
+    print("Or, to install Pieces OS, please visit this link:")
     print("https://docs.pieces.app/installation-getting-started/what-am-i-installing")
     print()
     print("############################")
     print()
 
 def double_space(text):
     print()
```

### Comparing `pieces_cli-1.3.1/src/pieces/pieces_argparser.py` & `pieces_cli-1.3.2/src/pieces/pieces_argparser.py`

 * *Files identical despite different names*

### Comparing `pieces_cli-1.3.1/src/pieces/settings.py` & `pieces_cli-1.3.2/src/pieces/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import urllib.request
 import json
 import pickle
 from typing import Union,Dict,Optional
 import time
 import subprocess
 import platform
 import os
 from pathlib import Path
-
+import sys
+import threading
 from platformdirs import user_data_dir
 
 from pieces import __version__
 from pieces.gui import server_startup_failed
 
 from pieces_os_client.api.well_known_api import WellKnownApi
 from pieces_os_client.api.connector_api import ConnectorApi
@@ -131,50 +131,55 @@
 	def get_models_ids(cls) -> Dict[str, Dict[str, Union[str, int]]]:
 		# api_instance = pos_client.ModelsApi(api_client)
 
 		# api_response = api_instance.models_snapshot()
 		# models = {model.name: {"uuid":model.id,"word_limit":model.max_tokens.input} for model in api_response.iterable if model.cloud or model.downloading} # getting the models that are available in the cloud or is downloaded
 		
 		# call the api until the sdks updated
-		response = urllib.request.urlopen(f'{cls.host}/models').read()
+		response = cls.api_client.call_api('/models', 'GET',{},[],response_types_map={'200': "str",'500': "str"}).raw_data
 		response = json.loads(response)["iterable"]
 		models = {model["name"]:{"uuid":model["id"]} for model in response if model["cloud"] or model.get("downloaded",False)}
 		return models
 	
 	@classmethod
 	def startup(cls):
 		pieces_os_version = cls.open_pieces_os()
 		if pieces_os_version:
-			cls.connect_api()
-			cls.load_models()
-			
+			model_thread = threading.Thread(target=cls.load_models)
+			connector_thread = threading.Thread(target=cls.connect_api)
+			model_thread.start()
+			connector_thread.start()
+			model_thread.join() # Wait for it to finish
+			connector_thread.join() # Wait for it to finish
 		else:
 			server_startup_failed()
+			sys.exit(0) # Exit the program
 
 	@classmethod
 	def open_pieces_os(cls) -> Optional[str]:
 		"""Open pieces os and return its version"""
 		version = cls.get_version()
 		if version:
 			return version
 		else:
 			pl = platform.system()
 			if pl == "Windows":
-				subprocess.Popen(["start", "os_server"], shell=True)
-			elif pl == "Linux":
-				subprocess.Popen(["os_server"])
+				subprocess.run(["start", "pieces://launch"], shell=True)
 			elif pl == "Darwin":
-				subprocess.Popen(["open", "os_server"])
-		
+				subprocess.run(["open","pieces://launch"])
+			elif pl == "Linux":
+				subprocess.run(["xdg-open","pieces://launch"])
+			
 			for _ in range(2):
 				version = cls.get_version()
 				if version:
 					return version
 				time.sleep(2) # wait for the server to open
 			return cls.get_version() # pieces os version
+		
 	@classmethod
 	def get_version(cls) -> Optional[str]:
 		"""Get pieces os version return None if there is a problem"""
 		if cls.pieces_os_version:
 			return cls.pieces_os_version
 		try:
 			cls.pieces_os_version = WellKnownApi(cls.api_client).get_well_known_version()
@@ -189,8 +194,8 @@
 		Returns:
 		bool: True if the health status is 'ok', False otherwise.
 		"""
 		try:
 			health = WellKnownApi(cls.api_client).get_well_known_health()
 			return health == "ok"
 		except Exception as e:
-			return False
+			return False
```

### Comparing `pieces_cli-1.3.1/src/pieces/utils.py` & `pieces_cli-1.3.2/src/pieces/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,16 +22,20 @@
     if not os.path.exists(Settings.open_snippet_dir):
         os.makedirs(Settings.open_snippet_dir)
 
     # Path to save the extracted code
     file_path = os.path.join(Settings.open_snippet_dir, f'{filename}{file_extension}')
 
     # Writing the extracted code to a new file
-    with open(file_path, 'w') as file:
-        file.write(code)
+    if isinstance(code, str): # Code string raw
+        with open(file_path, 'w') as file:
+            file.write(code)
+    else: # Image bytes data
+        with open(file_path, 'wb') as file:
+            file.write(bytes(code))
 
     return file_path
 
 def get_file_extension(language):
     with open(Settings.extensions_dir) as f:
         extension_mapping = json.load(f)
```

### Comparing `pieces_cli-1.3.1/PKG-INFO` & `pieces_cli-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pieces-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: A powerful cli tool to interact with the pieces os 
 Home-page: https://pieces.app
 License: MIT
 Keywords: copilot,pieces,ai,snippets
 Author: Pieces
 Author-email: development@pieces.app
 Requires-Python: >=3.9,<3.13
@@ -29,15 +29,18 @@
 
 <p align="center"> This is a comprehensive command-line interface (CLI) tool designed to interact seamlessly with Pieces OS. It provides a range of functionalities such as asset management, application interaction, and integration with various Pieces OS features.
 
 </p>
   
 ##### <p align="center"> [Website](https://pieces.app/) • [Pieces OS Documentation](https://docs.pieces.app/) • [Pieces Python CLI Documentation](https://github.com/pieces-app/cli-agent/blob/prod/Documentation.md)
 </p>
-<br>
+
+# Important
+
+Make sure you have [**Pieces OS**](https://docs.pieces.app/installation-getting-started/what-am-i-installing) installed in order to run the Pieces CLI tool.
 
 ### Table of Contents
 - [Operating System Support](#operating-system-support)
 - [Installing](#installing)
 - [Getting Started](#getting-started)
 - [Terminologies](#some-important-terminologies)
 - [Usage](#usage)
```

