# Comparing `tmp/pih-answ_auto-0.22.tar.gz` & `tmp/pih-answ_auto-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.22.tar", last modified: Wed May  8 06:46:39 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.23.tar", last modified: Mon May 13 01:53:06 2024, max compression
```

## Comparing `pih-answ_auto-0.22.tar` & `pih-answ_auto-0.23.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:39.317679 pih-answ_auto-0.22/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:36.298643 pih-answ_auto-0.22/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.22/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.22/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-05-08 06:46:21.000000 pih-answ_auto-0.22/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0    10093 2024-05-08 06:40:05.000000 pih-answ_auto-0.22/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-05-08 06:46:39.270801 pih-answ_auto-0.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:39.223965 pih-answ_auto-0.22/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-08 06:46:36.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 06:46:39.317679 pih-answ_auto-0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.482904 pih-answ_auto-0.23/
+drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.036154 pih-answ_auto-0.23/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.23/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.23/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-05-13 01:49:11.000000 pih-answ_auto-0.23/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0    10088 2024-05-08 14:19:07.000000 pih-answ_auto-0.23/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-05-13 01:53:06.434983 pih-answ_auto-0.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 01:53:06.388111 pih-answ_auto-0.23/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-13 01:53:05.000000 pih-answ_auto-0.23/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 01:53:06.482904 pih-answ_auto-0.23/setup.cfg
```

### Comparing `pih-answ_auto-0.22/AnswerAutomationService/service.py` & `pih-answ_auto-0.23/AnswerAutomationService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 class ANSWER_TYPE:
 
     VISIT = 1
     TAX_CERTIFICATE = 2
     VISIT_MODIFICATION = 4
     HOW_TO_GET = 8
-    OTHER_QUESTION: int = 16
+    OTHER_QUESTION = 16
     # LATE = 8
 
 
 def start(as_standalone: bool = False) -> None:
 
     from pih.collections import (
         Message,
         PolibasePerson,
         WhatsAppMessage,
         PolibasePersonVisitDS as PPVDS,
         PolibasePersonNotificationConfirmation as PPNC,
     )
 
     from pih import serve, subscribe_on
-    from pih.tools import ParameterList, j, js, ne, nn, one, nnt
+    from pih.tools import j, js, ne, nn, one, nnt, ParameterList
 
     SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.CALL_CENTRE)
 
     def polibase_person_name_format(value: str, polibase_person: PolibasePerson) -> str:
         return value.format(name=A.D.to_given_name(polibase_person))
 
     def server_call_handler(sc: SC, pl: ParameterList) -> bool | None:
```

