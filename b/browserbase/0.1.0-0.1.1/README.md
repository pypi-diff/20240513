# Comparing `tmp/browserbase-0.1.0.tar.gz` & `tmp/browserbase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.1.0.tar", last modified: Fri May 10 12:23:01 2024, max compression
+gzip compressed data, was "browserbase-0.1.1.tar", last modified: Mon May 13 09:41:00 2024, max compression
```

## Comparing `browserbase-0.1.0.tar` & `browserbase-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.816158 browserbase-0.1.0/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.0/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-10 12:23:01.815942 browserbase-0.1.0/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.0/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.814439 browserbase-0.1.0/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)    11429 2024-05-10 12:20:14.000000 browserbase-0.1.0/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.815550 browserbase-0.1.0/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.0/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.0/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-10 12:23:01.815726 browserbase-0.1.0/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-10 12:23:01.000000 browserbase-0.1.0/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-10 12:22:32.000000 browserbase-0.1.0/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-10 12:23:01.816203 browserbase-0.1.0/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 09:41:00.675203 browserbase-0.1.1/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.1/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-13 09:41:00.674934 browserbase-0.1.1/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.1/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 09:41:00.673025 browserbase-0.1.1/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)    10720 2024-05-13 09:39:02.000000 browserbase-0.1.1/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 09:41:00.674344 browserbase-0.1.1/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.1/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.1/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 09:41:00.674697 browserbase-0.1.1/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-13 09:41:00.000000 browserbase-0.1.1/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-13 09:41:00.000000 browserbase-0.1.1/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-13 09:41:00.000000 browserbase-0.1.1/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-13 09:41:00.000000 browserbase-0.1.1/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-13 09:41:00.000000 browserbase-0.1.1/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-13 09:40:53.000000 browserbase-0.1.1/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-13 09:41:00.675246 browserbase-0.1.1/setup.cfg
```

### Comparing `browserbase-0.1.0/LICENSE` & `browserbase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.0/PKG-INFO` & `browserbase-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.0/README.md` & `browserbase-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.0/browserbase/__init__.py` & `browserbase-0.1.1/browserbase/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,91 +34,89 @@
     RUNNING = "RUNNING"
     REQUEST_RELEASE = "REQUEST_RELEASE"
     RELEASING = "RELEASING"
     COMPLETED = "COMPLETED"
 
 
 class Screen(BaseModel):
-    max_height: Optional[int] = Field(None, alias="maxHeight")
-    max_width: Optional[int] = Field(None, alias="maxWidth")
-    min_height: Optional[int] = Field(None, alias="minHeight")
-    min_width: Optional[int] = Field(None, alias="minWidth")
+    maxHeight: Optional[int] = None
+    maxWidth: Optional[int] = None
+    minHeight: Optional[int] = None
+    minWidth: Optional[int] = None
 
 
 class Fingerprint(BaseModel):
-    browser_list_query: Optional[str] = Field(None, alias="browserListQuery")
-    http_version: Optional[int] = Field(None, alias="httpVersion")
+    browserListQuery: Optional[str] = None
+    httpVersion: Optional[int] = None
     browsers: Optional[List[BrowserType]] = None
     devices: Optional[List[DeviceType]] = None
     locales: Optional[List[str]] = None
-    operating_systems: Optional[List[OperatingSystem]] = Field(
-        None, alias="operatingSystems"
-    )
+    operatingSystems: Optional[List[OperatingSystem]] = None
     screen: Optional[Screen] = None
 
 
 class CreateSessionOptions(BaseModel):
-    project_id: Optional[str] = Field(None, alias="projectId")
-    extension_id: Optional[str] = Field(None, alias="extensionId")
+    projectId: Optional[str] = None
+    extensionId: Optional[str] = None
     fingerprint: Optional[Fingerprint] = None
 
 
 class Session(BaseModel):
     id: str
-    created_at: str = Field(..., alias="createdAt")
-    started_at: str = Field(..., alias="startedAt")
-    ended_at: Optional[str] = Field(..., alias="endedAt")
-    project_id: str = Field(..., alias="projectId")
+    createdAt: str
+    startedAt: str
+    endedAt: Optional[str]
+    projectId: str
     status: Optional[SessionStatus] = None
-    task_id: Optional[str] = Field(None, alias="taskId")
-    proxy_bytes: Optional[int] = Field(None, alias="proxyBytes")
-    expires_at: Optional[str] = Field(None, alias="expiresAt")
-    avg_cpu_usage: Optional[float] = Field(None, alias="avg_cpu_usage")
+    taskId: Optional[str] = None
+    proxyBytes: Optional[int] = None
+    expiresAt: Optional[str] = None
+    avg_cpu_usage: Optional[float] = None
     memory_usage: Optional[int] = None
     details: Optional[str] = None
     logs: Optional[str] = None
 
 
 class UpdateSessionOptions(BaseModel):
-    project_id: Optional[str] = Field(None, alias="projectId")
+    projectId: Optional[str] = None
     status: Optional[SessionStatus] = None
 
 
 class SessionRecording(BaseModel):
     type: Optional[str] = None
     time: Optional[str] = None
     data: Optional[dict] = None
 
 
 class DebugConnectionURLs(BaseModel):
-    debugger_fullscreen_url: Optional[str] = Field(None, alias="debuggerFullscreenUrl")
-    debugger_url: Optional[str] = Field(None, alias="debuggerUrl")
-    ws_url: Optional[str] = Field(None, alias="wsUrl")
+    debuggerFullscreenUrl: Optional[str] = None
+    debuggerUrl: Optional[str] = None
+    wsUrl: Optional[str] = None
 
 
 class Request(BaseModel):
     timestamp: Optional[str]
     params: Optional[dict]
-    raw_body: Optional[str] = Field(alias="rawBody")
+    rawBody: Optional[str] = None
 
 
 class Response(BaseModel):
     timestamp: Optional[str]
     result: Optional[dict]
-    raw_body: Optional[str] = Field(alias="rawBody")
+    rawBody: Optional[str] = None
 
 
 class SessionLog(BaseModel):
-    session_id: Optional[str] = Field(alias="sessionId")
+    sessionId: Optional[str] = None
     id: str
     timestamp: Optional[str]
     method: Optional[str]
     request: Optional[Request]
     response: Optional[Response]
-    page_id: Optional[str] = Field(alias="pageId")
+    pageId: Optional[str] = None
 
 
 class Browserbase:
     def __init__(
         self,
         api_key: Optional[str] = None,
         project_id: Optional[str] = None,
@@ -127,14 +125,22 @@
     ):
         """Create new Browserbase SDK client instance"""
         self.api_key = api_key or os.environ["BROWSERBASE_API_KEY"]
         self.project_id = project_id or os.environ["BROWSERBASE_PROJECT_ID"]
         self.connect_url = connect_url or "wss://connect.browserbase.com"
         self.api_url = api_url or "https://www.browserbase.com"
 
+    def get_connect_url(self, session_id=None, proxy=False):
+        base_url = f"{self.connect_url}?apiKey={self.api_key}"
+        if session_id:
+            base_url += f"&sessionId={session_id}"
+        if proxy:
+            base_url += "&enableProxy=true"
+        return base_url
+
     def list_sessions(self) -> List[Session]:
         response = httpx.get(
             f"{self.api_url}/v1/sessions",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
@@ -250,22 +256,14 @@
             },
         )
 
         response.raise_for_status()
         data = response.json()
         return [SessionLog(**item) for item in data]
 
-    def get_connect_url(self, session_id=None, proxy=False):
-        base_url = f"{self.connect_url}?apiKey={self.api_key}"
-        if session_id:
-            base_url += f"&sessionId={session_id}"
-        if proxy:
-            base_url += "&enableProxy=true"
-        return base_url
-
     def load(self, url: Union[str, Sequence[str]], **args):
         if isinstance(url, str):
             return self.load_url(url, **args)
         elif isinstance(url, Sequence):
             return self.load_urls(url, **args)
         else:
             raise TypeError("Input must be a URL string or a Sequence of URLs")
```

### Comparing `browserbase-0.1.0/browserbase.egg-info/PKG-INFO` & `browserbase-0.1.1/browserbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.0/pyproject.toml` & `browserbase-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

