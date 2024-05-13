# Comparing `tmp/PrusaLinkPy-2.1.0.tar.gz` & `tmp/prusalinkpy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrusaLinkPy-2.1.0.tar", last modified: Fri Dec 15 12:49:10 2023, max compression
+gzip compressed data, was "prusalinkpy-2.2.0.tar", last modified: Mon May 13 14:23:26 2024, max compression
```

## Comparing `PrusaLinkPy-2.1.0.tar` & `prusalinkpy-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 12:49:10.747504 PrusaLinkPy-2.1.0/
--rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 PrusaLinkPy-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    12822 2023-12-15 12:49:10.747504 PrusaLinkPy-2.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-15 12:49:10.699821 PrusaLinkPy-2.1.0/PrusaLinkPy/
--rw-rw-rw-   0        0        0     8373 2023-12-15 12:36:04.000000 PrusaLinkPy-2.1.0/PrusaLinkPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-15 12:49:10.731862 PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/
--rw-rw-rw-   0        0        0    12822 2023-12-15 12:49:10.000000 PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-12-15 12:49:10.000000 PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 12:49:10.000000 PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-12-15 12:49:10.000000 PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10896 2023-12-15 12:48:06.000000 PrusaLinkPy-2.1.0/README.md
--rw-rw-rw-   0        0        0      691 2023-12-15 12:48:27.000000 PrusaLinkPy-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-15 12:49:10.747504 PrusaLinkPy-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      206 2023-12-15 12:47:04.000000 PrusaLinkPy-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-15 12:49:10.731862 PrusaLinkPy-2.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-2.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 PrusaLinkPy-2.1.0/tests/test_PrusaLinkPy.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/
+-rw-rw-rw-   0        0        0     1075 2023-05-15 15:07:17.000000 prusalinkpy-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    15045 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.789161 prusalinkpy-2.2.0/PrusaLinkPy/
+-rw-rw-rw-   0        0        0    10059 2024-05-13 14:15:23.000000 prusalinkpy-2.2.0/PrusaLinkPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/
+-rw-rw-rw-   0        0        0    15045 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 14:23:26.000000 prusalinkpy-2.2.0/PrusaLinkPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13119 2024-05-13 14:22:01.000000 prusalinkpy-2.2.0/README.md
+-rw-rw-rw-   0        0        0      691 2024-05-13 14:20:46.000000 prusalinkpy-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:23:26.819156 prusalinkpy-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      206 2024-05-13 14:20:35.000000 prusalinkpy-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:23:26.809212 prusalinkpy-2.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 11:24:02.000000 prusalinkpy-2.2.0/tests/test_PrusaLinkPy.py
```

### Comparing `PrusaLinkPy-2.1.0/LICENSE` & `prusalinkpy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PrusaLinkPy-2.1.0/PKG-INFO` & `prusalinkpy-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 2.1.0
+Version: 2.2.0
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -70,14 +70,33 @@
     
 
 The library changed its name in May 2024. Before it was called prusaLink.
 Prusa staff asked me to leave them the name.
 
 # Change Log 
 
+## 2.2 :
+
+  Version made by [enrgarci](https://github.com/enrgarci)
+ - Update README.md
+ - Modified delete_job() to fix request from get to delete
+ - added :
+
+ * pause_print
+ * resume_print
+ * stop_print
+
+## 2.1.1 :
+
+ - Update README.md
+ - added :
+
+ * get_transfer
+ * get_settings
+ 
 ## 2.1.0 :
 
  - Update README.md
  - added :
 
  * delete
  * get_status
@@ -126,22 +145,26 @@
 
 [get_storage()](#prusalinkpyget_storage)
 
 [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
 
 [delete(remotePath)](#prusalinkpydeleteremotepath)
 
-[post_gcode(filePathLocal, remoteDir)](#prusalinkpyput_post_gcode)
+[post_gcode(remotePath)](#prusalinkpyput_post_gcode)
 
 [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath)
 
-[post_gcode(filePathLocal, remoteDir)](#prusalinkpyput_post_gcode)
-
 [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
 
+[pause_print()](#prusalinkpypause_print)
+
+[resume_print()](#prusalinkpyresume_print)
+
+[stop_print()](#prusalinkpystop_print)
+
 ## High Level Functions 
 
 [get_recursive_files(remoteDir)](#prusalinkpyget_recursive_files-remotedir--)
 
 
 # User Guide
 
@@ -175,14 +198,19 @@
 Get printer :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_printer()
     obj.json()
     
+Waiting for Changing Filament :
+
+    'link_state': 'ATTENTION' 
+    'error': True
+    
 Return something like :
 
     {
         'telemetry': 
         {
             'temp-bed': 16.3,
             'temp-nozzle': 16.7,
@@ -256,14 +284,23 @@
 Get job :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_status()
     obj.json()
     
+Value of printer->state :
+
+    IDLE (Main Screen)
+    PRINTING
+    FINISHED (Print finish, screen not on main screen)
+    PAUSED (Pause by user, Print fan error)
+    STOPPED (Print finish, stopped by user)
+    ATTENTION (Filament Change)
+    
 Return something like :
 
     {
         "job":
         {
             "id":43,
             "progress":0.00,
@@ -298,16 +335,65 @@
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_storage()
     obj.json()
     
 Return something like :
 
+    {
+        'storage_list': 
+        [
+            {
+                'path': '/usb/', 
+                'name': 'usb',
+                'type': 'USB', 
+                'read_only': False, 
+                'available': True
+            }
+        ]
+    }
+    
+## PrusaLinkPy.get_transfer()
+
+Not Tested
+
+Get job :
+
+    import PrusaLinkPy
+    prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
+    obj = prusaMini.get_transfer()
+    obj.text
+    
+Return something like :
+
     TODO
+    
+## PrusaLinkPy.get_settings()
+
+Completely useless
+
+See here :
+
+https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/4bea923810302d654b932291ba324eaedff072fc/lib/WUI/link_content/prusa_link_api.cpp#L181C16-L181C16
+
+Comment from Prusa Developper :
+
+     // Some stubs for now, to make more clients (including the web page) happier.
+
+Get job :
+
+    import PrusaLinkPy
+    prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
+    obj = prusaMini.get_transfer()
+    obj.text
+    
+Return something like :
 
+    {"printer": {}}
+    
 ## PrusaLinkPy.get_files( remoteDir = '/')
 
 Get Files on USB Drive :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_files()
@@ -340,15 +426,15 @@
     
 Workalso with subfolder
 
     obj = prusaMini.get_files(remoteDir = '/SUBFOLDER')
 
 ## PrusaLinkPy.get_recursive_files( remoteDir = '/')
 
-Get all files in a folder and subfolder.
+Get all files (only gcode and bgcode) in a folder and subfolder.
 
 Warning : return nested dict.
 
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     dictt = prusaMini.get_recursive_files()
@@ -374,32 +460,38 @@
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.delete('/DEBOUC~1.GCO')
 
 
 ## PrusaLinkPy.post_gcode(remotePath) 
 
-Print a file 
+Print a file already poresent on USB key 
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.post_gcode('/DEBOUC~1.GCO')
 
 ## PrusaLinkPy.put_gcode(remotePath, printAfterUpload = False, overwrite = False) 
 
 Send a file on USB Drive.
 
 Can create a folder !
 
 if ret.status_code = 409 -> Conflict : File already exists
+if ret.status_code = 415 -> {"title": "415: Unsupported Media Type","message":"Not a GCODE"}
 
-printAfterUpload : Set at True to print after upload. Warning : Printer LCD must be on main screen !
+printAfterUpload : Set at True to print after upload. 
 
 overwrite : Allow file Overwrite
 
+FW 5.1.0 :
+
+ * Warning: printing starts even if the bed is not empty
+ * Can only send bgcode and gcode
+    
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     status = prusaMini.put('C:/MTN/DEBOUCHAGE.gcode' , 'MTN/DEBOUCHAGE.gcode')
     # Overwrite
     status = prusaMini.put('C:/MTN/DEBOUCHAGE.gcode' , 'MTN/DEBOUCHAGE.gcode', False, True)
     # Overwrite and Print
@@ -411,23 +503,40 @@
 
 Return True or False
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     status = prusaMini.exists_gcode('/DEBOUC~1.GCO')
 
+## PrusaLinkPy.pause_print() 
+
+Pause actual print.
+
+Added in 2.2.0 .
+
+## PrusaLinkPy.resume_print() 
+
+Resume paused print.
+
+Added in 2.2.0 .
+
+## PrusaLinkPy.stop_print() 
+
+Stop actual print.
+
+Added in 2.2.0 .
+
 # API
 
 API not implemented in my lib  : 
 
-retrieve thumbnail 
+ * retrieve thumbnail :
 
     r = requests.get('http://192.168.0.123:8017/thumb/l/usb/TAVERN~1.GCO', headers=headers)
 
-
 /api/settings
 
 
 POST /api/job
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L276)**
 
 GET/POST /api/download
```

### Comparing `PrusaLinkPy-2.1.0/PrusaLinkPy/__init__.py` & `prusalinkpy-2.2.0/PrusaLinkPy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,35 +46,53 @@
 
     def delete_job(self, job) :
         """
         
             Delete the job.
             
         """
-        r = requests.get('http://' + self.host + ':' + self.port + '/api/v1/job/' + str(job), headers=self.headers)
+        r = requests.delete('http://' + self.host + ':' + self.port + '/api/v1/job/' + str(job), headers=self.headers)
         return r
         
     def get_status(self) :
         """
         
             Get the status.
             
         """
         r = requests.get('http://' + self.host + ':' + self.port + '/api/v1/status', headers=self.headers)
         return r
 
     def get_storage(self) :
         """
         
-            Get the get_storage.
+            Get the storage.
             
         """
         r = requests.get('http://' + self.host + ':' + self.port + '/api/v1/storage', headers=self.headers)
         return r
 
+    def get_transfer(self) :
+        """
+        
+            Get the transfer
+            
+        """
+        r = requests.get('http://' + self.host + ':' + self.port + '/api/v1/transfer', headers=self.headers)
+        return r
+        
+    def get_settings(self) :
+        """
+        
+            Get the settings
+            
+        """
+        r = requests.get('http://' + self.host + ':' + self.port + '/api/settings', headers=self.headers)
+        return r
+        
     def get_files(self, remoteDir = '/') :
         """
         List files and folder on USB Drive.
         
         Test code :
         import PrusaLinkPy
         prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.1.211", "44Da9wHhThmzFFJ")
@@ -229,14 +247,62 @@
         # Check if response is json 
         if "{" in ret.text :
             for filejson in ret.json()['files'][0]['children'] :
                 print("Delete file : " + filejson["path"])
                 self.delete( filejson["path"])
         else :
             return ret
+
+	def pause_print(self) :
+		"""
+		
+			Pause job.
+			None if no active job.
+			
+		"""
+		r = None
+		job_info = self.get_job()
+		# Check if response is json
+		if "{" in job_info.text :
+			if "id" in job_info.json():
+				id = str(job_info.json()['id'])
+				r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/pause', headers=self.headers)
+		return r
+
+	def resume_print(self) :
+		"""
+		
+			Resume current job.
+			None if no active job.
+			
+		"""
+		r = None
+		job_info = self.get_job()
+		# Check if response is json 
+		if "{" in job_info.text :
+			if "id" in job_info.json():
+				id = str(job_info.json()['id'])
+				r = requests.put('http://' + self.host + ':' + self.port + '/api/v1/job/'+ id + '/resume', headers=self.headers)
+		return r
+	
+	def stop_print(self) :
+		"""
+		
+			Stop current job.
+			None if no active job
+			
+		"""
+		r = None
+		job_info = self.get_job()
+		# Check if response is json 
+		if "{" in job_info.text :
+			if "id" in job_info.json():
+				id = str(job_info.json()['id'])
+				r = requests.delete('http://' + self.host + ':' + self.port + '/api/v1/job/'+ str(id), headers=self.headers)
+		return r
         
         
 # Utilisation :
 # import PrusaLinkPy
 # prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM", port=8017)
 # prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.1.211", "44Da9wHhThmzFFJ")
-# obj = prusaMini.get_version()
+# obj = prusaMini.get_version()
```

### Comparing `PrusaLinkPy-2.1.0/PrusaLinkPy.egg-info/PKG-INFO` & `prusalinkpy-2.2.0/PrusaLinkPy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrusaLinkPy
-Version: 2.1.0
+Version: 2.2.0
 Summary: A library to interface with the PrusaLink API
 Author: Guillaume RICO
 Author-email: Guillaume RICO <guillaume.rico@alpesmesures.fr>
 License: Copyright (c) 2023 Guillaume RICO
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -70,14 +70,33 @@
     
 
 The library changed its name in May 2024. Before it was called prusaLink.
 Prusa staff asked me to leave them the name.
 
 # Change Log 
 
+## 2.2 :
+
+  Version made by [enrgarci](https://github.com/enrgarci)
+ - Update README.md
+ - Modified delete_job() to fix request from get to delete
+ - added :
+
+ * pause_print
+ * resume_print
+ * stop_print
+
+## 2.1.1 :
+
+ - Update README.md
+ - added :
+
+ * get_transfer
+ * get_settings
+ 
 ## 2.1.0 :
 
  - Update README.md
  - added :
 
  * delete
  * get_status
@@ -126,22 +145,26 @@
 
 [get_storage()](#prusalinkpyget_storage)
 
 [get_files(remoteDir)](#prusalinkpyget_files-remotedir--)
 
 [delete(remotePath)](#prusalinkpydeleteremotepath)
 
-[post_gcode(filePathLocal, remoteDir)](#prusalinkpyput_post_gcode)
+[post_gcode(remotePath)](#prusalinkpyput_post_gcode)
 
 [put_gcode(filePathLocal, remoteDir, printAfterUpload = False, overwrite = False)](#prusalinkpyput_gcoderemotepath)
 
-[post_gcode(filePathLocal, remoteDir)](#prusalinkpyput_post_gcode)
-
 [exists_gcode(remotePath)](#prusalinkpyexists_gcoderemotepath)
 
+[pause_print()](#prusalinkpypause_print)
+
+[resume_print()](#prusalinkpyresume_print)
+
+[stop_print()](#prusalinkpystop_print)
+
 ## High Level Functions 
 
 [get_recursive_files(remoteDir)](#prusalinkpyget_recursive_files-remotedir--)
 
 
 # User Guide
 
@@ -175,14 +198,19 @@
 Get printer :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_printer()
     obj.json()
     
+Waiting for Changing Filament :
+
+    'link_state': 'ATTENTION' 
+    'error': True
+    
 Return something like :
 
     {
         'telemetry': 
         {
             'temp-bed': 16.3,
             'temp-nozzle': 16.7,
@@ -256,14 +284,23 @@
 Get job :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_status()
     obj.json()
     
+Value of printer->state :
+
+    IDLE (Main Screen)
+    PRINTING
+    FINISHED (Print finish, screen not on main screen)
+    PAUSED (Pause by user, Print fan error)
+    STOPPED (Print finish, stopped by user)
+    ATTENTION (Filament Change)
+    
 Return something like :
 
     {
         "job":
         {
             "id":43,
             "progress":0.00,
@@ -298,16 +335,65 @@
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_storage()
     obj.json()
     
 Return something like :
 
+    {
+        'storage_list': 
+        [
+            {
+                'path': '/usb/', 
+                'name': 'usb',
+                'type': 'USB', 
+                'read_only': False, 
+                'available': True
+            }
+        ]
+    }
+    
+## PrusaLinkPy.get_transfer()
+
+Not Tested
+
+Get job :
+
+    import PrusaLinkPy
+    prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
+    obj = prusaMini.get_transfer()
+    obj.text
+    
+Return something like :
+
     TODO
+    
+## PrusaLinkPy.get_settings()
+
+Completely useless
+
+See here :
+
+https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/4bea923810302d654b932291ba324eaedff072fc/lib/WUI/link_content/prusa_link_api.cpp#L181C16-L181C16
+
+Comment from Prusa Developper :
+
+     // Some stubs for now, to make more clients (including the web page) happier.
+
+Get job :
+
+    import PrusaLinkPy
+    prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
+    obj = prusaMini.get_transfer()
+    obj.text
+    
+Return something like :
 
+    {"printer": {}}
+    
 ## PrusaLinkPy.get_files( remoteDir = '/')
 
 Get Files on USB Drive :
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.get_files()
@@ -340,15 +426,15 @@
     
 Workalso with subfolder
 
     obj = prusaMini.get_files(remoteDir = '/SUBFOLDER')
 
 ## PrusaLinkPy.get_recursive_files( remoteDir = '/')
 
-Get all files in a folder and subfolder.
+Get all files (only gcode and bgcode) in a folder and subfolder.
 
 Warning : return nested dict.
 
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     dictt = prusaMini.get_recursive_files()
@@ -374,32 +460,38 @@
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.delete('/DEBOUC~1.GCO')
 
 
 ## PrusaLinkPy.post_gcode(remotePath) 
 
-Print a file 
+Print a file already poresent on USB key 
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     obj = prusaMini.post_gcode('/DEBOUC~1.GCO')
 
 ## PrusaLinkPy.put_gcode(remotePath, printAfterUpload = False, overwrite = False) 
 
 Send a file on USB Drive.
 
 Can create a folder !
 
 if ret.status_code = 409 -> Conflict : File already exists
+if ret.status_code = 415 -> {"title": "415: Unsupported Media Type","message":"Not a GCODE"}
 
-printAfterUpload : Set at True to print after upload. Warning : Printer LCD must be on main screen !
+printAfterUpload : Set at True to print after upload. 
 
 overwrite : Allow file Overwrite
 
+FW 5.1.0 :
+
+ * Warning: printing starts even if the bed is not empty
+ * Can only send bgcode and gcode
+    
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     status = prusaMini.put('C:/MTN/DEBOUCHAGE.gcode' , 'MTN/DEBOUCHAGE.gcode')
     # Overwrite
     status = prusaMini.put('C:/MTN/DEBOUCHAGE.gcode' , 'MTN/DEBOUCHAGE.gcode', False, True)
     # Overwrite and Print
@@ -411,23 +503,40 @@
 
 Return True or False
 
     import PrusaLinkPy
     prusaMini = PrusaLinkPy.PrusaLinkPy("192.168.0.123", "8ojHKHGNuAHA2bM")
     status = prusaMini.exists_gcode('/DEBOUC~1.GCO')
 
+## PrusaLinkPy.pause_print() 
+
+Pause actual print.
+
+Added in 2.2.0 .
+
+## PrusaLinkPy.resume_print() 
+
+Resume paused print.
+
+Added in 2.2.0 .
+
+## PrusaLinkPy.stop_print() 
+
+Stop actual print.
+
+Added in 2.2.0 .
+
 # API
 
 API not implemented in my lib  : 
 
-retrieve thumbnail 
+ * retrieve thumbnail :
 
     r = requests.get('http://192.168.0.123:8017/thumb/l/usb/TAVERN~1.GCO', headers=headers)
 
-
 /api/settings
 
 
 POST /api/job
 **[Link to Buddy code](https://github.com/prusa3d/Prusa-Firmware-Buddy/blob/master/lib/WUI/link_content/prusa_link_api.cpp#L276)**
 
 GET/POST /api/download
```

### Comparing `PrusaLinkPy-2.1.0/README.md` & `prusalinkpy-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -64,618 +64,757 @@
 000003f0: 616d 6520 696e 204d 6179 2032 3032 342e  ame in May 2024.
 00000400: 2042 6566 6f72 6520 6974 2077 6173 2063   Before it was c
 00000410: 616c 6c65 6420 7072 7573 614c 696e 6b2e  alled prusaLink.
 00000420: 0d0a 5072 7573 6120 7374 6166 6620 6173  ..Prusa staff as
 00000430: 6b65 6420 6d65 2074 6f20 6c65 6176 6520  ked me to leave 
 00000440: 7468 656d 2074 6865 206e 616d 652e 0d0a  them the name...
 00000450: 0d0a 2320 4368 616e 6765 204c 6f67 200d  ..# Change Log .
-00000460: 0a0d 0a23 2320 322e 312e 3020 3a0d 0a0d  ...## 2.1.0 :...
-00000470: 0a20 2d20 5570 6461 7465 2052 4541 444d  . - Update READM
-00000480: 452e 6d64 0d0a 202d 2061 6464 6564 203a  E.md.. - added :
-00000490: 0d0a 0d0a 202a 2064 656c 6574 650d 0a20  .... * delete.. 
-000004a0: 2a20 6765 745f 7374 6174 7573 0d0a 202a  * get_status.. *
-000004b0: 2067 6574 5f73 746f 7261 6765 0d0a 202a   get_storage.. *
-000004c0: 2064 656c 6574 655f 6a6f 620d 0a20 0d0a   delete_job.. ..
-000004d0: 2323 2032 2e30 2e31 203a 0d0a 0d0a 202d  ## 2.0.1 :.... -
-000004e0: 2042 7567 2063 6f72 7265 6374 696f 6e20   Bug correction 
-000004f0: 6f6e 2070 7574 5f67 636f 6465 0d0a 200d  on put_gcode.. .
-00000500: 0a23 2320 322e 302e 3020 3a0d 0a0d 0a20  .## 2.0.0 :.... 
-00000510: 2d20 5375 7070 6f72 7420 6669 726d 7761  - Support firmwa
-00000520: 7265 2035 2e31 2e30 0d0a 202d 2041 6464  re 5.1.0.. - Add
-00000530: 6564 203a 200d 0a0d 0a20 2a20 6765 745f  ed : .... * get_
-00000540: 6669 6c65 730d 0a20 2a20 7075 745f 6763  files.. * put_gc
-00000550: 6f64 650d 0a20 2a20 6578 6973 7473 5f67  ode.. * exists_g
-00000560: 636f 6465 0d0a 200d 0a23 2320 312e 302e  code.. ..## 1.0.
-00000570: 3020 3a0d 0a0d 0a20 2d20 4669 7273 7420  0 :.... - First 
-00000580: 5265 6c65 6173 650d 0a0d 0a23 2049 6e73  Release....# Ins
-00000590: 7461 6c6c 696e 6720 5072 7573 614c 696e  talling PrusaLin
-000005a0: 6b50 7920 616e 6420 5375 7070 6f72 7465  kPy and Supporte
-000005b0: 6420 5665 7273 696f 6e73 0d0a 0d0a 5072  d Versions....Pr
-000005c0: 7573 614c 696e 6b50 7920 6973 2061 7661  usaLinkPy is ava
-000005d0: 696c 6162 6c65 206f 6e20 7069 7020 3a0d  ilable on pip :.
-000005e0: 0a0d 0a20 2020 2070 7974 686f 6e20 2d6d  ...    python -m
-000005f0: 2070 6970 2069 6e73 7461 6c6c 2050 7275   pip install Pru
-00000600: 7361 4c69 6e6b 5079 0d0a 0d0a 5072 7573  saLinkPy....Prus
-00000610: 614c 696e 6b50 7920 6f66 6669 6369 616c  aLinkPy official
-00000620: 6c79 2073 7570 706f 7274 7320 5079 7468  ly supports Pyth
-00000630: 6f6e 2033 2e39 2b20 7769 7468 2050 7275  on 3.9+ with Pru
-00000640: 7361 204d 494e 4920 7072 696e 7465 7220  sa MINI printer 
-00000650: 6669 726d 7761 7265 2035 2e31 2e30 2e0d  firmware 5.1.0..
-00000660: 0a0d 0a0d 0a23 2041 5049 2052 6566 6572  .....# API Refer
-00000670: 656e 6365 0d0a 0d0a 2323 204c 6f77 204c  ence....## Low L
-00000680: 6576 656c 2046 756e 6374 696f 6e73 0d0a  evel Functions..
-00000690: 0d0a 5b67 6574 5f76 6572 7369 6f6e 2829  ..[get_version()
-000006a0: 5d28 2370 7275 7361 6c69 6e6b 7079 6765  ](#prusalinkpyge
-000006b0: 745f 7665 7273 696f 6e29 0d0a 0d0a 5b67  t_version)....[g
-000006c0: 6574 5f70 7269 6e74 6572 2829 5d28 2370  et_printer()](#p
-000006d0: 7275 7361 6c69 6e6b 7079 6765 745f 7072  rusalinkpyget_pr
-000006e0: 696e 7465 7229 0d0a 0d0a 5b67 6574 5f6a  inter)....[get_j
-000006f0: 6f62 2829 5d28 2370 7275 7361 6c69 6e6b  ob()](#prusalink
-00000700: 7079 6765 745f 6a6f 6229 0d0a 0d0a 5b64  pyget_job)....[d
-00000710: 656c 6574 655f 6a6f 6228 295d 2823 7072  elete_job()](#pr
-00000720: 7573 616c 696e 6b70 7964 656c 6574 655f  usalinkpydelete_
-00000730: 6a6f 6229 0d0a 0d0a 5b67 6574 5f73 7461  job)....[get_sta
-00000740: 7475 7328 295d 2823 7072 7573 616c 696e  tus()](#prusalin
-00000750: 6b70 7967 6574 5f73 7461 7475 7329 0d0a  kpyget_status)..
-00000760: 0d0a 5b67 6574 5f73 746f 7261 6765 2829  ..[get_storage()
-00000770: 5d28 2370 7275 7361 6c69 6e6b 7079 6765  ](#prusalinkpyge
-00000780: 745f 7374 6f72 6167 6529 0d0a 0d0a 5b67  t_storage)....[g
-00000790: 6574 5f66 696c 6573 2872 656d 6f74 6544  et_files(remoteD
-000007a0: 6972 295d 2823 7072 7573 616c 696e 6b70  ir)](#prusalinkp
-000007b0: 7967 6574 5f66 696c 6573 2d72 656d 6f74  yget_files-remot
-000007c0: 6564 6972 2d2d 290d 0a0d 0a5b 6465 6c65  edir--)....[dele
-000007d0: 7465 2872 656d 6f74 6550 6174 6829 5d28  te(remotePath)](
-000007e0: 2370 7275 7361 6c69 6e6b 7079 6465 6c65  #prusalinkpydele
-000007f0: 7465 7265 6d6f 7465 7061 7468 290d 0a0d  teremotepath)...
-00000800: 0a5b 706f 7374 5f67 636f 6465 2866 696c  .[post_gcode(fil
-00000810: 6550 6174 684c 6f63 616c 2c20 7265 6d6f  ePathLocal, remo
-00000820: 7465 4469 7229 5d28 2370 7275 7361 6c69  teDir)](#prusali
-00000830: 6e6b 7079 7075 745f 706f 7374 5f67 636f  nkpyput_post_gco
-00000840: 6465 290d 0a0d 0a5b 7075 745f 6763 6f64  de)....[put_gcod
-00000850: 6528 6669 6c65 5061 7468 4c6f 6361 6c2c  e(filePathLocal,
-00000860: 2072 656d 6f74 6544 6972 2c20 7072 696e   remoteDir, prin
-00000870: 7441 6674 6572 5570 6c6f 6164 203d 2046  tAfterUpload = F
-00000880: 616c 7365 2c20 6f76 6572 7772 6974 6520  alse, overwrite 
-00000890: 3d20 4661 6c73 6529 5d28 2370 7275 7361  = False)](#prusa
-000008a0: 6c69 6e6b 7079 7075 745f 6763 6f64 6572  linkpyput_gcoder
-000008b0: 656d 6f74 6570 6174 6829 0d0a 0d0a 5b70  emotepath)....[p
-000008c0: 6f73 745f 6763 6f64 6528 6669 6c65 5061  ost_gcode(filePa
-000008d0: 7468 4c6f 6361 6c2c 2072 656d 6f74 6544  thLocal, remoteD
-000008e0: 6972 295d 2823 7072 7573 616c 696e 6b70  ir)](#prusalinkp
-000008f0: 7970 7574 5f70 6f73 745f 6763 6f64 6529  yput_post_gcode)
-00000900: 0d0a 0d0a 5b65 7869 7374 735f 6763 6f64  ....[exists_gcod
-00000910: 6528 7265 6d6f 7465 5061 7468 295d 2823  e(remotePath)](#
-00000920: 7072 7573 616c 696e 6b70 7965 7869 7374  prusalinkpyexist
-00000930: 735f 6763 6f64 6572 656d 6f74 6570 6174  s_gcoderemotepat
-00000940: 6829 0d0a 0d0a 2323 2048 6967 6820 4c65  h)....## High Le
-00000950: 7665 6c20 4675 6e63 7469 6f6e 7320 0d0a  vel Functions ..
-00000960: 0d0a 5b67 6574 5f72 6563 7572 7369 7665  ..[get_recursive
-00000970: 5f66 696c 6573 2872 656d 6f74 6544 6972  _files(remoteDir
-00000980: 295d 2823 7072 7573 616c 696e 6b70 7967  )](#prusalinkpyg
-00000990: 6574 5f72 6563 7572 7369 7665 5f66 696c  et_recursive_fil
-000009a0: 6573 2d72 656d 6f74 6564 6972 2d2d 290d  es-remotedir--).
-000009b0: 0a0d 0a0d 0a23 2055 7365 7220 4775 6964  .....# User Guid
-000009c0: 650d 0a0d 0a23 2320 5072 7573 614c 696e  e....## PrusaLin
-000009d0: 6b50 792e 6765 745f 7665 7273 696f 6e28  kPy.get_version(
-000009e0: 290d 0a0d 0a52 6561 6420 7665 7273 696f  )....Read versio
-000009f0: 6e20 3a0d 0a0d 0a0d 0a20 2020 2069 6d70  n :......    imp
-00000a00: 6f72 7420 5072 7573 614c 696e 6b50 790d  ort PrusaLinkPy.
-00000a10: 0a20 2020 2070 7275 7361 4d69 6e69 203d  .    prusaMini =
-00000a20: 2050 7275 7361 4c69 6e6b 5079 2e50 7275   PrusaLinkPy.Pru
-00000a30: 7361 4c69 6e6b 5079 2822 3139 322e 3136  saLinkPy("192.16
-00000a40: 382e 302e 3132 3322 2c20 2238 6f6a 484b  8.0.123", "8ojHK
-00000a50: 4847 4e75 4148 4132 624d 222c 2070 6f72  HGNuAHA2bM", por
-00000a60: 743d 3830 3137 290d 0a20 2020 206f 626a  t=8017)..    obj
-00000a70: 203d 2070 7275 7361 4d69 6e69 2e67 6574   = prusaMini.get
-00000a80: 5f76 6572 7369 6f6e 2829 0d0a 2020 2020  _version()..    
-00000a90: 6f62 6a2e 6a73 6f6e 2829 0d0a 2020 2020  obj.json()..    
-00000aa0: 0d0a 5265 7475 726e 2073 6f6d 6574 6869  ..Return somethi
-00000ab0: 6e67 206c 696b 6520 3a0d 0a0d 0a20 2020  ng like :....   
-00000ac0: 207b 0d0a 2020 2020 2020 2020 2761 7069   {..        'api
-00000ad0: 273a 2027 322e 302e 3027 2c20 0d0a 2020  ': '2.0.0', ..  
-00000ae0: 2020 2020 2020 2773 6572 7665 7227 3a20        'server': 
-00000af0: 2732 2e31 2e32 272c 200d 0a20 2020 2020  '2.1.2', ..     
-00000b00: 2020 2027 6e6f 7a7a 6c65 5f64 6961 6d65     'nozzle_diame
-00000b10: 7465 7227 3a20 302e 342c 200d 0a20 2020  ter': 0.4, ..   
-00000b20: 2020 2020 2027 7465 7874 273a 2027 5072       'text': 'Pr
-00000b30: 7573 614c 696e 6b27 2c20 0d0a 2020 2020  usaLink', ..    
-00000b40: 2020 2020 2768 6f73 746e 616d 6527 3a20      'hostname': 
-00000b50: 2727 2c20 0d0a 2020 2020 2020 2020 2763  '', ..        'c
-00000b60: 6170 6162 696c 6974 6965 7327 3a20 0d0a  apabilities': ..
-00000b70: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00000b80: 2020 2020 2020 2027 7570 6c6f 6164 2d62         'upload-b
-00000b90: 792d 7075 7427 3a20 5472 7565 0d0a 2020  y-put': True..  
-00000ba0: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
-00000bb0: 0d0a 0d0a 2323 2050 7275 7361 4c69 6e6b  ....## PrusaLink
-00000bc0: 5079 2e67 6574 5f70 7269 6e74 6572 2829  Py.get_printer()
-00000bd0: 0d0a 0d0a 4765 7420 7072 696e 7465 7220  ....Get printer 
-00000be0: 3a0d 0a0d 0a20 2020 2069 6d70 6f72 7420  :....    import 
-00000bf0: 5072 7573 614c 696e 6b50 790d 0a20 2020  PrusaLinkPy..   
-00000c00: 2070 7275 7361 4d69 6e69 203d 2050 7275   prusaMini = Pru
-00000c10: 7361 4c69 6e6b 5079 2e50 7275 7361 4c69  saLinkPy.PrusaLi
-00000c20: 6e6b 5079 2822 3139 322e 3136 382e 302e  nkPy("192.168.0.
-00000c30: 3132 3322 2c20 2238 6f6a 484b 4847 4e75  123", "8ojHKHGNu
-00000c40: 4148 4132 624d 2229 0d0a 2020 2020 6f62  AHA2bM")..    ob
-00000c50: 6a20 3d20 7072 7573 614d 696e 692e 6765  j = prusaMini.ge
-00000c60: 745f 7072 696e 7465 7228 290d 0a20 2020  t_printer()..   
-00000c70: 206f 626a 2e6a 736f 6e28 290d 0a20 2020   obj.json()..   
-00000c80: 200d 0a52 6574 7572 6e20 736f 6d65 7468   ..Return someth
-00000c90: 696e 6720 6c69 6b65 203a 0d0a 0d0a 2020  ing like :....  
-00000ca0: 2020 7b0d 0a20 2020 2020 2020 2027 7465    {..        'te
-00000cb0: 6c65 6d65 7472 7927 3a20 0d0a 2020 2020  lemetry': ..    
-00000cc0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000cd0: 2020 2027 7465 6d70 2d62 6564 273a 2031     'temp-bed': 1
-00000ce0: 362e 332c 0d0a 2020 2020 2020 2020 2020  6.3,..          
-00000cf0: 2020 2774 656d 702d 6e6f 7a7a 6c65 273a    'temp-nozzle':
-00000d00: 2031 362e 372c 0d0a 2020 2020 2020 2020   16.7,..        
-00000d10: 2020 2020 2770 7269 6e74 2d73 7065 6564      'print-speed
-00000d20: 273a 2031 3030 2c0d 0a20 2020 2020 2020  ': 100,..       
-00000d30: 2020 2020 2027 7a2d 6865 6967 6874 273a       'z-height':
-00000d40: 2038 322e 302c 0d0a 2020 2020 2020 2020   82.0,..        
-00000d50: 2020 2020 276d 6174 6572 6961 6c27 3a20      'material': 
-00000d60: 2750 4c41 270d 0a20 2020 2020 2020 207d  'PLA'..        }
-00000d70: 2c20 0d0a 2020 2020 2020 2020 2774 656d  , ..        'tem
-00000d80: 7065 7261 7475 7265 273a 200d 0a20 2020  perature': ..   
-00000d90: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00000da0: 2020 2020 2774 6f6f 6c30 273a 200d 0a20      'tool0': .. 
-00000db0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00000dd0: 6374 7561 6c27 3a20 3136 2e37 2c0d 0a20  ctual': 16.7,.. 
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000df0: 7461 7267 6574 273a 2030 2e30 2c0d 0a20  target': 0.0,.. 
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000e10: 6469 7370 6c61 7927 3a20 302e 302c 0d0a  display': 0.0,..
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 276f 6666 7365 7427 3a20 300d 0a20 2020  'offset': 0..   
-00000e40: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-00000e50: 2020 2020 2020 2020 2027 6265 6427 3a20           'bed': 
-00000e60: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
-00000e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e80: 2027 6163 7475 616c 273a 3136 2e33 2c0d   'actual':16.3,.
-00000e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ea0: 2027 7461 7267 6574 273a 2030 2e30 2c0d   'target': 0.0,.
-00000eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ec0: 2027 6f66 6673 6574 273a 2030 0d0a 2020   'offset': 0..  
-00000ed0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00000ee0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
-00000ef0: 2027 7374 6174 6527 3a20 0d0a 2020 2020   'state': ..    
-00000f00: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000f10: 2020 2027 7465 7874 273a 2027 4f70 6572     'text': 'Oper
-00000f20: 6174 696f 6e61 6c27 2c0d 0a20 2020 2020  ational',..     
-00000f30: 2020 2020 2020 2027 666c 6167 7327 3a20         'flags': 
-00000f40: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
-00000f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f60: 2027 6f70 6572 6174 696f 6e61 6c27 3a20   'operational': 
-00000f70: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00000f80: 2020 2020 2020 2027 7061 7573 6564 273a         'paused':
-00000f90: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00000fa0: 2020 2020 2020 2020 2027 7072 696e 7469           'printi
-00000fb0: 6e67 273a 2046 616c 7365 2c0d 0a20 2020  ng': False,..   
-00000fc0: 2020 2020 2020 2020 2020 2020 2027 6361               'ca
-00000fd0: 6e63 656c 6c69 6e67 273a 2046 616c 7365  ncelling': False
-00000fe0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000ff0: 2020 2027 7061 7573 696e 6727 3a20 4661     'pausing': Fa
-00001000: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00001010: 2020 2020 2020 2765 7272 6f72 273a 2046        'error': F
-00001020: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-00001030: 2020 2020 2020 2027 7364 5265 6164 7927         'sdReady'
-00001040: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
-00001050: 2020 2020 2020 2020 2020 2763 6c6f 7365            'close
-00001060: 644f 6e45 7272 6f72 273a 2046 616c 7365  dOnError': False
-00001070: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001080: 2020 2027 7265 6164 7927 3a20 5472 7565     'ready': True
-00001090: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000010a0: 2020 2027 6275 7379 273a 2046 616c 7365     'busy': False
-000010b0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
-000010c0: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-000010d0: 7d0d 0a0d 0a23 2320 5072 7573 614c 696e  }....## PrusaLin
-000010e0: 6b50 792e 6765 745f 6a6f 6228 290d 0a0d  kPy.get_job()...
-000010f0: 0a47 6574 206a 6f62 203a 0d0a 0d0a 2020  .Get job :....  
-00001100: 2020 696d 706f 7274 2050 7275 7361 4c69    import PrusaLi
-00001110: 6e6b 5079 0d0a 2020 2020 7072 7573 614d  nkPy..    prusaM
-00001120: 696e 6920 3d20 5072 7573 614c 696e 6b50  ini = PrusaLinkP
-00001130: 792e 5072 7573 614c 696e 6b50 7928 2231  y.PrusaLinkPy("1
-00001140: 3932 2e31 3638 2e30 2e31 3233 222c 2022  92.168.0.123", "
-00001150: 386f 6a48 4b48 474e 7541 4841 3262 4d22  8ojHKHGNuAHA2bM"
-00001160: 290d 0a20 2020 206f 626a 203d 2070 7275  )..    obj = pru
-00001170: 7361 4d69 6e69 2e67 6574 5f6a 6f62 2829  saMini.get_job()
-00001180: 0d0a 2020 2020 6f62 6a2e 6a73 6f6e 2829  ..    obj.json()
-00001190: 0d0a 2020 2020 0d0a 5265 7475 726e 2073  ..    ..Return s
-000011a0: 6f6d 6574 6869 6e67 206c 696b 6520 3a0d  omething like :.
-000011b0: 0a0d 0a20 2020 207b 0d0a 2020 2020 2020  ...    {..      
-000011c0: 2020 2273 7461 7465 223a 224f 7065 7261    "state":"Opera
-000011d0: 7469 6f6e 616c 222c 0d0a 2020 2020 2020  tional",..      
-000011e0: 2020 226a 6f62 223a 204e 6f6e 652c 0d0a    "job": None,..
-000011f0: 2020 2020 2020 2020 2270 726f 6772 6573          "progres
-00001200: 7322 3a20 4e6f 6e65 0d0a 2020 2020 7d0d  s": None..    }.
-00001210: 0a20 2020 200d 0a23 2320 5072 7573 614c  .    ..## PrusaL
-00001220: 696e 6b50 792e 6465 6c65 7465 5f6a 6f62  inkPy.delete_job
-00001230: 286a 6f62 290d 0a0d 0a44 656c 6574 6520  (job)....Delete 
-00001240: 6120 6a6f 622e 204a 6f62 206e 756d 6265  a job. Job numbe
-00001250: 7220 6973 2061 7661 696c 6162 6c65 2077  r is available w
-00001260: 6974 6820 6765 745f 6a6f 6228 2920 6f72  ith get_job() or
-00001270: 2067 6574 5f73 7461 7475 7328 290d 0a0d   get_status()...
-00001280: 0a20 2020 2069 6d70 6f72 7420 5072 7573  .    import Prus
-00001290: 614c 696e 6b50 790d 0a20 2020 2070 7275  aLinkPy..    pru
-000012a0: 7361 4d69 6e69 203d 2050 7275 7361 4c69  saMini = PrusaLi
-000012b0: 6e6b 5079 2e50 7275 7361 4c69 6e6b 5079  nkPy.PrusaLinkPy
-000012c0: 2822 3139 322e 3136 382e 302e 3132 3322  ("192.168.0.123"
-000012d0: 2c20 2238 6f6a 484b 4847 4e75 4148 4132  , "8ojHKHGNuAHA2
-000012e0: 624d 2229 0d0a 2020 2020 6f62 6a20 3d20  bM")..    obj = 
-000012f0: 7072 7573 614d 696e 692e 6465 6c65 7465  prusaMini.delete
-00001300: 5f6a 6f62 2822 3433 2229 0d0a 2020 2020  _job("43")..    
-00001310: 0d0a 0d0a 2323 2050 7275 7361 4c69 6e6b  ....## PrusaLink
-00001320: 5079 2e67 6574 5f73 7461 7475 7328 290d  Py.get_status().
-00001330: 0a0d 0a47 6574 206a 6f62 203a 0d0a 0d0a  ...Get job :....
-00001340: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
-00001350: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
-00001360: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
-00001370: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
-00001380: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
-00001390: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
-000013a0: 4d22 290d 0a20 2020 206f 626a 203d 2070  M")..    obj = p
-000013b0: 7275 7361 4d69 6e69 2e67 6574 5f73 7461  rusaMini.get_sta
-000013c0: 7475 7328 290d 0a20 2020 206f 626a 2e6a  tus()..    obj.j
-000013d0: 736f 6e28 290d 0a20 2020 200d 0a52 6574  son()..    ..Ret
-000013e0: 7572 6e20 736f 6d65 7468 696e 6720 6c69  urn something li
-000013f0: 6b65 203a 0d0a 0d0a 2020 2020 7b0d 0a20  ke :....    {.. 
-00001400: 2020 2020 2020 2022 6a6f 6222 3a0d 0a20         "job":.. 
-00001410: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00001420: 2020 2020 2020 2269 6422 3a34 332c 0d0a        "id":43,..
-00001430: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-00001440: 6772 6573 7322 3a30 2e30 302c 0d0a 2020  gress":0.00,..  
-00001450: 2020 2020 2020 2020 2020 2274 696d 655f            "time_
-00001460: 7265 6d61 696e 696e 6722 3a31 3230 2c0d  remaining":120,.
-00001470: 0a20 2020 2020 2020 2020 2020 2022 7469  .            "ti
-00001480: 6d65 5f70 7269 6e74 696e 6722 3a31 3433  me_printing":143
-00001490: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000014a0: 2020 2020 2020 2273 746f 7261 6765 223a        "storage":
-000014b0: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-000014c0: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
-000014d0: 222f 7573 622f 222c 0d0a 2020 2020 2020  "/usb/",..      
-000014e0: 2020 2020 2020 226e 616d 6522 3a22 7573        "name":"us
-000014f0: 6222 2c0d 0a20 2020 2020 2020 2020 2020  b",..           
-00001500: 2022 7265 6164 5f6f 6e6c 7922 3a66 616c   "read_only":fal
-00001510: 7365 0d0a 2020 2020 2020 2020 7d2c 0d0a  se..        },..
-00001520: 2020 2020 2020 2020 2270 7269 6e74 6572          "printer
-00001530: 223a 0d0a 2020 2020 2020 2020 7b0d 0a20  ":..        {.. 
-00001540: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
-00001550: 6522 3a22 5052 494e 5449 4e47 222c 0d0a  e":"PRINTING",..
-00001560: 2020 2020 2020 2020 2020 2020 2274 656d              "tem
-00001570: 705f 6265 6422 3a35 372e 332c 0d0a 2020  p_bed":57.3,..  
-00001580: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
-00001590: 745f 6265 6422 3a30 2e30 2c0d 0a20 2020  t_bed":0.0,..   
-000015a0: 2020 2020 2020 2020 2022 7465 6d70 5f6e           "temp_n
-000015b0: 6f7a 7a6c 6522 3a32 342e 312c 0d0a 2020  ozzle":24.1,..  
-000015c0: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
-000015d0: 745f 6e6f 7a7a 6c65 223a 302e 302c 0d0a  t_nozzle":0.0,..
-000015e0: 2020 2020 2020 2020 2020 2020 2261 7869              "axi
-000015f0: 735f 7a22 3a31 3632 2e32 2c0d 0a20 2020  s_z":162.2,..   
-00001600: 2020 2020 2020 2020 2022 666c 6f77 223a           "flow":
-00001610: 3130 302c 0d0a 2020 2020 2020 2020 2020  100,..          
-00001620: 2020 2273 7065 6564 223a 3130 302c 0d0a    "speed":100,..
-00001630: 2020 2020 2020 2020 2020 2020 2266 616e              "fan
-00001640: 5f68 6f74 656e 6422 3a30 2c0d 0a20 2020  _hotend":0,..   
-00001650: 2020 2020 2020 2020 2022 6661 6e5f 7072           "fan_pr
-00001660: 696e 7422 3a30 0d0a 2020 2020 2020 2020  int":0..        
-00001670: 7d0d 0a20 2020 207d 0d0a 2020 2020 0d0a  }..    }..    ..
-00001680: 2323 2050 7275 7361 4c69 6e6b 5079 2e67  ## PrusaLinkPy.g
-00001690: 6574 5f73 746f 7261 6765 2829 0d0a 0d0a  et_storage()....
-000016a0: 4765 7420 6a6f 6220 3a0d 0a0d 0a20 2020  Get job :....   
-000016b0: 2069 6d70 6f72 7420 5072 7573 614c 696e   import PrusaLin
-000016c0: 6b50 790d 0a20 2020 2070 7275 7361 4d69  kPy..    prusaMi
-000016d0: 6e69 203d 2050 7275 7361 4c69 6e6b 5079  ni = PrusaLinkPy
-000016e0: 2e50 7275 7361 4c69 6e6b 5079 2822 3139  .PrusaLinkPy("19
-000016f0: 322e 3136 382e 302e 3132 3322 2c20 2238  2.168.0.123", "8
-00001700: 6f6a 484b 4847 4e75 4148 4132 624d 2229  ojHKHGNuAHA2bM")
-00001710: 0d0a 2020 2020 6f62 6a20 3d20 7072 7573  ..    obj = prus
-00001720: 614d 696e 692e 6765 745f 7374 6f72 6167  aMini.get_storag
-00001730: 6528 290d 0a20 2020 206f 626a 2e6a 736f  e()..    obj.jso
-00001740: 6e28 290d 0a20 2020 200d 0a52 6574 7572  n()..    ..Retur
-00001750: 6e20 736f 6d65 7468 696e 6720 6c69 6b65  n something like
-00001760: 203a 0d0a 0d0a 2020 2020 544f 444f 0d0a   :....    TODO..
-00001770: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
-00001780: 2e67 6574 5f66 696c 6573 2820 7265 6d6f  .get_files( remo
-00001790: 7465 4469 7220 3d20 272f 2729 0d0a 0d0a  teDir = '/')....
-000017a0: 4765 7420 4669 6c65 7320 6f6e 2055 5342  Get Files on USB
-000017b0: 2044 7269 7665 203a 0d0a 0d0a 2020 2020   Drive :....    
-000017c0: 696d 706f 7274 2050 7275 7361 4c69 6e6b  import PrusaLink
-000017d0: 5079 0d0a 2020 2020 7072 7573 614d 696e  Py..    prusaMin
-000017e0: 6920 3d20 5072 7573 614c 696e 6b50 792e  i = PrusaLinkPy.
-000017f0: 5072 7573 614c 696e 6b50 7928 2231 3932  PrusaLinkPy("192
-00001800: 2e31 3638 2e30 2e31 3233 222c 2022 386f  .168.0.123", "8o
-00001810: 6a48 4b48 474e 7541 4841 3262 4d22 290d  jHKHGNuAHA2bM").
-00001820: 0a20 2020 206f 626a 203d 2070 7275 7361  .    obj = prusa
-00001830: 4d69 6e69 2e67 6574 5f66 696c 6573 2829  Mini.get_files()
-00001840: 0d0a 2020 2020 6669 6c65 7352 6574 203d  ..    filesRet =
-00001850: 206f 626a 2e6a 736f 6e28 290d 0a20 2020   obj.json()..   
-00001860: 200d 0a52 6574 7572 6e20 736f 6d65 7468   ..Return someth
-00001870: 696e 6720 6c69 6b65 203a 0d0a 0d0a 2020  ing like :....  
-00001880: 2020 7b0d 0a20 2020 2020 2020 2027 7479    {..        'ty
-00001890: 7065 273a 2027 464f 4c44 4552 272c 200d  pe': 'FOLDER', .
-000018a0: 0a20 2020 2020 2020 2027 726f 273a 2046  .        'ro': F
-000018b0: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
-000018c0: 276e 616d 6527 3a20 2775 7362 272c 200d  'name': 'usb', .
-000018d0: 0a20 2020 2020 2020 2027 6368 696c 6472  .        'childr
-000018e0: 656e 273a 200d 0a20 2020 2020 2020 205b  en': ..        [
-000018f0: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00001900: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
-00001910: 2027 4d54 4e27 2c20 0d0a 2020 2020 2020   'MTN', ..      
-00001920: 2020 2020 2020 2772 6f27 3a20 4661 6c73        'ro': Fals
-00001930: 652c 200d 0a20 2020 2020 2020 2020 2020  e, ..           
-00001940: 2027 7479 7065 273a 2027 464f 4c44 4552   'type': 'FOLDER
-00001950: 272c 200d 0a20 2020 2020 2020 2020 2020  ', ..           
-00001960: 2027 6d5f 7469 6d65 7374 616d 7027 3a20   'm_timestamp': 
-00001970: 3137 3032 3632 3839 3435 2c20 0d0a 2020  1702628945, ..  
-00001980: 2020 2020 2020 2020 2020 2764 6973 706c            'displ
-00001990: 6179 5f6e 616d 6527 3a20 274d 544e 270d  ay_name': 'MTN'.
-000019a0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-000019b0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-000019c0: 2020 2020 276e 616d 6527 3a20 2753 325f      'name': 'S2_
-000019d0: 5632 4953 272c 200d 0a20 2020 2020 2020  V2IS', ..       
-000019e0: 2020 2020 2027 726f 273a 2046 616c 7365       'ro': False
-000019f0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00001a00: 2774 7970 6527 3a20 2746 4f4c 4445 5227  'type': 'FOLDER'
-00001a10: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00001a20: 276d 5f74 696d 6573 7461 6d70 273a 2031  'm_timestamp': 1
-00001a30: 3730 3235 3635 3138 322c 200d 0a20 2020  702565182, ..   
-00001a40: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
-00001a50: 795f 6e61 6d65 273a 2027 5332 5f56 3249  y_name': 'S2_V2I
-00001a60: 5327 0d0a 2020 2020 2020 2020 7d0d 0a20  S'..        }.. 
-00001a70: 2020 2020 2020 205d 0d0a 2020 2020 7d0d         ]..    }.
-00001a80: 0a20 2020 200d 0a57 6f72 6b61 6c73 6f20  .    ..Workalso 
-00001a90: 7769 7468 2073 7562 666f 6c64 6572 0d0a  with subfolder..
-00001aa0: 0d0a 2020 2020 6f62 6a20 3d20 7072 7573  ..    obj = prus
-00001ab0: 614d 696e 692e 6765 745f 6669 6c65 7328  aMini.get_files(
-00001ac0: 7265 6d6f 7465 4469 7220 3d20 272f 5355  remoteDir = '/SU
-00001ad0: 4246 4f4c 4445 5227 290d 0a0d 0a23 2320  BFOLDER')....## 
-00001ae0: 5072 7573 614c 696e 6b50 792e 6765 745f  PrusaLinkPy.get_
-00001af0: 7265 6375 7273 6976 655f 6669 6c65 7328  recursive_files(
-00001b00: 2072 656d 6f74 6544 6972 203d 2027 2f27   remoteDir = '/'
-00001b10: 290d 0a0d 0a47 6574 2061 6c6c 2066 696c  )....Get all fil
-00001b20: 6573 2069 6e20 6120 666f 6c64 6572 2061  es in a folder a
-00001b30: 6e64 2073 7562 666f 6c64 6572 2e0d 0a0d  nd subfolder....
-00001b40: 0a57 6172 6e69 6e67 203a 2072 6574 7572  .Warning : retur
-00001b50: 6e20 6e65 7374 6564 2064 6963 742e 0d0a  n nested dict...
-00001b60: 0d0a 0d0a 2020 2020 696d 706f 7274 2050  ....    import P
-00001b70: 7275 7361 4c69 6e6b 5079 0d0a 2020 2020  rusaLinkPy..    
-00001b80: 7072 7573 614d 696e 6920 3d20 5072 7573  prusaMini = Prus
-00001b90: 614c 696e 6b50 792e 5072 7573 614c 696e  aLinkPy.PrusaLin
-00001ba0: 6b50 7928 2231 3932 2e31 3638 2e30 2e31  kPy("192.168.0.1
-00001bb0: 3233 222c 2022 386f 6a48 4b48 474e 7541  23", "8ojHKHGNuA
-00001bc0: 4841 3262 4d22 290d 0a20 2020 2064 6963  HA2bM")..    dic
-00001bd0: 7474 203d 2070 7275 7361 4d69 6e69 2e67  tt = prusaMini.g
-00001be0: 6574 5f72 6563 7572 7369 7665 5f66 696c  et_recursive_fil
-00001bf0: 6573 2829 0d0a 2020 2020 0d0a 2020 2020  es()..    ..    
-00001c00: 7b0d 0a20 2020 2020 2020 2027 4d54 4e27  {..        'MTN'
-00001c10: 3a20 0d0a 2020 2020 2020 2020 7b0d 0a20  : ..        {.. 
-00001c20: 2020 2020 2020 2020 2020 2027 4348 4754             'CHGT
-00001c30: 5f42 5553 452e 6763 6f64 6527 3a20 272f  _BUSE.gcode': '/
-00001c40: 4d54 4e2f 4348 4754 5f42 7e31 2e47 434f  MTN/CHGT_B~1.GCO
-00001c50: 272c 200d 0a20 2020 2020 2020 2020 2020  ', ..           
-00001c60: 2027 4445 424f 5543 4841 4745 2e67 636f   'DEBOUCHAGE.gco
-00001c70: 6465 273a 2027 2f4d 544e 2f44 4542 4f55  de': '/MTN/DEBOU
-00001c80: 437e 312e 4743 4f27 2c20 0d0a 2020 2020  C~1.GCO', ..    
-00001c90: 2020 2020 2020 2020 2750 5245 4348 4155          'PRECHAU
-00001ca0: 4646 452e 6763 6f64 6527 3a20 272f 4d54  FFE.gcode': '/MT
-00001cb0: 4e2f 5052 4543 4841 7e31 2e47 434f 270d  N/PRECHA~1.GCO'.
-00001cc0: 0a20 2020 2020 2020 207d 2c20 0d0a 2020  .        }, ..  
-00001cd0: 2020 2020 2020 2753 325f 5632 4953 273a        'S2_V2IS':
-00001ce0: 200d 0a20 2020 2020 2020 207b 0d0a 2020   ..        {..  
-00001cf0: 2020 2020 2020 2020 2020 2732 6833 336d            '2h33m
-00001d00: 2e62 6763 6f64 6527 3a20 272f 5332 5f56  .bgcode': '/S2_V
-00001d10: 3249 532f 3248 3333 4d7e 312e 4247 4327  2IS/2H33M~1.BGC'
-00001d20: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00001d30: 3568 356d 2e62 6763 6f64 6527 3a20 272f  5h5m.bgcode': '/
-00001d40: 5332 5f56 3249 532f 3548 354d 7e31 2e42  S2_V2IS/5H5M~1.B
-00001d50: 4743 270d 0a20 2020 2020 2020 207d 0d0a  GC'..        }..
-00001d60: 2020 2020 7d0d 0a0d 0a23 2320 5072 7573      }....## Prus
-00001d70: 614c 696e 6b50 792e 6465 6c65 7465 2872  aLinkPy.delete(r
-00001d80: 656d 6f74 6550 6174 6829 200d 0a0d 0a44  emotePath) ....D
-00001d90: 656c 6574 6520 6120 6669 6c65 206f 7220  elete a file or 
-00001da0: 6120 666f 6c64 6572 206f 6e20 5553 4220  a folder on USB 
-00001db0: 6472 6976 650d 0a0d 0a20 2020 2069 6d70  drive....    imp
-00001dc0: 6f72 7420 5072 7573 614c 696e 6b50 790d  ort PrusaLinkPy.
-00001dd0: 0a20 2020 2070 7275 7361 4d69 6e69 203d  .    prusaMini =
-00001de0: 2050 7275 7361 4c69 6e6b 5079 2e50 7275   PrusaLinkPy.Pru
-00001df0: 7361 4c69 6e6b 5079 2822 3139 322e 3136  saLinkPy("192.16
-00001e00: 382e 302e 3132 3322 2c20 2238 6f6a 484b  8.0.123", "8ojHK
-00001e10: 4847 4e75 4148 4132 624d 2229 0d0a 2020  HGNuAHA2bM")..  
-00001e20: 2020 6f62 6a20 3d20 7072 7573 614d 696e    obj = prusaMin
-00001e30: 692e 6465 6c65 7465 2827 2f44 4542 4f55  i.delete('/DEBOU
-00001e40: 437e 312e 4743 4f27 290d 0a0d 0a0d 0a23  C~1.GCO')......#
-00001e50: 2320 5072 7573 614c 696e 6b50 792e 706f  # PrusaLinkPy.po
-00001e60: 7374 5f67 636f 6465 2872 656d 6f74 6550  st_gcode(remoteP
-00001e70: 6174 6829 200d 0a0d 0a50 7269 6e74 2061  ath) ....Print a
-00001e80: 2066 696c 6520 0d0a 0d0a 2020 2020 696d   file ....    im
-00001e90: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
-00001ea0: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
-00001eb0: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
-00001ec0: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
-00001ed0: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
-00001ee0: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
-00001ef0: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
-00001f00: 6e69 2e70 6f73 745f 6763 6f64 6528 272f  ni.post_gcode('/
-00001f10: 4445 424f 5543 7e31 2e47 434f 2729 0d0a  DEBOUC~1.GCO')..
-00001f20: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
-00001f30: 2e70 7574 5f67 636f 6465 2872 656d 6f74  .put_gcode(remot
-00001f40: 6550 6174 682c 2070 7269 6e74 4166 7465  ePath, printAfte
-00001f50: 7255 706c 6f61 6420 3d20 4661 6c73 652c  rUpload = False,
-00001f60: 206f 7665 7277 7269 7465 203d 2046 616c   overwrite = Fal
-00001f70: 7365 2920 0d0a 0d0a 5365 6e64 2061 2066  se) ....Send a f
-00001f80: 696c 6520 6f6e 2055 5342 2044 7269 7665  ile on USB Drive
-00001f90: 2e0d 0a0d 0a43 616e 2063 7265 6174 6520  .....Can create 
-00001fa0: 6120 666f 6c64 6572 2021 0d0a 0d0a 6966  a folder !....if
-00001fb0: 2072 6574 2e73 7461 7475 735f 636f 6465   ret.status_code
-00001fc0: 203d 2034 3039 202d 3e20 436f 6e66 6c69   = 409 -> Confli
-00001fd0: 6374 203a 2046 696c 6520 616c 7265 6164  ct : File alread
-00001fe0: 7920 6578 6973 7473 0d0a 0d0a 7072 696e  y exists....prin
-00001ff0: 7441 6674 6572 5570 6c6f 6164 203a 2053  tAfterUpload : S
-00002000: 6574 2061 7420 5472 7565 2074 6f20 7072  et at True to pr
-00002010: 696e 7420 6166 7465 7220 7570 6c6f 6164  int after upload
-00002020: 2e20 5761 726e 696e 6720 3a20 5072 696e  . Warning : Prin
-00002030: 7465 7220 4c43 4420 6d75 7374 2062 6520  ter LCD must be 
-00002040: 6f6e 206d 6169 6e20 7363 7265 656e 2021  on main screen !
-00002050: 0d0a 0d0a 6f76 6572 7772 6974 6520 3a20  ....overwrite : 
-00002060: 416c 6c6f 7720 6669 6c65 204f 7665 7277  Allow file Overw
-00002070: 7269 7465 0d0a 0d0a 0d0a 2020 2020 696d  rite......    im
-00002080: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
-00002090: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
-000020a0: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
-000020b0: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
-000020c0: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
-000020d0: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
-000020e0: 2020 2073 7461 7475 7320 3d20 7072 7573     status = prus
-000020f0: 614d 696e 692e 7075 7428 2743 3a2f 4d54  aMini.put('C:/MT
-00002100: 4e2f 4445 424f 5543 4841 4745 2e67 636f  N/DEBOUCHAGE.gco
-00002110: 6465 2720 2c20 274d 544e 2f44 4542 4f55  de' , 'MTN/DEBOU
-00002120: 4348 4147 452e 6763 6f64 6527 290d 0a20  CHAGE.gcode').. 
-00002130: 2020 2023 204f 7665 7277 7269 7465 0d0a     # Overwrite..
-00002140: 2020 2020 7374 6174 7573 203d 2070 7275      status = pru
-00002150: 7361 4d69 6e69 2e70 7574 2827 433a 2f4d  saMini.put('C:/M
-00002160: 544e 2f44 4542 4f55 4348 4147 452e 6763  TN/DEBOUCHAGE.gc
-00002170: 6f64 6527 202c 2027 4d54 4e2f 4445 424f  ode' , 'MTN/DEBO
-00002180: 5543 4841 4745 2e67 636f 6465 272c 2046  UCHAGE.gcode', F
-00002190: 616c 7365 2c20 5472 7565 290d 0a20 2020  alse, True)..   
-000021a0: 2023 204f 7665 7277 7269 7465 2061 6e64   # Overwrite and
-000021b0: 2050 7269 6e74 0d0a 2020 2020 7374 6174   Print..    stat
-000021c0: 7573 203d 2070 7275 7361 4d69 6e69 2e70  us = prusaMini.p
-000021d0: 7574 2827 433a 2f4d 544e 2f44 4542 4f55  ut('C:/MTN/DEBOU
-000021e0: 4348 4147 452e 6763 6f64 6527 202c 2027  CHAGE.gcode' , '
-000021f0: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
-00002200: 636f 6465 272c 2054 7275 652c 2054 7275  code', True, Tru
-00002210: 6529 0d0a 2020 2020 0d0a 2323 2050 7275  e)..    ..## Pru
-00002220: 7361 4c69 6e6b 5079 2e65 7869 7374 735f  saLinkPy.exists_
-00002230: 6763 6f64 6528 7265 6d6f 7465 5061 7468  gcode(remotePath
-00002240: 2920 0d0a 0d0a 4368 6563 6b20 6966 2061  ) ....Check if a
-00002250: 2066 696c 6520 6578 6973 7473 206f 6e20   file exists on 
-00002260: 5553 4220 6472 6976 652e 200d 0a0d 0a52  USB drive. ....R
-00002270: 6574 7572 6e20 5472 7565 206f 7220 4661  eturn True or Fa
-00002280: 6c73 650d 0a0d 0a20 2020 2069 6d70 6f72  lse....    impor
-00002290: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
-000022a0: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
-000022b0: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
-000022c0: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
-000022d0: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
-000022e0: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
-000022f0: 7374 6174 7573 203d 2070 7275 7361 4d69  status = prusaMi
-00002300: 6e69 2e65 7869 7374 735f 6763 6f64 6528  ni.exists_gcode(
-00002310: 272f 4445 424f 5543 7e31 2e47 434f 2729  '/DEBOUC~1.GCO')
-00002320: 0d0a 0d0a 2320 4150 490d 0a0d 0a41 5049  ....# API....API
-00002330: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
-00002340: 2069 6e20 6d79 206c 6962 2020 3a20 0d0a   in my lib  : ..
-00002350: 0d0a 7265 7472 6965 7665 2074 6875 6d62  ..retrieve thumb
-00002360: 6e61 696c 200d 0a0d 0a20 2020 2072 203d  nail ....    r =
-00002370: 2072 6571 7565 7374 732e 6765 7428 2768   requests.get('h
-00002380: 7474 703a 2f2f 3139 322e 3136 382e 302e  ttp://192.168.0.
-00002390: 3132 333a 3830 3137 2f74 6875 6d62 2f6c  123:8017/thumb/l
-000023a0: 2f75 7362 2f54 4156 4552 4e7e 312e 4743  /usb/TAVERN~1.GC
-000023b0: 4f27 2c20 6865 6164 6572 733d 6865 6164  O', headers=head
-000023c0: 6572 7329 0d0a 0d0a 0d0a 2f61 7069 2f73  ers)....../api/s
-000023d0: 6574 7469 6e67 730d 0a0d 0a0d 0a50 4f53  ettings......POS
-000023e0: 5420 2f61 7069 2f6a 6f62 0d0a 2a2a 5b4c  T /api/job..**[L
-000023f0: 696e 6b20 746f 2042 7564 6479 2063 6f64  ink to Buddy cod
-00002400: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00002410: 622e 636f 6d2f 7072 7573 6133 642f 5072  b.com/prusa3d/Pr
-00002420: 7573 612d 4669 726d 7761 7265 2d42 7564  usa-Firmware-Bud
-00002430: 6479 2f62 6c6f 622f 6d61 7374 6572 2f6c  dy/blob/master/l
-00002440: 6962 2f57 5549 2f6c 696e 6b5f 636f 6e74  ib/WUI/link_cont
-00002450: 656e 742f 7072 7573 615f 6c69 6e6b 5f61  ent/prusa_link_a
-00002460: 7069 2e63 7070 234c 3237 3629 2a2a 0d0a  pi.cpp#L276)**..
-00002470: 0d0a 4745 542f 504f 5354 202f 6170 692f  ..GET/POST /api/
-00002480: 646f 776e 6c6f 6164 200d 0a2a 2a5b 4c69  download ..**[Li
-00002490: 6e6b 2074 6f20 4275 6464 7920 636f 6465  nk to Buddy code
-000024a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000024b0: 2e63 6f6d 2f70 7275 7361 3364 2f50 7275  .com/prusa3d/Pru
-000024c0: 7361 2d46 6972 6d77 6172 652d 4275 6464  sa-Firmware-Budd
-000024d0: 792f 626c 6f62 2f6d 6173 7465 722f 6c69  y/blob/master/li
-000024e0: 622f 5755 492f 6c69 6e6b 5f63 6f6e 7465  b/WUI/link_conte
-000024f0: 6e74 2f70 7275 7361 5f6c 696e 6b5f 6170  nt/prusa_link_ap
-00002500: 692e 6370 7023 4c32 3839 292a 2a0d 0a0d  i.cpp#L289)**...
-00002510: 0a0d 0a23 2020 4275 6773 2070 7265 7365  ...#  Bugs prese
-00002520: 6e74 2069 6e20 5072 7573 6120 4d49 4e49  nt in Prusa MINI
-00002530: 2070 7269 6e74 6572 2066 6972 6d77 6172   printer firmwar
-00002540: 6520 342e 342e 313a 0d0a 0d0a 202a 2054  e 4.4.1:.... * T
-00002550: 6865 7265 2069 7320 6e6f 2070 6f73 7369  here is no possi
-00002560: 6269 6c69 7479 2074 6f20 6861 7665 2074  bility to have t
-00002570: 6865 206c 6973 7420 6f66 2066 6f6c 6465  he list of folde
-00002580: 7273 2070 7265 7365 6e74 2069 6e20 6120  rs present in a 
-00002590: 6469 7265 6374 6f72 790d 0a20 2020 202a  directory..    *
-000025a0: 2053 6f6c 7665 6420 696e 2066 6972 6d77   Solved in firmw
-000025b0: 6172 6520 350d 0a20 2a20 596f 7520 6361  are 5.. * You ca
-000025c0: 6e6e 6f74 2075 706c 6f61 6420 6120 6763  nnot upload a gc
-000025d0: 6f64 6520 696e 2061 2073 7562 666f 6c64  ode in a subfold
-000025e0: 6572 206f 6620 7468 6520 5553 4220 6b65  er of the USB ke
-000025f0: 790d 0a20 2020 202a 2053 6f6c 7665 6420  y..    * Solved 
-00002600: 696e 2066 6972 6d77 6172 6520 350d 0a20  in firmware 5.. 
-00002610: 2a20 5768 656e 2074 6865 2070 7269 6e74  * When the print
-00002620: 6572 2064 6574 6563 7473 2074 6865 2065  er detects the e
-00002630: 6e64 206f 6620 7468 6520 6669 6c61 6d65  nd of the filame
-00002640: 6e74 2061 6e64 2069 7420 6469 7370 6c61  nt and it displa
-00002650: 7973 2022 4368 616e 6765 2046 696c 616d  ys "Change Filam
-00002660: 656e 7422 2074 6865 2074 656c 656d 6574  ent" the telemet
-00002670: 7279 2069 6e66 6f72 6d61 7469 6f6e 2069  ry information i
-00002680: 7320 6e6f 206c 6f6e 6765 7220 676f 6f64  s no longer good
-00002690: 2e20 4865 7265 2069 7320 7468 6520 696e  . Here is the in
-000026a0: 666f 726d 6174 696f 6e20 7265 7475 726e  formation return
-000026b0: 6564 2062 7920 7468 6520 7072 696e 7465  ed by the printe
-000026c0: 7220 696e 2074 6869 7320 6361 7365 3a0d  r in this case:.
-000026d0: 0a20 0d0a 2020 2020 2774 656c 656d 6574  . ..    'telemet
-000026e0: 7279 273a 207b 2774 656d 702d 6265 6427  ry': {'temp-bed'
-000026f0: 3a20 302e 302c 2027 7465 6d70 2d6e 6f7a  : 0.0, 'temp-noz
-00002700: 7a6c 6527 3a20 302e 302c 2027 7072 696e  zle': 0.0, 'prin
-00002710: 742d 7370 6565 6427 3a20 3130 302c 2027  t-speed': 100, '
-00002720: 7a2d 6865 6967 6874 273a 2030 2e30 2c20  z-height': 0.0, 
-00002730: 276d 6174 6572 6961 6c27 3a20 272d 2d2d  'material': '---
-00002740: 277d 0d0a 2020 2020 0d0a 202a 2053 7469  '}..    .. * Sti
-00002750: 6c6c 2069 6e20 7468 6520 6361 7365 206f  ll in the case o
-00002760: 6620 6120 6669 6c61 6d65 6e74 2063 6861  f a filament cha
-00002770: 6e67 652c 2074 6865 2073 7461 7475 7320  nge, the status 
-00002780: 696e 666f 726d 6174 696f 6e20 6973 2069  information is i
-00002790: 6e63 6f72 7265 6374 3a0d 0a0d 0a20 2020  ncorrect:....   
-000027a0: 2027 7374 6174 6527 3a20 7b27 7465 7874   'state': {'text
-000027b0: 273a 2027 4f70 6572 6174 696f 6e61 6c27  ': 'Operational'
-000027c0: 2c20 2766 6c61 6773 273a 207b 276f 7065  , 'flags': {'ope
-000027d0: 7261 7469 6f6e 616c 273a 2054 7275 652c  rational': True,
-000027e0: 2027 7061 7573 6564 273a 2046 616c 7365   'paused': False
-000027f0: 2c20 2770 7269 6e74 696e 6727 3a20 4661  , 'printing': Fa
-00002800: 6c73 652c 2027 6361 6e63 656c 6c69 6e67  lse, 'cancelling
-00002810: 273a 2046 616c 7365 2c20 2770 6175 7369  ': False, 'pausi
-00002820: 6e67 273a 2046 616c 7365 2c20 2773 6452  ng': False, 'sdR
-00002830: 6561 6479 273a 2046 616c 7365 2c20 2765  eady': False, 'e
-00002840: 7272 6f72 273a 2046 616c 7365 2c20 2763  rror': False, 'c
-00002850: 6c6f 7365 644f 6e45 7272 6f72 273a 2046  losedOnError': F
-00002860: 616c 7365 2c20 2772 6561 6479 273a 2054  alse, 'ready': T
-00002870: 7275 652c 2027 6275 7379 273a 2046 616c  rue, 'busy': Fal
-00002880: 7365 7d0d 0a0d 0a0d 0a23 2049 6e73 7069  se}......# Inspi
-00002890: 7261 7469 6f6e 0d0a 0d0a 416e 206f 7468  ration....An oth
-000028a0: 6572 206c 6962 203a 200d 0a0d 0a68 7474  er lib : ....htt
-000028b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000028c0: 686f 6d65 2d61 7373 6973 7461 6e74 2d6c  home-assistant-l
-000028d0: 6962 732f 5072 7573 614c 696e 6b50 792f  ibs/PrusaLinkPy/
-000028e0: 626c 6f62 2f6d 6169 6e2f 5072 7573 614c  blob/main/PrusaL
-000028f0: 696e 6b50 792f 0d0a 0d0a 0d0a 4c65 7320  inkPy/......Les 
-00002900: 636f 6d6d 616e 6465 7320 6461 6e73 206c  commandes dans l
-00002910: 6120 6d69 6e69 203a 0d0a 6874 7470 733a  a mini :..https:
-00002920: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7275  //github.com/pru
-00002930: 7361 3364 2f50 7275 7361 2d46 6972 6d77  sa3d/Prusa-Firmw
-00002940: 6172 652d 4275 6464 792f 626c 6f62 2f6d  are-Buddy/blob/m
-00002950: 6173 7465 722f 6c69 622f 5755 492f 6c69  aster/lib/WUI/li
-00002960: 6e6b 5f63 6f6e 7465 6e74 2f62 6173 6963  nk_content/basic
-00002970: 5f67 6574 732e 6370 700d 0a0d 0a0d 0a0d  _gets.cpp.......
-00002980: 0a23 2043 6f6e 7374 7275 6972 6520 6c61  .# Construire la
-00002990: 206c 6962 0d0a 0d0a 2020 2020 7079 202d   lib....    py -
-000029a0: 6d20 6275 696c 640d 0a0d 0a54 6f20 7570  m build....To up
-000029b0: 6c6f 6164 2074 6f20 7465 7374 7069 2072  load to testpi r
-000029c0: 6570 6f20 3a0d 0a0d 0a20 2020 2070 7920  epo :....    py 
-000029d0: 2d6d 2074 7769 6e65 2075 706c 6f61 6420  -m twine upload 
-000029e0: 2d2d 7265 706f 7369 746f 7279 2074 6573  --repository tes
-000029f0: 7470 6920 6469 7374 2f2a 0d0a 0d0a 546f  tpi dist/*....To
-00002a00: 2075 706c 6f61 6420 746f 2070 7970 6920   upload to pypi 
-00002a10: 7265 706f 203a 0d0a 0d0a 2020 2020 7079  repo :....    py
-00002a20: 202d 6d20 7477 696e 6520 7570 6c6f 6164   -m twine upload
-00002a30: 2064 6973 742f 2a0d 0a0d 0a0d 0a68 7474   dist/*......htt
-00002a40: 7073 3a2f 2f6d 6564 6975 6d2e 636f 6d2f  ps://medium.com/
-00002a50: 616e 616c 7974 6963 732d 7669 6468 7961  analytics-vidhya
-00002a60: 2f68 6f77 2d74 6f2d 6372 6561 7465 2d61  /how-to-create-a
-00002a70: 2d70 7974 686f 6e2d 6c69 6272 6172 792d  -python-library-
-00002a80: 3764 3561 6561 3830 6363 3366 0d0a 0d0a  7d5aea80cc3f....
+00000460: 0a0d 0a23 2320 322e 3220 3a0d 0a0d 0a20  ...## 2.2 :.... 
+00000470: 2056 6572 7369 6f6e 206d 6164 6520 6279   Version made by
+00000480: 205b 656e 7267 6172 6369 5d28 6874 7470   [enrgarci](http
+00000490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+000004a0: 6e72 6761 7263 6929 0d0a 202d 2055 7064  nrgarci).. - Upd
+000004b0: 6174 6520 5245 4144 4d45 2e6d 640d 0a20  ate README.md.. 
+000004c0: 2d20 4d6f 6469 6669 6564 2064 656c 6574  - Modified delet
+000004d0: 655f 6a6f 6228 2920 746f 2066 6978 2072  e_job() to fix r
+000004e0: 6571 7565 7374 2066 726f 6d20 6765 7420  equest from get 
+000004f0: 746f 2064 656c 6574 650d 0a20 2d20 6164  to delete.. - ad
+00000500: 6465 6420 3a0d 0a0d 0a20 2a20 7061 7573  ded :.... * paus
+00000510: 655f 7072 696e 740d 0a20 2a20 7265 7375  e_print.. * resu
+00000520: 6d65 5f70 7269 6e74 0d0a 202a 2073 746f  me_print.. * sto
+00000530: 705f 7072 696e 740d 0a0d 0a23 2320 322e  p_print....## 2.
+00000540: 312e 3120 3a0d 0a0d 0a20 2d20 5570 6461  1.1 :.... - Upda
+00000550: 7465 2052 4541 444d 452e 6d64 0d0a 202d  te README.md.. -
+00000560: 2061 6464 6564 203a 0d0a 0d0a 202a 2067   added :.... * g
+00000570: 6574 5f74 7261 6e73 6665 720d 0a20 2a20  et_transfer.. * 
+00000580: 6765 745f 7365 7474 696e 6773 0d0a 200d  get_settings.. .
+00000590: 0a23 2320 322e 312e 3020 3a0d 0a0d 0a20  .## 2.1.0 :.... 
+000005a0: 2d20 5570 6461 7465 2052 4541 444d 452e  - Update README.
+000005b0: 6d64 0d0a 202d 2061 6464 6564 203a 0d0a  md.. - added :..
+000005c0: 0d0a 202a 2064 656c 6574 650d 0a20 2a20  .. * delete.. * 
+000005d0: 6765 745f 7374 6174 7573 0d0a 202a 2067  get_status.. * g
+000005e0: 6574 5f73 746f 7261 6765 0d0a 202a 2064  et_storage.. * d
+000005f0: 656c 6574 655f 6a6f 620d 0a20 0d0a 2323  elete_job.. ..##
+00000600: 2032 2e30 2e31 203a 0d0a 0d0a 202d 2042   2.0.1 :.... - B
+00000610: 7567 2063 6f72 7265 6374 696f 6e20 6f6e  ug correction on
+00000620: 2070 7574 5f67 636f 6465 0d0a 200d 0a23   put_gcode.. ..#
+00000630: 2320 322e 302e 3020 3a0d 0a0d 0a20 2d20  # 2.0.0 :.... - 
+00000640: 5375 7070 6f72 7420 6669 726d 7761 7265  Support firmware
+00000650: 2035 2e31 2e30 0d0a 202d 2041 6464 6564   5.1.0.. - Added
+00000660: 203a 200d 0a0d 0a20 2a20 6765 745f 6669   : .... * get_fi
+00000670: 6c65 730d 0a20 2a20 7075 745f 6763 6f64  les.. * put_gcod
+00000680: 650d 0a20 2a20 6578 6973 7473 5f67 636f  e.. * exists_gco
+00000690: 6465 0d0a 200d 0a23 2320 312e 302e 3020  de.. ..## 1.0.0 
+000006a0: 3a0d 0a0d 0a20 2d20 4669 7273 7420 5265  :.... - First Re
+000006b0: 6c65 6173 650d 0a0d 0a23 2049 6e73 7461  lease....# Insta
+000006c0: 6c6c 696e 6720 5072 7573 614c 696e 6b50  lling PrusaLinkP
+000006d0: 7920 616e 6420 5375 7070 6f72 7465 6420  y and Supported 
+000006e0: 5665 7273 696f 6e73 0d0a 0d0a 5072 7573  Versions....Prus
+000006f0: 614c 696e 6b50 7920 6973 2061 7661 696c  aLinkPy is avail
+00000700: 6162 6c65 206f 6e20 7069 7020 3a0d 0a0d  able on pip :...
+00000710: 0a20 2020 2070 7974 686f 6e20 2d6d 2070  .    python -m p
+00000720: 6970 2069 6e73 7461 6c6c 2050 7275 7361  ip install Prusa
+00000730: 4c69 6e6b 5079 0d0a 0d0a 5072 7573 614c  LinkPy....PrusaL
+00000740: 696e 6b50 7920 6f66 6669 6369 616c 6c79  inkPy officially
+00000750: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
+00000760: 2033 2e39 2b20 7769 7468 2050 7275 7361   3.9+ with Prusa
+00000770: 204d 494e 4920 7072 696e 7465 7220 6669   MINI printer fi
+00000780: 726d 7761 7265 2035 2e31 2e30 2e0d 0a0d  rmware 5.1.0....
+00000790: 0a0d 0a23 2041 5049 2052 6566 6572 656e  ...# API Referen
+000007a0: 6365 0d0a 0d0a 2323 204c 6f77 204c 6576  ce....## Low Lev
+000007b0: 656c 2046 756e 6374 696f 6e73 0d0a 0d0a  el Functions....
+000007c0: 5b67 6574 5f76 6572 7369 6f6e 2829 5d28  [get_version()](
+000007d0: 2370 7275 7361 6c69 6e6b 7079 6765 745f  #prusalinkpyget_
+000007e0: 7665 7273 696f 6e29 0d0a 0d0a 5b67 6574  version)....[get
+000007f0: 5f70 7269 6e74 6572 2829 5d28 2370 7275  _printer()](#pru
+00000800: 7361 6c69 6e6b 7079 6765 745f 7072 696e  salinkpyget_prin
+00000810: 7465 7229 0d0a 0d0a 5b67 6574 5f6a 6f62  ter)....[get_job
+00000820: 2829 5d28 2370 7275 7361 6c69 6e6b 7079  ()](#prusalinkpy
+00000830: 6765 745f 6a6f 6229 0d0a 0d0a 5b64 656c  get_job)....[del
+00000840: 6574 655f 6a6f 6228 295d 2823 7072 7573  ete_job()](#prus
+00000850: 616c 696e 6b70 7964 656c 6574 655f 6a6f  alinkpydelete_jo
+00000860: 6229 0d0a 0d0a 5b67 6574 5f73 7461 7475  b)....[get_statu
+00000870: 7328 295d 2823 7072 7573 616c 696e 6b70  s()](#prusalinkp
+00000880: 7967 6574 5f73 7461 7475 7329 0d0a 0d0a  yget_status)....
+00000890: 5b67 6574 5f73 746f 7261 6765 2829 5d28  [get_storage()](
+000008a0: 2370 7275 7361 6c69 6e6b 7079 6765 745f  #prusalinkpyget_
+000008b0: 7374 6f72 6167 6529 0d0a 0d0a 5b67 6574  storage)....[get
+000008c0: 5f66 696c 6573 2872 656d 6f74 6544 6972  _files(remoteDir
+000008d0: 295d 2823 7072 7573 616c 696e 6b70 7967  )](#prusalinkpyg
+000008e0: 6574 5f66 696c 6573 2d72 656d 6f74 6564  et_files-remoted
+000008f0: 6972 2d2d 290d 0a0d 0a5b 6465 6c65 7465  ir--)....[delete
+00000900: 2872 656d 6f74 6550 6174 6829 5d28 2370  (remotePath)](#p
+00000910: 7275 7361 6c69 6e6b 7079 6465 6c65 7465  rusalinkpydelete
+00000920: 7265 6d6f 7465 7061 7468 290d 0a0d 0a5b  remotepath)....[
+00000930: 706f 7374 5f67 636f 6465 2872 656d 6f74  post_gcode(remot
+00000940: 6550 6174 6829 5d28 2370 7275 7361 6c69  ePath)](#prusali
+00000950: 6e6b 7079 7075 745f 706f 7374 5f67 636f  nkpyput_post_gco
+00000960: 6465 290d 0a0d 0a5b 7075 745f 6763 6f64  de)....[put_gcod
+00000970: 6528 6669 6c65 5061 7468 4c6f 6361 6c2c  e(filePathLocal,
+00000980: 2072 656d 6f74 6544 6972 2c20 7072 696e   remoteDir, prin
+00000990: 7441 6674 6572 5570 6c6f 6164 203d 2046  tAfterUpload = F
+000009a0: 616c 7365 2c20 6f76 6572 7772 6974 6520  alse, overwrite 
+000009b0: 3d20 4661 6c73 6529 5d28 2370 7275 7361  = False)](#prusa
+000009c0: 6c69 6e6b 7079 7075 745f 6763 6f64 6572  linkpyput_gcoder
+000009d0: 656d 6f74 6570 6174 6829 0d0a 0d0a 5b65  emotepath)....[e
+000009e0: 7869 7374 735f 6763 6f64 6528 7265 6d6f  xists_gcode(remo
+000009f0: 7465 5061 7468 295d 2823 7072 7573 616c  tePath)](#prusal
+00000a00: 696e 6b70 7965 7869 7374 735f 6763 6f64  inkpyexists_gcod
+00000a10: 6572 656d 6f74 6570 6174 6829 0d0a 0d0a  eremotepath)....
+00000a20: 5b70 6175 7365 5f70 7269 6e74 2829 5d28  [pause_print()](
+00000a30: 2370 7275 7361 6c69 6e6b 7079 7061 7573  #prusalinkpypaus
+00000a40: 655f 7072 696e 7429 0d0a 0d0a 5b72 6573  e_print)....[res
+00000a50: 756d 655f 7072 696e 7428 295d 2823 7072  ume_print()](#pr
+00000a60: 7573 616c 696e 6b70 7972 6573 756d 655f  usalinkpyresume_
+00000a70: 7072 696e 7429 0d0a 0d0a 5b73 746f 705f  print)....[stop_
+00000a80: 7072 696e 7428 295d 2823 7072 7573 616c  print()](#prusal
+00000a90: 696e 6b70 7973 746f 705f 7072 696e 7429  inkpystop_print)
+00000aa0: 0d0a 0d0a 2323 2048 6967 6820 4c65 7665  ....## High Leve
+00000ab0: 6c20 4675 6e63 7469 6f6e 7320 0d0a 0d0a  l Functions ....
+00000ac0: 5b67 6574 5f72 6563 7572 7369 7665 5f66  [get_recursive_f
+00000ad0: 696c 6573 2872 656d 6f74 6544 6972 295d  iles(remoteDir)]
+00000ae0: 2823 7072 7573 616c 696e 6b70 7967 6574  (#prusalinkpyget
+00000af0: 5f72 6563 7572 7369 7665 5f66 696c 6573  _recursive_files
+00000b00: 2d72 656d 6f74 6564 6972 2d2d 290d 0a0d  -remotedir--)...
+00000b10: 0a0d 0a23 2055 7365 7220 4775 6964 650d  ...# User Guide.
+00000b20: 0a0d 0a23 2320 5072 7573 614c 696e 6b50  ...## PrusaLinkP
+00000b30: 792e 6765 745f 7665 7273 696f 6e28 290d  y.get_version().
+00000b40: 0a0d 0a52 6561 6420 7665 7273 696f 6e20  ...Read version 
+00000b50: 3a0d 0a0d 0a0d 0a20 2020 2069 6d70 6f72  :......    impor
+00000b60: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
+00000b70: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
+00000b80: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
+00000b90: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
+00000ba0: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
+00000bb0: 4e75 4148 4132 624d 222c 2070 6f72 743d  NuAHA2bM", port=
+00000bc0: 3830 3137 290d 0a20 2020 206f 626a 203d  8017)..    obj =
+00000bd0: 2070 7275 7361 4d69 6e69 2e67 6574 5f76   prusaMini.get_v
+00000be0: 6572 7369 6f6e 2829 0d0a 2020 2020 6f62  ersion()..    ob
+00000bf0: 6a2e 6a73 6f6e 2829 0d0a 2020 2020 0d0a  j.json()..    ..
+00000c00: 5265 7475 726e 2073 6f6d 6574 6869 6e67  Return something
+00000c10: 206c 696b 6520 3a0d 0a0d 0a20 2020 207b   like :....    {
+00000c20: 0d0a 2020 2020 2020 2020 2761 7069 273a  ..        'api':
+00000c30: 2027 322e 302e 3027 2c20 0d0a 2020 2020   '2.0.0', ..    
+00000c40: 2020 2020 2773 6572 7665 7227 3a20 2732      'server': '2
+00000c50: 2e31 2e32 272c 200d 0a20 2020 2020 2020  .1.2', ..       
+00000c60: 2027 6e6f 7a7a 6c65 5f64 6961 6d65 7465   'nozzle_diamete
+00000c70: 7227 3a20 302e 342c 200d 0a20 2020 2020  r': 0.4, ..     
+00000c80: 2020 2027 7465 7874 273a 2027 5072 7573     'text': 'Prus
+00000c90: 614c 696e 6b27 2c20 0d0a 2020 2020 2020  aLink', ..      
+00000ca0: 2020 2768 6f73 746e 616d 6527 3a20 2727    'hostname': ''
+00000cb0: 2c20 0d0a 2020 2020 2020 2020 2763 6170  , ..        'cap
+00000cc0: 6162 696c 6974 6965 7327 3a20 0d0a 2020  abilities': ..  
+00000cd0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00000ce0: 2020 2020 2027 7570 6c6f 6164 2d62 792d       'upload-by-
+00000cf0: 7075 7427 3a20 5472 7565 0d0a 2020 2020  put': True..    
+00000d00: 2020 2020 7d0d 0a20 2020 207d 0d0a 0d0a      }..    }....
+00000d10: 0d0a 2323 2050 7275 7361 4c69 6e6b 5079  ..## PrusaLinkPy
+00000d20: 2e67 6574 5f70 7269 6e74 6572 2829 0d0a  .get_printer()..
+00000d30: 0d0a 4765 7420 7072 696e 7465 7220 3a0d  ..Get printer :.
+00000d40: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
+00000d50: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
+00000d60: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
+00000d70: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
+00000d80: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
+00000d90: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
+00000da0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
+00000db0: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
+00000dc0: 7072 696e 7465 7228 290d 0a20 2020 206f  printer()..    o
+00000dd0: 626a 2e6a 736f 6e28 290d 0a20 2020 200d  bj.json()..    .
+00000de0: 0a57 6169 7469 6e67 2066 6f72 2043 6861  .Waiting for Cha
+00000df0: 6e67 696e 6720 4669 6c61 6d65 6e74 203a  nging Filament :
+00000e00: 0d0a 0d0a 2020 2020 276c 696e 6b5f 7374  ....    'link_st
+00000e10: 6174 6527 3a20 2741 5454 454e 5449 4f4e  ate': 'ATTENTION
+00000e20: 2720 0d0a 2020 2020 2765 7272 6f72 273a  ' ..    'error':
+00000e30: 2054 7275 650d 0a20 2020 200d 0a52 6574   True..    ..Ret
+00000e40: 7572 6e20 736f 6d65 7468 696e 6720 6c69  urn something li
+00000e50: 6b65 203a 0d0a 0d0a 2020 2020 7b0d 0a20  ke :....    {.. 
+00000e60: 2020 2020 2020 2027 7465 6c65 6d65 7472         'telemetr
+00000e70: 7927 3a20 0d0a 2020 2020 2020 2020 7b0d  y': ..        {.
+00000e80: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
+00000e90: 6d70 2d62 6564 273a 2031 362e 332c 0d0a  mp-bed': 16.3,..
+00000ea0: 2020 2020 2020 2020 2020 2020 2774 656d              'tem
+00000eb0: 702d 6e6f 7a7a 6c65 273a 2031 362e 372c  p-nozzle': 16.7,
+00000ec0: 0d0a 2020 2020 2020 2020 2020 2020 2770  ..            'p
+00000ed0: 7269 6e74 2d73 7065 6564 273a 2031 3030  rint-speed': 100
+00000ee0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00000ef0: 7a2d 6865 6967 6874 273a 2038 322e 302c  z-height': 82.0,
+00000f00: 0d0a 2020 2020 2020 2020 2020 2020 276d  ..            'm
+00000f10: 6174 6572 6961 6c27 3a20 2750 4c41 270d  aterial': 'PLA'.
+00000f20: 0a20 2020 2020 2020 207d 2c20 0d0a 2020  .        }, ..  
+00000f30: 2020 2020 2020 2774 656d 7065 7261 7475        'temperatu
+00000f40: 7265 273a 200d 0a20 2020 2020 2020 207b  re': ..        {
+00000f50: 0d0a 2020 2020 2020 2020 2020 2020 2774  ..            't
+00000f60: 6f6f 6c30 273a 200d 0a20 2020 2020 2020  ool0': ..       
+00000f70: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00000f80: 2020 2020 2020 2020 2761 6374 7561 6c27          'actual'
+00000f90: 3a20 3136 2e37 2c0d 0a20 2020 2020 2020  : 16.7,..       
+00000fa0: 2020 2020 2020 2020 2027 7461 7267 6574           'target
+00000fb0: 273a 2030 2e30 2c0d 0a20 2020 2020 2020  ': 0.0,..       
+00000fc0: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
+00000fd0: 7927 3a20 302e 302c 0d0a 2020 2020 2020  y': 0.0,..      
+00000fe0: 2020 2020 2020 2020 2020 276f 6666 7365            'offse
+00000ff0: 7427 3a20 300d 0a20 2020 2020 2020 2020  t': 0..         
+00001000: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
+00001010: 2020 2027 6265 6427 3a20 0d0a 2020 2020     'bed': ..    
+00001020: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00001030: 2020 2020 2020 2020 2020 2027 6163 7475             'actu
+00001040: 616c 273a 3136 2e33 2c0d 0a20 2020 2020  al':16.3,..     
+00001050: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
+00001060: 6574 273a 2030 2e30 2c0d 0a20 2020 2020  et': 0.0,..     
+00001070: 2020 2020 2020 2020 2020 2027 6f66 6673             'offs
+00001080: 6574 273a 2030 0d0a 2020 2020 2020 2020  et': 0..        
+00001090: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
+000010a0: 2c0d 0a20 2020 2020 2020 2027 7374 6174  ,..        'stat
+000010b0: 6527 3a20 0d0a 2020 2020 2020 2020 7b0d  e': ..        {.
+000010c0: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
+000010d0: 7874 273a 2027 4f70 6572 6174 696f 6e61  xt': 'Operationa
+000010e0: 6c27 2c0d 0a20 2020 2020 2020 2020 2020  l',..           
+000010f0: 2027 666c 6167 7327 3a20 0d0a 2020 2020   'flags': ..    
+00001100: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00001110: 2020 2020 2020 2020 2020 2027 6f70 6572             'oper
+00001120: 6174 696f 6e61 6c27 3a20 5472 7565 2c0d  ational': True,.
+00001130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001140: 2027 7061 7573 6564 273a 2046 616c 7365   'paused': False
+00001150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001160: 2020 2027 7072 696e 7469 6e67 273a 2046     'printing': F
+00001170: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00001180: 2020 2020 2020 2027 6361 6e63 656c 6c69         'cancelli
+00001190: 6e67 273a 2046 616c 7365 2c0d 0a20 2020  ng': False,..   
+000011a0: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+000011b0: 7573 696e 6727 3a20 4661 6c73 652c 0d0a  using': False,..
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2765 7272 6f72 273a 2046 616c 7365 2c0d  'error': False,.
+000011e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011f0: 2027 7364 5265 6164 7927 3a20 4661 6c73   'sdReady': Fals
+00001200: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00001210: 2020 2020 2763 6c6f 7365 644f 6e45 7272      'closedOnErr
+00001220: 6f72 273a 2046 616c 7365 2c0d 0a20 2020  or': False,..   
+00001230: 2020 2020 2020 2020 2020 2020 2027 7265               're
+00001240: 6164 7927 3a20 5472 7565 2c0d 0a20 2020  ady': True,..   
+00001250: 2020 2020 2020 2020 2020 2020 2027 6275               'bu
+00001260: 7379 273a 2046 616c 7365 0d0a 2020 2020  sy': False..    
+00001270: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+00001280: 2020 207d 0d0a 2020 2020 7d0d 0a0d 0a23     }..    }....#
+00001290: 2320 5072 7573 614c 696e 6b50 792e 6765  # PrusaLinkPy.ge
+000012a0: 745f 6a6f 6228 290d 0a0d 0a47 6574 206a  t_job()....Get j
+000012b0: 6f62 203a 0d0a 0d0a 2020 2020 696d 706f  ob :....    impo
+000012c0: 7274 2050 7275 7361 4c69 6e6b 5079 0d0a  rt PrusaLinkPy..
+000012d0: 2020 2020 7072 7573 614d 696e 6920 3d20      prusaMini = 
+000012e0: 5072 7573 614c 696e 6b50 792e 5072 7573  PrusaLinkPy.Prus
+000012f0: 614c 696e 6b50 7928 2231 3932 2e31 3638  aLinkPy("192.168
+00001300: 2e30 2e31 3233 222c 2022 386f 6a48 4b48  .0.123", "8ojHKH
+00001310: 474e 7541 4841 3262 4d22 290d 0a20 2020  GNuAHA2bM")..   
+00001320: 206f 626a 203d 2070 7275 7361 4d69 6e69   obj = prusaMini
+00001330: 2e67 6574 5f6a 6f62 2829 0d0a 2020 2020  .get_job()..    
+00001340: 6f62 6a2e 6a73 6f6e 2829 0d0a 2020 2020  obj.json()..    
+00001350: 0d0a 5265 7475 726e 2073 6f6d 6574 6869  ..Return somethi
+00001360: 6e67 206c 696b 6520 3a0d 0a0d 0a20 2020  ng like :....   
+00001370: 207b 0d0a 2020 2020 2020 2020 2273 7461   {..        "sta
+00001380: 7465 223a 224f 7065 7261 7469 6f6e 616c  te":"Operational
+00001390: 222c 0d0a 2020 2020 2020 2020 226a 6f62  ",..        "job
+000013a0: 223a 204e 6f6e 652c 0d0a 2020 2020 2020  ": None,..      
+000013b0: 2020 2270 726f 6772 6573 7322 3a20 4e6f    "progress": No
+000013c0: 6e65 0d0a 2020 2020 7d0d 0a20 2020 200d  ne..    }..    .
+000013d0: 0a23 2320 5072 7573 614c 696e 6b50 792e  .## PrusaLinkPy.
+000013e0: 6465 6c65 7465 5f6a 6f62 286a 6f62 290d  delete_job(job).
+000013f0: 0a0d 0a44 656c 6574 6520 6120 6a6f 622e  ...Delete a job.
+00001400: 204a 6f62 206e 756d 6265 7220 6973 2061   Job number is a
+00001410: 7661 696c 6162 6c65 2077 6974 6820 6765  vailable with ge
+00001420: 745f 6a6f 6228 2920 6f72 2067 6574 5f73  t_job() or get_s
+00001430: 7461 7475 7328 290d 0a0d 0a20 2020 2069  tatus()....    i
+00001440: 6d70 6f72 7420 5072 7573 614c 696e 6b50  mport PrusaLinkP
+00001450: 790d 0a20 2020 2070 7275 7361 4d69 6e69  y..    prusaMini
+00001460: 203d 2050 7275 7361 4c69 6e6b 5079 2e50   = PrusaLinkPy.P
+00001470: 7275 7361 4c69 6e6b 5079 2822 3139 322e  rusaLinkPy("192.
+00001480: 3136 382e 302e 3132 3322 2c20 2238 6f6a  168.0.123", "8oj
+00001490: 484b 4847 4e75 4148 4132 624d 2229 0d0a  HKHGNuAHA2bM")..
+000014a0: 2020 2020 6f62 6a20 3d20 7072 7573 614d      obj = prusaM
+000014b0: 696e 692e 6465 6c65 7465 5f6a 6f62 2822  ini.delete_job("
+000014c0: 3433 2229 0d0a 2020 2020 0d0a 0d0a 2323  43")..    ....##
+000014d0: 2050 7275 7361 4c69 6e6b 5079 2e67 6574   PrusaLinkPy.get
+000014e0: 5f73 7461 7475 7328 290d 0a0d 0a47 6574  _status()....Get
+000014f0: 206a 6f62 203a 0d0a 0d0a 2020 2020 696d   job :....    im
+00001500: 706f 7274 2050 7275 7361 4c69 6e6b 5079  port PrusaLinkPy
+00001510: 0d0a 2020 2020 7072 7573 614d 696e 6920  ..    prusaMini 
+00001520: 3d20 5072 7573 614c 696e 6b50 792e 5072  = PrusaLinkPy.Pr
+00001530: 7573 614c 696e 6b50 7928 2231 3932 2e31  usaLinkPy("192.1
+00001540: 3638 2e30 2e31 3233 222c 2022 386f 6a48  68.0.123", "8ojH
+00001550: 4b48 474e 7541 4841 3262 4d22 290d 0a20  KHGNuAHA2bM").. 
+00001560: 2020 206f 626a 203d 2070 7275 7361 4d69     obj = prusaMi
+00001570: 6e69 2e67 6574 5f73 7461 7475 7328 290d  ni.get_status().
+00001580: 0a20 2020 206f 626a 2e6a 736f 6e28 290d  .    obj.json().
+00001590: 0a20 2020 200d 0a56 616c 7565 206f 6620  .    ..Value of 
+000015a0: 7072 696e 7465 722d 3e73 7461 7465 203a  printer->state :
+000015b0: 0d0a 0d0a 2020 2020 4944 4c45 2028 4d61  ....    IDLE (Ma
+000015c0: 696e 2053 6372 6565 6e29 0d0a 2020 2020  in Screen)..    
+000015d0: 5052 494e 5449 4e47 0d0a 2020 2020 4649  PRINTING..    FI
+000015e0: 4e49 5348 4544 2028 5072 696e 7420 6669  NISHED (Print fi
+000015f0: 6e69 7368 2c20 7363 7265 656e 206e 6f74  nish, screen not
+00001600: 206f 6e20 6d61 696e 2073 6372 6565 6e29   on main screen)
+00001610: 0d0a 2020 2020 5041 5553 4544 2028 5061  ..    PAUSED (Pa
+00001620: 7573 6520 6279 2075 7365 722c 2050 7269  use by user, Pri
+00001630: 6e74 2066 616e 2065 7272 6f72 290d 0a20  nt fan error).. 
+00001640: 2020 2053 544f 5050 4544 2028 5072 696e     STOPPED (Prin
+00001650: 7420 6669 6e69 7368 2c20 7374 6f70 7065  t finish, stoppe
+00001660: 6420 6279 2075 7365 7229 0d0a 2020 2020  d by user)..    
+00001670: 4154 5445 4e54 494f 4e20 2846 696c 616d  ATTENTION (Filam
+00001680: 656e 7420 4368 616e 6765 290d 0a20 2020  ent Change)..   
+00001690: 200d 0a52 6574 7572 6e20 736f 6d65 7468   ..Return someth
+000016a0: 696e 6720 6c69 6b65 203a 0d0a 0d0a 2020  ing like :....  
+000016b0: 2020 7b0d 0a20 2020 2020 2020 2022 6a6f    {..        "jo
+000016c0: 6222 3a0d 0a20 2020 2020 2020 207b 0d0a  b":..        {..
+000016d0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+000016e0: 3a34 332c 0d0a 2020 2020 2020 2020 2020  :43,..          
+000016f0: 2020 2270 726f 6772 6573 7322 3a30 2e30    "progress":0.0
+00001700: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00001710: 2274 696d 655f 7265 6d61 696e 696e 6722  "time_remaining"
+00001720: 3a31 3230 2c0d 0a20 2020 2020 2020 2020  :120,..         
+00001730: 2020 2022 7469 6d65 5f70 7269 6e74 696e     "time_printin
+00001740: 6722 3a31 3433 0d0a 2020 2020 2020 2020  g":143..        
+00001750: 7d2c 0d0a 2020 2020 2020 2020 2273 746f  },..        "sto
+00001760: 7261 6765 223a 0d0a 2020 2020 2020 2020  rage":..        
+00001770: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
+00001780: 7061 7468 223a 222f 7573 622f 222c 0d0a  path":"/usb/",..
+00001790: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+000017a0: 6522 3a22 7573 6222 2c0d 0a20 2020 2020  e":"usb",..     
+000017b0: 2020 2020 2020 2022 7265 6164 5f6f 6e6c         "read_onl
+000017c0: 7922 3a66 616c 7365 0d0a 2020 2020 2020  y":false..      
+000017d0: 2020 7d2c 0d0a 2020 2020 2020 2020 2270    },..        "p
+000017e0: 7269 6e74 6572 223a 0d0a 2020 2020 2020  rinter":..      
+000017f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00001800: 2022 7374 6174 6522 3a22 5052 494e 5449   "state":"PRINTI
+00001810: 4e47 222c 0d0a 2020 2020 2020 2020 2020  NG",..          
+00001820: 2020 2274 656d 705f 6265 6422 3a35 372e    "temp_bed":57.
+00001830: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
+00001840: 2274 6172 6765 745f 6265 6422 3a30 2e30  "target_bed":0.0
+00001850: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001860: 7465 6d70 5f6e 6f7a 7a6c 6522 3a32 342e  temp_nozzle":24.
+00001870: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
+00001880: 2274 6172 6765 745f 6e6f 7a7a 6c65 223a  "target_nozzle":
+00001890: 302e 302c 0d0a 2020 2020 2020 2020 2020  0.0,..          
+000018a0: 2020 2261 7869 735f 7a22 3a31 3632 2e32    "axis_z":162.2
+000018b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000018c0: 666c 6f77 223a 3130 302c 0d0a 2020 2020  flow":100,..    
+000018d0: 2020 2020 2020 2020 2273 7065 6564 223a          "speed":
+000018e0: 3130 302c 0d0a 2020 2020 2020 2020 2020  100,..          
+000018f0: 2020 2266 616e 5f68 6f74 656e 6422 3a30    "fan_hotend":0
+00001900: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001910: 6661 6e5f 7072 696e 7422 3a30 0d0a 2020  fan_print":0..  
+00001920: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
+00001930: 2020 2020 0d0a 2323 2050 7275 7361 4c69      ..## PrusaLi
+00001940: 6e6b 5079 2e67 6574 5f73 746f 7261 6765  nkPy.get_storage
+00001950: 2829 0d0a 0d0a 4765 7420 6a6f 6220 3a0d  ()....Get job :.
+00001960: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
+00001970: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
+00001980: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
+00001990: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
+000019a0: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
+000019b0: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
+000019c0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
+000019d0: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
+000019e0: 7374 6f72 6167 6528 290d 0a20 2020 206f  storage()..    o
+000019f0: 626a 2e6a 736f 6e28 290d 0a20 2020 200d  bj.json()..    .
+00001a00: 0a52 6574 7572 6e20 736f 6d65 7468 696e  .Return somethin
+00001a10: 6720 6c69 6b65 203a 0d0a 0d0a 2020 2020  g like :....    
+00001a20: 7b0d 0a20 2020 2020 2020 2027 7374 6f72  {..        'stor
+00001a30: 6167 655f 6c69 7374 273a 200d 0a20 2020  age_list': ..   
+00001a40: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
+00001a50: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+00001a60: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
+00001a70: 2f75 7362 2f27 2c20 0d0a 2020 2020 2020  /usb/', ..      
+00001a80: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+00001a90: 3a20 2775 7362 272c 0d0a 2020 2020 2020  : 'usb',..      
+00001aa0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+00001ab0: 3a20 2755 5342 272c 200d 0a20 2020 2020  : 'USB', ..     
+00001ac0: 2020 2020 2020 2020 2020 2027 7265 6164             'read
+00001ad0: 5f6f 6e6c 7927 3a20 4661 6c73 652c 200d  _only': False, .
+00001ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001af0: 2027 6176 6169 6c61 626c 6527 3a20 5472   'available': Tr
+00001b00: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00001b10: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
+00001b20: 2020 7d0d 0a20 2020 200d 0a23 2320 5072    }..    ..## Pr
+00001b30: 7573 614c 696e 6b50 792e 6765 745f 7472  usaLinkPy.get_tr
+00001b40: 616e 7366 6572 2829 0d0a 0d0a 4e6f 7420  ansfer()....Not 
+00001b50: 5465 7374 6564 0d0a 0d0a 4765 7420 6a6f  Tested....Get jo
+00001b60: 6220 3a0d 0a0d 0a20 2020 2069 6d70 6f72  b :....    impor
+00001b70: 7420 5072 7573 614c 696e 6b50 790d 0a20  t PrusaLinkPy.. 
+00001b80: 2020 2070 7275 7361 4d69 6e69 203d 2050     prusaMini = P
+00001b90: 7275 7361 4c69 6e6b 5079 2e50 7275 7361  rusaLinkPy.Prusa
+00001ba0: 4c69 6e6b 5079 2822 3139 322e 3136 382e  LinkPy("192.168.
+00001bb0: 302e 3132 3322 2c20 2238 6f6a 484b 4847  0.123", "8ojHKHG
+00001bc0: 4e75 4148 4132 624d 2229 0d0a 2020 2020  NuAHA2bM")..    
+00001bd0: 6f62 6a20 3d20 7072 7573 614d 696e 692e  obj = prusaMini.
+00001be0: 6765 745f 7472 616e 7366 6572 2829 0d0a  get_transfer()..
+00001bf0: 2020 2020 6f62 6a2e 7465 7874 0d0a 2020      obj.text..  
+00001c00: 2020 0d0a 5265 7475 726e 2073 6f6d 6574    ..Return somet
+00001c10: 6869 6e67 206c 696b 6520 3a0d 0a0d 0a20  hing like :.... 
+00001c20: 2020 2054 4f44 4f0d 0a20 2020 200d 0a23     TODO..    ..#
+00001c30: 2320 5072 7573 614c 696e 6b50 792e 6765  # PrusaLinkPy.ge
+00001c40: 745f 7365 7474 696e 6773 2829 0d0a 0d0a  t_settings()....
+00001c50: 436f 6d70 6c65 7465 6c79 2075 7365 6c65  Completely usele
+00001c60: 7373 0d0a 0d0a 5365 6520 6865 7265 203a  ss....See here :
+00001c70: 0d0a 0d0a 6874 7470 733a 2f2f 6769 7468  ....https://gith
+00001c80: 7562 2e63 6f6d 2f70 7275 7361 3364 2f50  ub.com/prusa3d/P
+00001c90: 7275 7361 2d46 6972 6d77 6172 652d 4275  rusa-Firmware-Bu
+00001ca0: 6464 792f 626c 6f62 2f34 6265 6139 3233  ddy/blob/4bea923
+00001cb0: 3831 3033 3032 6436 3534 6239 3332 3239  810302d654b93229
+00001cc0: 3162 6133 3234 6561 6564 6666 3037 3266  1ba324eaedff072f
+00001cd0: 632f 6c69 622f 5755 492f 6c69 6e6b 5f63  c/lib/WUI/link_c
+00001ce0: 6f6e 7465 6e74 2f70 7275 7361 5f6c 696e  ontent/prusa_lin
+00001cf0: 6b5f 6170 692e 6370 7023 4c31 3831 4331  k_api.cpp#L181C1
+00001d00: 362d 4c31 3831 4331 360d 0a0d 0a43 6f6d  6-L181C16....Com
+00001d10: 6d65 6e74 2066 726f 6d20 5072 7573 6120  ment from Prusa 
+00001d20: 4465 7665 6c6f 7070 6572 203a 0d0a 0d0a  Developper :....
+00001d30: 2020 2020 202f 2f20 536f 6d65 2073 7475       // Some stu
+00001d40: 6273 2066 6f72 206e 6f77 2c20 746f 206d  bs for now, to m
+00001d50: 616b 6520 6d6f 7265 2063 6c69 656e 7473  ake more clients
+00001d60: 2028 696e 636c 7564 696e 6720 7468 6520   (including the 
+00001d70: 7765 6220 7061 6765 2920 6861 7070 6965  web page) happie
+00001d80: 722e 0d0a 0d0a 4765 7420 6a6f 6220 3a0d  r.....Get job :.
+00001d90: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
+00001da0: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
+00001db0: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
+00001dc0: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
+00001dd0: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
+00001de0: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
+00001df0: 4132 624d 2229 0d0a 2020 2020 6f62 6a20  A2bM")..    obj 
+00001e00: 3d20 7072 7573 614d 696e 692e 6765 745f  = prusaMini.get_
+00001e10: 7472 616e 7366 6572 2829 0d0a 2020 2020  transfer()..    
+00001e20: 6f62 6a2e 7465 7874 0d0a 2020 2020 0d0a  obj.text..    ..
+00001e30: 5265 7475 726e 2073 6f6d 6574 6869 6e67  Return something
+00001e40: 206c 696b 6520 3a0d 0a0d 0a20 2020 207b   like :....    {
+00001e50: 2270 7269 6e74 6572 223a 207b 7d7d 0d0a  "printer": {}}..
+00001e60: 2020 2020 0d0a 2323 2050 7275 7361 4c69      ..## PrusaLi
+00001e70: 6e6b 5079 2e67 6574 5f66 696c 6573 2820  nkPy.get_files( 
+00001e80: 7265 6d6f 7465 4469 7220 3d20 272f 2729  remoteDir = '/')
+00001e90: 0d0a 0d0a 4765 7420 4669 6c65 7320 6f6e  ....Get Files on
+00001ea0: 2055 5342 2044 7269 7665 203a 0d0a 0d0a   USB Drive :....
+00001eb0: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
+00001ec0: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
+00001ed0: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
+00001ee0: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
+00001ef0: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
+00001f00: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
+00001f10: 4d22 290d 0a20 2020 206f 626a 203d 2070  M")..    obj = p
+00001f20: 7275 7361 4d69 6e69 2e67 6574 5f66 696c  rusaMini.get_fil
+00001f30: 6573 2829 0d0a 2020 2020 6669 6c65 7352  es()..    filesR
+00001f40: 6574 203d 206f 626a 2e6a 736f 6e28 290d  et = obj.json().
+00001f50: 0a20 2020 200d 0a52 6574 7572 6e20 736f  .    ..Return so
+00001f60: 6d65 7468 696e 6720 6c69 6b65 203a 0d0a  mething like :..
+00001f70: 0d0a 2020 2020 7b0d 0a20 2020 2020 2020  ..    {..       
+00001f80: 2027 7479 7065 273a 2027 464f 4c44 4552   'type': 'FOLDER
+00001f90: 272c 200d 0a20 2020 2020 2020 2027 726f  ', ..        'ro
+00001fa0: 273a 2046 616c 7365 2c20 0d0a 2020 2020  ': False, ..    
+00001fb0: 2020 2020 276e 616d 6527 3a20 2775 7362      'name': 'usb
+00001fc0: 272c 200d 0a20 2020 2020 2020 2027 6368  ', ..        'ch
+00001fd0: 696c 6472 656e 273a 200d 0a20 2020 2020  ildren': ..     
+00001fe0: 2020 205b 0d0a 2020 2020 2020 2020 7b0d     [..        {.
+00001ff0: 0a20 2020 2020 2020 2020 2020 2027 6e61  .            'na
+00002000: 6d65 273a 2027 4d54 4e27 2c20 0d0a 2020  me': 'MTN', ..  
+00002010: 2020 2020 2020 2020 2020 2772 6f27 3a20            'ro': 
+00002020: 4661 6c73 652c 200d 0a20 2020 2020 2020  False, ..       
+00002030: 2020 2020 2027 7479 7065 273a 2027 464f       'type': 'FO
+00002040: 4c44 4552 272c 200d 0a20 2020 2020 2020  LDER', ..       
+00002050: 2020 2020 2027 6d5f 7469 6d65 7374 616d       'm_timestam
+00002060: 7027 3a20 3137 3032 3632 3839 3435 2c20  p': 1702628945, 
+00002070: 0d0a 2020 2020 2020 2020 2020 2020 2764  ..            'd
+00002080: 6973 706c 6179 5f6e 616d 6527 3a20 274d  isplay_name': 'M
+00002090: 544e 270d 0a20 2020 2020 2020 207d 2c0d  TN'..        },.
+000020a0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
+000020b0: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
+000020c0: 2753 325f 5632 4953 272c 200d 0a20 2020  'S2_V2IS', ..   
+000020d0: 2020 2020 2020 2020 2027 726f 273a 2046           'ro': F
+000020e0: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
+000020f0: 2020 2020 2774 7970 6527 3a20 2746 4f4c      'type': 'FOL
+00002100: 4445 5227 2c20 0d0a 2020 2020 2020 2020  DER', ..        
+00002110: 2020 2020 276d 5f74 696d 6573 7461 6d70      'm_timestamp
+00002120: 273a 2031 3730 3235 3635 3138 322c 200d  ': 1702565182, .
+00002130: 0a20 2020 2020 2020 2020 2020 2027 6469  .            'di
+00002140: 7370 6c61 795f 6e61 6d65 273a 2027 5332  splay_name': 'S2
+00002150: 5f56 3249 5327 0d0a 2020 2020 2020 2020  _V2IS'..        
+00002160: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
+00002170: 2020 7d0d 0a20 2020 200d 0a57 6f72 6b61    }..    ..Worka
+00002180: 6c73 6f20 7769 7468 2073 7562 666f 6c64  lso with subfold
+00002190: 6572 0d0a 0d0a 2020 2020 6f62 6a20 3d20  er....    obj = 
+000021a0: 7072 7573 614d 696e 692e 6765 745f 6669  prusaMini.get_fi
+000021b0: 6c65 7328 7265 6d6f 7465 4469 7220 3d20  les(remoteDir = 
+000021c0: 272f 5355 4246 4f4c 4445 5227 290d 0a0d  '/SUBFOLDER')...
+000021d0: 0a23 2320 5072 7573 614c 696e 6b50 792e  .## PrusaLinkPy.
+000021e0: 6765 745f 7265 6375 7273 6976 655f 6669  get_recursive_fi
+000021f0: 6c65 7328 2072 656d 6f74 6544 6972 203d  les( remoteDir =
+00002200: 2027 2f27 290d 0a0d 0a47 6574 2061 6c6c   '/')....Get all
+00002210: 2066 696c 6573 2028 6f6e 6c79 2067 636f   files (only gco
+00002220: 6465 2061 6e64 2062 6763 6f64 6529 2069  de and bgcode) i
+00002230: 6e20 6120 666f 6c64 6572 2061 6e64 2073  n a folder and s
+00002240: 7562 666f 6c64 6572 2e0d 0a0d 0a57 6172  ubfolder.....War
+00002250: 6e69 6e67 203a 2072 6574 7572 6e20 6e65  ning : return ne
+00002260: 7374 6564 2064 6963 742e 0d0a 0d0a 0d0a  sted dict.......
+00002270: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
+00002280: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
+00002290: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
+000022a0: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
+000022b0: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
+000022c0: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
+000022d0: 4d22 290d 0a20 2020 2064 6963 7474 203d  M")..    dictt =
+000022e0: 2070 7275 7361 4d69 6e69 2e67 6574 5f72   prusaMini.get_r
+000022f0: 6563 7572 7369 7665 5f66 696c 6573 2829  ecursive_files()
+00002300: 0d0a 2020 2020 0d0a 2020 2020 7b0d 0a20  ..    ..    {.. 
+00002310: 2020 2020 2020 2027 4d54 4e27 3a20 0d0a         'MTN': ..
+00002320: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00002330: 2020 2020 2020 2027 4348 4754 5f42 5553         'CHGT_BUS
+00002340: 452e 6763 6f64 6527 3a20 272f 4d54 4e2f  E.gcode': '/MTN/
+00002350: 4348 4754 5f42 7e31 2e47 434f 272c 200d  CHGT_B~1.GCO', .
+00002360: 0a20 2020 2020 2020 2020 2020 2027 4445  .            'DE
+00002370: 424f 5543 4841 4745 2e67 636f 6465 273a  BOUCHAGE.gcode':
+00002380: 2027 2f4d 544e 2f44 4542 4f55 437e 312e   '/MTN/DEBOUC~1.
+00002390: 4743 4f27 2c20 0d0a 2020 2020 2020 2020  GCO', ..        
+000023a0: 2020 2020 2750 5245 4348 4155 4646 452e      'PRECHAUFFE.
+000023b0: 6763 6f64 6527 3a20 272f 4d54 4e2f 5052  gcode': '/MTN/PR
+000023c0: 4543 4841 7e31 2e47 434f 270d 0a20 2020  ECHA~1.GCO'..   
+000023d0: 2020 2020 207d 2c20 0d0a 2020 2020 2020       }, ..      
+000023e0: 2020 2753 325f 5632 4953 273a 200d 0a20    'S2_V2IS': .. 
+000023f0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00002400: 2020 2020 2020 2732 6833 336d 2e62 6763        '2h33m.bgc
+00002410: 6f64 6527 3a20 272f 5332 5f56 3249 532f  ode': '/S2_V2IS/
+00002420: 3248 3333 4d7e 312e 4247 4327 2c0d 0a20  2H33M~1.BGC',.. 
+00002430: 2020 2020 2020 2020 2020 2027 3568 356d             '5h5m
+00002440: 2e62 6763 6f64 6527 3a20 272f 5332 5f56  .bgcode': '/S2_V
+00002450: 3249 532f 3548 354d 7e31 2e42 4743 270d  2IS/5H5M~1.BGC'.
+00002460: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
+00002470: 7d0d 0a0d 0a23 2320 5072 7573 614c 696e  }....## PrusaLin
+00002480: 6b50 792e 6465 6c65 7465 2872 656d 6f74  kPy.delete(remot
+00002490: 6550 6174 6829 200d 0a0d 0a44 656c 6574  ePath) ....Delet
+000024a0: 6520 6120 6669 6c65 206f 7220 6120 666f  e a file or a fo
+000024b0: 6c64 6572 206f 6e20 5553 4220 6472 6976  lder on USB driv
+000024c0: 650d 0a0d 0a20 2020 2069 6d70 6f72 7420  e....    import 
+000024d0: 5072 7573 614c 696e 6b50 790d 0a20 2020  PrusaLinkPy..   
+000024e0: 2070 7275 7361 4d69 6e69 203d 2050 7275   prusaMini = Pru
+000024f0: 7361 4c69 6e6b 5079 2e50 7275 7361 4c69  saLinkPy.PrusaLi
+00002500: 6e6b 5079 2822 3139 322e 3136 382e 302e  nkPy("192.168.0.
+00002510: 3132 3322 2c20 2238 6f6a 484b 4847 4e75  123", "8ojHKHGNu
+00002520: 4148 4132 624d 2229 0d0a 2020 2020 6f62  AHA2bM")..    ob
+00002530: 6a20 3d20 7072 7573 614d 696e 692e 6465  j = prusaMini.de
+00002540: 6c65 7465 2827 2f44 4542 4f55 437e 312e  lete('/DEBOUC~1.
+00002550: 4743 4f27 290d 0a0d 0a0d 0a23 2320 5072  GCO')......## Pr
+00002560: 7573 614c 696e 6b50 792e 706f 7374 5f67  usaLinkPy.post_g
+00002570: 636f 6465 2872 656d 6f74 6550 6174 6829  code(remotePath)
+00002580: 200d 0a0d 0a50 7269 6e74 2061 2066 696c   ....Print a fil
+00002590: 6520 616c 7265 6164 7920 706f 7265 7365  e already porese
+000025a0: 6e74 206f 6e20 5553 4220 6b65 7920 0d0a  nt on USB key ..
+000025b0: 0d0a 2020 2020 696d 706f 7274 2050 7275  ..    import Pru
+000025c0: 7361 4c69 6e6b 5079 0d0a 2020 2020 7072  saLinkPy..    pr
+000025d0: 7573 614d 696e 6920 3d20 5072 7573 614c  usaMini = PrusaL
+000025e0: 696e 6b50 792e 5072 7573 614c 696e 6b50  inkPy.PrusaLinkP
+000025f0: 7928 2231 3932 2e31 3638 2e30 2e31 3233  y("192.168.0.123
+00002600: 222c 2022 386f 6a48 4b48 474e 7541 4841  ", "8ojHKHGNuAHA
+00002610: 3262 4d22 290d 0a20 2020 206f 626a 203d  2bM")..    obj =
+00002620: 2070 7275 7361 4d69 6e69 2e70 6f73 745f   prusaMini.post_
+00002630: 6763 6f64 6528 272f 4445 424f 5543 7e31  gcode('/DEBOUC~1
+00002640: 2e47 434f 2729 0d0a 0d0a 2323 2050 7275  .GCO')....## Pru
+00002650: 7361 4c69 6e6b 5079 2e70 7574 5f67 636f  saLinkPy.put_gco
+00002660: 6465 2872 656d 6f74 6550 6174 682c 2070  de(remotePath, p
+00002670: 7269 6e74 4166 7465 7255 706c 6f61 6420  rintAfterUpload 
+00002680: 3d20 4661 6c73 652c 206f 7665 7277 7269  = False, overwri
+00002690: 7465 203d 2046 616c 7365 2920 0d0a 0d0a  te = False) ....
+000026a0: 5365 6e64 2061 2066 696c 6520 6f6e 2055  Send a file on U
+000026b0: 5342 2044 7269 7665 2e0d 0a0d 0a43 616e  SB Drive.....Can
+000026c0: 2063 7265 6174 6520 6120 666f 6c64 6572   create a folder
+000026d0: 2021 0d0a 0d0a 6966 2072 6574 2e73 7461   !....if ret.sta
+000026e0: 7475 735f 636f 6465 203d 2034 3039 202d  tus_code = 409 -
+000026f0: 3e20 436f 6e66 6c69 6374 203a 2046 696c  > Conflict : Fil
+00002700: 6520 616c 7265 6164 7920 6578 6973 7473  e already exists
+00002710: 0d0a 6966 2072 6574 2e73 7461 7475 735f  ..if ret.status_
+00002720: 636f 6465 203d 2034 3135 202d 3e20 7b22  code = 415 -> {"
+00002730: 7469 746c 6522 3a20 2234 3135 3a20 556e  title": "415: Un
+00002740: 7375 7070 6f72 7465 6420 4d65 6469 6120  supported Media 
+00002750: 5479 7065 222c 226d 6573 7361 6765 223a  Type","message":
+00002760: 224e 6f74 2061 2047 434f 4445 227d 0d0a  "Not a GCODE"}..
+00002770: 0d0a 7072 696e 7441 6674 6572 5570 6c6f  ..printAfterUplo
+00002780: 6164 203a 2053 6574 2061 7420 5472 7565  ad : Set at True
+00002790: 2074 6f20 7072 696e 7420 6166 7465 7220   to print after 
+000027a0: 7570 6c6f 6164 2e20 0d0a 0d0a 6f76 6572  upload. ....over
+000027b0: 7772 6974 6520 3a20 416c 6c6f 7720 6669  write : Allow fi
+000027c0: 6c65 204f 7665 7277 7269 7465 0d0a 0d0a  le Overwrite....
+000027d0: 4657 2035 2e31 2e30 203a 0d0a 0d0a 202a  FW 5.1.0 :.... *
+000027e0: 2057 6172 6e69 6e67 3a20 7072 696e 7469   Warning: printi
+000027f0: 6e67 2073 7461 7274 7320 6576 656e 2069  ng starts even i
+00002800: 6620 7468 6520 6265 6420 6973 206e 6f74  f the bed is not
+00002810: 2065 6d70 7479 0d0a 202a 2043 616e 206f   empty.. * Can o
+00002820: 6e6c 7920 7365 6e64 2062 6763 6f64 6520  nly send bgcode 
+00002830: 616e 6420 6763 6f64 650d 0a20 2020 200d  and gcode..    .
+00002840: 0a0d 0a20 2020 2069 6d70 6f72 7420 5072  ...    import Pr
+00002850: 7573 614c 696e 6b50 790d 0a20 2020 2070  usaLinkPy..    p
+00002860: 7275 7361 4d69 6e69 203d 2050 7275 7361  rusaMini = Prusa
+00002870: 4c69 6e6b 5079 2e50 7275 7361 4c69 6e6b  LinkPy.PrusaLink
+00002880: 5079 2822 3139 322e 3136 382e 302e 3132  Py("192.168.0.12
+00002890: 3322 2c20 2238 6f6a 484b 4847 4e75 4148  3", "8ojHKHGNuAH
+000028a0: 4132 624d 2229 0d0a 2020 2020 7374 6174  A2bM")..    stat
+000028b0: 7573 203d 2070 7275 7361 4d69 6e69 2e70  us = prusaMini.p
+000028c0: 7574 2827 433a 2f4d 544e 2f44 4542 4f55  ut('C:/MTN/DEBOU
+000028d0: 4348 4147 452e 6763 6f64 6527 202c 2027  CHAGE.gcode' , '
+000028e0: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
+000028f0: 636f 6465 2729 0d0a 2020 2020 2320 4f76  code')..    # Ov
+00002900: 6572 7772 6974 650d 0a20 2020 2073 7461  erwrite..    sta
+00002910: 7475 7320 3d20 7072 7573 614d 696e 692e  tus = prusaMini.
+00002920: 7075 7428 2743 3a2f 4d54 4e2f 4445 424f  put('C:/MTN/DEBO
+00002930: 5543 4841 4745 2e67 636f 6465 2720 2c20  UCHAGE.gcode' , 
+00002940: 274d 544e 2f44 4542 4f55 4348 4147 452e  'MTN/DEBOUCHAGE.
+00002950: 6763 6f64 6527 2c20 4661 6c73 652c 2054  gcode', False, T
+00002960: 7275 6529 0d0a 2020 2020 2320 4f76 6572  rue)..    # Over
+00002970: 7772 6974 6520 616e 6420 5072 696e 740d  write and Print.
+00002980: 0a20 2020 2073 7461 7475 7320 3d20 7072  .    status = pr
+00002990: 7573 614d 696e 692e 7075 7428 2743 3a2f  usaMini.put('C:/
+000029a0: 4d54 4e2f 4445 424f 5543 4841 4745 2e67  MTN/DEBOUCHAGE.g
+000029b0: 636f 6465 2720 2c20 274d 544e 2f44 4542  code' , 'MTN/DEB
+000029c0: 4f55 4348 4147 452e 6763 6f64 6527 2c20  OUCHAGE.gcode', 
+000029d0: 5472 7565 2c20 5472 7565 290d 0a20 2020  True, True)..   
+000029e0: 200d 0a23 2320 5072 7573 614c 696e 6b50   ..## PrusaLinkP
+000029f0: 792e 6578 6973 7473 5f67 636f 6465 2872  y.exists_gcode(r
+00002a00: 656d 6f74 6550 6174 6829 200d 0a0d 0a43  emotePath) ....C
+00002a10: 6865 636b 2069 6620 6120 6669 6c65 2065  heck if a file e
+00002a20: 7869 7374 7320 6f6e 2055 5342 2064 7269  xists on USB dri
+00002a30: 7665 2e20 0d0a 0d0a 5265 7475 726e 2054  ve. ....Return T
+00002a40: 7275 6520 6f72 2046 616c 7365 0d0a 0d0a  rue or False....
+00002a50: 2020 2020 696d 706f 7274 2050 7275 7361      import Prusa
+00002a60: 4c69 6e6b 5079 0d0a 2020 2020 7072 7573  LinkPy..    prus
+00002a70: 614d 696e 6920 3d20 5072 7573 614c 696e  aMini = PrusaLin
+00002a80: 6b50 792e 5072 7573 614c 696e 6b50 7928  kPy.PrusaLinkPy(
+00002a90: 2231 3932 2e31 3638 2e30 2e31 3233 222c  "192.168.0.123",
+00002aa0: 2022 386f 6a48 4b48 474e 7541 4841 3262   "8ojHKHGNuAHA2b
+00002ab0: 4d22 290d 0a20 2020 2073 7461 7475 7320  M")..    status 
+00002ac0: 3d20 7072 7573 614d 696e 692e 6578 6973  = prusaMini.exis
+00002ad0: 7473 5f67 636f 6465 2827 2f44 4542 4f55  ts_gcode('/DEBOU
+00002ae0: 437e 312e 4743 4f27 290d 0a0d 0a23 2320  C~1.GCO')....## 
+00002af0: 5072 7573 614c 696e 6b50 792e 7061 7573  PrusaLinkPy.paus
+00002b00: 655f 7072 696e 7428 2920 0d0a 0d0a 5061  e_print() ....Pa
+00002b10: 7573 6520 6163 7475 616c 2070 7269 6e74  use actual print
+00002b20: 2e0d 0a0d 0a41 6464 6564 2069 6e20 322e  .....Added in 2.
+00002b30: 322e 3020 2e0d 0a0d 0a23 2320 5072 7573  2.0 .....## Prus
+00002b40: 614c 696e 6b50 792e 7265 7375 6d65 5f70  aLinkPy.resume_p
+00002b50: 7269 6e74 2829 200d 0a0d 0a52 6573 756d  rint() ....Resum
+00002b60: 6520 7061 7573 6564 2070 7269 6e74 2e0d  e paused print..
+00002b70: 0a0d 0a41 6464 6564 2069 6e20 322e 322e  ...Added in 2.2.
+00002b80: 3020 2e0d 0a0d 0a23 2320 5072 7573 614c  0 .....## PrusaL
+00002b90: 696e 6b50 792e 7374 6f70 5f70 7269 6e74  inkPy.stop_print
+00002ba0: 2829 200d 0a0d 0a53 746f 7020 6163 7475  () ....Stop actu
+00002bb0: 616c 2070 7269 6e74 2e0d 0a0d 0a41 6464  al print.....Add
+00002bc0: 6564 2069 6e20 322e 322e 3020 2e0d 0a0d  ed in 2.2.0 ....
+00002bd0: 0a23 2041 5049 0d0a 0d0a 4150 4920 6e6f  .# API....API no
+00002be0: 7420 696d 706c 656d 656e 7465 6420 696e  t implemented in
+00002bf0: 206d 7920 6c69 6220 203a 200d 0a0d 0a20   my lib  : .... 
+00002c00: 2a20 7265 7472 6965 7665 2074 6875 6d62  * retrieve thumb
+00002c10: 6e61 696c 203a 0d0a 0d0a 2020 2020 7220  nail :....    r 
+00002c20: 3d20 7265 7175 6573 7473 2e67 6574 2827  = requests.get('
+00002c30: 6874 7470 3a2f 2f31 3932 2e31 3638 2e30  http://192.168.0
+00002c40: 2e31 3233 3a38 3031 372f 7468 756d 622f  .123:8017/thumb/
+00002c50: 6c2f 7573 622f 5441 5645 524e 7e31 2e47  l/usb/TAVERN~1.G
+00002c60: 434f 272c 2068 6561 6465 7273 3d68 6561  CO', headers=hea
+00002c70: 6465 7273 290d 0a0d 0a2f 6170 692f 7365  ders)..../api/se
+00002c80: 7474 696e 6773 0d0a 0d0a 0d0a 504f 5354  ttings......POST
+00002c90: 202f 6170 692f 6a6f 620d 0a2a 2a5b 4c69   /api/job..**[Li
+00002ca0: 6e6b 2074 6f20 4275 6464 7920 636f 6465  nk to Buddy code
+00002cb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002cc0: 2e63 6f6d 2f70 7275 7361 3364 2f50 7275  .com/prusa3d/Pru
+00002cd0: 7361 2d46 6972 6d77 6172 652d 4275 6464  sa-Firmware-Budd
+00002ce0: 792f 626c 6f62 2f6d 6173 7465 722f 6c69  y/blob/master/li
+00002cf0: 622f 5755 492f 6c69 6e6b 5f63 6f6e 7465  b/WUI/link_conte
+00002d00: 6e74 2f70 7275 7361 5f6c 696e 6b5f 6170  nt/prusa_link_ap
+00002d10: 692e 6370 7023 4c32 3736 292a 2a0d 0a0d  i.cpp#L276)**...
+00002d20: 0a47 4554 2f50 4f53 5420 2f61 7069 2f64  .GET/POST /api/d
+00002d30: 6f77 6e6c 6f61 6420 0d0a 2a2a 5b4c 696e  ownload ..**[Lin
+00002d40: 6b20 746f 2042 7564 6479 2063 6f64 655d  k to Buddy code]
+00002d50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002d60: 636f 6d2f 7072 7573 6133 642f 5072 7573  com/prusa3d/Prus
+00002d70: 612d 4669 726d 7761 7265 2d42 7564 6479  a-Firmware-Buddy
+00002d80: 2f62 6c6f 622f 6d61 7374 6572 2f6c 6962  /blob/master/lib
+00002d90: 2f57 5549 2f6c 696e 6b5f 636f 6e74 656e  /WUI/link_conten
+00002da0: 742f 7072 7573 615f 6c69 6e6b 5f61 7069  t/prusa_link_api
+00002db0: 2e63 7070 234c 3238 3929 2a2a 0d0a 0d0a  .cpp#L289)**....
+00002dc0: 0d0a 2320 2042 7567 7320 7072 6573 656e  ..#  Bugs presen
+00002dd0: 7420 696e 2050 7275 7361 204d 494e 4920  t in Prusa MINI 
+00002de0: 7072 696e 7465 7220 6669 726d 7761 7265  printer firmware
+00002df0: 2034 2e34 2e31 3a0d 0a0d 0a20 2a20 5468   4.4.1:.... * Th
+00002e00: 6572 6520 6973 206e 6f20 706f 7373 6962  ere is no possib
+00002e10: 696c 6974 7920 746f 2068 6176 6520 7468  ility to have th
+00002e20: 6520 6c69 7374 206f 6620 666f 6c64 6572  e list of folder
+00002e30: 7320 7072 6573 656e 7420 696e 2061 2064  s present in a d
+00002e40: 6972 6563 746f 7279 0d0a 2020 2020 2a20  irectory..    * 
+00002e50: 536f 6c76 6564 2069 6e20 6669 726d 7761  Solved in firmwa
+00002e60: 7265 2035 0d0a 202a 2059 6f75 2063 616e  re 5.. * You can
+00002e70: 6e6f 7420 7570 6c6f 6164 2061 2067 636f  not upload a gco
+00002e80: 6465 2069 6e20 6120 7375 6266 6f6c 6465  de in a subfolde
+00002e90: 7220 6f66 2074 6865 2055 5342 206b 6579  r of the USB key
+00002ea0: 0d0a 2020 2020 2a20 536f 6c76 6564 2069  ..    * Solved i
+00002eb0: 6e20 6669 726d 7761 7265 2035 0d0a 202a  n firmware 5.. *
+00002ec0: 2057 6865 6e20 7468 6520 7072 696e 7465   When the printe
+00002ed0: 7220 6465 7465 6374 7320 7468 6520 656e  r detects the en
+00002ee0: 6420 6f66 2074 6865 2066 696c 616d 656e  d of the filamen
+00002ef0: 7420 616e 6420 6974 2064 6973 706c 6179  t and it display
+00002f00: 7320 2243 6861 6e67 6520 4669 6c61 6d65  s "Change Filame
+00002f10: 6e74 2220 7468 6520 7465 6c65 6d65 7472  nt" the telemetr
+00002f20: 7920 696e 666f 726d 6174 696f 6e20 6973  y information is
+00002f30: 206e 6f20 6c6f 6e67 6572 2067 6f6f 642e   no longer good.
+00002f40: 2048 6572 6520 6973 2074 6865 2069 6e66   Here is the inf
+00002f50: 6f72 6d61 7469 6f6e 2072 6574 7572 6e65  ormation returne
+00002f60: 6420 6279 2074 6865 2070 7269 6e74 6572  d by the printer
+00002f70: 2069 6e20 7468 6973 2063 6173 653a 0d0a   in this case:..
+00002f80: 200d 0a20 2020 2027 7465 6c65 6d65 7472   ..    'telemetr
+00002f90: 7927 3a20 7b27 7465 6d70 2d62 6564 273a  y': {'temp-bed':
+00002fa0: 2030 2e30 2c20 2774 656d 702d 6e6f 7a7a   0.0, 'temp-nozz
+00002fb0: 6c65 273a 2030 2e30 2c20 2770 7269 6e74  le': 0.0, 'print
+00002fc0: 2d73 7065 6564 273a 2031 3030 2c20 277a  -speed': 100, 'z
+00002fd0: 2d68 6569 6768 7427 3a20 302e 302c 2027  -height': 0.0, '
+00002fe0: 6d61 7465 7269 616c 273a 2027 2d2d 2d27  material': '---'
+00002ff0: 7d0d 0a20 2020 200d 0a20 2a20 5374 696c  }..    .. * Stil
+00003000: 6c20 696e 2074 6865 2063 6173 6520 6f66  l in the case of
+00003010: 2061 2066 696c 616d 656e 7420 6368 616e   a filament chan
+00003020: 6765 2c20 7468 6520 7374 6174 7573 2069  ge, the status i
+00003030: 6e66 6f72 6d61 7469 6f6e 2069 7320 696e  nformation is in
+00003040: 636f 7272 6563 743a 0d0a 0d0a 2020 2020  correct:....    
+00003050: 2773 7461 7465 273a 207b 2774 6578 7427  'state': {'text'
+00003060: 3a20 274f 7065 7261 7469 6f6e 616c 272c  : 'Operational',
+00003070: 2027 666c 6167 7327 3a20 7b27 6f70 6572   'flags': {'oper
+00003080: 6174 696f 6e61 6c27 3a20 5472 7565 2c20  ational': True, 
+00003090: 2770 6175 7365 6427 3a20 4661 6c73 652c  'paused': False,
+000030a0: 2027 7072 696e 7469 6e67 273a 2046 616c   'printing': Fal
+000030b0: 7365 2c20 2763 616e 6365 6c6c 696e 6727  se, 'cancelling'
+000030c0: 3a20 4661 6c73 652c 2027 7061 7573 696e  : False, 'pausin
+000030d0: 6727 3a20 4661 6c73 652c 2027 7364 5265  g': False, 'sdRe
+000030e0: 6164 7927 3a20 4661 6c73 652c 2027 6572  ady': False, 'er
+000030f0: 726f 7227 3a20 4661 6c73 652c 2027 636c  ror': False, 'cl
+00003100: 6f73 6564 4f6e 4572 726f 7227 3a20 4661  osedOnError': Fa
+00003110: 6c73 652c 2027 7265 6164 7927 3a20 5472  lse, 'ready': Tr
+00003120: 7565 2c20 2762 7573 7927 3a20 4661 6c73  ue, 'busy': Fals
+00003130: 657d 0d0a 0d0a 0d0a 2320 496e 7370 6972  e}......# Inspir
+00003140: 6174 696f 6e0d 0a0d 0a41 6e20 6f74 6865  ation....An othe
+00003150: 7220 6c69 6220 3a20 0d0a 0d0a 6874 7470  r lib : ....http
+00003160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00003170: 6f6d 652d 6173 7369 7374 616e 742d 6c69  ome-assistant-li
+00003180: 6273 2f50 7275 7361 4c69 6e6b 5079 2f62  bs/PrusaLinkPy/b
+00003190: 6c6f 622f 6d61 696e 2f50 7275 7361 4c69  lob/main/PrusaLi
+000031a0: 6e6b 5079 2f0d 0a0d 0a0d 0a4c 6573 2063  nkPy/......Les c
+000031b0: 6f6d 6d61 6e64 6573 2064 616e 7320 6c61  ommandes dans la
+000031c0: 206d 696e 6920 3a0d 0a68 7474 7073 3a2f   mini :..https:/
+000031d0: 2f67 6974 6875 622e 636f 6d2f 7072 7573  /github.com/prus
+000031e0: 6133 642f 5072 7573 612d 4669 726d 7761  a3d/Prusa-Firmwa
+000031f0: 7265 2d42 7564 6479 2f62 6c6f 622f 6d61  re-Buddy/blob/ma
+00003200: 7374 6572 2f6c 6962 2f57 5549 2f6c 696e  ster/lib/WUI/lin
+00003210: 6b5f 636f 6e74 656e 742f 6261 7369 635f  k_content/basic_
+00003220: 6765 7473 2e63 7070 0d0a 0d0a 0d0a 0d0a  gets.cpp........
+00003230: 2320 436f 6e73 7472 7569 7265 206c 6120  # Construire la 
+00003240: 6c69 620d 0a0d 0a20 2020 2070 7920 2d6d  lib....    py -m
+00003250: 2062 7569 6c64 0d0a 0d0a 546f 2075 706c   build....To upl
+00003260: 6f61 6420 746f 2074 6573 7470 6920 7265  oad to testpi re
+00003270: 706f 203a 0d0a 0d0a 2020 2020 7079 202d  po :....    py -
+00003280: 6d20 7477 696e 6520 7570 6c6f 6164 202d  m twine upload -
+00003290: 2d72 6570 6f73 6974 6f72 7920 7465 7374  -repository test
+000032a0: 7069 2064 6973 742f 2a0d 0a0d 0a54 6f20  pi dist/*....To 
+000032b0: 7570 6c6f 6164 2074 6f20 7079 7069 2072  upload to pypi r
+000032c0: 6570 6f20 3a0d 0a0d 0a20 2020 2070 7920  epo :....    py 
+000032d0: 2d6d 2074 7769 6e65 2075 706c 6f61 6420  -m twine upload 
+000032e0: 6469 7374 2f2a 0d0a 0d0a 0d0a 6874 7470  dist/*......http
+000032f0: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f61  s://medium.com/a
+00003300: 6e61 6c79 7469 6373 2d76 6964 6879 612f  nalytics-vidhya/
+00003310: 686f 772d 746f 2d63 7265 6174 652d 612d  how-to-create-a-
+00003320: 7079 7468 6f6e 2d6c 6962 7261 7279 2d37  python-library-7
+00003330: 6435 6165 6138 3063 6333 660d 0a0d 0a    d5aea80cc3f....
```

### Comparing `PrusaLinkPy-2.1.0/pyproject.toml` & `prusalinkpy-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PrusaLinkPy"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
   { name="Guillaume RICO", email="guillaume.rico@alpesmesures.fr" },
 ]
 description = "A library to interface with the PrusaLink API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

