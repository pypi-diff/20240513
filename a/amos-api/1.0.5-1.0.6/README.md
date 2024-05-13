# Comparing `tmp/amos_api-1.0.5.tar.gz` & `tmp/amos_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amos_api-1.0.5.tar", last modified: Wed May  8 08:45:57 2024, max compression
+gzip compressed data, was "amos_api-1.0.6.tar", last modified: Mon May 13 06:25:40 2024, max compression
```

## Comparing `amos_api-1.0.5.tar` & `amos_api-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:45:57.755013 amos_api-1.0.5/
--rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.5/.gitignore
--rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1927 2024-05-08 08:45:57.755013 amos_api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1475 2024-05-08 08:45:52.000000 amos_api-1.0.5/README.md
--rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.5/_descr.md
--rw-rw-rw-   0        0        0      565 2024-05-08 08:44:26.000000 amos_api-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 08:45:57.755013 amos_api-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 08:45:57.750022 amos_api-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 08:45:57.754017 amos_api-1.0.5/src/amos_api.egg-info/
--rw-rw-rw-   0        0        0     1927 2024-05-08 08:45:57.000000 amos_api-1.0.5/src/amos_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-08 08:45:57.000000 amos_api-1.0.5/src/amos_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:45:57.000000 amos_api-1.0.5/src/amos_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 08:45:57.000000 amos_api-1.0.5/src/amos_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-08 08:45:57.000000 amos_api-1.0.5/src/amos_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2024-05-08 08:22:51.000000 amos_api-1.0.5/src/amos_api.py
--rw-rw-rw-   0        0        0      599 2024-05-08 08:44:20.000000 amos_api-1.0.5/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:40.879440 amos_api-1.0.6/
+-rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.6/.gitignore
+-rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2498 2024-05-13 06:25:40.879440 amos_api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2012 2024-05-13 06:23:34.000000 amos_api-1.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.6/_descr.md
+-rw-rw-rw-   0        0        0      625 2024-05-13 06:25:16.000000 amos_api-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:25:40.880436 amos_api-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:40.873942 amos_api-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 06:25:40.878438 amos_api-1.0.6/src/amos_api.egg-info/
+-rw-rw-rw-   0        0        0     2498 2024-05-13 06:25:40.000000 amos_api-1.0.6/src/amos_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-13 06:25:40.000000 amos_api-1.0.6/src/amos_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:25:40.000000 amos_api-1.0.6/src/amos_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 06:25:40.000000 amos_api-1.0.6/src/amos_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 06:25:40.000000 amos_api-1.0.6/src/amos_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2024-05-13 06:10:14.000000 amos_api-1.0.6/src/amos_api.py
+-rw-rw-rw-   0        0        0     2666 2024-05-13 06:10:14.000000 amos_api-1.0.6/src/utils.py
```

### Comparing `amos_api-1.0.5/PKG-INFO` & `amos_api-1.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 Metadata-Version: 2.1
 Name: amos_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: AMOS common api
-Author-email: "ilex.h" <390132625@qq.com>
+Author-email: "ilex.h" <390132625@qq.com>, leavor <lint.hit@163.com>
 Project-URL: Homepage, https://github.com/aptray/python-pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Requires-Dist: pydantic
+Requires-Dist: pydantic==2.6.4
 
 # amos api
 
 主要用于定义离线分析中的 API 规范以及通用的 Response 等
 
 ## 快速开始
 
 ```py
+import logging
 from fastapi import (FastAPI, Body)
-from amos_api import (BaseResponse, HttpCode)
+from fastapi.responses import JSONResponse
+from pydantic import ValidationError
+
+from amos_api import (
+    ResponseBase,
+    ResponseOK,
+    ResponseValidationError,
+    ResponseAlgorithmError,
+    CheckAssertionError,
+    CheckValueError
+)
+
 from starlette.responses import RedirectResponse
 
+logger = logging.getLogger()
+
 async def document():
     # return RedirectResponse(url="/docs")
     return RedirectResponse(url="/redoc")
 
 def mount_app_routes(app: FastAPI):
     app.get("/",
-            response_model=BaseResponse,
+            response_model=ResponseBase,
             summary="swagger 文档")(document)
     # tag items
     app.post("/user",
              tags=["User"],
              summary="用户信息",
              )(userInfo)
 
-async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
-    return BaseResponse(data={"seq":"1", "name": name,})
+async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
+    return ResponseBase(data={"seq":"1", "name": name,})
 
-async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
+async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
     try:
         dblist()
+        return ResponseOK(data=[])
     except Exception as e:
-        msg = f"未知错误{e}"
-        return BaseResponse(code=HttpCode._500, msg=msg)
-    return BaseResponse(data=[])
+        if isinstance(e, (ValidationError, CheckAssertionError, CheckValueError)):
+            ret = ResponseValidationError(data='校验错误的详细信息')
+        else:
+            ret = ResponseAlgorithmError(data='算法错误的详细信息')
+        logger.error() #错误日志
+        return JSONResponse(status_code=ret.code, content=ret.model_dump())
 ```
 
-- `HttpCode._200` 请求成功,正常 code 值，BaseResponse 如果不设置code时，默认值。
+- `HttpCode._200` 请求成功,正常 code 值，ResponseBase 如果不设置code时，默认值。
 - `HttpCode._400` 错误的请求，比如参数错误
 - `HttpCode._403` 禁止访问的资源
 - `HttpCode._404` 未找到
 - `HttpCode._422` 常用于参数错误
 - `HttpCode._500` 服务器错误，内部错误
 - `HttpCode._522` 服务器错误，内部错误
```

### Comparing `amos_api-1.0.5/README.md` & `amos_api-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 # amos api
 
 主要用于定义离线分析中的 API 规范以及通用的 Response 等
 
 ## 快速开始
 
 ```py
+import logging
 from fastapi import (FastAPI, Body)
-from amos_api import (BaseResponse, HttpCode)
+from fastapi.responses import JSONResponse
+from pydantic import ValidationError
+
+from amos_api import (
+    ResponseBase,
+    ResponseOK,
+    ResponseValidationError,
+    ResponseAlgorithmError,
+    CheckAssertionError,
+    CheckValueError
+)
+
 from starlette.responses import RedirectResponse
 
+logger = logging.getLogger()
+
 async def document():
     # return RedirectResponse(url="/docs")
     return RedirectResponse(url="/redoc")
 
 def mount_app_routes(app: FastAPI):
     app.get("/",
-            response_model=BaseResponse,
+            response_model=ResponseBase,
             summary="swagger 文档")(document)
     # tag items
     app.post("/user",
              tags=["User"],
              summary="用户信息",
              )(userInfo)
 
-async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
-    return BaseResponse(data={"seq":"1", "name": name,})
+async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
+    return ResponseBase(data={"seq":"1", "name": name,})
 
-async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
+async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
     try:
         dblist()
+        return ResponseOK(data=[])
     except Exception as e:
-        msg = f"未知错误{e}"
-        return BaseResponse(code=HttpCode._500, msg=msg)
-    return BaseResponse(data=[])
+        if isinstance(e, (ValidationError, CheckAssertionError, CheckValueError)):
+            ret = ResponseValidationError(data='校验错误的详细信息')
+        else:
+            ret = ResponseAlgorithmError(data='算法错误的详细信息')
+        logger.error() #错误日志
+        return JSONResponse(status_code=ret.code, content=ret.model_dump())
 ```
 
-- `HttpCode._200` 请求成功,正常 code 值，BaseResponse 如果不设置code时，默认值。
+- `HttpCode._200` 请求成功,正常 code 值，ResponseBase 如果不设置code时，默认值。
 - `HttpCode._400` 错误的请求，比如参数错误
 - `HttpCode._403` 禁止访问的资源
 - `HttpCode._404` 未找到
 - `HttpCode._422` 常用于参数错误
 - `HttpCode._500` 服务器错误，内部错误
 - `HttpCode._522` 服务器错误，内部错误
```

### Comparing `amos_api-1.0.5/pyproject.toml` & `amos_api-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "amos_api"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name = "ilex.h", email = "390132625@qq.com" },
+    { name = "leavor", email = "lint.hit@163.com" }
 ]
-dependencies = ['pydantic']
+dependencies = ['pydantic==2.6.4']
 description = "AMOS common api"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `amos_api-1.0.5/src/amos_api.egg-info/PKG-INFO` & `amos_api-1.0.6/src/amos_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 Metadata-Version: 2.1
 Name: amos_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: AMOS common api
-Author-email: "ilex.h" <390132625@qq.com>
+Author-email: "ilex.h" <390132625@qq.com>, leavor <lint.hit@163.com>
 Project-URL: Homepage, https://github.com/aptray/python-pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Requires-Dist: pydantic
+Requires-Dist: pydantic==2.6.4
 
 # amos api
 
 主要用于定义离线分析中的 API 规范以及通用的 Response 等
 
 ## 快速开始
 
 ```py
+import logging
 from fastapi import (FastAPI, Body)
-from amos_api import (BaseResponse, HttpCode)
+from fastapi.responses import JSONResponse
+from pydantic import ValidationError
+
+from amos_api import (
+    ResponseBase,
+    ResponseOK,
+    ResponseValidationError,
+    ResponseAlgorithmError,
+    CheckAssertionError,
+    CheckValueError
+)
+
 from starlette.responses import RedirectResponse
 
+logger = logging.getLogger()
+
 async def document():
     # return RedirectResponse(url="/docs")
     return RedirectResponse(url="/redoc")
 
 def mount_app_routes(app: FastAPI):
     app.get("/",
-            response_model=BaseResponse,
+            response_model=ResponseBase,
             summary="swagger 文档")(document)
     # tag items
     app.post("/user",
              tags=["User"],
              summary="用户信息",
              )(userInfo)
 
-async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
-    return BaseResponse(data={"seq":"1", "name": name,})
+async def userInfo(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
+    return ResponseBase(data={"seq":"1", "name": name,})
 
-async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> BaseResponse:
+async def userList(name: str=Body(..., description="用户名称", examples=["ray"])) -> ResponseBase:
     try:
         dblist()
+        return ResponseOK(data=[])
     except Exception as e:
-        msg = f"未知错误{e}"
-        return BaseResponse(code=HttpCode._500, msg=msg)
-    return BaseResponse(data=[])
+        if isinstance(e, (ValidationError, CheckAssertionError, CheckValueError)):
+            ret = ResponseValidationError(data='校验错误的详细信息')
+        else:
+            ret = ResponseAlgorithmError(data='算法错误的详细信息')
+        logger.error() #错误日志
+        return JSONResponse(status_code=ret.code, content=ret.model_dump())
 ```
 
-- `HttpCode._200` 请求成功,正常 code 值，BaseResponse 如果不设置code时，默认值。
+- `HttpCode._200` 请求成功,正常 code 值，ResponseBase 如果不设置code时，默认值。
 - `HttpCode._400` 错误的请求，比如参数错误
 - `HttpCode._403` 禁止访问的资源
 - `HttpCode._404` 未找到
 - `HttpCode._422` 常用于参数错误
 - `HttpCode._500` 服务器错误，内部错误
 - `HttpCode._522` 服务器错误，内部错误
```

