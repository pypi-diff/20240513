# Comparing `tmp/djangoldp_community-3.1.8.tar.gz` & `tmp/djangoldp_community-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_community-3.1.8.tar", last modified: Wed Jan 24 20:17:43 2024, max compression
+gzip compressed data, was "djangoldp_community-3.1.9.tar", last modified: Fri Jan 26 18:11:47 2024, max compression
```

## Comparing `djangoldp_community-3.1.8.tar` & `djangoldp_community-3.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/
--rw-r--r--   0 root         (0) root         (0)      268 2024-01-24 20:17:43.718799 djangoldp_community-3.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      438 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.710799 djangoldp_community-3.1.8/djangoldp_community/
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-01-24 20:17:40.000000 djangoldp_community-3.1.8/djangoldp_community/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/djangoldp_community/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:17:23.000000 djangoldp_community-3.1.8/djangoldp_community/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/djangoldp_community/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:17:23.000000 djangoldp_community-3.1.8/djangoldp_community/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/management/commands/create_community.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/djangoldp_community/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0002_auto_20210217_1205.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0003_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0004_auto_20210323_1121.py
--rw-rw-rw-   0 root         (0) root         (0)     4391 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0005_communityaddress_communityprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0006_auto_20210324_1113.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0007_auto_20210324_1146.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0008_auto_20210415_1744.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0009_auto_20220630_0033.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0010_auto_20220630_0034.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0011_auto_20220711_0837.py
--rw-rw-rw-   0 root         (0) root         (0)     6541 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0012_alter_community_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     2460 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0013_auto_20231014_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/0014_community_owner.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:17:23.000000 djangoldp_community-3.1.8/djangoldp_community/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11669 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/djangoldp_community/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:17:23.000000 djangoldp_community-3.1.8/djangoldp_community/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1766 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/tests/tests_model.py
--rw-rw-rw-   0 root         (0) root         (0)    11653 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/djangoldp_community/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:17:43.714799 djangoldp_community-3.1.8/djangoldp_community.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2024-01-24 20:17:43.000000 djangoldp_community-3.1.8/djangoldp_community.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1615 2024-01-24 20:17:43.000000 djangoldp_community-3.1.8/djangoldp_community.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 20:17:43.000000 djangoldp_community-3.1.8/djangoldp_community.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2024-01-24 20:17:43.000000 djangoldp_community-3.1.8/djangoldp_community.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-01-24 20:17:43.000000 djangoldp_community-3.1.8/djangoldp_community.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-01-24 20:17:43.718799 djangoldp_community-3.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-24 20:17:22.000000 djangoldp_community-3.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      438 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.018541 djangoldp_community-3.1.9/djangoldp_community/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-01-26 18:11:43.000000 djangoldp_community-3.1.9/djangoldp_community/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/djangoldp_community/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/djangoldp_community/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/management/commands/create_community.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/djangoldp_community/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0002_auto_20210217_1205.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0003_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0004_auto_20210323_1121.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0005_communityaddress_communityprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0006_auto_20210324_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0007_auto_20210324_1146.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0008_auto_20210415_1744.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0009_auto_20220630_0033.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0010_auto_20220630_0034.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0011_auto_20220711_0837.py
+-rw-rw-rw-   0 root         (0) root         (0)     6541 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0012_alter_community_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     2460 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0013_auto_20231014_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/0014_community_owner.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11669 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/djangoldp_community/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1766 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/tests/tests_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    11618 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/djangoldp_community/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 18:11:47.022541 djangoldp_community-3.1.9/djangoldp_community.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-01-26 18:11:46.000000 djangoldp_community-3.1.9/djangoldp_community.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-01-26 18:11:46.000000 djangoldp_community-3.1.9/djangoldp_community.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 18:11:46.000000 djangoldp_community-3.1.9/djangoldp_community.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2024-01-26 18:11:46.000000 djangoldp_community-3.1.9/djangoldp_community.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-01-26 18:11:46.000000 djangoldp_community-3.1.9/djangoldp_community.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-01-26 18:11:47.026541 djangoldp_community-3.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-26 18:11:24.000000 djangoldp_community-3.1.9/setup.py
```

### Comparing `djangoldp_community-3.1.8/djangoldp_community/admin.py` & `djangoldp_community-3.1.9/djangoldp_community/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/djangoldp_urls.py` & `djangoldp_community-3.1.9/djangoldp_community/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/management/commands/create_community.py` & `djangoldp_community-3.1.9/djangoldp_community/management/commands/create_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0001_initial.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0002_auto_20210217_1205.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0002_auto_20210217_1205.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0003_auto_20210218_1145.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0003_auto_20210218_1145.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0004_auto_20210323_1121.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0004_auto_20210323_1121.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0005_communityaddress_communityprofile.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0005_communityaddress_communityprofile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0006_auto_20210324_1113.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0006_auto_20210324_1113.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0007_auto_20210324_1146.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0007_auto_20210324_1146.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0010_auto_20220630_0034.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0010_auto_20220630_0034.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0011_auto_20220711_0837.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0011_auto_20220711_0837.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0012_alter_community_options_and_more.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0012_alter_community_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0013_auto_20231014_1439.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0013_auto_20231014_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/migrations/0014_community_owner.py` & `djangoldp_community-3.1.9/djangoldp_community/migrations/0014_community_owner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/models.py` & `djangoldp_community-3.1.9/djangoldp_community/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/tests/runner.py` & `djangoldp_community-3.1.9/djangoldp_community/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/tests/tests_model.py` & `djangoldp_community-3.1.9/djangoldp_community/tests/tests_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community/tests/tests_permissions.py` & `djangoldp_community-3.1.9/djangoldp_community/tests/tests_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 import json
 from rest_framework.test import APITestCase, APIClient
 
 from djangoldp_community.models import Community
 from djangoldp_account.models import LDPUser as User
 
-context = {'@context': {'@vocab': "http://happy-dev.fr/owl/#"}}
+context = {'@context': {'@vocab': "https://cdn.startinblox.com/owl#"}}
 
 class PermissionsTestCase(APITestCase):
     # Django runs setUp automatically before every test
     def setUp(self):
         # we set up a client, that allows us
         self.client = APIClient()
 
@@ -104,19 +104,19 @@
     def test_get_community_is_member(self):
         self.setUpLoggedInUser(is_superuser=False)
         community = self._get_random_community()
         self._add_community_member(user=self.user, community=community, is_admin=False)
 
         response = self.client.get('/communities/{}/'.format(community.slug))
         self.assertEqual(response.status_code, 200)
-        self.assertNotIn({'mode': {'@type': 'add'}}, response.data['permissions'])
+        self.assertNotIn('add', response.data['permissions'])
         self.assertEqual(len(response.data['permissions']), 1)
         response = self.client.get('/groups/{}/'.format(community.members.id))
         self.assertEqual(response.status_code, 200)
-        self.assertNotIn({'mode': {'@type': 'add'}}, response.data['permissions'])
+        self.assertNotIn('add', response.data['permissions'])
         self.assertEqual(len(response.data['permissions']), 1)
 
     def test_get_communities_is_member(self):
         self.setUpLoggedInUser(is_superuser=False)
         community = self._get_random_community()
         self._add_community_member(user=self.user, community=community, is_admin=False)
         response = self.client.get('/communities/')
```

### Comparing `djangoldp_community-3.1.8/djangoldp_community/views.py` & `djangoldp_community-3.1.9/djangoldp_community/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/djangoldp_community.egg-info/SOURCES.txt` & `djangoldp_community-3.1.9/djangoldp_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_community-3.1.8/setup.cfg` & `djangoldp_community-3.1.9/setup.cfg`

 * *Files identical despite different names*

