# Comparing `tmp/redis_cached-0.4.0.tar.gz` & `tmp/redis_cached-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_cached-0.4.0.tar", max compression
+gzip compressed data, was "redis_cached-0.4.1.tar", max compression
```

## Comparing `redis_cached-0.4.0.tar` & `redis_cached-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.4.0/LICENSE
--rw-r--r--   0        0        0     2185 2024-04-26 07:30:19.823667 redis_cached-0.4.0/README.md
--rw-r--r--   0        0        0      623 2024-04-26 07:30:19.824574 redis_cached-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-26 07:30:19.824920 redis_cached-0.4.0/redis_cached/__init__.py
--rw-r--r--   0        0        0     3378 2024-04-26 07:30:19.825139 redis_cached-0.4.0/redis_cached/core.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 redis_cached-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2185 2024-04-26 07:30:19.823667 redis_cached-0.4.1/README.md
+-rw-r--r--   0        0        0      623 2024-05-13 05:29:42.499211 redis_cached-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-26 07:30:19.824920 redis_cached-0.4.1/redis_cached/__init__.py
+-rw-r--r--   0        0        0     3824 2024-05-13 05:25:28.120681 redis_cached-0.4.1/redis_cached/core.py
+-rw-r--r--   0        0        0      368 2024-05-13 05:14:17.333310 redis_cached-0.4.1/redis_cached/utils.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 redis_cached-0.4.1/PKG-INFO
```

### Comparing `redis_cached-0.4.0/LICENSE` & `redis_cached-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_cached-0.4.0/README.md` & `redis_cached-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_cached-0.4.0/pyproject.toml` & `redis_cached-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-cached"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python cache decorator and other itils with support for Redis or KeyDB"
 authors = ["Dmitry Babanov <85852989+dmitrybabanovforreal@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/dmitrybabanovforreal/redis-cached"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `redis_cached-0.4.0/redis_cached/core.py` & `redis_cached-0.4.1/redis_cached/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from typing import Callable, TypeVar, Coroutine, Any, ParamSpec, TypeAlias
-import asyncio, inspect, functools, hashlib, pickle, os
+import asyncio, inspect, functools, hashlib, pickle, os, logging
 
 from redis.asyncio.client import Redis
 
+from redis_cached.utils import lock_release_retry
 
+
+logger = logging.getLogger('redis_cached')
 _P = ParamSpec('_P')
 _R = TypeVar('_R')
 _AsyncFunc: TypeAlias = Callable[_P, Coroutine[Any, Any, _R]]
 
 
 class KeyNotFound(Exception):
     pass
 
 
 class Cache:
-    def __init__(self, cache_key_salt: str = '', redis_: Redis = None):
+    def __init__(
+        self,
+        cache_key_salt: str = '',
+        redis_: Redis = None,
+        cache_refresh_lock_timeout: int = 5
+    ):
         self.cache_key_salt = cache_key_salt
+        self.cache_refresh_lock_timeout = cache_refresh_lock_timeout
         if redis_:
             assert isinstance(redis_, Redis), '`redis_` has to be an instance of redis.asyncio.client.Redis'
             self.redis = redis_
         else:
             host = os.getenv('REDIS_HOST')
             assert host, 'REDIS_HOST env var not found'
             self.redis = Redis(
@@ -61,26 +70,28 @@
         for k, v in sorted(kwargs.items()):
             key_parts += f':{k}'.encode('utf-8')
             key_parts += pickle.dumps(v)
         key_hash = hashlib.sha256(key_parts).hexdigest()
         return key_hash
 
     async def _get_value(self, key: str, func: _AsyncFunc, kwargs: dict, ttl: int) -> _R:
-        while 1:
+        while True:
             try:
                 return await self._redis_get(key)
             except KeyNotFound:
-                lock = self.redis.lock(name=f'{key}_lock', blocking=False)
+                lock_key = f'{key}_lock'
+                lock = self.redis.lock(name=lock_key, blocking=False, timeout=self.cache_refresh_lock_timeout)
                 if await lock.acquire():
                     try:
                         result = await func(**kwargs)
                         await self._redis_set(name=key, value=result, ex=ttl)
+                        return result
                     finally:
-                        await lock.release()
-                    return result
+                        if not await lock_release_retry(lock):
+                            logger.error(f'Failed to release cache refresh lock for {lock_key}')
                 else:
                     await asyncio.sleep(0.1)
 
     async def _redis_get(self, name: str) -> Any:
         res = await self.redis.get(name)
         if not res:
             raise KeyNotFound()
```

### Comparing `redis_cached-0.4.0/PKG-INFO` & `redis_cached-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-cached
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python cache decorator and other itils with support for Redis or KeyDB
 Home-page: https://github.com/dmitrybabanovforreal/redis-cached
 Author: Dmitry Babanov
 Author-email: 85852989+dmitrybabanovforreal@users.noreply.github.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

