# Comparing `tmp/pih-auto-0.20.tar.gz` & `tmp/pih-auto-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-auto-0.20.tar", last modified: Thu Apr 18 05:26:05 2024, max compression
+gzip compressed data, was "pih-auto-0.21.tar", last modified: Mon May 13 03:17:11 2024, max compression
```

## Comparing `pih-auto-0.20.tar` & `pih-auto-0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.845057 pih-auto-0.20/
-drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.433960 pih-auto-0.20/AutomationService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.20/AutomationService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.20/AutomationService/__main__.py
--rw-rw-rw-   0        0        0      559 2024-04-18 05:21:39.000000 pih-auto-0.20/AutomationService/const.py
--rw-rw-rw-   0        0        0    19242 2024-04-18 05:21:31.000000 pih-auto-0.20/AutomationService/service.py
--rw-rw-rw-   0        0        0      295 2024-04-18 05:26:05.812589 pih-auto-0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.780310 pih-auto-0.20/pih_auto.egg-info/
--rw-rw-rw-   0        0        0      295 2024-04-18 05:26:04.000000 pih-auto-0.20/pih_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:26:05.860745 pih-auto-0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.736954 pih-auto-0.21/
+drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.249475 pih-auto-0.21/AutomationService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.21/AutomationService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.21/AutomationService/__main__.py
+-rw-rw-rw-   0        0        0      632 2024-05-13 01:13:01.000000 pih-auto-0.21/AutomationService/const.py
+-rw-rw-rw-   0        0        0    19210 2024-05-13 01:12:44.000000 pih-auto-0.21/AutomationService/service.py
+-rw-rw-rw-   0        0        0      295 2024-05-13 03:17:11.705699 pih-auto-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 03:17:11.658823 pih-auto-0.21/pih_auto.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-13 03:17:11.000000 pih-auto-0.21/pih_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 03:17:10.000000 pih-auto-0.21/pih_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:17:11.738986 pih-auto-0.21/setup.cfg
```

### Comparing `pih-auto-0.20/AutomationService/const.py` & `pih-auto-0.21/AutomationService/const.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Automation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.20"
+VERSION: str = "0.21"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Automation service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="auto",
     version=VERSION,
 )
 
+UNISEND_API_URL: str = "https://api.unisender.com/ru/api/subscribe"
+
+
 class ProblemState(IntEnum):
     AT_FIX = auto()
     WAIT_FOR_FIX_RESULT = auto()
     NOT_FIXED = auto()
     FIXED = auto()
```

### Comparing `pih-auto-0.20/AutomationService/service.py` & `pih-auto-0.21/AutomationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import ipih
 
 from pih.tools import *
 from pih.consts import *
 from pih.collections import *
 from AutomationService.const import *
 from pih.consts.errors import NotFound
-from pih import A, PIHThread, serve, subscribe_on
+from pih import A, PIHThread, serve, subscribe_on, strdict
 
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
@@ -58,15 +58,15 @@
                                 ),
                             ),
                             title="Показания в помещение КТ:",
                         )
 
                 @staticmethod
                 def all_indications() -> None:
-                    A.A_MIO.send_command_to(
+                    A.A_MIO.send(
                         js(
                             (
                                 "indications",
                                 FLAG_KEYWORDS.ALL_SYMBOL,
                                 FLAG_KEYWORDS.SILENCE,
                             )
                         ),
@@ -290,15 +290,15 @@
                                             text_list[1].strip()
                                             if has_separator
                                             else None
                                         )
                                         mobile_output.write_line(b(title))
                                         if ne(text):
                                             mobile_output.write_line(text)
-                                A.A_MIO.send_command_to(
+                                A.A_MIO.send(
                                     js(
                                         (
                                             mio_command(COMMAND_KEYWORDS.CREATE),
                                             mio_command(COMMAND_KEYWORDS.USER),
                                         )
                                     ),
                                     recipient,
@@ -342,24 +342,24 @@
                         email_information: EmailInformation = A.D.fill_data_from_source(
                             EmailInformation(),
                             A.E.get_parameter(event, event_parameters),
                         )
                         polibase_person: PolibasePerson = A.R_P.person_by_pin(
                             email_information.person_pin
                         ).data
-                        params: dict[str, str | None] = {
+                        params: strdict = {
                             "format": "json",
-                            "api_key": "65ddrin3zh791hxarbkwe4fmah5p44hkg4cjwsuy",
-                            "list_ids": "407",
+                            "api_key": A.S.get(A.CT_S.UNISENDER_API_KEY),
+                            "list_ids": A.S.get(A.CT_S.UNISENDER_API_LIST_IDS),
                             "fields[email]": polibase_person.email,
                             "fields[Name]": polibase_person.FullName,
                             "tags": "Polibase",
                         }
                         requests.get(
-                            "https://api.unisender.com/ru/api/subscribe",
+                            UNISEND_API_URL,
                             verify=False,
                             params=params,
                         )
 
                     if event == A.E_B.action_was_done():
                         action_data: ActionWasDone = A.D_Ex_E.action(event_parameters)
                         action: A.CT_ACT = action_data.action
```

