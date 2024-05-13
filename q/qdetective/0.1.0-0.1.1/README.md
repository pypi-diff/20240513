# Comparing `tmp/QDetective-0.1.0.tar.gz` & `tmp/QDetective-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QDetective-0.1.0.tar", max compression
+gzip compressed data, was "QDetective-0.1.1.tar", max compression
```

## Comparing `QDetective-0.1.0.tar` & `QDetective-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1075 2023-04-07 06:32:40.671062 QDetective-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      327 2024-05-11 14:59:37.767132 QDetective-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     5208 2024-05-11 15:00:15.701022 QDetective-0.1.0/qdetective/__init__.py
--rw-r--r--   0        0        0      525 2024-05-11 15:02:19.705232 QDetective-0.1.0/setup.py
--rw-r--r--   0        0        0      271 2024-05-11 15:02:19.705363 QDetective-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1075 2023-04-07 06:32:40.671062 QDetective-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      327 2024-05-12 04:05:58.566462 QDetective-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     5372 2024-05-12 04:01:54.065545 QDetective-0.1.1/qdetective/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-12 04:06:01.541521 QDetective-0.1.1/setup.py
+-rw-r--r--   0        0        0      271 2024-05-12 04:06:01.541608 QDetective-0.1.1/PKG-INFO
```

### Comparing `QDetective-0.1.0/LICENSE.txt` & `QDetective-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QDetective-0.1.0/qdetective/__init__.py` & `QDetective-0.1.1/qdetective/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 Email: suliang_321@sina.com
 
 TO: QDer, GO GO GO!
 
 """
 
-__version__ = '0.1.0'
-
 import csv
 import paramiko
 import warnings
 warnings.filterwarnings('ignore')
 import pandas as pd
 import datetime as dt
 
@@ -37,16 +35,18 @@
         
         try:
             ssh = paramiko.SSHClient()
             ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())   # 这句话很重要，否则无法识别
             ssh.connect(self.host, self.port, self.username, self.password)
             ssh.close()
             print("【{}】已成功链接服务器...有问题请联系suliang".format(username))
+            self.get_factor_info()
         except:
             print("服务器下线，请联系管理员")
+            ssh.close()
     
     def get_factor_info(self):
         ssh = paramiko.SSHClient()
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())   # 这句话很重要，否则无法识别
         ssh.connect(self.host, self.port, self.username, self.password)
         sftp = ssh.open_sftp()
         
@@ -58,15 +58,14 @@
             file_list = sorted([x.split(' ')[-1].split('.')[0] for x in sftp.listdir('【量化大侦探】因子库/{}'.format(factor_name))])
             if len(file_list) == 0:
                 continue
             result.append((factor_name, min(file_list), max(file_list)))
             # result.loc[factor_name, '起始日期'], result.loc[factor_name, '最新日期'] = min(file_list), max(file_list)
         
         result = pd.DataFrame(result, columns=['因子名称', '起始日期', '最新日期']).set_index(['因子名称'])
-        print(result)
         self.contents = result
         ssh.close()
         return None
     
     def get_factor(self, factor_name, start_date='20180101', end_date=None):
         ssh = paramiko.SSHClient()
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())   # 这句话很重要，否则无法识别
@@ -88,19 +87,22 @@
             end_date = dt.datetime.now().strftime('%Y%m%d')   # 取当前最新一期
             temp_date_list = sorted(date_list[(date_list>=start_date)&(date_list<=end_date)])
         elif isinstance(end_date, list):
             temp_date_list = sorted(set(end_date).intersection(set(date_list)))
         else:
             temp_date_list = sorted(date_list[(date_list>=start_date)&(date_list<=end_date)])
         
-        # 读取数据, 速度可能偏慢
-        result = []
-        for date in tqdm(temp_date_list):
-            result.append(read_file(sftp, r'/【量化大侦探】因子库/{}/{}.csv'.format(factor_name, date)))
-        result = pd.concat(result,keys=temp_date_list,names=['日期']).reset_index().set_index(['日期', '﻿证券代码'])['因子暴露'].unstack()
+        try:
+            # 读取数据, 速度可能偏慢
+            result = []
+            for date in tqdm(temp_date_list):
+                result.append(read_file(sftp, r'/【量化大侦探】因子库/{}/{}.csv'.format(factor_name, date)))
+            result = pd.concat(result,keys=temp_date_list,names=['日期']).reset_index().set_index(['日期', '﻿证券代码'])['因子暴露'].unstack()
+        except PermissionError:
+            print('权限错误，无法提取该因子，请与管理员联系！')
         
         ssh.close()
         return result
     
     def download_file(self, remotepath, localpath):
         """
         remotepath: 远程路径
@@ -132,8 +134,8 @@
         return None
 
     
 
 if __name__ == '__main__':
     pass
     
-    
+
```

### Comparing `QDetective-0.1.0/setup.py` & `QDetective-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['qdetective']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'qdetective',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '量化大侦探-数据通道',
     'long_description': None,
     'author': 'suliang',
     'author_email': 'suliang_321@sina.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

