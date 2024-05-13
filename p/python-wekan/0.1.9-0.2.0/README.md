# Comparing `tmp/python-wekan-0.1.9.tar.gz` & `tmp/python_wekan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-wekan-0.1.9.tar", last modified: Sat Nov 18 14:23:15 2023, max compression
+gzip compressed data, was "python_wekan-0.2.0.tar", last modified: Mon May 13 18:14:11 2024, max compression
```

## Comparing `python-wekan-0.1.9.tar` & `python_wekan-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 14:23:15.602634 python-wekan-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-18 14:23:05.000000 python-wekan-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2023-11-18 14:23:15.602634 python-wekan-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2023-11-18 14:23:05.000000 python-wekan-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 14:23:15.602634 python-wekan-0.1.9/python_wekan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2023-11-18 14:23:15.000000 python-wekan-0.1.9/python_wekan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-18 14:23:15.000000 python-wekan-0.1.9/python_wekan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 14:23:15.000000 python-wekan-0.1.9/python_wekan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-18 14:23:15.000000 python-wekan-0.1.9/python_wekan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-18 14:23:15.000000 python-wekan-0.1.9/python_wekan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-18 14:23:15.602634 python-wekan-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-18 14:23:05.000000 python-wekan-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 14:23:15.602634 python-wekan-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 14:23:05.000000 python-wekan-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2023-11-18 14:23:05.000000 python-wekan-0.1.9/tests/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 14:23:15.602634 python-wekan-0.1.9/wekan/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15921 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/board.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/card.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/card_checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/card_checklist_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/card_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/customfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/swimlane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/wekan_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2023-11-18 14:23:05.000000 python-wekan-0.1.9/wekan/wekan_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:14:11.338043 python_wekan-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-13 18:14:07.000000 python_wekan-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-13 18:14:11.338043 python_wekan-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-13 18:14:07.000000 python_wekan-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:14:11.338043 python_wekan-0.2.0/python_wekan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-13 18:14:11.000000 python_wekan-0.2.0/python_wekan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 18:14:11.000000 python_wekan-0.2.0/python_wekan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:14:11.000000 python_wekan-0.2.0/python_wekan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 18:14:11.000000 python_wekan-0.2.0/python_wekan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 18:14:11.000000 python_wekan-0.2.0/python_wekan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:14:11.338043 python_wekan-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-13 18:14:07.000000 python_wekan-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:14:11.338043 python_wekan-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:14:07.000000 python_wekan-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-13 18:14:07.000000 python_wekan-0.2.0/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:14:11.338043 python_wekan-0.2.0/wekan/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/card_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/card_checklist_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/card_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/customfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/swimlane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/wekan_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-13 18:14:07.000000 python_wekan-0.2.0/wekan/wekan_list.py
```

### Comparing `python-wekan-0.1.9/LICENSE` & `python_wekan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.9/PKG-INFO` & `python_wekan-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.9
+Version: 0.2.0
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.9/README.md` & `python_wekan-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.9/python_wekan.egg-info/PKG-INFO` & `python_wekan-0.2.0/python_wekan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.9
+Version: 0.2.0
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.9/setup.py` & `python_wekan-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='python-wekan',
-    version='0.1.9',
+    version='0.2.0',
     packages=['tests', 'wekan'],
     url='https://github.com/bastianwenske/python-wekan',
     download_url='https://github.com/bastianwenske/python-wekan',
     license='BSD 3-Clause License',
     author='Bastian Wenske',
     author_email='',
     description='This is a python client for interacting with the WeKan® REST-API',
```

### Comparing `python-wekan-0.1.9/tests/test_cases.py` & `python_wekan-0.2.0/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.9/wekan/board.py` & `python_wekan-0.2.0/wekan/board.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.wekan_client import WekanClient
 
 import re
 
 from wekan.base import WekanBase
 from wekan.customfield import Customfield
 from wekan.integration import Integration
 from wekan.label import Label
 from wekan.swimlane import Swimlane
 from wekan.wekan_list import List
 
 
 class Board(WekanBase):
-    def __init__(self, client, board_id: str) -> None:
+    def __init__(self, client: WekanClient, board_id: str) -> None:
         """ Reference to a Wekan board. """
         super().__init__()
         self.client = client
         self.id = board_id
 
         self.__raw_data = self.client.fetch_json(f'/api/boards/{self.id}')
         self.title = self.__raw_data['title']
@@ -60,74 +63,74 @@
         self.sort = self.__raw_data['sort']
 
 
     def __repr__(self) -> str:
         return f"<Board (id: {self.id}, title: {self.title})>"
 
     @classmethod
-    def from_dict(cls, client, data: dict, ) -> Board:
+    def from_dict(cls, client: WekanClient, data: dict, ) -> Board:
         """
         Creates an instance of class Customfield by using the API-Response of Customfield creation.
         :param client: Instance of the wekan api client
         :param data: Response of CustomField creation
         :return: Instance of class CustomField
         """
         return cls(client=client, board_id=data['_id'])
 
     @classmethod
-    def from_list(cls, client, data: dict) -> list:
+    def from_list(cls, client: WekanClient, data: dict) -> list[Board]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param client: Instance of the wekan api client
         :param data: Responses of GET Boards
         :return Instances of class Board
         :rtype list
         """
         instances = []
         for board in data:
             instances.append(cls(client=client, board_id=board['_id']))
         return instances
 
-    def list_custom_fields(self, regex_filter='.*') -> list:
+    def list_custom_fields(self, regex_filter='.*') -> list[Customfield]:
         """
         List all (matching) custom field
         :param regex_filter: Regex filter that will be applied to the search.
-        :return: list of users
+        :return: Instances of class Customfield
         """
         all_custom_fields = Customfield.from_list(parent_board=self, data=self.__get_all_custom_fields())
         return [field for field in all_custom_fields if re.search(regex_filter, field.name)]
 
-    def list_labels(self, regex_filter='.*') -> list:
+    def list_labels(self, regex_filter='.*') -> list[Label]:
         """
         List all (matching) labels
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of labels
         """
         all_labels = Label.from_list(parent_board=self, data=self.__raw_data.get('labels', []))
-        return [label for label in all_labels if re.search(regex_filter, label.title)]
+        return [label for label in all_labels if re.search(regex_filter, label.name)]
 
-    def list_lists(self, regex_filter='.*') -> list:
+    def list_lists(self, regex_filter='.*') -> list[List]:
         """
         List all (matching) labels
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of lists
         """
         all_lists = List.from_list(parent_board=self, data=self.__get_all_lists())
         return [w_list for w_list in all_lists if re.search(regex_filter, w_list.title)]
 
-    def list_swimlanes(self, regex_filter='.*') -> list:
+    def list_swimlanes(self, regex_filter='.*') -> list[Swimlane]:
         """
         List all (matching) swimlanes
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of swimlanes
         """
         all_swimlanes = Swimlane.from_list(parent_board=self, data=self.__get_all_swimlanes())
         return [swimlane for swimlane in all_swimlanes if re.search(regex_filter, swimlane.title)]
 
-    def list_integrations(self, regex_filter='.*') -> list:
+    def list_integrations(self, regex_filter='.*') -> list[Integration]:
         """
         List all (matching) integrations
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of integrations
         """
         all_integrations = Integration.from_list(parent_board=self, data=self.__get_all_integrations())
         return [integration for integration in all_integrations if re.search(regex_filter, integration.title)]
@@ -166,78 +169,78 @@
         :return: Instance of type Customfield
         """
         response = self.client.fetch_json(f'/api/boards/{self.id}/custom-fields/{custom_field_id}')
         return Customfield.from_dict(parent_board=self, data=response)
 
     def __get_all_custom_fields(self) -> list:
         """
-        Get all custom fields by calling the API according to https://wekan.github.io/api/v6.22/#get_all_custom_fields
+        Get all custom fields by calling the API according to https://wekan.github.io/api/v7.42/#get_all_custom_fields
         :return: All custom field instances as list
         """
         return self.client.fetch_json(f'/api/boards/{self.id}/custom-fields')
 
     def __get_all_lists(self) -> list:
         """
-        Get all lists by calling the API according to https://wekan.github.io/api/v6.22/#get_all_lists
+        Get all lists by calling the API according to https://wekan.github.io/api/v7.42/#get_all_lists
         :return: All lists as list
         """
         return self.client.fetch_json(f'/api/boards/{self.id}/lists')
 
     def __get_all_swimlanes(self) -> list:
         """
-        Get all swimlanes by calling the API according to https://wekan.github.io/api/v6.22/#get_all_swimlanes
+        Get all swimlanes by calling the API according to https://wekan.github.io/api/v7.42/#get_all_swimlanes
         :return: All swimlanes as list
         """
         return self.client.fetch_json(f'/api/boards/{self.id}/swimlanes')
 
     def __get_all_integrations(self) -> list:
         """
-        Get all integrations by calling the API according to https://wekan.github.io/api/v6.22/#get_integration
+        Get all integrations by calling the API according to https://wekan.github.io/api/v7.42/#get_integration
         :return: All integrations as list
         """
         return self.client.fetch_json(f'/api/boards/{self.id}/integrations')
 
     def add_list(self, title: str) -> List:
         """
-        Creates a new list instance according to https://wekan.github.io/api/v6.22/#new_list
+        Creates a new list instance according to https://wekan.github.io/api/v7.42/#new_list
         :param title: Name of the new list
         :return: Instance of Class List
         """
         payload = {"title": title}
         response = self.client.fetch_json(uri_path=f'/api/boards/{self.id}/lists',
                                           http_method="POST", payload=payload)
         return List.from_dict(parent_board=self, data=response)
 
     def add_swimlane(self, title: str) -> Swimlane:
         """
-        Creates a new swimlane instance according to https://wekan.github.io/api/v6.22/#new_swimlane
+        Creates a new swimlane instance according to https://wekan.github.io/api/v7.42/#new_swimlane
         :param title: Name of the new swimlane
         :return: Instance of Class Swimlane
         """
         payload = {"title": title}
         response = self.client.fetch_json(uri_path=f'/api/boards/{self.id}/swimlanes',
                                           http_method="POST", payload=payload)
         return Swimlane.from_dict(parent_board=self, data=response)
 
     def add_integration(self, url: str) -> Integration:
         """
-        Creates a new integration instance according to https://wekan.github.io/api/v6.22/#new_integration
+        Creates a new integration instance according to https://wekan.github.io/api/v7.42/#new_integration
         :param url: the URL of the integration
         :return: Instance of Class Integration
         """
         payload = {"url": url}
         response = self.client.fetch_json(uri_path=f'/api/boards/{self.id}/integrations',
                                           http_method="POST", payload=payload)
         return Integration.from_dict(parent_board=self, data=response)
 
     def add_custom_field(self, name: str, field_type: str, show_on_card: bool,
                          automatically_on_card: bool, show_label_on_minicard: bool,
                          show_sum_at_top_of_list: bool, settings=dict) -> Customfield:
         """
-        Creates a new customfield instance according to https://wekan.github.io/api/v6.22/#new_custom_field
+        Creates a new customfield instance according to https://wekan.github.io/api/v7.42/#new_custom_field
         :param name: Name of the new custom field.
         :param field_type: Type of field. See also allowed_fields.
         :param show_on_card: Determines if the custom field should be placed on card.
         :param automatically_on_card: Determines if the custom field should be placed automatically on card.
         :param show_label_on_minicard: Determines if the custom field should be showed on the mini card.
         :param show_sum_at_top_of_list: Determines if summary of all values should be placed on top of the list.
         :param settings: Setting to apply to custom field.
@@ -258,38 +261,38 @@
         }
         response = self.client.fetch_json(uri_path=f'/api/boards/{self.id}/custom-fields',
                                           http_method="POST", payload=payload)
         return Customfield.from_dict(parent_board=self, data=response)
 
     def delete(self) -> None:
         """
-        Delete this board instance according to https://wekan.github.io/api/v6.22/#delete_board
+        Delete this board instance according to https://wekan.github.io/api/v7.42/#delete_board
         :return: None
         """
         self.client.fetch_json(f'/api/boards/{self.id}', http_method="DELETE")
 
     def export(self) -> dict:
         """
-        Export the instance Board according to https://wekan.github.io/api/v6.22/#export
+        Export the instance Board according to https://wekan.github.io/api/v7.42/#export
         :return: Export of the board in dict format.
         """
         return self.client.fetch_json(f'/api/boards/{self.id}/export')
 
     def add_label(self):
         """
-        Create a new Label instance according to https://wekan.github.io/api/v6.22/#add_board_label
+        Create a new Label instance according to https://wekan.github.io/api/v7.42/#add_board_label
         Currently, there is a problem when api handles the request:
         Api docs do not match with actual behaviour.
-        see also: https://wekan.github.io/api/v6.22/?shell#add_board_label
+        see also: https://wekan.github.io/api/v7.42/?shell#add_board_label
         """
         raise NotImplementedError
 
     def add_member(self, user_id: str, is_admin: bool, is_no_comments: bool, is_comments_only: bool) -> None:
         """
-        Add a member to a board according to https://wekan.github.io/api/v6.22/#add_board_member
+        Add a member to a board according to https://wekan.github.io/api/v7.42/#add_board_member
         :param user_id: ID of user to add as member to the board.
         :param is_admin: Defines if the user an admin of the board
         :param is_no_comments: Defines if user is allowed to comment (only)
         :param is_comments_only: Defines if user is allowed to comment (only)
         :return: None
         """
         payload = {
@@ -299,25 +302,25 @@
             "isCommentOnly": is_comments_only
         }
         self.client.fetch_json(uri_path=f'/api/boards/{self.id}/members/{user_id}/add',
                                http_method="POST", payload=payload)
 
     def remove_member(self, user_id: str) -> None:
         """
-        Remove a member from a board according to https://wekan.github.io/api/v6.22/#remove_board_member
+        Remove a member from a board according to https://wekan.github.io/api/v7.42/#remove_board_member
         :param user_id: ID of user that will be removed as member of the board.
         :return: None
         """
         self.client.fetch_json(uri_path=f'/api/boards/{self.id}/members/{user_id}/remove',
                                http_method="POST", payload={"action": "remove"})
 
     def change_member_permission(self, user_id: str, is_admin: bool, is_no_comments: bool,
                                  is_comments_only: bool) -> None:
         """
-        Change the board member permission according to https://wekan.github.io/api/v6.22/#set_board_member_permission
+        Change the board member permission according to https://wekan.github.io/api/v7.42/#set_board_member_permission
         :param user_id: ID of user that permissions need to change.
         :param is_admin: Defines if the user an admin of the board
         :param is_no_comments: Defines if user is allowed to comment (only)
         :param is_comments_only: Defines if user is allowed to comment (only)
         :return: None
         """
         payload = {
```

### Comparing `python-wekan-0.1.9/wekan/card.py` & `python_wekan-0.2.0/wekan/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.wekan_list import List
 
 from datetime import date
 import re
 
 from wekan.base import WekanBase
 from wekan.card_checklist import CardChecklist
 from wekan.card_comment import CardComment
 
 
 class Card(WekanBase):
-    def __init__(self, parent_list, card_id: str) -> None:
+    def __init__(self, parent_list: List, card_id: str) -> None:
         """ Reference to a Wekan Card """
         super().__init__()
         self.list = parent_list
         self.id = card_id
 
         uri = f'/api/boards/{self.list.board.id}/lists/{self.list.id}/cards/{self.id}'
         data = self.list.board.client.fetch_json(uri)
@@ -22,28 +25,31 @@
         self.label_ids = data['labelIds']
         self.custom_fields = data['customFields']
         self.sort = data['sort']
         self.swimlane_id = data['swimlaneId']
         self.card_number = data['cardNumber']
         self.archived = data['archived']
         self.parent_id = data['parentId']
-        self.cover_id = data['coverId']
         self.created_at = self.list.board.client.parse_iso_date(data['createdAt'])
         self.modified_at = self.list.board.client.parse_iso_date(data['modifiedAt'])
         self.date_last_activity = self.list.board.client.parse_iso_date(data['dateLastActivity'])
         self.description = data['description']
         self.requested_by = data['requestedBy']
         self.assigned_by = data['assignedBy']
         self.assignees = data['assignees']
         self.spent_time = data['spentTime']
         self.is_overtime = data['isOvertime']
         self.subtask_sort = data['subtaskSort']
         self.linked_id = data['linkedId']
         # Following things are not always defined if card was created on a very old version of WeKan
         try:
+            self.cover_id = data['coverId']
+        except KeyError:
+            self.cover_id = None
+        try:
             self.vote = data['vote']
         except KeyError:
             self.vote = None
         try:
             self.poker = data['poker']
         except KeyError:
             self.poker = None
@@ -56,103 +62,104 @@
         except KeyError:
             self.link_type_gantt = None
         try:
             self.link_id_gantt = data['linkId_gantt']
         except KeyError:
             self.link_id_gantt = None
         try:
-            self.due_at = self.list.board.client.parse_iso_date(data['dueAt'])
+            if data['dueAt']:
+                self.due_at = self.list.board.client.parse_iso_date(data['dueAt'])
         except KeyError:
             self.due_at = None
 
     def __repr__(self) -> str:
         return f"<Card (id: {self.id}, title: {self.title})>"
 
     @classmethod
-    def from_dict(cls, parent_list, data: dict) -> Card:
+    def from_dict(cls, parent_list: List, data: dict) -> Card:
         """
         Creates an instance of class Card by using the API-Response of Card GET.
         :param parent_list: Instance of Class List pointing to the current Board
         :param data: Response of Card GET.
         :return: Instance of class Card
         """
         return cls(parent_list=parent_list, card_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_list, data: list) -> list:
+    def from_list(cls, parent_list: List, data: list) -> list[Card]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_list: Instance of Class List pointing to the current Board
         :param data: Response of Card GET.
         :return: Instances of class Card
         """
         instances = []
         for card in data:
             instances.append(cls(parent_list=parent_list, card_id=card['_id']))
         return instances
 
     def __get_all_checklists(self) -> list:
         """
-        Get all Checklists by calling the API according to https://wekan.github.io/api/v6.22/#get_all_checklists
+        Get all Checklists by calling the API according to https://wekan.github.io/api/v7.42/#get_all_checklists
         :return: All Checklists
         """
         return self.list.board.client.fetch_json(f'/api/boards/{self.list.board.id}/cards/{self.id}/checklists')
 
-    def list_checklists(self, regex_filter='.*') -> list:
+    def list_checklists(self, regex_filter='.*') -> list[CardChecklist]:
         """
         List all (matching) checklists
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of checklists
         """
         all_checklists = CardChecklist.from_list(parent_card=self, data=self.__get_all_checklists())
         return [checklist for checklist in all_checklists if re.search(regex_filter, checklist.title)]
 
     def __get_all_comments(self) -> list:
         """
-        Get all Comments by calling the API according to https://wekan.github.io/api/v6.22/#get_all_comments
+        Get all Comments by calling the API according to https://wekan.github.io/api/v7.42/#get_all_comments
         :return: All Checklists
         """
         return self.list.board.client.fetch_json(f'/api/boards/{self.list.board.id}/cards/{self.id}/comments')
 
-    def list_comments(self, author_id=None) -> list:
+    def list_comments(self, author_id=None) -> list[CardComment]:
         """
-        List all (matching) checklists
+        List all (matching) comments
         :param author_id: author_id filter that will be applied to the search.
-        :return: list of checklists
+        :return: list of comments
         """
         all_comments = CardComment.from_list(parent_card=self, data=self.__get_all_comments())
         if author_id:
             return [comment for comment in all_comments if author_id == comment.author_id]
         else:
             return all_comments
 
     def delete(self) -> None:
         """
-        Delete the Card instance according to https://wekan.github.io/api/v6.22/#delete_card
+        Delete the Card instance according to https://wekan.github.io/api/v7.42/#delete_card
         :return: API Response as type dict containing the id of the deleted card
         """
         uri = f'/api/boards/{self.list.board.id}/lists/{self.list.id}/cards/{self.id}'
         self.list.board.client.fetch_json(uri, http_method="DELETE")
 
     def add_checklist(self, title: str) -> CardChecklist:
         """
-        Create a new CardChecklist instance according to https://wekan.github.io/api/v6.22/#new_checklist
+        Create a new CardChecklist instance according to https://wekan.github.io/api/v7.42/#new_checklist
         :param title: Title of the new checklist.
         :return: Instance of class CardChecklist
         """
         payload = {
             "title": title
         }
         uri = f'/api/boards/{self.list.board.id}/cards/{self.id}/checklists'
         response = self.list.board.client.fetch_json(uri_path=uri, http_method="POST", payload=payload)
         return CardChecklist.from_dict(parent_card=self, data=response)
 
     def add_comment(self, text: str) -> CardComment:
         """
-        Create a new CardChecklist instance according to https://wekan.github.io/api/v6.22/#new_comment
+        Create a new CardChecklist instance according to https://wekan.github.io/api/v7.42/#new_comment
         :param text: Text of the new comment.
         :return: Instance of class CardComment
         """
         payload = {
             "authorId": self.list.board.client.user_id,
             "comment": text
         }
@@ -161,15 +168,15 @@
         return CardComment.from_dict(parent_card=self, data=response)
 
     def edit(self, title=None, new_list=None, author_id=None, description=None, color=None, label_ids=None,
              requested_by=None, assigned_by=None, received_at=None, start_at=None, due_at=None, end_at=None,
              spent_time=None, is_overtime=None, custom_fields=None, members=None, new_swimlane=None) -> None:
         """
         Edit the current instance by sending a PUT Request to the API
-        according to https://wekan.github.io/api/v6.22/#edit_card
+        according to https://wekan.github.io/api/v7.42/#edit_card
         :param title: the new title of the card
         :param new_list: instance of class List of the new list (move operation)
         :param author_id: change the owner of the card
         :param description: the new description of the card
         :param color: the new color of the card
         :param label_ids: the new list of label IDs attached to the card
         :param requested_by: the new requestedBy field of the card
@@ -223,11 +230,11 @@
             payload['isOverTime'] = is_overtime
         if custom_fields:
             payload['customFields'] = custom_fields
         if members:
             assert isinstance(members, list)
             payload['members'] = members
         if new_swimlane:
-            payload['swimlaneId	'] = new_swimlane.id
+            payload['swimlaneId'] = new_swimlane.id
 
         uri = f'/api/boards/{self.list.board.id}/lists/{self.list.id}/cards/{self.id}'
         self.list.board.client.fetch_json(uri, payload=payload, http_method="PUT")
```

### Comparing `python-wekan-0.1.9/wekan/card_checklist.py` & `python_wekan-0.2.0/wekan/card_checklist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.card import Card
 
 from wekan.base import WekanBase
 from wekan.card_checklist_item import CardChecklistItem
 
 
 class CardChecklist(WekanBase):
-    def __init__(self, parent_card, checklist_id: str) -> None:
+    def __init__(self, parent_card: Card, checklist_id: str) -> None:
         """ Reference to a Wekan Card Checklist """
         super().__init__()
         self.card = parent_card
         self.id = checklist_id
 
         uri = f'/api/boards/{self.card.list.board.id}/cards/{self.card.id}/checklists/{self.id}'
         self.__raw_data = self.card.list.board.client.fetch_json(uri)
         self.title = self.__raw_data['title']
         self.sort = self.__raw_data['sort']
         self.createdAt = self.card.list.board.client.parse_iso_date(self.__raw_data['createdAt'])
         self.modified_at = self.card.list.board.client.parse_iso_date(self.__raw_data['modifiedAt'])
 
-    def list_checklists(self) -> list:
+    def list_checklists(self) -> list[CardChecklist]:
         """
         List all checklist items
         :return: list of checklist items
         """
         return CardChecklistItem.from_list(parent_checklist=self, data=self.__raw_data['items'])
 
     def __repr__(self) -> str:
         return f"<CardChecklist (id: {self.id}, title: {self.title})>"
 
     @classmethod
-    def from_dict(cls, parent_card, data: dict) -> CardChecklist:
+    def from_dict(cls, parent_card: Card, data: dict) -> CardChecklist:
         """
         Creates an instance of class CardChecklist by using the API-Response of CardChecklist GET.
         :param parent_card: Instance of Class Card pointing to the current Card of this Checklist
         :param data: Response of CardChecklist GET.
         :return: Instance of class CardChecklist
         """
         return cls(parent_card=parent_card, checklist_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_card, data: list) -> list:
+    def from_list(cls, parent_card: Card, data: list) -> list[CardChecklist]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_card: Instance of Class Card pointing to the current Card of this Checklist
         :param data: Response of CardChecklist GET.
         :return: Instances of class CardChecklist
         """
         instances = []
         for checklist in data:
             instances.append(cls(parent_card=parent_card, checklist_id=checklist['_id']))
         return instances
 
     def edit(self, data: dict) -> None:
         """
         Edit the current instance by sending a PUT Request to the API.
-        Currently, this is not supported by API. See also: https://wekan.github.io/api/v6.22/#wekan-rest-api-checklists
+        Currently, this is not supported by API. See also: https://wekan.github.io/api/v7.42/#wekan-rest-api-checklists
         """
         raise NotImplementedError
 
     def delete(self) -> None:
         """
-        Delete the Card Checklist instance according to https://wekan.github.io/api/v6.22/#delete_checklist
+        Delete the Card Checklist instance according to https://wekan.github.io/api/v7.42/#delete_checklist
         :return: None
         """
         uri = f'/api/boards/{self.card.list.board.id}/cards/{self.card.id}/checklists/{self.id}'
         self.card.list.board.client.fetch_json(uri, http_method="DELETE")
 
     def add_item(self) -> CardChecklistItem:
         """
         Add a new CardCheckListItem.
         Currently, this is not supported by API.
-        See also: https://wekan.github.io/api/v6.22/#wekan-rest-api-checklistitems
+        See also: https://wekan.github.io/api/v7.42/#wekan-rest-api-checklistitems
         """
         raise NotImplementedError
```

### Comparing `python-wekan-0.1.9/wekan/card_checklist_item.py` & `python_wekan-0.2.0/wekan/card_checklist_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.card_checklist import CardChecklist
 
 from wekan.base import WekanBase
 
 
 class CardChecklistItem(WekanBase):
-    def __init__(self, parent_checklist, item_id: str, title: str, is_finished: bool) -> None:
+    def __init__(self, parent_checklist: CardChecklist, item_id: str, title: str, is_finished: bool) -> None:
         """ Reference to a Wekan CardChecklistItem """
         super().__init__()
         self.checklist = parent_checklist
         self.id = item_id
         self.title = title
         self.is_finished = is_finished
 
@@ -17,42 +20,42 @@
         data = self.checklist.card.list.board.client.fetch_json(uri)
         self.sort = data['sort']
 
     def __repr__(self) -> str:
         return f"<CardChecklistItem (id: {self.id}, title: {self.title}, is_finished: {self.is_finished})>"
 
     @classmethod
-    def from_dict(cls, parent_checklist, data: dict) -> CardChecklistItem:
+    def from_dict(cls, parent_checklist: CardChecklist, data: dict) -> CardChecklistItem:
         """
         Creates an instance of class CardChecklist by using the API-Response of CardChecklist GET.
         :param parent_checklist: Instance of Class CardChecklist pointing to the current Checklist of this ChecklistItem
         :param data: Response of CardChecklist GET.
         :return: Instance of class CardChecklistItem
         """
         return cls(parent_checklist=parent_checklist, item_id=data['_id'],
                    title=data['title'], is_finished=data['isFinished'])
 
     @classmethod
-    def from_list(cls, parent_checklist, data: list) -> list:
+    def from_list(cls, parent_checklist: CardChecklist, data: list) -> list[CardChecklistItem]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_checklist: Instance of Class CardChecklist pointing to the current Checklist of this ChecklistItem
         :param data: Response of CardChecklist GET.
-        :return: Instances of class CardChecklist
+        :return: Instances of class CardChecklistItem
         """
         instances = []
         for item in data:
             instances.append(cls(parent_checklist=parent_checklist, item_id=item['_id'],
                                  title=item['title'], is_finished=item['isFinished']))
         return instances
 
     def edit(self, is_finished=None, title=None) -> None:
         """
         Edit the current instance by sending a PUT Request to the API
-        according to https://wekan.github.io/api/v6.22/#edit_checklist_item
+        according to https://wekan.github.io/api/v7.42/#edit_checklist_item
         :param is_finished: is the item checked?
         :param title: the new text of the item
         :return: None
         """
         payload = {}
         if is_finished:
             payload["isFinished"] = is_finished
@@ -66,23 +69,23 @@
     def mark_as_finished(self) -> None:
         """
         Mark this instance as finished.
         :return: None
         """
         self.edit(is_finished=True)
 
-    def change_title(self, new_title) -> None:
+    def change_title(self, new_title: str) -> None:
         """
         Set a new title for this instance.
         :param new_title: The new title.
         :return: None
         """
         self.edit(title=new_title)
 
     def delete(self) -> None:
         """
-        Delete the Card Checklist instance according to https://wekan.github.io/api/v6.22/#delete_checklist_item
+        Delete the Card Checklist instance according to https://wekan.github.io/api/v7.42/#delete_checklist_item
         :return: None
         """
         uri = f'/api/boards/{self.checklist.card.board.id}/cards/{self.checklist.card.id}/' \
               f'checklists/{self.checklist.id}/items/{self.id}'
         self.checklist.card.board.client.fetch_json(uri, http_method="DELETE")
```

### Comparing `python-wekan-0.1.9/wekan/card_comment.py` & `python_wekan-0.2.0/wekan/card_comment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.card import Card
 
 from wekan.base import WekanBase
 
 
 class CardComment(WekanBase):
-    def __init__(self, parent_card, comment_id: str) -> None:
+    def __init__(self, parent_card: Card, comment_id: str) -> None:
         """ Reference to a Wekan CardComment """
         super().__init__()
         self.card = parent_card
         self.id = comment_id
 
         uri = f'/api/boards/{self.card.list.board.id}/cards/{self.card.id}/comments/{self.id}'
         data = self.card.list.board.client.fetch_json(uri)
@@ -17,25 +20,25 @@
         self.createdAt = self.card.list.board.client.parse_iso_date(data['createdAt'])
         self.modified_at = self.card.list.board.client.parse_iso_date(data['modifiedAt'])
 
     def __repr__(self) -> str:
         return f"<CardComment (id: {self.id}, text: {self.text})>"
 
     @classmethod
-    def from_dict(cls, parent_card, data: dict) -> CardComment:
+    def from_dict(cls, parent_card: Card, data: dict) -> CardComment:
         """
         Creates an instance of class CardComment by using the API-Response of CardComment GET.
         :param parent_card: Instance of Class Card pointing to the Card of this Comment
         :param data: Response of CardComment GET.
         :return: Instance of class CardComment
         """
         return cls(parent_card=parent_card, comment_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_card, data: list) -> list:
+    def from_list(cls, parent_card: Card, data: list) -> list[CardComment]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_card: Instance of Class Card pointing to the current Card of this Comment
         :param data: Response of CardComment GET.
         :return: Instances of class CardComment
         """
         instances = []
@@ -43,18 +46,18 @@
             instances.append(cls(parent_card=parent_card, comment_id=comment['_id']))
         return instances
 
     def edit(self, data: dict) -> None:
         """
         Edit the current instance by sending a PUT Request to the API.
         Currently, this is not supported by API.
-        See also: https://wekan.github.io/api/v6.22/#wekan-rest-api-cardcomments
+        See also: https://wekan.github.io/api/v7.42/#wekan-rest-api-cardcomments
         """
         raise NotImplementedError
 
     def delete(self) -> None:
         """
-        Delete the CardComment instance according to https://wekan.github.io/api/v6.22/#delete_comment
+        Delete the CardComment instance according to https://wekan.github.io/api/v7.42/#delete_comment
         :return: None
         """
         uri = f'/api/boards/{self.card.list.board.id}/cards/{self.card.id}/comments/{self.id}'
         self.card.list.board.client.fetch_json(uri, http_method="DELETE")
```

### Comparing `python-wekan-0.1.9/wekan/customfield.py` & `python_wekan-0.2.0/wekan/customfield.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.board import Board
 
 from wekan.base import WekanBase
 
 
 class Customfield(WekanBase):
-    def __init__(self, parent_board, custom_field_id: str) -> None:
+    def __init__(self, parent_board: Board, custom_field_id: str) -> None:
         """ Reference to a Customfield within a Wekan Board """
         super().__init__()
         self.board = parent_board
         self.id = custom_field_id
 
         data = self.board.client.fetch_json(f'/api/boards/{self.board.id}/custom-fields/{self.id}')
         self.name = data['name']
@@ -20,37 +23,39 @@
         self.automatically_on_card = data['automaticallyOnCard']
         self.show_label_on_mini_card = data['showLabelOnMiniCard']
 
     def __repr__(self) -> str:
         return f"<Customfield (name: {self.name}, id: {self.id})>"
 
     @classmethod
-    def from_dict(cls, parent_board, data: dict) -> Customfield:
+    def from_dict(cls, parent_board: Board, data: dict) -> Customfield:
         """
         Creates an instance of class Customfield by using the API-Response of Customfield GET.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of CustomField creation.
         :return: Instance of class CustomField
         """
         return cls(parent_board=parent_board, custom_field_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_board, data: list) -> list:
+    def from_list(cls, parent_board: Board, data: list) -> list[Customfield]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of CustomField creation.
         :return: Instances of class CustomField
         """
-        instances = [cls(parent_board=parent_board, custom_field_id=field['_id']) for field in data]
+        instances = []
+        for field in data:
+            instances.append(cls(parent_board=parent_board, custom_field_id=field['_id']))
         return instances
 
     def delete(self) -> dict:
         """
-        Delete the CustomField instance according to https://wekan.github.io/api/v6.22/#get_custom_field
+        Delete the CustomField instance according to https://wekan.github.io/api/v7.42/#get_custom_field
         :return: API Response as type dict containing the id of the deleted CustomField
         """
         return self.board.client.fetch_json(f'/api/boards/{self.board.id}/custom-fields/{self.id}',
                                             http_method="DELETE")
 
     def edit(self, data: dict) -> None:
         """
```

### Comparing `python-wekan-0.1.9/wekan/integration.py` & `python_wekan-0.2.0/wekan/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.board import Board
 
 from wekan.base import WekanBase
 
 
 class Integration(WekanBase):
-    def __init__(self, parent_board, integration_id: str) -> None:
+    def __init__(self, parent_board: Board, integration_id: str) -> None:
         """ Reference to a Wekan Integration """
         super().__init__()
         self.board = parent_board
         self.id = integration_id
         data = self.board.client.fetch_json(f'/api/boards/{self.board.id}/integrations/{self.id}')
         self.title = data.get('title', '')
         self.url = data['url']
@@ -18,59 +21,59 @@
         self.created_at = self.board.client.parse_iso_date(data['createdAt'])
         self.modified_at = self.board.client.parse_iso_date(data['modifiedAt'])
 
     def __repr__(self) -> str:
         return f"<Integration (id: {self.id}, title: {self.title})>"
 
     @classmethod
-    def from_dict(cls, parent_board, data: dict) -> Integration:
+    def from_dict(cls, parent_board: Board, data: dict) -> Integration:
         """
         Creates an instance of class Integration by using the API-Response of Integration creation.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of Integration creation.
         :return: Instance of class Integration
         """
         return cls(parent_board=parent_board, integration_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_board, data: list) -> list:
+    def from_list(cls, parent_board: Board, data: list) -> list[Integration]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of Integration creation.
         :return: Instances of class Integration
         """
         instances = []
         for integration in data:
             instances.append(cls(parent_board=parent_board, integration_id=integration['_id']))
         return instances
 
     def delete(self) -> None:
         """
-        Delete the Integration instance according to https://wekan.github.io/api/v6.22/#delete_integration
+        Delete the Integration instance according to https://wekan.github.io/api/v7.42/#delete_integration
         :return: None
         """
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/integrations/{self.id}', http_method="DELETE")
 
     def delete_activities(self, activities: list) -> None:
         """
-        Delete all subscribed activities according to https://wekan.github.io/api/v6.22/#delete_integration_activities
+        Delete all subscribed activities according to https://wekan.github.io/api/v7.42/#delete_integration_activities
         :return: None
         """
         payload = {
             "activities": activities
         }
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/integrations/{self.id}/activities',
                                      payload=payload,
                                      http_method="DELETE")
 
     def edit(self, enabled=None, title=None, url=None, token=None, activities=None) -> None:
         """
         Edit the current instance by sending a PUT Request to the API
-        according to https://wekan.github.io/api/v6.22/#edit_integration
+        according to https://wekan.github.io/api/v7.42/#edit_integration
         :param enabled: is the integration enabled?
         :param title: new name of the integration
         :param url: new URL of the integration
         :param token: new token of the integration
         :param activities: new list of activities of the integration
         :return: None
         """
@@ -85,15 +88,15 @@
             payload["token"] = token
         if activities:
             payload["activities"] = activities
 
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/integrations/{self.id}',
                                      payload=payload, http_method="PUT")
 
-    def change_title(self, new_title) -> None:
+    def change_title(self, new_title: str) -> None:
         """
         Set a new title for this instance.
         :param new_title: The new title.
         :return: None
         """
         self.edit(title=new_title)
 
@@ -103,15 +106,15 @@
         :return: None
         """
         self.edit(enabled=True)
 
     def add_activities(self, activities: list) -> None:
         """
         Add subscribed activities by sending a POST Request to the API
-        according to https://wekan.github.io/api/v6.22/#new_integration_activities
+        according to https://wekan.github.io/api/v7.42/#new_integration_activities
         :param activities: the activities value
         :return: None
         """
         assert isinstance(activities, list)
         payload = {"activities": activities}
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/integrations/{self.id}/activities',
                                      payload=payload, http_method="POST")
```

### Comparing `python-wekan-0.1.9/wekan/label.py` & `python_wekan-0.2.0/wekan/label.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.board import Board
 
 from wekan.base import WekanBase
 
 
 class Label(WekanBase):
-    def __init__(self, parent_board, label_id: str, name: str, color="") -> None:
+    def __init__(self, parent_board: Board, label_id: str, name: str, color="") -> None:
         """ Reference to a Wekan Label """
         super().__init__()
         self.board = parent_board
         self.id = label_id
         self.name = name
         self.color = color
 
     def __repr__(self) -> str:
         return f"<Label (name: {self.name}, id: {self.id}, color={self.color})>"
 
     @classmethod
-    def from_dict(cls, parent_board, data: dict) -> Label:
+    def from_dict(cls, parent_board: Board, data: dict) -> Label:
         """
         Creates an instance of class Label by using the API-Response of Label GET.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of Label creation.
         :return: Instance of class Label
         """
         return cls(parent_board=parent_board, label_id=data['_id'], name=data['name'], color=data['color'])
 
     @classmethod
-    def from_list(cls, parent_board, data: list) -> list:
+    def from_list(cls, parent_board: Board, data: list) -> list[Label]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of Label creation.
         :return: Instances of class Label
         """
         instances = []
@@ -38,17 +41,17 @@
             instances.append(cls(parent_board=parent_board, label_id=label['_id'],
                                  name=label['name'], color=label['color']))
         return instances
 
     def delete(self) -> None:
         """
         Delete this Label instance.
-        Currently, not supported by API: https://wekan.github.io/api/v6.22/#wekan-rest-api-boards
+        Currently, not supported by API: https://wekan.github.io/api/v7.42/#wekan-rest-api-boards
         """
         raise NotImplementedError
 
     def edit(self, data: dict) -> None:
         """
         Edit the current instance by sending a PUT Request to the API.
-        Currently, not supported by API: https://wekan.github.io/api/v6.22/#wekan-rest-api-boards
+        Currently, not supported by API: https://wekan.github.io/api/v7.42/#wekan-rest-api-boards
         """
         raise NotImplementedError
```

### Comparing `python-wekan-0.1.9/wekan/swimlane.py` & `python_wekan-0.2.0/wekan/swimlane.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.board import Board
 
 from wekan.base import WekanBase
 
-
 class Swimlane(WekanBase):
-    def __init__(self, parent_board, swimlane_id: str) -> None:
+    def __init__(self, parent_board: Board, swimlane_id: str) -> None:
         """ Reference to a Wekan Swimlane """
         super().__init__()
         self.board = parent_board
         self.id = swimlane_id
 
         data = self.board.client.fetch_json(f'/api/boards/{self.board.id}/swimlanes/{self.id}')
         self.title = data['title']
@@ -19,35 +21,35 @@
         self.color = data.get('color', '')
         self.type = data['type']
 
     def __repr__(self) -> str:
         return f"<Swimlane (id: {self.id}, title: {self.title})>"
 
     @classmethod
-    def from_dict(cls, parent_board, data: dict) -> Swimlane:
+    def from_dict(cls, parent_board: Board, data: dict) -> Swimlane:
         """
         Creates an instance of class Swimlane by using the API-Response of Swimlane GET.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of Swimlane GET.
         :return: Instance of class Swimlane
         """
         return cls(parent_board=parent_board, swimlane_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_board, data: list) -> list:
+    def from_list(cls, parent_board: Board, data: list) -> list[Swimlane]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Responses of Swimlane GET.
         :return: Instances of class Swimlane
         """
         instances = []
         for swimlane in data:
             instances.append(cls(parent_board=parent_board, swimlane_id=swimlane['_id']))
         return instances
 
     def delete(self) -> None:
         """
-        Delete the Swimlane instance according to https://wekan.github.io/api/v6.22/#get_swimlane
+        Delete the Swimlane instance according to https://wekan.github.io/api/v7.42/#get_swimlane
         :return: None
         """
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/swimlanes/{self.id}', http_method="DELETE")
```

### Comparing `python-wekan-0.1.9/wekan/user.py` & `python_wekan-0.2.0/wekan/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.wekan_client import WekanClient
 
 from wekan.base import WekanBase
 
-
 class User(WekanBase):
-    def __init__(self, client, user_id: str) -> None:
+    def __init__(self, client: WekanClient, user_id: str) -> None:
         """ Reference to a Wekan User """
         super().__init__()
         self.id = user_id
         self.client = client
 
         data = self.client.fetch_json(f'/api/users/{self.id}')
         self.username = data['username']
@@ -25,46 +27,46 @@
         self.boards = data.get('boards', [])
         self.is_admin = data.get('isAdmin', False)
 
     def __repr__(self) -> str:
         return f"<User (id: {self.id}, username: {self.username})>"
 
     @classmethod
-    def from_dict(cls, client, data: dict) -> User:
+    def from_dict(cls, client: WekanClient, data: dict) -> User:
         """
         Creates an instance of class User by using the API-Response of User GET.
         :param client: Instance of Class WekanClient pointing to the Client
         :param data: Response of User GET.
         :return: Instance of class User
         """
         return cls(client=client, user_id=data['_id'])
 
     @classmethod
-    def from_list(cls, client, data: list) -> list:
+    def from_list(cls, client: WekanClient, data: list) -> list[User]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param client: Instance of Class WekanClient pointing to the Client
         :param data: Responses of User GET.
         :return: Instances of class User
         """
         instances = []
         for user in data:
             instances.append(cls(client=client, user_id=user['_id']))
         return instances
 
     def delete(self) -> None:
         """
-        Delete the User instance according to https://wekan.github.io/api/v6.22/delete_user
+        Delete the User instance according to https://wekan.github.io/api/v7.42/delete_user
         :return: None
         """
         self.client.fetch_json(f'/api/users/{self.id}', http_method="DELETE")
 
     def edit(self, action: str) -> None:
         """
         Edit the current instance by sending a PUT Request to the API
-        according to https://wekan.github.io/api/v6.22/#edit_user.
+        according to https://wekan.github.io/api/v7.42/#edit_user.
         :param action: Type of action. See also allowed_actions.
         :return: None
         """
         allowed_actions = ["takeOwnership", "disableLogin", "enableLogin"]
         assert action in allowed_actions, f"action not in {allowed_actions}"
         self.client.fetch_json(f'/api/user/{self.id}', payload={"action": action}, http_method="PUT")
```

### Comparing `python-wekan-0.1.9/wekan/wekan_client.py` & `python_wekan-0.2.0/wekan/wekan_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,33 +37,33 @@
     def __get_boards(self) -> dict:
         """
         Returns all boards for your Wekan user.
         :return: a list of Python objects representing the Wekan boards.
         """
         return self.fetch_json(uri_path=f'/api/users/{self.user_id}/boards')
 
-    def list_boards(self, regex_filter='.*') -> list:
+    def list_boards(self, regex_filter='.*') -> list[Board]:
         """
         List all (matching) boards
         :return: list of boards
         """
         public_boards = Board.from_list(self, data=self.__get_public_boards())
         private_boards = Board.from_list(self, data=self.__get_boards())
         all_boards = public_boards + private_boards
         return [board for board in all_boards if re.search(regex_filter, board.title)]
 
     def __get_all_users(self) -> list:
         """
-        Get all users by calling the API according to https://wekan.github.io/api/v6.22/#get_all_users
+        Get all users by calling the API according to https://wekan.github.io/api/v7.42/#get_all_users
         IMPORTANT: Only the admin user (the first user) can call this REST API Endpoint.
         :return: List of instances of class User
         """
         return self.fetch_json('/api/users')
 
-    def list_users(self, regex_filter='.*') -> list:
+    def list_users(self, regex_filter='.*') -> list[User]:
         """
         List all (matching) users
         :return: list of users
         """
         all_users = User.from_list(client=self, data=self.__get_all_users())
         return [user for user in all_users if re.search(regex_filter, user.username)]
 
@@ -138,15 +138,15 @@
 
         return response.json()
 
     def add_board(self, title: str, color: str, owner=None,
                   is_admin=True, is_active=True, is_no_comments=False,
                   is_comment_only=False, permission='private') -> Board:
         """
-        Creates a new board according to https://wekan.github.io/api/v6.22/#new_board
+        Creates a new board according to https://wekan.github.io/api/v7.42/#new_board
         :param title: Title of the board.
         :param color: Color of the board.
         :param owner: Owner (ID) of the board.
         :param is_admin: Bool defines if the board creator is admin.
         :param is_active: Bool defines if the board is active.
         :param is_no_comments: Bool defines if comments are allowed.
         :param is_comment_only: Bool defines if only comments are allowed.
@@ -165,15 +165,15 @@
             'color': color
         }
         response = self.fetch_json(uri_path='/api/boards', http_method="POST", payload=payload)
         return Board.from_dict(client=self, data=response)
 
     def add_user(self, username: str, email: str, password: str) -> User:
         """
-        Creates a new board according to https://wekan.github.io/api/v6.22/#new_user
+        Creates a new board according to https://wekan.github.io/api/v7.42/#new_user
         :param username: Username of the new user.
         :param email: E-Mail of the new user.
         :param password: Passwort of the new user.
         :return: Instance of class User
         """
         payload = {
             'username': username,
```

### Comparing `python-wekan-0.1.9/wekan/wekan_list.py` & `python_wekan-0.2.0/wekan/wekan_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
+import typing
+if typing.TYPE_CHECKING:
+	from wekan.board import Board
 
 import re
 
 from wekan.base import WekanBase
 from wekan.card import Card
 from wekan.swimlane import Swimlane
 
 
 class List(WekanBase):
-    def __init__(self, parent_board, list_id: str) -> None:
+    def __init__(self, parent_board: Board, list_id: str) -> None:
         """ Reference to a Wekan List. """
         super().__init__()
         self.board = parent_board
         self.id = list_id
 
         data = self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}')
         self.title = data['title']
@@ -31,20 +34,20 @@
             print("Failed getting cards_count, instance possibly too old (stable snap?)")
 
     def __repr__(self) -> str:
         return f"<List (id: {self.id}, title: {self.title})>"
 
     def __get_all_cards_on_list(self) -> list:
         """
-        Get all cards by calling the API according to https://wekan.github.io/api/v6.22/#get_list
+        Get all cards by calling the API according to https://wekan.github.io/api/v7.42/#get_list
         :return: All cards
         """
         return self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}/cards')
 
-    def list_cards(self, regex_filter='.*') -> list:
+    def list_cards(self, regex_filter='.*') -> list[Card]:
         """
         List all (matching) cards
         :param regex_filter: Regex filter that will be applied to the search.
         :return: list of cards
         """
         all_cards = Card.from_list(parent_list=self, data=self.__get_all_cards_on_list())
         return [card for card in all_cards if re.search(regex_filter, card.title)]
@@ -55,25 +58,25 @@
         :param card_id: id of the card to fetch data from
         :return: Instance of type Card
         """
         response = self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}/cards/{card_id}')
         return Card.from_dict(parent_list=self, data=response)
 
     @classmethod
-    def from_dict(cls, parent_board, data: dict) -> List:
+    def from_dict(cls, parent_board: Board, data: dict) -> List:
         """
         Creates an instance of class List by using the API-Response of List creation.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of List creation.
         :return: Instance of class List
         """
         return cls(parent_board=parent_board, list_id=data['_id'])
 
     @classmethod
-    def from_list(cls, parent_board, data: list) -> list:
+    def from_list(cls, parent_board: Board, data: list) -> list[List]:
         """
         Wrapper around function from_dict to process multiple objects within one function call.
         :param parent_board: Instance of Class Board pointing to the current Board
         :param data: Response of List creation.
         :return: Instances of class List
         """
         instances = []
@@ -87,15 +90,15 @@
         :return: None
         """
         self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}',
                                      http_method="DELETE")
 
     def add_card(self, title: str, swimlane: Swimlane, description: str = "", members=None) -> Card:
         """
-        Creates a new card instance according to https://wekan.github.io/api/v6.22/#new_card
+        Creates a new card instance according to https://wekan.github.io/api/v7.42/#new_card
         :param title: Title of the new card.
         :param swimlane: Swimlane ID of the new card.
         :param members: Members of the new card.
         :param description: Description of the new card.
         :return: Instance of type Card
         """
         if members is None:
```

