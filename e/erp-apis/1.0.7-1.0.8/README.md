# Comparing `tmp/erp_apis-1.0.7-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11006 bytes, number of entries: 15
+Zip file size: 11298 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
--rw-rw-rw-  2.0 fat     3499 b- defN 24-May-07 06:09 erp_apis/erpRequest.py
+-rw-rw-rw-  2.0 fat     3577 b- defN 24-May-08 03:10 erp_apis/erpRequest.py
 -rw-rw-rw-  2.0 fat      143 b- defN 24-May-07 03:26 erp_apis/apis/__init__.py
 -rw-rw-rw-  2.0 fat     2587 b- defN 24-May-07 06:09 erp_apis/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     1538 b- defN 24-May-07 06:09 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-07 03:18 erp_apis/apis/inventory.py
--rw-rw-rw-  2.0 fat     3701 b- defN 24-May-07 06:09 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat     1994 b- defN 24-May-07 06:09 erp_apis/apis/test.py
--rw-rw-rw-  2.0 fat      789 b- defN 24-May-07 06:09 erp_apis/apis/user.py
+-rw-rw-rw-  2.0 fat     4346 b- defN 24-May-08 06:17 erp_apis/apis/order.py
+-rw-rw-rw-  2.0 fat     2091 b- defN 24-May-08 06:19 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat     1139 b- defN 24-May-07 12:41 erp_apis/apis/user.py
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-30 10:11 erp_apis/utils/__init__.py
--rw-rw-rw-  2.0 fat     2042 b- defN 24-May-06 03:23 erp_apis/utils/util.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 06:10 erp_apis-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 06:10 erp_apis-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-May-07 06:10 erp_apis-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1177 b- defN 24-May-07 06:10 erp_apis-1.0.7.dist-info/RECORD
-15 files, 20737 bytes uncompressed, 9076 bytes compressed:  56.2%
+-rw-rw-rw-  2.0 fat     2063 b- defN 24-May-08 06:18 erp_apis/utils/util.py
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1178 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/RECORD
+15 files, 21929 bytes uncompressed, 9368 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: erp_apis/utils/__init__.py
 Comment: 
 
 Filename: erp_apis/utils/util.py
 Comment: 
 
-Filename: erp_apis-1.0.7.dist-info/METADATA
+Filename: erp_apis-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.7.dist-info/WHEEL
+Filename: erp_apis-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.7.dist-info/top_level.txt
+Filename: erp_apis-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.7.dist-info/RECORD
+Filename: erp_apis-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/erpRequest.py

```diff
@@ -5,15 +5,15 @@
 # Date ：2024-04-09 11:20
 # IDE：PyCharm
 import os
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
 from lxml import etree
-from requests import Session as S, Request as R
+from requests import Session as S, Request as Req, Response as Res
 import time, json as j
 from erp_apis.config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
 
 
 @dataclass
 class UserInfoType:
     u_cid: Optional[str]
@@ -32,15 +32,15 @@
         self.headers.update(DEFAULT_HEADERS)
         self.proxies = {'http': "", 'https': ""}
         self.viewstateItems = dict()
         self.userInfo : Optional[UserInfoType]
 
 
 
-    def erpSend(self, request:R, **kwargs) -> R:
+    def erpSend(self, request:Req, **kwargs) -> Res:
         if not request.headers: request.headers = self.headers
         hostType = getattr(request, 'hostType', None)
         if hostType:
             resp = getattr(self, hostType + "Send", None)(request, **kwargs)
             if resp is None:
                 raise Exception(f"{hostType}没有这个域的send方法")
             return resp
@@ -58,15 +58,16 @@
         return res
 
     def erpApiSend(self, request, **kwargs) :
         request.url = urljoin(ErpApiBaseUrl, request.url)
         res = super().send(self.prepare_request(request), **kwargs)
         if request.callback:
             if request.callback == 'login':
-                self.userInfo = UserInfoType(**res.json().get('cookie'))
+                if res.json().get('code') == 0:
+                    self.userInfo = UserInfoType(**res.json().get('cookie'))
             else:
                 return request.callback(res)
         return res
 
     def get_viewstate(self, url):
         if self.viewstateItems.get(url) and self.viewstateItems.get(url).get("updateTime") > time.time() - 60 * 5:
             return self.viewstateItems.get(url)
@@ -85,15 +86,15 @@
                 "__VIEWSTATEGENERATOR": extract_first("//*[@id='__VIEWSTATEGENERATOR']/@value"),
                 "__EVENTVALIDATION": extract_first("//*[@id='__EVENTVALIDATION']/@value"),
             }
         )
         return self.viewstateItems.get(url)
 
 
-class Request(R):
+class Request(Req):
 
     def __init__(self,
                  hostType: str = 'erp321',
                  callback: callable=None,
                  **kwargs
         ):
         self.hostType = hostType
```

## erp_apis/apis/order.py

```diff
@@ -4,21 +4,32 @@
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 订单API
 from typing import Optional, Union
 from erp_apis.erpRequest import Request
 from erp_apis.utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
-def OrderRequest(data: dict, method: str = 'LoadDataToJSON') -> Request:
+
+
+def OrderRequest(
+        data: dict,
+        method: str = 'LoadDataToJSON',
+        url='/app/order/order/list.aspx',
+        callbackid: str = 'JTable1',
+        **kwargs
+) -> Request:
+    params = getDefaultParams({'defaultParams': ["ts___", "_c"], 'am___': method})
+    if kwargs.get('params'):
+        params.update(kwargs.get('params'))
     return Request(
         method='POST',
-        url='/app/order/order/list.aspx',
-        params=getDefaultParams({'defaultParams': ["ts___", "_c"], 'am___': method}),
+        url=url,
+        params=params,
         data={
-            '__CALLBACKID': 'JTable1',
+            '__CALLBACKID': callbackid,
             **data
         },
         callback=JTable1
     )
 
 
 # 获取订单
@@ -115,7 +126,24 @@
     :return: 执行结果
     '''
     return OrderRequest({
         '__CALLBACKPARAM': dumps({"Method": "ChangeBatchItem",
                                   "Args": [str(oid), dumps({"items": generateChangeBatchItems(items, newBatchItems)})],
                                   "CallControl": "{page}"}),
     }, method='ChangeBatchItem')
+
+
+# 获取单号物流信息
+def LogisticsInfo(params: dict):
+    '''
+    获取单号物流信息
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return OrderRequest(
+        url='/app/order/order/lookExpress.aspx',
+        params=params,
+        data={
+            '__CALLBACKPARAM': dumps({"Method": "LoadTrace", "CallControl": "{page}"}),
+        }, method='LoadTrace',
+        callbackid='ACall1'
+    )
```

## erp_apis/apis/test.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # Project：erp_out_of_stock
 # File：test.py
 # Author：李福成
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
 from apis.inventory import WmsSkuStock
-from apis.order import OrderList, ChangeBatchItems
+from apis.order import OrderList, ChangeBatchItems, LogisticsInfo
 from erp_apis.apis.user import login
 from apis.afterSales import aftersaleList, aftersaleCommon, clearException
 from erp_apis.apis.goods import ItemList
 from erpRequest import Session
 
 if __name__ == '__main__':
     session = Session()
@@ -36,10 +36,15 @@
     #     "c": "@="}, {"k": "status", "v": "waitconfirm", "c": "@="}, {"k": "type", "v": "换货", "c": "@="},
     #     {"k": "shop_type", "v": "换货", "c": "@="}, {"k": "as_date", "v": "30天前", "c": ">=", "t": "date"},
     #     {"k": "as_date", "v": "今天 23:59:59.999", "c": "<=", "t": "date"}])
     # )
     # res = session.erpSend(aftersaleCommon(1452451077))
     # res = session.erpSend(clearException(1452451077))
 
-
-    res = session.erp321Send(ItemList(queryData=[{"k":"shop_i_id","v":"793265551325","c":"@="}]))
+    res = session.erpSend(LogisticsInfo(
+        {
+            "from": "aftersale",
+            "l_id": "78791674020636",
+            "l_name": "中通速递"
+        }
+    ))
     print(res.json())
```

## erp_apis/apis/user.py

```diff
@@ -28,9 +28,24 @@
             },
             "ipAddress": ""
         },
         callback='login',
         hostType='erpApi'
     )
 
+def getUserInfo(coid: int,uid: int):
+    '''
+    获取用户信息
+    :return:
+    '''
+    return Request(
+        method='post',
+        url='https://api.erp321.com/erp/webapi/UserApi/Passport/GetUserInfo',
+        json={
+          "data": {},
+          "uid": uid,
+          "coid": coid
+        },
+        hostType='erpApi'
+    )
```

## erp_apis/utils/util.py

```diff
@@ -27,14 +27,15 @@
         for k in params.get('defaultParams'):
             params.update({k: rand_params.get(k)()})
     del params['defaultParams']
     return params
 
 
 def JTable1(res: Response):
+    print(res.text)
     res_data = json.loads(res.text[2:])
     if res_data.get('ReturnValue'):
         try:res_data['ReturnValue'] = json.loads(res_data.get('ReturnValue'))
         except:pass
     res._content = json.dumps(res_data).encode('utf-8')
     return res
```

## Comparing `erp_apis-1.0.7.dist-info/METADATA` & `erp_apis-1.0.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.7
+Version: 1.0.8
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis-1.0.7.dist-info/RECORD` & `erp_apis-1.0.8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 erp_apis/config.py,sha256=tXtGQtsW-Wdbhh2X1AKyGx_X8B_ShMvdVF4rOXf8zDg,403
-erp_apis/erpRequest.py,sha256=DmOUXyF8LQpH2J6o51IjXyeSJbrYJtI5_Ei2lPTOGvo,3499
+erp_apis/erpRequest.py,sha256=RDCcdYiW7doHGZBoIRG97WSXg7suuIKoZSlgy9FMCMQ,3577
 erp_apis/apis/__init__.py,sha256=L6HaO-zN2-mMbaZUFJ8YFFgFScFE4aizJCVPed8CluY,143
 erp_apis/apis/afterSales.py,sha256=biTQql3R1JgOS4fluuOT76F40Fu3KA8KggmLYrE68as,2587
 erp_apis/apis/goods.py,sha256=3HplLv-feqNMiV46ANuzhRfL9RDiOovF8RAAvNydmdI,1538
 erp_apis/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
-erp_apis/apis/order.py,sha256=GNhF3DHJs8OCsyakmD_JYVPP8Ht9HFtgEwcQqpLcFd0,3701
-erp_apis/apis/test.py,sha256=6zjx7ly0Se7IKqa9MHY1XnPFWm3taL9D-0fL1CR2UAg,1994
-erp_apis/apis/user.py,sha256=hvlgD9vBvdVt_zm2Rrqge8fsugvuj6TYaIwTgxyk7dQ,789
+erp_apis/apis/order.py,sha256=ybUJ8i1oSsu9TfP4HE99HFk8sbiO8qWy4f8ssdBFzM0,4346
+erp_apis/apis/test.py,sha256=ZrR-jcO6S6xGulPVMoVdAr7RAAyuuCux9UhGto2viZc,2091
+erp_apis/apis/user.py,sha256=vosgBp1QNesLIRMQyafe9y9PDFJyIjpPdmiE1jvVzOA,1139
 erp_apis/utils/__init__.py,sha256=4OS0q-GbgI0b14i4ErUYKUo-t1jzw8wSvtJZu3nXSMM,141
-erp_apis/utils/util.py,sha256=FL8-Mo2CZWR-Pv09hqxgTE7oQVhNt6tl2AJolFdZE30,2042
-erp_apis-1.0.7.dist-info/METADATA,sha256=W60IId7E9-c2Yc4t1Ygqu5_0-s_UvIgIu5_Hc9nyVMs,1580
-erp_apis-1.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis-1.0.7.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
-erp_apis-1.0.7.dist-info/RECORD,,
+erp_apis/utils/util.py,sha256=xkmwXqGWbh7Qz_rRtXk5BclnvQz8PgMaS73UpR-Fm4s,2063
+erp_apis-1.0.8.dist-info/METADATA,sha256=7CqHa7TXkoBoLldT-L-MESKiUAJzcD_Vma36fdKt264,1580
+erp_apis-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis-1.0.8.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
+erp_apis-1.0.8.dist-info/RECORD,,
```

