# Comparing `tmp/zamino_fix-1.1.4.tar.gz` & `tmp/zamino_fix-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zamino_fix-1.1.4.tar", last modified: Sun May 12 08:25:36 2024, max compression
+gzip compressed data, was "zamino_fix-1.1.5.tar", last modified: Mon May 13 11:07:42 2024, max compression
```

## Comparing `zamino_fix-1.1.4.tar` & `zamino_fix-1.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.4/LICENSE
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/PKG-INFO
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.4/README.md
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAmino.fix.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/requires.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-12 08:25:36.000000 zamino_fix-1.1.4/ZAmino.fix.egg-info/top_level.txt
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-04-10 15:12:24.000000 zamino_fix-1.1.4/ZAminofix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.4/ZAminofix/acm.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/asyncfix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/acm.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.4/ZAminofix/asyncfix/sub_client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-12 08:17:35.000000 zamino_fix-1.1.4/ZAminofix/client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/lib/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/lib/__init__.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/ZAminofix/lib/util/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.4/ZAminofix/lib/util/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.4/ZAminofix/lib/util/exceptions.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.4/ZAminofix/lib/util/headers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.4/ZAminofix/lib/util/helpers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.4/ZAminofix/lib/util/objects.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 zamino_fix-1.1.4/ZAminofix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   117552 2023-04-06 18:02:18.000000 zamino_fix-1.1.4/ZAminofix/sub_client.py
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-12 08:25:36.070656 zamino_fix-1.1.4/setup.cfg
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      696 2024-05-12 08:19:11.000000 zamino_fix-1.1.4/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.5/LICENSE
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/PKG-INFO
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.5/README.md
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAmino.fix.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/requires.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/top_level.txt
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-04-10 15:12:24.000000 zamino_fix-1.1.5/ZAminofix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.5/ZAminofix/acm.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/asyncfix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/acm.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/sub_client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-12 08:17:35.000000 zamino_fix-1.1.5/ZAminofix/client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/lib/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/lib/__init__.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/lib/util/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.5/ZAminofix/lib/util/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/lib/util/exceptions.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.5/ZAminofix/lib/util/headers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.5/ZAminofix/lib/util/helpers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.5/ZAminofix/lib/util/objects.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 zamino_fix-1.1.5/ZAminofix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   107423 2024-05-13 10:55:56.000000 zamino_fix-1.1.5/ZAminofix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/setup.cfg
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      698 2024-05-13 11:06:36.000000 zamino_fix-1.1.5/setup.py
```

### Comparing `zamino_fix-1.1.4/LICENSE` & `zamino_fix-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/PKG-INFO` & `zamino_fix-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.4
+Version: 1.1.5
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
 Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
```

### Comparing `zamino_fix-1.1.4/ZAmino.fix.egg-info/PKG-INFO` & `zamino_fix-1.1.5/ZAmino.fix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.4
+Version: 1.1.5
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
 Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
```

### Comparing `zamino_fix-1.1.4/ZAmino.fix.egg-info/SOURCES.txt` & `zamino_fix-1.1.5/ZAmino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/acm.py` & `zamino_fix-1.1.5/ZAminofix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/asyncfix/acm.py` & `zamino_fix-1.1.5/ZAminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/asyncfix/client.py` & `zamino_fix-1.1.5/ZAminofix/asyncfix/client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/asyncfix/socket.py` & `zamino_fix-1.1.5/ZAminofix/asyncfix/socket.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/asyncfix/sub_client.py` & `zamino_fix-1.1.5/ZAminofix/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/client.py` & `zamino_fix-1.1.5/ZAminofix/client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/lib/util/exceptions.py` & `zamino_fix-1.1.5/ZAminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/lib/util/headers.py` & `zamino_fix-1.1.5/ZAminofix/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/lib/util/helpers.py` & `zamino_fix-1.1.5/ZAminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/lib/util/objects.py` & `zamino_fix-1.1.5/ZAminofix/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/socket.py` & `zamino_fix-1.1.5/ZAminofix/socket.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.4/ZAminofix/sub_client.py` & `zamino_fix-1.1.5/ZAminofix/sub_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,62 +29,60 @@
         }
 
         if data: vc_headers["Content-Length"] = str(len(data))
         self.vc_headers = vc_headers
 
 
 class SubClient(client.Client):
-    def __init__(self, comId: str = None, aminoId: str = None, *, profile: objects.UserProfile, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
+    def __init__(self, comId: str = None, aminoId: str = None, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
         client.Client.__init__(self, deviceId=deviceId, sub=True, proxies=proxies, certificatePath=certificatePath)
         self.vc_connect = False
 
         if comId is not None:
             self.comId = comId
             self.community: objects.Community = self.get_community_info(comId)
 
         if aminoId is not None:
             link = "http://aminoapps.com/c/"
             self.comId = self.get_from_code(link + aminoId).comId
             self.community: objects.Community = self.get_community_info(self.comId)
 
         if comId is None and aminoId is None: raise exceptions.NoCommunity()
 
-        try: self.profile: objects.UserProfile = self.get_user_info(userId=profile.userId)
-        except AttributeError: raise exceptions.FailedLogin()
-        except exceptions.UserUnavailable: pass
+
 
     def parse_headers(self, data: str = None, type: str = None) -> dict:
         return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
 
     def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25) -> objects.InviteCodeList:
-        response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.InviteCodeList(json.loads(response.text)["communityInvitationList"]).InviteCodeList
 
     def generate_invite_code(self, duration: int = 0, force: bool = True) -> objects.InviteCode:
         data = json.dumps({
             "duration": duration,
             "force": force,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/g/s-x{self.comId}/community/invitation", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s-x{self.comId}/community/invitation", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.InviteCode(json.loads(response.text)["communityInvitation"]).InviteCode
 
     def get_vip_users(self) -> objects.UserProfileList:
-        response = self.session.get(f"{self.api}/{self.comId}/s/influencer", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/{self.comId}/s/influencer", headers=self.parse_headers())
         if response.status_code != 200:
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def delete_invite_code(self, inviteId: str) -> int:
-        response = self.session.delete(f"{self.api}/g/s-x{self.comId}/community/invitation/{inviteId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/g/s-x{self.comId}/community/invitation/{inviteId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False) -> int:
         mediaList = []
 
@@ -112,15 +110,15 @@
 
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
         mediaList = []
 
@@ -137,15 +135,15 @@
 
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/item", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/item", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
         mediaList = []
 
@@ -164,27 +162,27 @@
         if title: data["title"] = title
         if content: data["content"] = content
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def delete_blog(self, blogId: str) -> int:
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def delete_wiki(self, wikiId: str) -> int:
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def repost_blog(self, content: str = None, blogId: str = None, wikiId: str = None) -> int:
         if blogId is not None: refObjectId, refObjectType = blogId, 1
         elif wikiId is not None: refObjectId, refObjectType = wikiId, 2
@@ -194,49 +192,49 @@
             "content": content,
             "refObjectId": refObjectId,
             "refObjectType": refObjectType,
             "type": 2,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def check_in(self, tz: int = -timezone // 1000) -> int:
         data = json.dumps({
             "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def repair_check_in(self, method: int = 0) -> int:
         data = {"timestamp": int(timestamp() * 1000)}
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/repair", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/repair", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
         data = json.dumps({
             "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/lottery", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/check-in/lottery", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.LotteryLog(json.loads(response.text)["lotteryLog"]).LotteryLog
 
     def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None) -> int:
         mediaList = []
 
@@ -268,27 +266,27 @@
             for titles, colors in zip(titles, colors):
                 tlt.append({"title": titles, "color": colors})
 
             data["extensions"] = {"customTitles": tlt}
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def vote_poll(self, blogId: str, optionId: str) -> int:
         data = json.dumps({
             "value": 1,
             "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False) -> int:
         data = {
             "content": message,
@@ -302,37 +300,37 @@
         if isGuest: comType = "g-comment"
         else: comType = "comment"
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/{comType}", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/{comType}", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/{comType}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/{comType}", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
-        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}", headers=self.parse_headers())
+        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.parse_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> int:
@@ -354,38 +352,38 @@
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = json.dumps(data)
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
 
             elif isinstance(blogId, list):
                 data["targetIdList"] = blogId
                 data = json.dumps(data)
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/feed/vote", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/feed/vote", headers=self.parse_headers(data=data), data=data)
 
             else: raise exceptions.WrongType
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self. comId}/s/item/{wikiId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self. comId}/s/item/{wikiId}/vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def unlike_blog(self, blogId: str = None, wikiId: str = None) -> int:
-        if blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/vote?eventSource=UserProfileView", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/vote?eventSource=PostDetailView", headers=self.parse_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
@@ -394,94 +392,94 @@
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
-        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if userId: response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers())
+        elif blogId: response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        elif wikiId: response = self.session.delete(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def upvote_comment(self, blogId: str, commentId: str):
         data = json.dumps({
             "value": 1,
             "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def downvote_comment(self, blogId: str, commentId: str):
         data = json.dumps({
             "value": -1,
             "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def unvote_comment(self, blogId: str, commentId: str):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def reply_wall(self, userId: str, commentId: str, message: str):
         data = json.dumps({
             "content": message,
             "stackedId": None,
             "respondTo": commentId,
             "type": 0,
             "eventSource": "UserProfileView",
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
         data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
         if timers: data["userActiveTimeChunkList"] = timers 
         data = json_minify(json.dumps(data))  
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/community/stats/user-active-time", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath) 
+        response = self.session.post(f"{self.api}/x{self.comId}/s/community/stats/user-active-time", headers=self.parse_headers(data=data), data=data) 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text) 
         else: return response.status_code
 
     def activity_status(self, status: str):
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
@@ -489,40 +487,40 @@
 
         data = json.dumps({
             "onlineStatus": status,
             "duration": 86400,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     # TODO : Finish this
     def watch_ad(self):
-        response = self.session.post(f"{self.api}/g/s/wallet/ads/video/start", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/g/s/wallet/ads/video/start", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def check_notifications(self):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notification/checked", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notification/checked", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def delete_notification(self, notificationId: str):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification/{notificationId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification/{notificationId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def clear_notifications(self):
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/notification", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
@@ -540,36 +538,36 @@
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = json.dumps({
             "uids": userIds,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def add_to_favorites(self, userId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         url = None
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
@@ -587,21 +585,21 @@
             data["objectType"] = 2
             url = f"{self.api}/x{self.comId}/s/tipping"
 
         if url is None: raise exceptions.SpecifyType()
 
         data = json.dumps(data)
         
-        response = self.session.post(url, headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(url, headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def thank_tip(self, chatId: str, userId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
         Follow an User or Multiple Users.
@@ -611,20 +609,20 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str):
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member", headers=self.parse_headers())
 
         elif isinstance(userId, list):
             data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.WrongType(type(userId))
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
@@ -636,15 +634,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def block(self, userId: str):
         """
         Block an User.
@@ -653,15 +651,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def unblock(self, userId: str):
         """
         Unblock an User.
@@ -670,15 +668,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/block/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def visit(self, userId: str):
         """
         Visit an User.
@@ -687,15 +685,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
         Flag a User, Blog or Wiki.
@@ -737,15 +735,15 @@
         else: raise exceptions.SpecifyType()
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/{flg}", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/{flg}", data=data, headers=self.parse_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
@@ -824,15 +822,15 @@
 
             else: raise exceptions.SpecifyType(fileType)
 
             data["mediaUploadValue"] = base64.b64encode(file.read()).decode()
 
         data = json.dumps(data)
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
         data = {
         "type": 0,
@@ -847,15 +845,15 @@
         },
             "clientRefId": int(timestamp() / 10 % 100000000),
             "timestamp": int(timestamp() * 1000),
             "attachedObject": None
         }
         
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
         """
         Delete a Message from a Chat.
 
@@ -876,16 +874,16 @@
             "timestamp": int(timestamp() * 1000)
         }
         if asStaff and reason:
             data["adminOpNote"] = {"content": reason}
 
         data = json.dumps(data)
         
-        if not asStaff: response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        if not asStaff: response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
+        else: response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
         Mark a Message from a Chat as Read.
@@ -900,15 +898,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
         Send a Message to a Chat.
@@ -951,120 +949,120 @@
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
                 data = json.dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
                 data = json.dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
                 
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not pinChat:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
             data = json.dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.parse_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if coHosts is not None:
             data = json.dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
             
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not viewOnly:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canInvite is not None:
             if canInvite:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canInvite:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canTip is not None:
             if canTip:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canTip:
-                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data), proxies=self.proxies, verify=self.certificatePath)
+                response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: res.append(exceptions.CheckException(response.text))
         else: res.append(response.status_code)
 
         return res
 
     def transfer_host(self, chatId: str, userIds: list):
         data = json.dumps({
             "uidList": userIds,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def transfer_organizer(self, chatId: str, userIds: list):
         self.transfer_host(chatId, userIds)
 
     def accept_host(self, chatId: str, requestId: str):
         data = json.dumps({})
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
         self.accept_host(chatId, requestId)
 
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
         if allowRejoin: allowRejoin = 1
         if not allowRejoin: allowRejoin = 0
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def join_chat(self, chatId: str):
         """
         Join an Chat.
@@ -1073,15 +1071,15 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def leave_chat(self, chatId: str):
         """
         Leave an Chat.
@@ -1090,15 +1088,15 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
         
     def delete_chat(self, chatId: str):
         """
         Delete a Chat.
@@ -1107,15 +1105,15 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.delete(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
         
     def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
@@ -1123,33 +1121,33 @@
             "paymentContext": {
                 "transactionId": transactionId,
                 "isAutoRenew": autoRenew
             },
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def promotion(self, noticeId: str, type: str = "accept"):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice/{noticeId}/{type}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice/{noticeId}/{type}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
         data = json.dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
         quizAnswerList = []
 
@@ -1164,15 +1162,15 @@
 
         data = json.dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def vc_permission(self, chatId: str, permission: int):
         """Voice Chat Join Permissions
         1 - Open to Everyone
@@ -1180,51 +1178,51 @@
         3 - Invite Only
         """
         data = json.dumps({
             "vvChatJoinType": permission,
             "timestamp": int(timestamp() * 1000)
         })
         
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def get_vc_reputation_info(self, chatId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.VcReputation(json.loads(response.text)).VcReputation
 
     def claim_vc_reputation(self, chatId: str):
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.VcReputation(json.loads(response.text)).VcReputation
 
     def get_all_users(self, type: str = "recent", start: int = 0, size: int = 25):
-        if type == "recent": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "banned": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=banned&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "featured": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "leaders": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=leaders&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif type == "curators": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=curators&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if type == "recent": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers())
+        elif type == "banned": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=banned&start={start}&size={size}", headers=self.parse_headers())
+        elif type == "featured": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers())
+        elif type == "leaders": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=leaders&start={start}&size={size}", headers=self.parse_headers())
+        elif type == "curators": response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=curators&start={start}&size={size}", headers=self.parse_headers())
         else: raise exceptions.WrongType(type)
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
     def get_online_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
     def get_online_favorite_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-group/quick-access?type=online&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-group/quick-access?type=online&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
     def get_user_info(self, userId: str):
         """
         Information of an User.
@@ -1233,15 +1231,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
 
     def get_user_following(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that the User is Following.
@@ -1252,15 +1250,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that are Following the User.
@@ -1271,15 +1269,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
         """
         List of Users that Visited the User.
@@ -1290,45 +1288,45 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.VisitorsList(json.loads(response.text)).VisitorsList
 
     def get_user_checkins(self, userId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserCheckIns(json.loads(response.text)).UserCheckIns
 
     def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_user_wikis(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
 
     def get_user_achievements(self, userId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserAchievements(json.loads(response.text)["achievements"]).UserAchievements
 
     def get_influencer_fans(self, userId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.InfluencerFans(json.loads(response.text)).InfluencerFans
 
     def get_blocked_users(self, start: int = 0, size: int = 25):
         """
         List of Users that the User Blocked.
@@ -1338,15 +1336,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_blocker_users(self, start: int = 0, size: int = 25):
         """
         List of Users that are Blocking the User.
@@ -1357,73 +1355,73 @@
 
         **Returns**
             - **Success** : :meth:`List of User IDs <List>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/block?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)["blockerUidList"]
 
     def search_users(self, nickname: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_saved_blogs(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/bookmark?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/bookmark?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserSavedBlogs(json.loads(response.text)["bookmarkList"]).UserSavedBlogs
 
     def get_leaderboard_info(self, type: str, start: int = 0, size: int = 25):
-        if "24" in type or "hour" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "7" in type or "day" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=2&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "rep" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=3&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "check" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=4", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif "quiz" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=5&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if "24" in type or "hour" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=1&start={start}&size={size}", headers=self.parse_headers())
+        elif "7" in type or "day" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=2&start={start}&size={size}", headers=self.parse_headers())
+        elif "rep" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=3&start={start}&size={size}", headers=self.parse_headers())
+        elif "check" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=4", headers=self.parse_headers())
+        elif "quiz" in type: response = self.session.get(f"{self.api}/g/s-x{self.comId}/community/leaderboard?rankingType=5&start={start}&size={size}", headers=self.parse_headers())
         else: raise exceptions.WrongType(type)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_wiki_info(self, wikiId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
 
     def get_recent_wiki_items(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=catalog-all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item?type=catalog-all&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.WikiList(json.loads(response.text)["itemList"]).WikiList
 
     def get_wiki_categories(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.WikiCategoryList(json.loads(response.text)["itemCategoryList"]).WikiCategoryList
 
     def get_wiki_category(self, categoryId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category/{categoryId}?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/item-category/{categoryId}?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.WikiCategory(json.loads(response.text)).WikiCategory
 
     def get_tipped_users(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, chatId: str = None, start: int = 0, size: int = 25):
         if blogId or quizId:
             if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif chatId: response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers())
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers())
+        elif chatId: response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers())
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.parse_headers())
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.TippedUsersSummary(json.loads(response.text)).TippedUsersSummary
 
     def get_chat_threads(self, start: int = 0, size: int = 25):
         """
@@ -1434,15 +1432,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
 
     def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
         """
         List of Public Chats of the Community.
@@ -1452,15 +1450,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
 
     def get_chat_thread(self, chatId: str):
         """
         Get the Chat Object from an Chat ID.
@@ -1469,15 +1467,15 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
         """
         List of Messages from an Chat.
@@ -1492,15 +1490,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         if pageToken is not None: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
-        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(url, headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.GetMessages(json.loads(response.text)).GetMessages
 
     def get_message_info(self, chatId: str, messageId: str):
         """
         Information of an Message from an Chat.
@@ -1510,71 +1508,71 @@
             - **message** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.Message(json.loads(response.text)["message"]).Message
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
         if blogId or quizId:
             if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}", headers=self.parse_headers())
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else: return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
 
         elif wikiId:
-            response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}", headers=self.parse_headers())
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else: return objects.GetWikiInfo(json.loads(response.text)).GetWikiInfo
 
         elif fileId:
-            response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}", headers=self.parse_headers())
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else: return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
 
         else: raise exceptions.SpecifyType()
 
     def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
 
         if blogId or quizId:
             if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
     def get_blog_categories(self, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category?size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category?size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogCategoryList(json.loads(response.text)["blogCategoryList"]).BlogCategoryList
 
     def get_blogs_by_category(self, categoryId: str,start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_quiz_rankings(self, quizId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.QuizRankings(json.loads(response.text)).QuizRankings
 
     def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
         """
         List of Wall Comments of an User.
@@ -1592,118 +1590,118 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
     def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
         if pageToken is not None: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"{self.api}/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
 
-        response = self.session.get(url, headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(url, headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.RecentBlogs(json.loads(response.text)).RecentBlogs
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
 
     def get_notifications(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.NotificationList(json.loads(response.text)["notificationList"]).NotificationList
 
     def get_notices(self, start: int = 0, size: int = 25):
         """
         :param start: Start of the List (Start: 0)
         :param size: Amount of Notices to Show
         :return: Notices List
         """
-        response = self.session.get(f"{self.api}/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.NoticeList(json.loads(response.text)["noticeList"]).NoticeList
 
     def get_sticker_pack_info(self, sticker_pack_id: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
     def get_sticker_packs(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
     # TODO : Finish this
     def get_store_chat_bubbles(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             response = json.loads(response.text)
             del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
             return response
 
     # TODO : Finish this
     def get_store_stickers(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             response = json.loads(response.text)
             del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
             return response
 
     def get_community_stickers(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?type=community-shared", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection?type=community-shared", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.CommunityStickerCollection(json.loads(response.text)).CommunityStickerCollection
 
     def get_sticker_collection(self, collectionId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.StickerCollection(json.loads(response.text)["stickerCollection"]).StickerCollection
 
     def get_shared_folder_info(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/stats", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/stats", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.GetSharedFolderInfo(json.loads(response.text)["stats"]).GetSharedFolderInfo
 
     def get_shared_folder_files(self, type: str = "latest", start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.SharedFolderFileList(json.loads(response.text)["fileList"]).SharedFolderFileList
 
     #
     # MODERATION MENU
     #
 
     def moderation_history(self, userId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, size: int = 25):
-        if userId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif blogId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif quizId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
-        else: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        if userId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}", headers=self.parse_headers())
+        elif blogId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers())
+        elif quizId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}", headers=self.parse_headers())
+        elif wikiId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.parse_headers())
+        elif fileId: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.parse_headers())
+        else: response = self.session.get(f"{self.api}/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.AdminLogList(json.loads(response.text)["adminLogList"]).AdminLogList
 
     def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
         if chatId:
             if time == 1: time = 3600
@@ -1723,30 +1721,30 @@
             },
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 4}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["adminOpValue"] = {"featuredType": 1}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["adminOpValue"] = {"featuredType": 1}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif chatId:
             data["adminOpValue"] = {"featuredType": 5}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
@@ -1755,30 +1753,30 @@
             "adminOpValue": {},
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 0}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["adminOpValue"] = {"featuredType": 0}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["adminOpValue"] = {"featuredType": 0}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif chatId:
             data["adminOpValue"] = {"featuredType": 0}
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
@@ -1788,45 +1786,45 @@
             },
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["adminOpName"] = 18
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif quizId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif chatId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif fileId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
@@ -1836,45 +1834,45 @@
             },
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["adminOpName"] = 19
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif blogId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif quizId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif wikiId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif chatId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data)
 
         elif fileId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
             data = json.dumps(data)
-            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+            response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data)
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def edit_titles(self, userId: str, titles: list, colors: list):
@@ -1886,15 +1884,15 @@
             "adminOpName": 207,
             "adminOpValue": {
                 "titles": tlt
             },
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     # TODO : List all warning texts
     def warn(self, userId: str, reason: str = None):
         data = json.dumps({
@@ -1907,15 +1905,15 @@
             },
             "penaltyType": 0,
             "adminOpNote": {},
             "noticeType": 7,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     # TODO : List all strike texts
     def strike(self, userId: str, time: int, title: str = None, reason: str = None):
         if time == 1: time = 86400
@@ -1936,89 +1934,89 @@
             "penaltyType": 1,
             "penaltyValue": time,
             "adminOpNote": {},
             "noticeType": 4,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def ban(self, userId: str, reason: str, banType: int = None):
         data = json.dumps({
             "reasonType": banType,
             "note": {
                 "content": reason
             },
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/ban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/ban", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def unban(self, userId: str, reason: str):
         data = json.dumps({
             "note": {
                 "content": reason
             },
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/unban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/unban", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def reorder_featured_users(self, userIds: list):
         data = json.dumps({
             "uidList": userIds,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/featured/reorder", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/featured/reorder", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return json.loads(response.text)
 
     def get_hidden_blogs(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_featured_users(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
     def review_quiz_questions(self, quizId: str):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}?action=review", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}?action=review", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.QuizQuestionList(json.loads(response.text)["blog"]["quizQuestionList"]).QuizQuestionList
 
     def get_recent_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_trending_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_best_quiz(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
         # Action List
         # Browsing
@@ -2079,15 +2077,15 @@
         data = {"frameId": avatarId,
                 "applyToAll": 0,
                 "timestamp": int(timestamp() * 1000)}
 
         if applyToAll: data["applyToAll"] = 1
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/avatar-frame/apply", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/avatar-frame/apply", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
@@ -2102,97 +2100,97 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = json.dumps({
             "uid": userId
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def add_poll_option(self, blogId: str, question: str):
         data = json.dumps({
             "mediaList": None,
             "title": question,
             "type": 0,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
         data = json.dumps({
             "content": content,
             "icon": None,
             "label": title,
             "mediaList": None,
             "parentCategoryId": parentCategoryId,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/item-category", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/item-category", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def create_shared_folder(self,title: str):
         data = json.dumps({
                 "title":title,
                 "timestamp":int(timestamp() * 1000)
             })
-        response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/folders", headers=self.parse_headers(data=data),data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/folders", headers=self.parse_headers(data=data),data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def submit_to_wiki(self, wikiId: str, message: str):
         data = json.dumps({
             "message": message,
             "itemId": wikiId,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
         data = json.dumps({
             "destinationCategoryIdList": destinationCategoryIdList,
             "actionType": "create",
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def reject_wiki_request(self, requestId: str):
         data = json.dumps({})
 
-        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
 
     def get_wiki_submissions(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.WikiRequestList(json.loads(response.text)["knowledgeBaseRequestList"]).WikiRequestList
 
     def get_live_layer(self):
-        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer/homepage?v=2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer/homepage?v=2", headers=self.parse_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return objects.LiveLayer(json.loads(response.text)["liveLayerList"]).LiveLayer
 
     def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
         data = {
             "applyToAll": 0,
@@ -2201,11 +2199,11 @@
             "timestamp": int(timestamp() * 1000)
         }
 
         if applyToAll is True:
             data["applyToAll"] = 1
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/apply-bubble", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+        response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/apply-bubble", headers=self.parse_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else: return response.status_code
```

### Comparing `zamino_fix-1.1.4/setup.py` & `zamino_fix-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="ZAmino.fix",
     author="ZOOM",
-    version="1.1.4",
+    version="1.1.5",
     description="Aminofix update. https://t.me/ZAminoZ",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
     	'ZAmino'
     	'ZAmino.fix'
         'aminoapps',
         'ZAminofix',
         'amino',
         'amino-bot',
     ],
     python_requires='>=3.6',
-)
+)
```

