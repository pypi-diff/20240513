# Comparing `tmp/wbddh-0.1.8-py3-none-any.whl.zip` & `tmp/wbddh-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 11423 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      420 b- defN 23-Sep-19 14:45 wbddh/__init__.py
 -rw-rw-rw-  2.0 fat     1077 b- defN 23-Aug-18 14:02 wbddh/ddh_exceptions.py
 -rw-rw-rw-  2.0 fat      990 b- defN 23-May-15 19:53 wbddh/exceptions.py
--rw-rw-rw-  2.0 fat    10783 b- defN 24-Feb-14 20:31 wbddh/request_manager.py
+-rw-rw-rw-  2.0 fat    10781 b- defN 24-Feb-21 17:18 wbddh/request_manager.py
 -rw-rw-rw-  2.0 fat     8796 b- defN 23-May-11 22:36 wbddh/session.py
 -rw-rw-rw-  2.0 fat     5993 b- defN 24-Jan-22 19:21 wbddh/session_manager.py
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-27 20:39 wbddh/test.py
 -rw-rw-rw-  2.0 fat     1709 b- defN 24-Jan-22 19:06 wbddh/utils.py
--rw-rw-rw-  2.0 fat     2294 b- defN 24-Feb-14 20:31 wbddh-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-14 20:31 wbddh-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Feb-14 20:31 wbddh-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      892 b- defN 24-Feb-14 20:31 wbddh-0.1.8.dist-info/RECORD
-12 files, 33125 bytes uncompressed, 9949 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat     2294 b- defN 24-Feb-21 17:19 wbddh-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-21 17:19 wbddh-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Feb-21 17:19 wbddh-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      892 b- defN 24-Feb-21 17:19 wbddh-0.1.9.dist-info/RECORD
+12 files, 33123 bytes uncompressed, 9949 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: wbddh/test.py
 Comment: 
 
 Filename: wbddh/utils.py
 Comment: 
 
-Filename: wbddh-0.1.8.dist-info/METADATA
+Filename: wbddh-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: wbddh-0.1.8.dist-info/WHEEL
+Filename: wbddh-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: wbddh-0.1.8.dist-info/top_level.txt
+Filename: wbddh-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wbddh-0.1.8.dist-info/RECORD
+Filename: wbddh-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbddh/request_manager.py

```diff
@@ -36,15 +36,15 @@
         session.check_tokens()
         print()
         return requests.get(get_request_url(endpoint) + special_query_string, params=regular_params, verify=session.verify, headers=session.get_headers(headers))
     else:
         return requests.get(get_request_url(endpoint) + special_query_string, params=regular_params)
 
 
-def try_get(endpoint, params=None, headers=None, session=None, num_try=3, interval=300):
+def try_get(endpoint, params=None, headers=None, session=None, num_try=3, interval=10):
     '''Repeat sending a GET request until it succeeds or it tries {num_try} times
 
     Additional arguments:
         num_try:        number of tries
         interval:       interval between tries in seconds
     '''
     count = 0
@@ -172,15 +172,15 @@
     '''
     if session:
         session.check_tokens()
         return requests.post(get_request_url(endpoint), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
     else:
         raise DDHSessionException("DDH POST request requires a session")
 
-def try_post(endpoint, params=None, json=None, headers=None, session=None, num_try=3, interval=300):
+def try_post(endpoint, params=None, json=None, headers=None, session=None, num_try=3, interval=10):
     '''Repeat sending a POST request until it succeeds or it tries {num_try} times
 
     Additional arguments:
         num_try:        number of tries
         interval:       interval between tries in seconds
     '''
     if session:
```

## Comparing `wbddh-0.1.8.dist-info/METADATA` & `wbddh-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbddh
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for DDH Open API
 Home-page: https://github.com/WB-DECIS/WBDDH
 Author: DECIS
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Provides-Extra: admin
 Requires-Dist: msal ; extra == 'admin'
```

## Comparing `wbddh-0.1.8.dist-info/RECORD` & `wbddh-0.1.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 wbddh/__init__.py,sha256=ehwZ1NnlTJKF9MplmSQx01OL3cUTvx0rBnHwYzfORJA,420
 wbddh/ddh_exceptions.py,sha256=bTPreVdxbFn_Wlhb1iKYxnlicIFh8MRYNQNaAyVCMBo,1077
 wbddh/exceptions.py,sha256=prNSwu_9o5NnGfRtZBe4OxifAcLM2eSlrgpiJkOz8-8,990
-wbddh/request_manager.py,sha256=jn_4EGVAO5-OkG_HXReiOdfHUFwsuyUuFn9k6YdqYSI,10783
+wbddh/request_manager.py,sha256=q6L2w5jU9RhMRdWtB0ZyUpkgmsT9esNFYMbnvmhVMi0,10781
 wbddh/session.py,sha256=pW5SqU2LaWcsFqRlzYMjSDM3Dlag_7HsRQHDOufTeC0,8796
 wbddh/session_manager.py,sha256=zG4IDAFA1Y3s21oQPpel1cB929QhyDz_YMgeJT3ifUw,5993
 wbddh/test.py,sha256=7c4JN9utd55Yz8i-7cUc0PEAWzbdCVb8OgodcAju9Xc,73
 wbddh/utils.py,sha256=zDZyx3S1cFzMxR6x4rsWnNLbZ7XkeL9qSEKR550YE0U,1709
-wbddh-0.1.8.dist-info/METADATA,sha256=BJm7HF-p6iQn8kJDeDSi7rZYeOtjuPou0eis7q5XI_U,2294
-wbddh-0.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-wbddh-0.1.8.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
-wbddh-0.1.8.dist-info/RECORD,,
+wbddh-0.1.9.dist-info/METADATA,sha256=5SgmZ1mwZz59t21VCTZAQw78ojyI6hZb35SU6Dwywp8,2294
+wbddh-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+wbddh-0.1.9.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
+wbddh-0.1.9.dist-info/RECORD,,
```

