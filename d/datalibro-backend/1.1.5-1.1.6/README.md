# Comparing `tmp/datalibro_backend-1.1.5.tar.gz` & `tmp/datalibro_backend-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.1.5.tar", last modified: Wed May  8 10:32:55 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.6.tar", last modified: Mon May 13 09:55:04 2024, max compression
```

## Comparing `datalibro_backend-1.1.5.tar` & `datalibro_backend-1.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.706574 datalibro_backend-1.1.5/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.5/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-08 10:32:55.706282 datalibro_backend-1.1.5/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.5/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.705229 datalibro_backend-1.1.5/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.5/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:06:10.000000 datalibro_backend-1.1.5/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    11228 2024-05-08 10:31:35.000000 datalibro_backend-1.1.5/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-08 10:32:55.706079 datalibro_backend-1.1.5/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-08 10:32:55.000000 datalibro_backend-1.1.5/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-08 10:32:55.706634 datalibro_backend-1.1.5/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-08 10:31:51.000000 datalibro_backend-1.1.5/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 09:55:04.864760 datalibro_backend-1.1.6/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.6/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-13 09:55:04.864350 datalibro_backend-1.1.6/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.6/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 09:55:04.862969 datalibro_backend-1.1.6/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.6/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15413 2024-05-13 07:14:09.000000 datalibro_backend-1.1.6/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    12823 2024-05-13 09:15:55.000000 datalibro_backend-1.1.6/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-13 09:55:04.864071 datalibro_backend-1.1.6/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-13 09:55:02.000000 datalibro_backend-1.1.6/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-13 09:55:04.000000 datalibro_backend-1.1.6/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-13 09:55:03.000000 datalibro_backend-1.1.6/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-13 09:55:04.000000 datalibro_backend-1.1.6/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-13 09:55:04.864837 datalibro_backend-1.1.6/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-13 09:15:53.000000 datalibro_backend-1.1.6/setup.py
```

### Comparing `datalibro_backend-1.1.5/LICENSE.txt` & `datalibro_backend-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.5/PKG-INFO` & `datalibro_backend-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.1.5
+Version: 1.1.6
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.5/README.md` & `datalibro_backend-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.5/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.6/datalibro_backend/quality_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,15 @@
     def check_missing_date(self,date_col='',start_date='',end_date='',notification='disabled',user_id=''):
         tb = self.df
         date_tb = self.date_df
         date_tb = date_tb.rename(columns = {'date':'date_map'})
         if date_col =='':
             date_col = self.date_col
         tb[date_col] = pd.to_datetime(tb[date_col]).apply(lambda x:x.strftime('%Y-%m-%d'))
+        date_tb['date_map'] = pd.to_datetime(date_tb['date_map']).apply(lambda x:x.strftime('%Y-%m-%d'))
         if start_date =='':
             date_tb = date_tb[date_tb['date_map']>=tb[date_col].min()].reset_index(drop=True)
         elif start_date !='':
             date_tb = date_tb[date_tb['date_map']>=start_date].reset_index(drop=True)
         if end_date !='':
             date_tb = date_tb[date_tb['date_map']<=end_date].reset_index(drop=True)
         data_list = tb[[date_col]].drop_duplicates()
```

### Comparing `datalibro_backend-1.1.5/datalibro_backend/read_file.py` & `datalibro_backend-1.1.6/datalibro_backend/read_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,8 +340,50 @@
     except:
         return f"{traceback.format_exc()}"
     response = requests.post(url, json=body, headers=headers)
     if response.status_code == 200:
         return "Data uploaded successfully."
     else:
         return f"Failed to upload data: {response.text}"
-    
+def send_beautiful_card_message(receive_type,receive_id,template_id,template_variable,template_version=""):
+    """Get the access token from Feishu."""
+    url = 'https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/'
+    headers = {'Content-Type': 'application/json'}
+    app_id = 'cli_a5eeb3ad3837100b'
+    app_secret = 'ftLZbDJOzDxSx0xiigALNev1tgHTvR4V'
+
+    payload = {
+        'app_id': app_id,
+        'app_secret': app_secret
+    }
+    response = requests.post(url, headers=headers, json=payload)
+    data = response.json()
+    token = data.get('tenant_access_token')
+    
+    # 卡片消息内容
+    if template_version == "":
+        template = {"type":"template",
+        "data":{"template_id":f"{template_id}",
+                "template_variable":template_variable}}
+    else:
+        template = {"type":"template",
+        "data":{"template_id":f"{template_id}",
+                "template_version_name":f"{template_version}",
+                "template_variable":template_variable}}
+    template = json.dumps(template,ensure_ascii=False)
+    template = template.replace('"', '\"')
+    payload = json.dumps({
+	"content": template,
+	"msg_type": "interactive",
+	"receive_id": f"{receive_id}",
+})
+    message_url = f"https://open.feishu.cn/open-apis/im/v1/messages?receive_id_type={receive_type}"
+
+    # 发送POST请求的headers
+    headers = {
+        'Authorization': f'Bearer {token}',
+        'Content-Type': 'application/json'
+    }
+
+    # 发送卡片消息
+    response = requests.request("POST", message_url, headers=headers, data=payload)
+    return response.text
```

### Comparing `datalibro_backend-1.1.5/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.6/datalibro_backend.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.1.5
+Version: 1.1.6
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.5/setup.py` & `datalibro_backend-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.1.5",
+  version="1.1.6",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

