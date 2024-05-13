# Comparing `tmp/aiobiketrax-1.1.2a1.tar.gz` & `tmp/aiobiketrax-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobiketrax-1.1.2a1.tar", max compression
+gzip compressed data, was "aiobiketrax-1.2.0.tar", max compression
```

## Comparing `aiobiketrax-1.1.2a1.tar` & `aiobiketrax-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-1.1.2a1/LICENSE.md
--rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-1.1.2a1/README.md
--rw-r--r--   0        0        0       55 2023-10-27 21:51:03.558293 aiobiketrax-1.1.2a1/aiobiketrax/__init__.py
--rw-r--r--   0        0        0    19826 2023-08-28 19:46:34.220687 aiobiketrax-1.1.2a1/aiobiketrax/api.py
--rw-r--r--   0        0        0     4697 2023-08-27 21:25:07.956316 aiobiketrax-1.1.2a1/aiobiketrax/cli.py
--rw-r--r--   0        0        0    16863 2023-10-27 21:49:19.260352 aiobiketrax-1.1.2a1/aiobiketrax/client.py
--rw-r--r--   0        0        0      163 2023-08-27 21:25:07.957706 aiobiketrax-1.1.2a1/aiobiketrax/consts.py
--rw-r--r--   0        0        0      412 2023-08-27 21:25:07.958448 aiobiketrax-1.1.2a1/aiobiketrax/exceptions.py
--rw-r--r--   0        0        0    34146 2023-10-27 21:49:19.254344 aiobiketrax-1.1.2a1/aiobiketrax/models.py
--rw-r--r--   0        0        0      984 2023-10-27 21:51:03.558588 aiobiketrax-1.1.2a1/pyproject.toml
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 aiobiketrax-1.1.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-1.2.0/README.md
+-rw-r--r--   0        0        0       53 2024-05-13 19:54:50.153267 aiobiketrax-1.2.0/aiobiketrax/__init__.py
+-rw-r--r--   0        0        0    19826 2024-01-24 21:38:06.690061 aiobiketrax-1.2.0/aiobiketrax/api.py
+-rw-r--r--   0        0        0     4774 2024-05-10 12:40:51.265662 aiobiketrax-1.2.0/aiobiketrax/cli.py
+-rw-r--r--   0        0        0    16875 2024-05-10 12:08:40.740386 aiobiketrax-1.2.0/aiobiketrax/client.py
+-rw-r--r--   0        0        0      163 2024-01-24 21:38:06.692494 aiobiketrax-1.2.0/aiobiketrax/consts.py
+-rw-r--r--   0        0        0      412 2024-01-24 21:38:06.693226 aiobiketrax-1.2.0/aiobiketrax/exceptions.py
+-rw-r--r--   0        0        0    33955 2024-05-10 12:17:11.768767 aiobiketrax-1.2.0/aiobiketrax/models.py
+-rw-r--r--   0        0        0      982 2024-05-13 19:54:33.294821 aiobiketrax-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 aiobiketrax-1.2.0/PKG-INFO
```

### Comparing `aiobiketrax-1.1.2a1/LICENSE.md` & `aiobiketrax-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.1.2a1/README.md` & `aiobiketrax-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.1.2a1/aiobiketrax/api.py` & `aiobiketrax-1.2.0/aiobiketrax/api.py`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.1.2a1/aiobiketrax/cli.py` & `aiobiketrax-1.2.0/aiobiketrax/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
                         for key, value in set(current.items()) - set(last.items())
                     }
 
                     if updates:
                         sys.stdout.write(pprint.pformat(updates) + "\n")
 
                 event.clear()
+        except (asyncio.CancelledError, KeyboardInterrupt):
+            pass
         finally:
             await account.stop()
 
 
 async def command_trips(arguments: argparse.Namespace):
     async with aiohttp.ClientSession() as session:
         account = Account(
```

### Comparing `aiobiketrax-1.1.2a1/aiobiketrax/client.py` & `aiobiketrax-1.2.0/aiobiketrax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,29 +190,29 @@
 
     async def update_position(self) -> None:
         """
         Update the position information of the device.
         """
         _LOGGER.debug("Updating positions of device %s.", self._id)
 
-        self._account._positions[
-            self._id
-        ] = await self._account.traccar_api.get_position(
-            self._id, self._device.position_id
+        self._account._positions[self._id] = (
+            await self._account.traccar_api.get_position(
+                self._id, self._device.position_id
+            )
         )
 
     async def update_subscription(self) -> None:
         """
         Update the subscription information of the device.
         """
         _LOGGER.debug("Updating subscription of device %s.", self._id)
 
-        self._account._subscriptions[
-            self._id
-        ] = await self._account.admin_api.get_subscription(self._device.unique_id)
+        self._account._subscriptions[self._id] = (
+            await self._account.admin_api.get_subscription(self._device.unique_id)
+        )
 
     async def update_trips(
         self, from_date: datetime = None, to_date: datetime = None
     ) -> None:
         """
         Update the trips information of the device.
```

### Comparing `aiobiketrax-1.1.2a1/aiobiketrax/models.py` & `aiobiketrax-1.2.0/aiobiketrax/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
 def to_float(x: Any) -> float:
-    assert isinstance(x, float)
+    assert isinstance(x, (int, float))
     return x
 
 
 def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
     assert isinstance(x, dict)
     return {k: f(v) for (k, v) in x.items()}
 
@@ -602,15 +602,14 @@
         return result
 
 
 @dataclass
 class Device:
     attributes: DeviceAttributes
     disabled: bool
-    geofence_ids: List[Any]
     group_id: int
     id: int
     last_update: datetime
     name: str
     position_id: int
     status: str
     unique_id: str
@@ -620,30 +619,28 @@
     phone: Optional[str] = None
 
     @staticmethod
     def from_dict(obj: Any) -> "Device":
         assert isinstance(obj, dict)
         attributes = DeviceAttributes.from_dict(obj.get("attributes"))
         disabled = from_bool(obj.get("disabled"))
-        geofence_ids = from_list(lambda x: x, obj.get("geofenceIds"))
         group_id = from_int(obj.get("groupId"))
         id = from_int(obj.get("id"))
         last_update = from_datetime(obj.get("lastUpdate"))
         name = from_str(obj.get("name"))
         position_id = from_int(obj.get("positionId"))
         status = from_str(obj.get("status"))
         unique_id = from_str(obj.get("uniqueId"))
         category = from_union([from_none, from_str], obj.get("category"))
         contact = from_union([from_none, from_str], obj.get("contact"))
         model = from_union([from_none, from_str], obj.get("model"))
         phone = from_union([from_none, from_str], obj.get("phone"))
         return Device(
             attributes,
             disabled,
-            geofence_ids,
             group_id,
             id,
             last_update,
             name,
             position_id,
             status,
             unique_id,
@@ -653,15 +650,14 @@
             phone,
         )
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["attributes"] = to_class(DeviceAttributes, self.attributes)
         result["disabled"] = from_bool(self.disabled)
-        result["geofenceIds"] = from_list(lambda x: x, self.geofence_ids)
         result["groupId"] = from_int(self.group_id)
         result["id"] = from_int(self.id)
         result["lastUpdate"] = self.last_update.isoformat()
         result["name"] = from_str(self.name)
         result["positionId"] = from_int(self.position_id)
         result["status"] = from_str(self.status)
         result["uniqueId"] = from_str(self.unique_id)
```

### Comparing `aiobiketrax-1.1.2a1/pyproject.toml` & `aiobiketrax-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [tool.black]
 line-length = 88
-target-version = ["py39"]
+target-version = ["py312"]
 exclude = '''
 (
     \.git/
   | \.vscode/
   | env/
 )
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "aiobiketrax"
-version = "1.1.2a1"
+version = "1.2.0"
 description = "Python library for interacting with the PowUnity BikeTrax GPS tracker."
 authors = ["Bas Stottelaar <basstottelaar@gmail.com>"]
 keywords = ["biketrax", "powunity", "asyncio", "iot", "gps"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/basilfx/aiobiketrax"
 repository = "https://github.com/basilfx/aiobiketrax"
 include = [
     "LICENSE.md",
 ]
 
 [tool.poetry.dependencies]
-aiohttp = "^3.8.1"
-auth0-python = "^3.23.1"
-python = "^3.9"
-PyJWT = "^2.4.0"
-python-dateutil = "^2.8.2"
-
-[tool.poetry.dev-dependencies]
-black = "^23.7.0"
-isort = "^5.12.0"
-pytest = "^7.4"
-flake8 = "^6.0.0"
-flake8-mypy = "^17.8.0"
+aiohttp = "3.9.5"
+auth0-python = "^3.24.0"
+python = "^3.12"
+PyJWT = "^2.8.0"
+python-dateutil = "^2.9.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^24.2.0"
+isort = "^5.13.0"
+pytest = "^8.2"
+flake8 = "^7.0.0"
+mypy = "^1.10.0"
 
 [tool.poetry.scripts]
 biketrax = 'aiobiketrax.cli:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aiobiketrax-1.1.2a1/PKG-INFO` & `aiobiketrax-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: aiobiketrax
-Version: 1.1.2a1
+Version: 1.2.0
 Summary: Python library for interacting with the PowUnity BikeTrax GPS tracker.
 Home-page: https://github.com/basilfx/aiobiketrax
 License: MIT
 Keywords: biketrax,powunity,asyncio,iot,gps
 Author: Bas Stottelaar
 Author-email: basstottelaar@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: auth0-python (>=3.23.1,<4.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyJWT (>=2.8.0,<3.0.0)
+Requires-Dist: aiohttp (==3.9.5)
+Requires-Dist: auth0-python (>=3.24.0,<4.0.0)
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Project-URL: Repository, https://github.com/basilfx/aiobiketrax
 Description-Content-Type: text/markdown
 
 # aiobiketrax
 Python library for interacting with the PowUnity BikeTrax GPS tracker.
 
 [![Linting](https://github.com/basilfx/aiobiketrax/actions/workflows/lint.yml/badge.svg)](https://github.com/basilfx/aiobiketrax/actions/workflows/lint.yml)
```

