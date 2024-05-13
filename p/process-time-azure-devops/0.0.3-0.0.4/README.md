# Comparing `tmp/process_time_azure_devops-0.0.3.tar.gz` & `tmp/process_time_azure_devops-0.0.4.tar.gz`

## Comparing `process_time_azure_devops-0.0.3.tar` & `process_time_azure_devops-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/azure-pipelines.yml
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.github/workflows/pr.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/process-time-azure-devops.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/arts/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/arts/process_time_logo.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/models/ArgumentParseResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/generate_test_run.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/tests/test_get_last_attempt_to_deliver.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/LICENSE
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/README.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/azure-pipelines.yml
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/process-time-azure-devops.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/arts/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/arts/process_time_logo.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/models/ArgumentParseResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/parsers/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/tests/generate_test_run.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/tests/test_get_last_attempt_to_deliver.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/LICENSE
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 process_time_azure_devops-0.0.4/PKG-INFO
```

### Comparing `process_time_azure_devops-0.0.3/azure-pipelines.yml` & `process_time_azure_devops-0.0.4/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/.github/workflows/pr.yml` & `process_time_azure_devops-0.0.4/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/.github/workflows/publish.yml` & `process_time_azure_devops-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/src/process_time_azure_devops/__main__.py` & `process_time_azure_devops-0.0.4/src/process_time_azure_devops/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     print(f'Pipeline ID: {pipeline_id}')
     print('================================')
     return ArgumentParseResult(azure_devops_organization, personal_access_token, project, pipeline_id)
 
 
 def calculate_process_tine(args: ArgumentParseResult) -> None:
     print('Calculating process time...')
-    credentials = BasicAuthentication('', args.personal_access_token)
+    url = f'https://dev.azure.com/{args.azure_devops_organization}'
+    print(f'Connecting to Azure DevOps Organization: {url}')
+    credentials = BasicAuthentication(args.personal_access_token)
     pipelines_client = PipelinesClient(f'https://dev.azure.com/{args.azure_devops_organization}', credentials)
     runs = pipelines_client.list_runs(args.project, args.pipeline_id)
     previous_attempt = get_last_attempt_to_deliver(runs)
     print(json.dumps(previous_attempt.as_dict(), sort_keys=True, indent=4))
     print('Process time calculated!')
```

### Comparing `process_time_azure_devops-0.0.3/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.4/src/process_time_azure_devops/parsers/get_last_attempt_to_deliver.py`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/tests/test_get_last_attempt_to_deliver.py` & `process_time_azure_devops-0.0.4/tests/test_get_last_attempt_to_deliver.py`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/.gitignore` & `process_time_azure_devops-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/LICENSE` & `process_time_azure_devops-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `process_time_azure_devops-0.0.3/pyproject.toml` & `process_time_azure_devops-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/process_time_azure_devops"]
 
 [project]
 name = "process_time_azure_devops"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Andrei Kniazev" },
 ]
 description = "Will collect process time for projects that are hosted in Azure DevOps"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
```

### Comparing `process_time_azure_devops-0.0.3/PKG-INFO` & `process_time_azure_devops-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 7072 6f63  : 2.3.Name: proc
 00000020: 6573 735f 7469 6d65 5f61 7a75 7265 5f64  ess_time_azure_d
 00000030: 6576 6f70 730a 5665 7273 696f 6e3a 2030  evops.Version: 0
-00000040: 2e30 2e33 0a53 756d 6d61 7279 3a20 5769  .0.3.Summary: Wi
+00000040: 2e30 2e34 0a53 756d 6d61 7279 3a20 5769  .0.4.Summary: Wi
 00000050: 6c6c 2063 6f6c 6c65 6374 2070 726f 6365  ll collect proce
 00000060: 7373 2074 696d 6520 666f 7220 7072 6f6a  ss time for proj
 00000070: 6563 7473 2074 6861 7420 6172 6520 686f  ects that are ho
 00000080: 7374 6564 2069 6e20 417a 7572 6520 4465  sted in Azure De
 00000090: 764f 7073 0a50 726f 6a65 6374 2d55 524c  vOps.Project-URL
 000000a0: 3a20 4769 7448 7562 2c20 6874 7470 733a  : GitHub, https:
 000000b0: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6f72  //github.com/wor
@@ -43,35 +43,56 @@
 000002a0: 7572 652d 6465 766f 7073 3d3d 372e 312e  ure-devops==7.1.
 000002b0: 3062 343b 2065 7874 7261 203d 3d20 2774  0b4; extra == 't
 000002c0: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
 000002d0: 7374 3a20 7079 7465 7374 3d3d 382e 322e  st: pytest==8.2.
 000002e0: 303b 2065 7874 7261 203d 3d20 2774 6573  0; extra == 'tes
 000002f0: 7427 0a44 6573 6372 6970 7469 6f6e 2d43  t'.Description-C
 00000300: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000310: 742f 6d61 726b 646f 776e 0a0a 3c69 6d67  t/markdown..<img
-00000320: 2077 6964 7468 3d22 3135 3937 2220 616c   width="1597" al
-00000330: 743d 2269 6d61 6765 2220 7372 633d 2268  t="image" src="h
-00000340: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000350: 6d2f 776f 726c 6470 776e 2f70 726f 6365  m/worldpwn/proce
-00000360: 7373 2d74 696d 652d 617a 7572 652d 6465  ss-time-azure-de
-00000370: 766f 7073 2f61 7373 6574 732f 3633 3531  vops/assets/6351
-00000380: 3738 302f 6438 6164 6237 6365 2d65 3238  780/d8adb7ce-e28
-00000390: 342d 3438 6532 2d61 3536 622d 3635 6561  4-48e2-a56b-65ea
-000003a0: 6437 3362 3137 6136 223e 0a0a 2320 4c6f  d73b17a6">..# Lo
-000003b0: 6361 6c20 4465 760a 4275 696c 6420 7072  cal Dev.Build pr
-000003c0: 6f6a 6563 7420 7769 7468 2061 2077 6174  oject with a wat
-000003d0: 6368 2d6c 696b 6520 6d6f 6465 2e0a 0a60  ch-like mode...`
-000003e0: 6060 6261 7368 0a70 7974 686f 6e20 2d6d  ``bash.python -m
-000003f0: 2070 6970 2069 6e73 7461 6c6c 202d 6520   pip install -e 
-00000400: 2e0a 6060 600a 2320 5465 7374 0a49 6e73  ..```.# Test.Ins
-00000410: 7461 6c6c 2044 6570 656e 6465 6e63 6965  tall Dependencie
-00000420: 7320 666f 7220 5465 7374 730a 6060 6062  s for Tests.```b
-00000430: 6173 680a 7079 202d 6d20 7069 7020 696e  ash.py -m pip in
-00000440: 7374 616c 6c20 2d65 202e 5b74 6573 745d  stall -e .[test]
-00000450: 0a60 6060 0a52 756e 2054 6573 7473 0a60  .```.Run Tests.`
-00000460: 6060 6261 7368 0a70 7920 2d6d 2070 7974  ``bash.py -m pyt
-00000470: 6573 7420 7465 7374 7320 2d2d 7665 7262  est tests --verb
-00000480: 6f73 650a 6060 600a 2320 5275 6e0a 6060  ose.```.# Run.``
-00000490: 6062 6173 680a 7079 2073 7263 2f65 7861  `bash.py src/exa
-000004a0: 6d70 6c65 2e70 790a 6060 600a 0a23 2042  mple.py.```..# B
-000004b0: 7569 6c64 0a60 6060 6261 7368 0a70 7920  uild.```bash.py 
-000004c0: 7372 632f 6d61 696e 0a60 6060 0a         src/main.```.
+00000310: 742f 6d61 726b 646f 776e 0a0a 5b21 5b50  t/markdown..[![P
+00000320: 7562 6c69 7368 5d28 6874 7470 733a 2f2f  ublish](https://
+00000330: 6769 7468 7562 2e63 6f6d 2f77 6f72 6c64  github.com/world
+00000340: 7077 6e2f 7072 6f63 6573 732d 7469 6d65  pwn/process-time
+00000350: 2d61 7a75 7265 2d64 6576 6f70 732f 6163  -azure-devops/ac
+00000360: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000370: 7075 626c 6973 682e 796d 6c2f 6261 6467  publish.yml/badg
+00000380: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000390: 6769 7468 7562 2e63 6f6d 2f77 6f72 6c64  github.com/world
+000003a0: 7077 6e2f 7072 6f63 6573 732d 7469 6d65  pwn/process-time
+000003b0: 2d61 7a75 7265 2d64 6576 6f70 732f 6163  -azure-devops/ac
+000003c0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000003d0: 7075 626c 6973 682e 796d 6c29 0a3c 6120  publish.yml).<a 
+000003e0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000003f0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
+00000400: 726f 6365 7373 2d74 696d 652d 617a 7572  rocess-time-azur
+00000410: 652d 6465 766f 7073 2f22 3e3c 696d 6720  e-devops/"><img 
+00000420: 616c 743d 2250 7950 4922 2073 7263 3d22  alt="PyPI" src="
+00000430: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000440: 6c64 732e 696f 2f70 7970 692f 762f 7072  lds.io/pypi/v/pr
+00000450: 6f63 6573 732d 7469 6d65 2d61 7a75 7265  ocess-time-azure
+00000460: 2d64 6576 6f70 7322 3e3c 2f61 3e0a 3c69  -devops"></a>.<i
+00000470: 6d67 2077 6964 7468 3d22 3135 3937 2220  mg width="1597" 
+00000480: 616c 743d 2269 6d61 6765 2220 7372 633d  alt="image" src=
+00000490: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000004a0: 636f 6d2f 776f 726c 6470 776e 2f70 726f  com/worldpwn/pro
+000004b0: 6365 7373 2d74 696d 652d 617a 7572 652d  cess-time-azure-
+000004c0: 6465 766f 7073 2f61 7373 6574 732f 3633  devops/assets/63
+000004d0: 3531 3738 302f 6438 6164 6237 6365 2d65  51780/d8adb7ce-e
+000004e0: 3238 342d 3438 6532 2d61 3536 622d 3635  284-48e2-a56b-65
+000004f0: 6561 6437 3362 3137 6136 223e 0a0a 2320  ead73b17a6">..# 
+00000500: 4c6f 6361 6c20 4465 760a 4275 696c 6420  Local Dev.Build 
+00000510: 7072 6f6a 6563 7420 7769 7468 2061 2077  project with a w
+00000520: 6174 6368 2d6c 696b 6520 6d6f 6465 2e0a  atch-like mode..
+00000530: 0a60 6060 6261 7368 0a70 7974 686f 6e20  .```bash.python 
+00000540: 2d6d 2070 6970 2069 6e73 7461 6c6c 202d  -m pip install -
+00000550: 6520 2e0a 6060 600a 2320 5465 7374 0a49  e ..```.# Test.I
+00000560: 6e73 7461 6c6c 2044 6570 656e 6465 6e63  nstall Dependenc
+00000570: 6965 7320 666f 7220 5465 7374 730a 6060  ies for Tests.``
+00000580: 6062 6173 680a 7079 202d 6d20 7069 7020  `bash.py -m pip 
+00000590: 696e 7374 616c 6c20 2d65 202e 5b74 6573  install -e .[tes
+000005a0: 745d 0a60 6060 0a52 756e 2054 6573 7473  t].```.Run Tests
+000005b0: 0a60 6060 6261 7368 0a70 7920 2d6d 2070  .```bash.py -m p
+000005c0: 7974 6573 7420 7465 7374 7320 2d2d 7665  ytest tests --ve
+000005d0: 7262 6f73 650a 6060 600a 2320 5275 6e0a  rbose.```.# Run.
+000005e0: 6060 6062 6173 680a 7079 2073 7263 2f65  ```bash.py src/e
+000005f0: 7861 6d70 6c65 2e70 790a 6060 600a 0a23  xample.py.```..#
+00000600: 2042 7569 6c64 0a60 6060 6261 7368 0a70   Build.```bash.p
+00000610: 7920 7372 632f 6d61 696e 0a60 6060 0a    y src/main.```.
```

