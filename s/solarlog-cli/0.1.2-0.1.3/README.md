# Comparing `tmp/solarlog_cli-0.1.2.tar.gz` & `tmp/solarlog_cli-0.1.3.tar.gz`

## Comparing `solarlog_cli-0.1.2.tar` & `solarlog_cli-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/__init__.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_client.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_connector.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_exceptions.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/src/solarlog_cli/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/src/solarlog_cli/solarlog_client.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/src/solarlog_cli/solarlog_connector.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/src/solarlog_cli/solarlog_exceptions.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/src/solarlog_cli/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.3/PKG-INFO
```

### Comparing `solarlog_cli-0.1.2/.github/workflows/pylint.yml` & `solarlog_cli-0.1.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.2/.github/workflows/python-publish.yml` & `solarlog_cli-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.2/.github/workflows/ruff.yml` & `solarlog_cli-0.1.3/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.2/src/solarlog_cli/solarlog_client.py` & `solarlog_cli-0.1.3/src/solarlog_cli/solarlog_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         except asyncio.TimeoutError as exception:
             msg = f"Timeout occurred while connecting to Solar-Log at {self.host}"
             raise SolarLogConnectionError(msg) from exception
 
         content_type = response.headers.get("Content-Type", "")
 
         if response.status != 200:
+            # pylint: disable-next=line-too-long
             msg = f"The server responded with error code {response.status} while fetching data from Solar-Log at {self.host}.\n{url}\n{header}\n{json_payload}"
             text = await response.text()
             raise SolarLogUpdateError(
                 msg,
                 {"Content-Type": content_type, "response": text},
             )
```

### Comparing `solarlog_cli-0.1.2/src/solarlog_cli/solarlog_connector.py` & `solarlog_cli-0.1.3/src/solarlog_cli/solarlog_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             )
 
         data["last_updated"] = data["last_updated"].astimezone(self.timezone)
 
         # print(f"basic data updated: {data}")
         if self.extended_data:
             data |= await self.client.get_energy()
-            if self._device_enabled is not {}:
+            if self._device_enabled != {} and self._device_enabled is not None:
                 data |= {"devices": await self.update_inverter_data()}
             # print(f"extended data updated: {data}")
 
         #calculated values (for downward compatibility)
         if data.get("power_dc") != 0:
             data |= {"efficiency": data.get("power_ac") / data.get("power_dc")}
         if data.get("power_ac") != 0:
```

### Comparing `solarlog_cli-0.1.2/src/solarlog_cli/utils.py` & `solarlog_cli-0.1.3/src/solarlog_cli/utils.py`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.2/LICENSE` & `solarlog_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.2/pyproject.toml` & `solarlog_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solarlog_cli"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the Solar-Log"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

### Comparing `solarlog_cli-0.1.2/PKG-INFO` & `solarlog_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solarlog_cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library to access the Solar-Log
 Project-URL: Repository, https://github.com/dontinelli/solarlog_cli.git
 Project-URL: Issues, https://github.com/dontinelli/solarlog_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/solarlog_cli/blob/master/CHANGELOG.md
 Project-URL: Solar-Log homepage, https://www.solar-log.com/
 Project-URL: API Documentation (inofficial), https://github.com/iobroker-community-adapters/ioBroker.solarlog/blob/master/docs/solarlog_dataobjects.md
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

