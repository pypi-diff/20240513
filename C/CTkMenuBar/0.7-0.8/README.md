# Comparing `tmp/ctkmenubar-0.7.tar.gz` & `tmp/ctkmenubar-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkmenubar-0.7.tar", last modified: Tue May  7 08:07:06 2024, max compression
+gzip compressed data, was "ctkmenubar-0.8.tar", last modified: Mon May 13 11:01:02 2024, max compression
```

## Comparing `ctkmenubar-0.7.tar` & `ctkmenubar-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.996886 ctkmenubar-0.7/
-drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.960703 ctkmenubar-0.7/CTkMenuBar/
--rw-rw-rw-   0        0        0      269 2024-05-07 08:00:37.000000 ctkmenubar-0.7/CTkMenuBar/__init__.py
--rw-rw-rw-   0        0        0    14973 2024-05-07 08:02:44.000000 ctkmenubar-0.7/CTkMenuBar/dropdown_menu.py
--rw-rw-rw-   0        0        0     2328 2024-05-07 07:47:33.000000 ctkmenubar-0.7/CTkMenuBar/menu_bar.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 07:48:19.000000 ctkmenubar-0.7/CTkMenuBar/title_menu_win.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:07:05.993354 ctkmenubar-0.7/CTkMenuBar.egg-info/
--rw-rw-rw-   0        0        0     4669 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 08:07:05.000000 ctkmenubar-0.7/CTkMenuBar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 ctkmenubar-0.7/LICENSE
--rw-rw-rw-   0        0        0     4669 2024-05-07 08:07:05.995875 ctkmenubar-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3944 2024-05-07 08:06:18.000000 ctkmenubar-0.7/README.md
--rw-rw-rw-   0        0        0      582 2024-05-07 08:07:06.005395 ctkmenubar-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1129 2024-05-07 08:01:32.000000 ctkmenubar-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:01:02.146029 ctkmenubar-0.8/
+drwxrwxrwx   0        0        0        0 2024-05-13 11:01:02.108949 ctkmenubar-0.8/CTkMenuBar/
+-rw-rw-rw-   0        0        0      269 2024-05-13 10:58:09.000000 ctkmenubar-0.8/CTkMenuBar/__init__.py
+-rw-rw-rw-   0        0        0    15540 2024-05-13 10:56:19.000000 ctkmenubar-0.8/CTkMenuBar/dropdown_menu.py
+-rw-rw-rw-   0        0        0     2328 2024-05-07 07:47:33.000000 ctkmenubar-0.8/CTkMenuBar/menu_bar.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 07:48:19.000000 ctkmenubar-0.8/CTkMenuBar/title_menu_win.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:01:02.143515 ctkmenubar-0.8/CTkMenuBar.egg-info/
+-rw-rw-rw-   0        0        0     4669 2024-05-13 11:01:02.000000 ctkmenubar-0.8/CTkMenuBar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-13 11:01:02.000000 ctkmenubar-0.8/CTkMenuBar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2024-05-13 11:01:02.000000 ctkmenubar-0.8/CTkMenuBar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 11:01:02.000000 ctkmenubar-0.8/CTkMenuBar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 11:01:02.000000 ctkmenubar-0.8/CTkMenuBar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 ctkmenubar-0.8/LICENSE
+-rw-rw-rw-   0        0        0     4669 2024-05-13 11:01:02.144520 ctkmenubar-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3944 2024-05-07 08:06:18.000000 ctkmenubar-0.8/README.md
+-rw-rw-rw-   0        0        0      582 2024-05-13 11:01:02.155054 ctkmenubar-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2024-05-13 10:58:59.000000 ctkmenubar-0.8/setup.py
```

### Comparing `ctkmenubar-0.7/CTkMenuBar/dropdown_menu.py` & `ctkmenubar-0.8/CTkMenuBar/dropdown_menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         self.font = font
         self.height = height
         self.width = width
         self.padx = padx
         self.pady = pady
         self.cursor = cursor
         self.hovered = False
+        self.is_submenu = False
 
         self.separator_color = separator_color
         self._options_list: list[_CDMOptionButton | _CDMSubmenuButton] = []
         
     def selectOption(self, command) -> None:
         self._hideAllMenus()
         if command:
@@ -129,16 +130,20 @@
 
         optionButton.pack(
             side="top",
             fill="both", 
             expand=True,
             padx=3+(self.corner_radius/5),
             pady=3+(self.corner_radius/5))
+        
+        if self.is_submenu:
+            optionButton.bind("<Enter>", lambda e, submenu=self: submenu.change_hover(self), add="+")
+   
         return optionButton
-    
+
     def add_submenu(self, submenu_name: str, **kwargs) -> "CustomDropdownMenu":
         submenuButtonSeed = _CDMSubmenuButton(self, text=submenu_name, anchor="w",
                                               text_color=self.text_color,
                                               width=self.width, height=self.height, **kwargs)
         submenuButtonSeed.setParentMenu(self)
         self._options_list.append(submenuButtonSeed)
         self._configureButton(submenuButtonSeed)
@@ -156,47 +161,59 @@
             border_color=self.border_color,
             separator_color=self.separator_color,
             text_color=self.text_color,
             font=self.font)
         
         submenuButtonSeed.setSubmenu(submenu=submenu)
         submenuButtonSeed.configure(command=submenu.toggleShow)
-        submenu.bind("<Enter>", lambda e: submenu._show_submenu(self, hovered=True))
-  
-        submenu.bind("<Enter>", lambda e, submenu=submenu: submenu._show_submenu(self, hovered=True), add="+")
-        submenuButtonSeed.bind("<Enter>", lambda e: self.after(500, lambda: submenu._show_submenu(self)), add="+")
-        submenuButtonSeed.bind("<Leave>", lambda e: self.after(500, lambda: submenu._left(self)), add="+")
+        submenu.is_submenu = True
+        
+        submenu.bind("<Enter>", lambda e, sub=self: self.change_hover(self), add="+")
+        submenuButtonSeed.bind("<Enter>", lambda e, sub=submenu, button=submenuButtonSeed: self.after(500, lambda: sub._show_submenu(self, button)), add="+")
+        submenuButtonSeed.bind("<Leave>", lambda e, sub=submenu: self.after(500, lambda: sub._left(self)), add="+")
+        
         submenuButtonSeed.configure(cursor=self.cursor)
         
         submenuButtonSeed.pack(
             side="top",
             fill="both", 
             expand=True,
             padx=3+(self.corner_radius/5),
             pady=3+(self.corner_radius/5))
         return submenu
         
     def _left(self, parent):
+  
         if parent.hovered:
+            parent.hovered = False
             return
         
         subMenus = parent._getSubMenus()
         
         for i in subMenus:
             i._hide()
-
-    def _show_submenu(self, parent, hovered=False) ->None:
-    
-        parent.hovered = hovered
+            
+    def change_hover(self, parent):
+        parent.hovered = True
+   
+    def _show_submenu(self, parent, button) ->None:
+        if self.winfo_viewable():
+            return
         
         subMenus = parent._getSubMenus()
         
         for i in subMenus:
             i._hide()
-
+            
+        x,y = self.winfo_pointerxy()
+        widget = self.winfo_containing(x,y)
+    
+        if (str(widget)!=str(button._canvas)) and (str(widget)!=str(button._text_label)) and (str(widget)!=str(button._image_label)):
+            return
+        
         self._show()
             
         
     def add_separator(self) -> None:
         separator = customtkinter.CTkFrame(
             master=self, 
             height=2,
```

### Comparing `ctkmenubar-0.7/CTkMenuBar/menu_bar.py` & `ctkmenubar-0.8/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `ctkmenubar-0.7/CTkMenuBar/title_menu_win.py` & `ctkmenubar-0.8/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `ctkmenubar-0.7/CTkMenuBar.egg-info/PKG-INFO` & `ctkmenubar-0.8/CTkMenuBar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ctkmenubar-0.7/LICENSE` & `ctkmenubar-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctkmenubar-0.7/PKG-INFO` & `ctkmenubar-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMenuBar
-Version: 0.7
+Version: 0.8
 Summary: Customtkinter Menu Widget
 Home-page: https://github.com/Akascape/CTkMenuBar
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-menu,ctkmenubar,titlemenu,menubar,tkinter,menu-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ctkmenubar-0.7/README.md` & `ctkmenubar-0.8/README.md`

 * *Files identical despite different names*

### Comparing `ctkmenubar-0.7/setup.cfg` & `ctkmenubar-0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 6e75 4261 720d 0a76   = CTkMenuBar..v
-00000020: 6572 7369 6f6e 203d 2030 2e37 0d0a 6465  ersion = 0.7..de
+00000020: 6572 7369 6f6e 203d 2030 2e38 0d0a 6465  ersion = 0.8..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 4d65 6e75 2057  omtkinter Menu W
 00000050: 6964 6765 740d 0a6c 6f6e 675f 6465 7363  idget..long_desc
 00000060: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000070: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
```

### Comparing `ctkmenubar-0.7/setup.py` & `ctkmenubar-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMenuBar',
-    version = '0.7',
+    version = '0.8',
     description = "Customtkinter Menu Widget",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMenuBar",
```

