# Comparing `tmp/nicotool-1.4.8.1.tar.gz` & `tmp/nicotool-1.4.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicotool-1.4.8.1.tar", last modified: Thu Apr 18 08:07:46 2024, max compression
+gzip compressed data, was "nicotool-1.4.8.4.tar", last modified: Mon May 13 11:30:21 2024, max compression
```

## Comparing `nicotool-1.4.8.1.tar` & `nicotool-1.4.8.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.333716 nicotool-1.4.8.1/
--rw-rw-rw-   0        0        0      307 2024-04-18 08:07:46.332711 nicotool-1.4.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 nicotool-1.4.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.314765 nicotool-1.4.8.1/nicotool/
--rw-rw-rw-   0        0        0     3885 2024-04-17 08:25:07.000000 nicotool-1.4.8.1/nicotool/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 nicotool-1.4.8.1/nicotool/additional_functions.py
--rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 nicotool-1.4.8.1/nicotool/ascii.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 nicotool-1.4.8.1/nicotool/data_manipulation.py
--rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 nicotool-1.4.8.1/nicotool/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 nicotool-1.4.8.1/nicotool/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 nicotool-1.4.8.1/nicotool/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 nicotool-1.4.8.1/nicotool/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 nicotool-1.4.8.1/nicotool/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 nicotool-1.4.8.1/nicotool/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 nicotool-1.4.8.1/nicotool/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 nicotool-1.4.8.1/nicotool/youtube.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.330716 nicotool-1.4.8.1/nicotool.egg-info/
--rw-rw-rw-   0        0        0      307 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 08:07:46.334706 nicotool-1.4.8.1/setup.cfg
--rw-rw-rw-   0        0        0      386 2024-04-18 08:07:39.000000 nicotool-1.4.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:30:21.420361 nicotool-1.4.8.4/
+-rw-rw-rw-   0        0        0      307 2024-05-13 11:30:21.418365 nicotool-1.4.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 nicotool-1.4.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 11:30:21.367668 nicotool-1.4.8.4/nicotool/
+-rw-rw-rw-   0        0        0     3963 2024-05-12 11:41:14.000000 nicotool-1.4.8.4/nicotool/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 nicotool-1.4.8.4/nicotool/additional_functions.py
+-rw-rw-rw-   0        0        0    15234 2024-04-23 14:40:29.000000 nicotool-1.4.8.4/nicotool/ascii.py
+-rw-rw-rw-   0        0        0    46861 2024-05-12 11:40:47.000000 nicotool-1.4.8.4/nicotool/colors.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 nicotool-1.4.8.4/nicotool/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 nicotool-1.4.8.4/nicotool/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 nicotool-1.4.8.4/nicotool/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 nicotool-1.4.8.4/nicotool/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 nicotool-1.4.8.4/nicotool/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 nicotool-1.4.8.4/nicotool/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 nicotool-1.4.8.4/nicotool/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 nicotool-1.4.8.4/nicotool/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 nicotool-1.4.8.4/nicotool/youtube.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:30:21.411871 nicotool-1.4.8.4/nicotool.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-05-13 11:30:20.000000 nicotool-1.4.8.4/nicotool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-05-13 11:30:21.000000 nicotool-1.4.8.4/nicotool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:30:20.000000 nicotool-1.4.8.4/nicotool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-13 11:30:20.000000 nicotool-1.4.8.4/nicotool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 11:30:20.000000 nicotool-1.4.8.4/nicotool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:30:21.421368 nicotool-1.4.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-05-13 11:29:50.000000 nicotool-1.4.8.4/setup.py
```

### Comparing `nicotool-1.4.8.1/nicotool/__init__.py` & `nicotool-1.4.8.4/nicotool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from .youtube import downloadYoutube
 
 from .database import(add_data_to_table,check_if_database_exists,check_if_key_exists,
 convert_to_db_format,create_sqlite_database,create_table,delete_database,unconvert,
 table_exists,edit_data_in_table,edit_table,get_primary_columns,load_all_data,load_data_from_key,
 purge_database,purge_table,remove_data_from_table,purge_database_data,remove_table,backup_database,check_if_table_exists)
 
-
+from .colors import (get_all_colors,get_color_hex,verify_hex_color,hex_to_int)
 # if is_connected():
 #     def get_latest_version(package_name):
 #         """Get the latest version of a package from PyPI."""
 #         try:
 #             client = xmlrpc.client.ServerProxy('https://pypi.org/pypi')
 #             releases = client.package_releases(package_name)
 #             if releases:
```

### Comparing `nicotool-1.4.8.1/nicotool/additional_functions.py` & `nicotool-1.4.8.4/nicotool/additional_functions.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/ascii.py` & `nicotool-1.4.8.4/nicotool/ascii.py`

 * *Files 21% similar despite different names*

```diff
@@ -513,15 +513,159 @@
 " ___   ",
 "|__ \  ",
 "   ) | ",
 "  / /  ",
 " |_|   ",
 " (_)   ",
 "       "
+],
+"-":[
+"         ",   
+"         ",
+" ______  ",
+"|______| ",
+"         ",     
+"         ",
+"         "
+         
+         
+
+],
+"_":[ 
+"         ",
+"         ",
+"         ",
+"         ",
+" ______  ",
+"|______| ",
+"         "
+],
+"1":[   
+" __  ",
+"/_ | ",
+" | | ",
+" | | ",
+" | | ",
+" |_| ",
+"     "
+],
+"2":[
+" ___   ",
+"|__ \  ",
+"   ) | ",
+"  / /  ",
+" / /_  ",
+"|____| ",
+"       "
+],
+"3":[      
+" ____   ",
+"|___ \  ",
+"  __) | ",
+" |__ <  ",
+" ___) | ",
+"|____/  ",
+"        "
+],
+"4":[
+    
+" _  _    ",
+"| || |   ",
+"| || |_  ",
+"|__   _| ",
+"   | |   ",
+"   |_|   ",
+"         "
+         
+
+],
+"5":[
+" _____  ",
+"| ____| ",
+"| |__   ",
+"|___ \  ",
+" ___) | ",
+"|____/  ",
+"        "
+],
+"6":[
+    
+"   __   ",
+"  / /   ",
+" / /_   ",
+"| '_ \  ",
+"| (_) | ",
+" \___/  ",
+"        "
+],
+"7":[
+" ______  ",
+"|____  | ",
+"    / /  ",
+"   / /   ",
+"  / /    ",
+" /_/     ",
+"         "
+],
+"8":[   
+"  ___   ",
+" / _ \  ",
+"| (_) | ",
+" > _ <  ",
+"| (_) | ",
+" \___/  ",
+"        "
+],
+"9":[
+"  ___   ",
+" / _ \  ",
+"| (_) | ",
+" \__, | ",
+"   / /  ",
+"  /_/   ",
+"        "
+],
+"0":[
+    
+"  ___   ",
+" / _ \  ",
+"| | | | ",
+"| | | | ",
+"| |_| | ",
+" \___/  ",
+"        "
+],
+"+":[
+    
+"        ",
+"   _    ",
+" _| |_  ",
+"|_   _| ",
+"  |_|   ",
+"        ",
+"        "
+        
+        
+        
+
+],
+"=":[
+    
+"         ",   
+" ______  ",
+"|______| ",
+" ______  ",
+"|______| ",
+"         ",
+"         "
+         
+         
+
 ]
+
 }
 
 def print_ascii(text):
 
     combined_art = ""
     for line_num in range(len(ascii_art_['A'])):
         for char in text:
@@ -558,20 +702,20 @@
 
     print(combined_art)
 
 def print_ascii_colored(text, hex_color):
     """
     Print the text in the specified color.
     
-    :param text: The text to be printed.
-    :param color: The color in which the text should be printed.
-                  Options: 'green', 'red', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'black', 'gray', 
-                           'lightgray', 'darkgray', 'lightblue', 'lightgreen', 'lightcyan', 'lightred', 'pink'
-                  Optionally, the color can be specified as a hexadecimal string.
-                  Optional: False
+    - Args:
+        - text (str): The text that should be printed
+        - hex_color: The color in hex
+    
+    - Returns:
+        - None
     """
     color_codes = {
         "green": "0;255;0",
         "red": "255;0;0",
         "yellow": "255;255;0",
         "blue": "0;0;255",
         "magenta": "255;0;255",
```

### Comparing `nicotool-1.4.8.1/nicotool/data_manipulation.py` & `nicotool-1.4.8.4/nicotool/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/database.py` & `nicotool-1.4.8.4/nicotool/database.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/files.py` & `nicotool-1.4.8.4/nicotool/files.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/id.py` & `nicotool-1.4.8.4/nicotool/id.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/jsonify.py` & `nicotool-1.4.8.4/nicotool/jsonify.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/keyboard.py` & `nicotool-1.4.8.4/nicotool/keyboard.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/print_additions.py` & `nicotool-1.4.8.4/nicotool/print_additions.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/profanities.py` & `nicotool-1.4.8.4/nicotool/profanities.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.4.8.1/nicotool/youtube.py` & `nicotool-1.4.8.4/nicotool/youtube.py`

 * *Files identical despite different names*

