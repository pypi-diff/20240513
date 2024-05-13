# Comparing `tmp/socketsecurity-0.0.42.tar.gz` & `tmp/socketsecurity-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.42.tar", last modified: Wed May  1 08:55:23 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.43.tar", last modified: Mon May 13 20:25:45 2024, max compression
```

## Comparing `socketsecurity-0.0.42.tar` & `socketsecurity-0.0.43.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:55:23.800408 socketsecurity-0.0.42/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:55:23.800193 socketsecurity-0.0.42/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-01 08:55:23.800446 socketsecurity-0.0.42/setup.cfg
--rw-r--r--   0 douglascoburn   (501) staff       (20)      347 2024-05-01 08:55:15.000000 socketsecurity-0.0.42/setup.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:55:23.798711 socketsecurity-0.0.42/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       45 2024-05-01 08:54:56.000000 socketsecurity-0.0.42/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:55:23.799738 socketsecurity-0.0.42/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    23060 2024-05-01 07:25:53.000000 socketsecurity-0.0.42/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     8053 2024-05-01 07:24:43.000000 socketsecurity-0.0.42/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-05-01 06:00:20.000000 socketsecurity-0.0.42/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11580 2024-05-01 06:39:19.000000 socketsecurity-0.0.42/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     2141 2024-05-01 07:36:53.000000 socketsecurity-0.0.42/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-01 08:55:23.799990 socketsecurity-0.0.42/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      154 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      422 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       35 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-01 08:55:23.000000 socketsecurity-0.0.42/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.626503 socketsecurity-0.0.43/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:25:45.626288 socketsecurity-0.0.43/PKG-INFO
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.625260 socketsecurity-0.0.43/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    25969 2024-05-08 17:09:44.000000 socketsecurity-0.0.43/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     8665 2024-05-07 20:28:21.000000 socketsecurity-0.0.43/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.43/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11251 2024-05-08 17:15:58.000000 socketsecurity-0.0.43/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11208 2024-05-05 18:30:58.000000 socketsecurity-0.0.43/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.43/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.43/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11834 2024-05-08 17:02:42.000000 socketsecurity-0.0.43/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-13 20:25:45.626541 socketsecurity-0.0.43/setup.cfg
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      330 2024-05-13 20:24:12.000000 socketsecurity-0.0.43/setup.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.626082 socketsecurity-0.0.43/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      370 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       60 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       37 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        5 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.42/socketsecurity/core/__init__.py` & `socketsecurity-0.0.43/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import requests
 from urllib.parse import urlencode
 import base64
 import json
 from core.exceptions import APIFailure, APIKeyMissing, APIAccessDenied, APIInsufficientQuota, APIResourceNotFound
+from core.licenses import Licenses
+from core.issues import AllIssues
 from core.classes import (
     Report,
     Issue,
     Package,
     Alert,
     FullScan,
     FullScanParams,
@@ -30,39 +32,24 @@
 
 global encoded_key
 version = __version__
 api_url = "https://api.socket.dev/v0"
 timeout = 30
 full_scan_path = ""
 repository_path = ""
+all_issues = AllIssues()
 org_id = None
 org_slug = None
 all_new_alerts = False
 issue_file = "core/issues.json"
-issue_text = {}
 security_policy = {}
 log = logging.getLogger("socketdev")
 log.addHandler(logging.NullHandler())
 
 
-def load_issue_data() -> dict:
-    """
-    Loads the issue data json and returns it as a dictionary. This data is used in the alert messages.
-    :return:
-    """
-    try:
-        file = open(issue_file, 'r')
-        data = json.load(file)
-        return data
-    except Exception as error:
-        print("Unable to load issue data")
-        print(error)
-        exit(1)
-
-
 def encode_key(token: str) -> None:
     """
     encode_key takes passed token string and does a base64 encoding. It sets this as a global variable
     :param token: str of the Socket API Security Token
     :return:
     """
     global encoded_key
@@ -136,16 +123,14 @@
     base_api_url: str
     request_timeout: int
     reports: list
 
     def __init__(self, token: str, base_api_url=None, request_timeout=None, enable_all_alerts=False):
         self.token = token + ":"
         encode_key(self.token)
-        global issue_text
-        issue_text = load_issue_data()
         self.socket_date_format = "%Y-%m-%dT%H:%M:%S.%fZ"
         self.base_api_url = base_api_url
         if self.base_api_url is not None:
             Core.set_api_url(self.base_api_url)
         self.request_timeout = request_timeout
         if self.request_timeout is not None:
             Core.set_timeout(self.request_timeout)
@@ -258,15 +243,14 @@
 
     @staticmethod
     def find_files(path: str) -> list:
         """
         Globs the path for supported manifest files.
         Note: Might move the source to a JSON file
         :param path: Str - path to where the manifest files are located
-        :param workspace: str - workspace path to be stripped from the name
         :return:
         """
         socket_globs = {
             "general": {
                 "readme": {
                     "pattern": "*readme*"
                 },
@@ -384,14 +368,24 @@
         response = do_request(full_uri, method="POST", files=send_files)
         results = response.json()
         full_scan = FullScan(**results)
         full_scan.sbom_artifacts = Core.get_sbom_data(full_scan.id)
         return full_scan
 
     @staticmethod
+    def get_license_details(package: Package) -> Package:
+        license_raw = package.license
+        all_licenses = Licenses()
+        license_str = Licenses.make_python_safe(license_raw)
+        if license_str is not None and hasattr(all_licenses, license_str):
+            license_obj = getattr(all_licenses, license_str)
+            package.license_text = license_obj.licenseText
+        return package
+
+    @staticmethod
     def get_head_scan_for_repo(repo_slug: str):
         """
         Get the head scan ID for a repository to use for the diff
         :param repo_slug: Str - Repo slug for the repository that is being diffed
         :return:
         """
         repo_path = f"{repository_path}/{repo_slug}"
@@ -438,18 +432,20 @@
                 total_head_time = head_end - head_start
                 print(f"Total time to get head sbom {total_head_time: .2f}")
         except APIResourceNotFound:
             head_full_scan = []
         if files is not None and len(files) > 0:
             new_scan_start = time.time()
             new_full_scan = Core.create_full_scan(files, params, workspace)
+            new_full_scan.packages = Core.create_sbom_dict(new_full_scan.sbom_artifacts)
             new_scan_end = time.time()
             total_new_time = new_scan_end - new_scan_start
             print(f"Total time to get new sbom {total_new_time: .2f}")
             diff_report = Core.compare_sboms(new_full_scan.sbom_artifacts, head_full_scan)
+            diff_report.packages = new_full_scan.packages
         else:
             diff_report = Diff()
         return diff_report
 
     @staticmethod
     def compare_sboms(new_scan: list, head_scan: list) -> Diff:
         """
@@ -473,17 +469,78 @@
             new_scan_alerts = Core.create_issue_alerts(package, new_scan_alerts, new_packages)
         for package_id in head_packages:
             purl, package = Core.create_purl(package_id, head_packages)
             if package_id not in new_packages:
                 diff.removed_packages.append(purl)
             head_scan_alerts = Core.create_issue_alerts(package, head_scan_alerts, head_packages)
         diff.new_alerts = Core.compare_issue_alerts(new_scan_alerts, head_scan_alerts, diff.new_alerts)
+        diff.new_capabilities = Core.compare_capabilities(new_packages, head_packages)
+        diff = Core.add_capabilities_to_purl(diff)
+        return diff
+
+    @staticmethod
+    def add_capabilities_to_purl(diff: Diff) -> Diff:
+        new_packages = []
+        for purl in diff.new_packages:
+            purl: Purl
+            if purl.id in diff.new_capabilities:
+                capabilities = diff.new_capabilities[purl.id]
+                if len(capabilities) > 0:
+                    purl.capabilities = capabilities
+                    new_packages.append(purl)
+            else:
+                new_packages.append(purl)
+        diff.new_packages = new_packages
         return diff
 
     @staticmethod
+    def compare_capabilities(new_packages: dict, head_packages: dict) -> dict:
+        capabilities = {}
+        for package_id in new_packages:
+            package: Package
+            head_package: Package
+            package = new_packages[package_id]
+            if package_id in head_packages:
+                head_package = head_packages[package_id]
+                for alert in package.alerts:
+                    if alert not in head_package.alerts:
+                        capabilities = Core.check_alert_capabilities(package, capabilities, package_id, head_package)
+            else:
+                capabilities = Core.check_alert_capabilities(package, capabilities, package_id)
+
+        return capabilities
+
+    @staticmethod
+    def check_alert_capabilities(
+            package: Package,
+            capabilities: dict,
+            package_id: str,
+            head_package: Package = None
+    ) -> dict:
+        alert_types = {
+            "envVars": "Environment",
+            "networkAccess": "Network",
+            "filesystemAccess": "File System",
+            "shellAccess": "Shell"
+        }
+
+        for alert in package.alerts:
+            new_alert = True
+            if head_package is not None and alert in head_package.alerts:
+                new_alert = False
+            if alert["type"] in alert_types and new_alert:
+                value = alert_types[alert["type"]]
+                if package_id not in capabilities:
+                    capabilities[package_id] = [value]
+                else:
+                    if value not in capabilities[package_id]:
+                        capabilities[package_id].append(value)
+        return capabilities
+
+    @staticmethod
     def compare_issue_alerts(new_scan_alerts: dict, head_scan_alerts: dict, alerts: list) -> list:
         """
         Compare the issue alerts from the new full scan and the head full scans. Return a list of new alerts that
         are in the new full scan and not in the head full scan
         :param new_scan_alerts: dictionary of alerts from the new full scan
         :param head_scan_alerts: dictionary of alerts from the new head scan
         :param alerts: List of new alerts that are only in the new Full Scan
@@ -524,20 +581,20 @@
         :param package: Package - Current package that is being looked at for Alerts
         :param alerts: Dict - All found Issue Alerts across all packages
         :param packages: Dict - All packages detected in the SBOM and needed to find top level packages
         :return:
         """
         for item in package.alerts:
             alert = Alert(**item)
-            props = issue_text.get(alert.type)
+            props = getattr(all_issues, alert.type)
             if props is not None:
-                description = props.get("description")
-                title = props.get("title")
-                suggestion = props.get("suggestion")
-                next_step_title = props.get("nextStepTitle")
+                description = props.description
+                title = props.title
+                suggestion = props.suggestion
+                next_step_title = props.nextStepTitle
             else:
                 description = ""
                 title = ""
                 suggestion = ""
                 next_step_title = ""
             introduced_by = Core.get_source_data(package, packages)
             issue_alert = Issue(
@@ -607,15 +664,15 @@
         purl = Purl(
             id=package.id,
             name=package.name,
             version=package.version,
             ecosystem=package.type,
             direct=package.direct,
             introduced_by=introduced_by,
-            author=package.author or '',
+            author=package.author or [],
             size=package.size,
             transitives=package.transitives
         )
         return purl, package
 
     @staticmethod
     def create_sbom_dict(sbom: list) -> dict:
@@ -627,18 +684,30 @@
         packages = {}
         top_level_count = {}
         for item in sbom:
             package = Package(**item)
             if package.id in packages:
                 print("Duplicate package?")
             else:
+                package = Core.get_license_details(package)
                 packages[package.id] = package
                 for top_id in package.topLevelAncestors:
                     if top_id not in top_level_count:
                         top_level_count[top_id] = 1
                     else:
                         top_level_count[top_id] += 1
         if len(top_level_count) > 0:
             for package_id in top_level_count:
                 packages[package_id].transitives = top_level_count[package_id]
         return packages
 
+    @staticmethod
+    def save_file(file_name: str, content: str) -> None:
+        file = open(file_name, "w")
+        file.write(content)
+        file.close()
+
+    # @staticmethod
+    # def create_license_file(diff: Diff) -> None:
+    #     output = []
+    #     for package_id in diff.packages:
+    #         purl =  Core.create_purl(package_id, diff.packages)
```

### Comparing `socketsecurity-0.0.42/socketsecurity/core/classes.py` & `socketsecurity-0.0.43/core/classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,16 @@
     scores: Score
     alerts: list
     error_alerts: list
     alert_counts: dict
     topLevelAncestors: list
     url: str
     transitives: int
+    license: str
+    license_text: str
 
     def __init__(self, **kwargs):
         if kwargs:
             for key, value in kwargs.items():
                 setattr(self, key, value)
         if not hasattr(self, "direct"):
             self.direct = False
@@ -95,31 +97,35 @@
             if str(self.direct).lower() == "true":
                 self.direct = True
         self.url = f"https://socket.dev/{self.type}/package/{self.name}/overview/{self.version}"
         if hasattr(self, 'score'):
             self.scores = Score(**self.score)
         if not hasattr(self, "alerts"):
             self.alerts = []
-        if not hasattr(self, "author"):
-            self.author = []
-        if not hasattr(self, "size"):
-            self.size = 0
         if not hasattr(self, "topLevelAncestors"):
             self.topLevelAncestors = []
         if not hasattr(self, "manifestFiles"):
             self.manifestFiles = []
         if not hasattr(self, "transitives"):
             self.transitives = 0
+        if not hasattr(self, "author"):
+            self.author = []
+        if not hasattr(self, "size"):
+            self.size = 0
         self.alert_counts = {
             "critical": 0,
             "high": 0,
             "middle": 0,
             "low": 0
         }
         self.error_alerts = []
+        if not hasattr(self, "license"):
+            self.license = "NoLicenseFound"
+        if not hasattr(self, "license_text"):
+            self.license_text = ""
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
 
 class Issue:
     pkg_type: str
@@ -225,14 +231,15 @@
     organization_id: str
     repository_id: str
     branch: str
     commit_message: str
     commit_hash: str
     pull_request: int
     sbom_artifacts: list
+    packages: dict
 
     def __init__(self, **kwargs):
         if kwargs:
             for key, value in kwargs.items():
                 setattr(self, key, value)
         if not hasattr(self, "sbom_artifacts"):
             self.sbom_artifacts = []
@@ -279,29 +286,33 @@
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
 
 class Diff:
     new_packages: list
+    new_capabilities: dict
     removed_packages: list
     new_alerts: list
     id: str
     sbom: str
+    packages: dict
 
     def __init__(self, **kwargs):
         if kwargs:
             for key, value in kwargs.items():
                 setattr(self, key, value)
         if not hasattr(self, "new_packages"):
             self.new_packages = []
         if not hasattr(self, "removed_packages"):
             self.removed_packages = []
         if not hasattr(self, "new_alerts"):
             self.new_alerts = []
+        if not hasattr(self, "new_capabilities"):
+            self.new_capabilities = {}
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
 
 class Purl:
     id: str
@@ -309,21 +320,27 @@
     version: str
     ecosystem: str
     direct: bool
     author: str
     size: int
     transitives: int
     introduced_by: list
+    capabilities: dict
+    is_new: bool
 
     def __init__(self, **kwargs):
         if kwargs:
             for key, value in kwargs.items():
                 setattr(self, key, value)
         if not hasattr(self, "introduced_by"):
             self.new_packages = []
+        if not hasattr(self, "capabilities"):
+            self.capabilities = {}
+        if not hasattr(self, "is_new"):
+            self.is_new = False
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
 
 class GithubComment:
     url: str
@@ -345,7 +362,12 @@
             for key, value in kwargs.items():
                 setattr(self, key, value)
         if not hasattr(self, "body_list"):
             self.body_list = []
 
     def __str__(self):
         return json.dumps(self.__dict__)
+
+class LicenseOutput(Purl):
+    licenses: list
+    license
+
```

### Comparing `socketsecurity-0.0.42/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.43/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.42/socketsecurity/core/messages.py` & `socketsecurity-0.0.43/core/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from mdutils import MdUtils
-from prettytable import PrettyTable
 from core.classes import Diff, Purl, Issue
+from prettytable import PrettyTable
 
 
 class Messages:
 
     @staticmethod
     def security_comment_template(diff: Diff) -> str:
         """
@@ -124,15 +124,15 @@
                     alert.description,
                     alert.suggestion
                 ]
             package_url, purl = Messages.create_package_link(alert)
             ignore = f"`SocketSecurity ignore {purl}`"
             if ignore not in ignore_commands:
                 ignore_commands.append(ignore)
-            manifest_str, sources = Messages.create_sources(alert)
+            manifest_str, sources = Messages.create_sources(alert, "console")
             row = [
                 alert.title,
                 package_url,
                 ", ".join(sources),
                 manifest_str
             ]
             alert_table.extend(row)
@@ -187,31 +187,37 @@
         :param diff: Diff - Diff report with the Added packages information
         :param md: MdUtils - Main markdown variable
         :return:
         """
         overview_table = [
             "Package",
             "Direct",
+            "Capabilities",
             "Transitives",
             "Size",
             "Author"
         ]
         num_of_overview_columns = len(overview_table)
+        count = 0
         for added in diff.new_packages:
             added: Purl
             package_url = Messages.create_purl_link(added)
-            row = [
-                package_url,
-                added.direct,
-                added.transitives,
-                f"{added.size} KB",
-                Messages.generate_author_data(added)
-            ]
-            overview_table.extend(row)
-        num_of_overview_rows = len(diff.new_packages) + 1
+            capabilities = ", ".join(added.capabilities)
+            if capabilities is not None and capabilities != "":
+                row = [
+                    package_url,
+                    added.direct,
+                    capabilities,
+                    added.transitives,
+                    f"{added.size} KB",
+                    Messages.generate_author_data(added)
+                ]
+                overview_table.extend(row)
+                count += 1
+        num_of_overview_rows = count + 1
         md.new_table(
             columns=num_of_overview_columns,
             rows=num_of_overview_rows,
             text=overview_table,
             text_align="left"
         )
         return md
```

