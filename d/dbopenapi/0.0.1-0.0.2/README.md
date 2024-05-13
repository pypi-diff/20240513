# Comparing `tmp/dbopenapi-0.0.1.tar.gz` & `tmp/dbopenapi-0.0.2.tar.gz`

## Comparing `dbopenapi-0.0.1.tar` & `dbopenapi-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/dbopenapi.pyproj
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/src/dbopenapi/OpenApi.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/src/dbopenapi/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/src/dbopenapi/code_realtime_account.py
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/src/dbopenapi/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/LICENSE
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dbopenapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/dbopenapi.pyproj
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/OpenApi.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/code_realtime_account.py
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/src/dbopenapi/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dbopenapi-0.0.2/PKG-INFO
```

### Comparing `dbopenapi-0.0.1/dbopenapi.pyproj` & `dbopenapi-0.0.2/dbopenapi.pyproj`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.1/src/dbopenapi/OpenApi.py` & `dbopenapi-0.0.2/src/dbopenapi/OpenApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,19 @@
         """last error message.
 
         A readonly property.
         """
         return self._last_message
 
     @property
+    def access_token(self) -> str:
+        """access_token 당일 재 로그인에 이용"""
+        return self._access_token
+
+    @property
     def mac_address(self) -> str:
         """법인인 경우 필수 세팅"""
         return self._mac_address
 
     @mac_address.setter
     def mac_address(self, value:str) : self._mac_address = value
 
@@ -107,37 +112,37 @@
         if self._http and not self._http.closed:
             await self._http.close()
 
     async def login(self, appkey:str, appsecretkey:str
                     ,*
                     , enable_wss:bool=True
                     , wss_domain:str=None
-                    , access_token:str='') -> bool:
+                    , access_token:str=None) -> bool:
         '''
         로그인 요청
         appkey: 앱키
         appsecretkey: 앱시크릿키
         *
         enable_wss: 웹소켓 연결허용(기본값: True), False로 설정하면 웹소켓 연결을 하지 않음
         wss_domain: 웹소켓 도메인(해외선물옵션인 경우에만 설정, wss://openapi.db-fi.com:7071 으로 설정)
         access_token: 토큰(기본값: ''), 토큰이 있는 경우에는 토큰을 사용하고, 없는 경우에는 새로 토큰을 가져옴
         return: True: 성공, False: 실패, 실패시 last_message에 실패사유가 저장됨
         '''
         if self._connected :
             self._last_message = "aleady connected";
             return True;
         
-        if appkey == "" or appsecretkey == "":
-            self._last_message = "appkey or appsecretkey is empty";
-            return False;
-    
-        # 토큰 가져오기
         timeout = aiohttp.ClientTimeout(total=10) # 10초 타임아웃
         httpclient = aiohttp.ClientSession(timeout=timeout);
-        if access_token == '':
+        if access_token is None or access_token == '':
+            # 토큰 가져오기
+            if appkey == "" or appsecretkey == "":
+                self._last_message = "appkey or appsecretkey is empty";
+                return False;
+    
             token_response = await httpclient.post(BASE_URL + "/oauth2/token"
                         , data={'grant_type': 'client_credentials', 'appkey': appkey, 'appsecretkey': appsecretkey, 'scope': 'oob'}
                         );
             if token_response.status != 200:
                 await httpclient.close();
                 self._last_message = "Failed to retrieve authentication key.";
                 return False;
```

### Comparing `dbopenapi-0.0.1/src/dbopenapi/tr_code_to_path.py` & `dbopenapi-0.0.2/src/dbopenapi/tr_code_to_path.py`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.1/.gitignore` & `dbopenapi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.1/LICENSE` & `dbopenapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.1/README.md` & `dbopenapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.1/pyproject.toml` & `dbopenapi-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbopenapi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for db openapi"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dbopenapi-0.0.1/PKG-INFO` & `dbopenapi-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbopenapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: package for db openapi
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/dbopenapi
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

