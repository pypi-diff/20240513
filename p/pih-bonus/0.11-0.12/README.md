# Comparing `tmp/pih-bonus-0.11.tar.gz` & `tmp/pih-bonus-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-bonus-0.11.tar", last modified: Fri Apr 19 02:21:12 2024, max compression
+gzip compressed data, was "pih-bonus-0.12.tar", last modified: Mon May 13 01:52:28 2024, max compression
```

## Comparing `pih-bonus-0.11.tar` & `pih-bonus-0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.774429 pih-bonus-0.11/
-drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.341264 pih-bonus-0.11/BonusProgramService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.11/BonusProgramService/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.11/BonusProgramService/__main__.py
--rw-rw-rw-   0        0        0     4076 2024-04-19 02:01:32.000000 pih-bonus-0.11/BonusProgramService/api.py
--rw-rw-rw-   0        0        0      400 2024-04-19 02:06:48.000000 pih-bonus-0.11/BonusProgramService/const.py
--rw-rw-rw-   0        0        0     5811 2024-04-19 01:51:55.000000 pih-bonus-0.11/BonusProgramService/service.py
--rw-rw-rw-   0        0        0      275 2024-04-19 02:21:12.743182 pih-bonus-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.711930 pih-bonus-0.11/pih_bonus.egg-info/
--rw-rw-rw-   0        0        0      275 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-04-19 02:21:12.000000 pih-bonus-0.11/pih_bonus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 02:21:12.790094 pih-bonus-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 01:52:28.345301 pih-bonus-0.12/
+drwxrwxrwx   0        0        0        0 2024-05-13 01:52:27.805645 pih-bonus-0.12/BonusProgramService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.12/BonusProgramService/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.12/BonusProgramService/__main__.py
+-rw-rw-rw-   0        0        0     4726 2024-04-22 02:31:18.000000 pih-bonus-0.12/BonusProgramService/api.py
+-rw-rw-rw-   0        0        0      400 2024-05-13 01:49:02.000000 pih-bonus-0.12/BonusProgramService/const.py
+-rw-rw-rw-   0        0        0     6269 2024-04-28 03:21:27.000000 pih-bonus-0.12/BonusProgramService/service.py
+-rw-rw-rw-   0        0        0      275 2024-05-13 01:52:28.297393 pih-bonus-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 01:52:28.219288 pih-bonus-0.12/pih_bonus.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 01:52:27.000000 pih-bonus-0.12/pih_bonus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 01:52:28.345301 pih-bonus-0.12/setup.cfg
```

### Comparing `pih-bonus-0.11/BonusProgramService/api.py` & `pih-bonus-0.12/BonusProgramService/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ipih
 
 from pih import A, strdict
 from pih.tools import nnt
 from pih.collections import PolibasePerson, BonusInformation
 
+from datetime import datetime
 import requests
 import json
 
 
 class BonusApi:
 
     @staticmethod
@@ -32,15 +33,15 @@
             "discount_percent": A.S.get(A.CT_S.BONUS_PROGRAM_DISCOUNT_PERCENT),
             "cashback_percent": A.S.get(A.CT_S.BONUS_PROGRAM_CASHBACK_PERCENT),
             "bonus_points": bonus_information.bonus_active,
             "total_paid_sum": bonus_information.money_all,
             "birth_date": A.D_F.datetime(value.Birth, A.CT.DATE_FORMAT),
             "first_name": full_name_list[1],
             "last_name": full_name_list[0],
-            "patronymic": full_name_list[2],
+            #"patronymic": full_name_list[2],
         }
 
     def create_bonus_card(self, value: PolibasePerson) -> str | None:
         data: strdict = BonusApi._make_call(BonusApi._create_bonus_card_data(value))
         return A.D.if_is_in(data["data"], "card_download_link", None)
 
     @staticmethod
@@ -58,51 +59,66 @@
     ) -> bool:
         data: strdict = self.get_data(value)
         result: bool = data["message"] != "Error: error 46 - pkpass file not found"
         if result and check_device_status:
             return data["data"]["device_status"] == 1
         return result
 
-    @staticmethod
-    def _update_bonuses_data(value: PolibasePerson, data: int | None = None) -> strdict:
+    def update_bonuses(self, value: PolibasePerson, data: int | None = None) -> bool:
         bonus_information: BonusInformation = A.R_P.bonus_information(value).data
-        return {
-            "operation_type": "update_client",
-            "bonus_points": data or bonus_information.bonus_active,
-            "PIN": str(value.pin),
-        }
+        return BonusApi._check_on_success(
+            BonusApi._make_call(
+                BonusApi._update_card_data(value,
+                    {"bonus_points": data or bonus_information.bonus_active}
+                )
+            )
+        )
 
-    def update_bonuses(self, value: PolibasePerson, data: int | None = None) -> None:
-        return (
-            BonusApi._make_call(BonusApi._update_bonuses_data(value, data))["message"] == "ok"
+    def update_visit_datetime(self, value: PolibasePerson, data: datetime) -> bool:
+        return BonusApi._check_on_success(
+            BonusApi._make_call(
+                BonusApi._update_card_data(
+                    value,
+                    {
+                        "closest_visit_date": A.D_F.datetime(
+                            data, A.CT.DATETIME_SECONDLESS_FORMAT
+                        )
+                    },
+                )
+            )
         )
 
     @staticmethod
     def _update_card_data(value: PolibasePerson, data: strdict) -> strdict:
+        full_name_list: list[str] = value.FullName.split(A.D.SPLIT_SYMBOL)
         data["operation_type"] = "update_client"
         data["PIN"] = str(value.pin)
+        data["first_name"] = full_name_list[1]
+        data["last_name"] = full_name_list[0]
         return data
 
     def update_card(self, value: PolibasePerson, data: strdict) -> bool:
-        return (
-            BonusApi._make_call(BonusApi._update_card_data(value, data))["message"]
-            == "ok"
+        return BonusApi._check_on_success(
+            BonusApi._make_call(BonusApi._update_card_data(value, data))
         )
 
     @staticmethod
     def _remove_bonus_card_data(value: PolibasePerson) -> strdict:
         return {
             "operation_type": "delete_client",
             "PIN": str(value.pin),
         }
 
+    @staticmethod
+    def _check_on_success(value: strdict) -> bool:
+        return value["message"] == "ok" and value["status"] == "ok"
+
     def remove_bonus_card(self, value: PolibasePerson) -> bool:
         if self.exists_bonus_card(value):
             A.A_E.remove(
-                A.CT_E.POLIBASE_PERSONS_BONUS_CARD_WAS_CREATED,
+                A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
                 (value.pin,),
             )
-            return (
-                BonusApi._make_call(BonusApi._remove_bonus_card_data(value))["status"]
-                == "ok"
+            return BonusApi._check_on_success(
+                BonusApi._make_call(BonusApi._remove_bonus_card_data(value))
             )
         return False
```

### Comparing `pih-bonus-0.11/BonusProgramService/service.py` & `pih-bonus-0.12/BonusProgramService/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                                 A.CT_S.BONUS_PROGRAM_BONUS_MINIMUM
                             ):
                                 link: str | None = None
                                 if api.exists_bonus_card(polibase_person):
                                     if not api.exists_bonus_card(polibase_person, True):
                                         event_ds: EventDS | None = one(
                                             A.R_E.get_last(
-                                                A.CT_E.POLIBASE_PERSONS_BONUS_CARD_WAS_CREATED,
+                                                A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
                                                 (polibase_person_pin,),
                                             )
                                         )
                                         link = A.D_Ex_E.value(
                                             event_ds,
                                             "url",
                                         )
@@ -81,35 +81,41 @@
                                             nn(last_timestamp)
                                             and (
                                                 A.D.now() - nnt(last_timestamp)
                                             ).total_seconds()
                                             < 5 * 60
                                         ):
                                             link = None
-
+                                        if one(A.R_E.get_count(
+                                            A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
+                                            (polibase_person_pin,),
+                                        )) > A.S.get(
+                                            A.CT_S.BONUS_PROGRAM_NOTIFICATION_COUNT_MAX
+                                        ):
+                                            link = None
                                         DH.timestamp[polibase_person_pin] = A.D.now()
                                     else:
                                         api.update_bonuses(polibase_person)
                                 else:
                                     link = api.create_bonus_card(polibase_person)
                                     if nn(link):
                                         A.E.send(
-                                            A.CT_E.POLIBASE_PERSONS_BONUS_CARD_WAS_CREATED,
+                                            A.CT_E.POLIBASE_PERSON_BONUS_CARD_WAS_CREATED,
                                             (
                                                 polibase_person_pin,
                                                 link,
                                             ),
                                         )
                                         DH.timestamp[polibase_person_pin] = A.D.now()
                                 if nn(link):
                                     A.ME_WH_W_Q.add_message(
                                         Message(
                                             js(("Перейдите по ссылке:", link)),
                                             polibase_person.telephoneNumber,
-                                            A.D.get(SENDER),
+                                            SENDER,
                                         )
                                     )
                                 else:
                                     pass
                         else:
                             pass
         return None
```

