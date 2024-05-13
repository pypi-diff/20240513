# Comparing `tmp/bestdori-api-1.1.0.tar.gz` & `tmp/bestdori-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori-api-1.1.0.tar", last modified: Mon Apr 29 04:21:49 2024, max compression
+gzip compressed data, was "bestdori-api-1.1.1.tar", last modified: Mon May 13 02:53:51 2024, max compression
```

## Comparing `bestdori-api-1.1.0.tar` & `bestdori-api-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.050933 bestdori-api-1.1.0/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.050933 bestdori-api-1.1.0/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    22526 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/festival.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/missions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/models/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-29 04:21:49.000000 bestdori-api-1.1.0/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 04:21:48.000000 bestdori-api-1.1.0/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:21:49.054933 bestdori-api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-29 04:21:38.000000 bestdori-api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22526 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/festival.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/missions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/setup.py
```

### Comparing `bestdori-api-1.1.0/LICENSE` & `bestdori-api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/PKG-INFO` & `bestdori-api-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -32,14 +32,18 @@
           <img src="https://img.shields.io/github/license/WindowsSov8forUs/bestdori-api" alt="License">
         </a>
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
         </a>
         
+        <a href="https://pypi.org/project/bestdori-api/">
+          <img src="https://img.shields.io/pypi/v/bestdori-api" alt="PyPI Version">
+        </a>
+        
         </p>
         
         > bestdori-api 现已全面支持同步与异步
         > 异步使用方法与同步类似，可几乎无缝切换
         
         ## 简介
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.1 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 > bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
 å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
 è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
 API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
 [BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
```

### Comparing `bestdori-api-1.1.0/README.md` & `bestdori-api-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
   <img src="https://img.shields.io/github/license/WindowsSov8forUs/bestdori-api" alt="License">
 </a>
 
 <a href="https://www.python.org/downloads/">
   <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
 </a>
 
+<a href="https://pypi.org/project/bestdori-api/">
+  <img src="https://img.shields.io/pypi/v/bestdori-api" alt="PyPI Version">
+</a>
+
 </p>
 
 > bestdori-api 现已全面支持同步与异步
 > 异步使用方法与同步类似，可几乎无缝切换
 
 ## 简介
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 > bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
 å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
 è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
 API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
 [BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
```

### Comparing `bestdori-api-1.1.0/bestdori/__init__.py` & `bestdori-api-1.1.1/bestdori/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/ayachan/__init__.py` & `bestdori-api-1.1.1/bestdori/ayachan/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/ayachan/exceptions.py` & `bestdori-api-1.1.1/bestdori/ayachan/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/ayachan/utils/network.py` & `bestdori-api-1.1.1/bestdori/ayachan/utils/network.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/ayachan/utils/utils.py` & `bestdori-api-1.1.1/bestdori/ayachan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/cards.py` & `bestdori-api-1.1.1/bestdori/cards.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/characters.py` & `bestdori-api-1.1.1/bestdori/characters.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/charts.py` & `bestdori-api-1.1.1/bestdori/charts.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/comics.py` & `bestdori-api-1.1.1/bestdori/comics.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/costumes.py` & `bestdori-api-1.1.1/bestdori/costumes.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/eventarchives.py` & `bestdori-api-1.1.1/bestdori/eventarchives.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/events.py` & `bestdori-api-1.1.1/bestdori/events.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/exceptions.py` & `bestdori-api-1.1.1/bestdori/exceptions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/festival.py` & `bestdori-api-1.1.1/bestdori/festival.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/gacha.py` & `bestdori-api-1.1.1/bestdori/gacha.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/logincampaigns.py` & `bestdori-api-1.1.1/bestdori/logincampaigns.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/miracleticket.py` & `bestdori-api-1.1.1/bestdori/miracleticket.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/missions.py` & `bestdori-api-1.1.1/bestdori/missions.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/models/__init__.py` & `bestdori-api-1.1.1/bestdori/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/models/content.py` & `bestdori-api-1.1.1/bestdori/models/content.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/models/note.py` & `bestdori-api-1.1.1/bestdori/models/note.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/player.py` & `bestdori-api-1.1.1/bestdori/player.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/post.py` & `bestdori-api-1.1.1/bestdori/post.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/settings.py` & `bestdori-api-1.1.1/bestdori/settings.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/songmeta.py` & `bestdori-api-1.1.1/bestdori/songmeta.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/songs.py` & `bestdori-api-1.1.1/bestdori/songs.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/upload.py` & `bestdori-api-1.1.1/bestdori/upload.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/user.py` & `bestdori-api-1.1.1/bestdori/user.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/utils/__init__.py` & `bestdori-api-1.1.1/bestdori/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori/utils/network.py` & `bestdori-api-1.1.1/bestdori/utils/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,16 @@
             async with ClientSession() as session:
                 response = await session.request(
                     method,
                     self._url,
                     cookies=cookies,
                     params=params,
                     data=cast(dict, dumps(data)) if data is not None else data,
-                    headers=self.headers if not self.api.endswith('/upload') else None
+                    headers=self.headers if not self.api.endswith('/upload') else None,
+                    proxy=self._proxies
                 )
                 response.raise_for_status()
         
         # 判断接收到的响应是否为 json 格式
         if 'application/json' not in (content_type := response.headers.get('content-type', '')):
             if content_type != '':
                 return response
```

### Comparing `bestdori-api-1.1.0/bestdori/utils/utils.py` & `bestdori-api-1.1.1/bestdori/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.0/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-1.1.1/bestdori_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -32,14 +32,18 @@
           <img src="https://img.shields.io/github/license/WindowsSov8forUs/bestdori-api" alt="License">
         </a>
         
         <a href="https://www.python.org/downloads/">
           <img src="https://img.shields.io/pypi/pyversions/bestdori-api" alt="Python Version">
         </a>
         
+        <a href="https://pypi.org/project/bestdori-api/">
+          <img src="https://img.shields.io/pypi/v/bestdori-api" alt="PyPI Version">
+        </a>
+        
         </p>
         
         > bestdori-api 现已全面支持同步与异步
         > 异步使用方法与同步类似，可几乎无缝切换
         
         ## 简介
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.0 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.1 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
                    æå¶ä»éè¦çæ¥å£è¯·åæ¶æåº**
-          _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
+   _[_l_i_c_e_n_s_e_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _V_e_r_s_i_o_n_]
 > bestdori-api ç°å·²å¨é¢æ¯æåæ­¥ä¸å¼æ­¥ >
 å¼æ­¥ä½¿ç¨æ¹æ³ä¸åæ­¥ç±»ä¼¼ï¼å¯å ä¹æ ç¼åæ¢ ## ç®ä»
 è¿æ¯ä¸ä¸ªç¨ Python ç¼åçè°ç¨ [Bestdori](https://bestdori.com/) åç§
 API ä¸èµæºä¸è½½çåºï¼å¤§è´åæ¬äºç¤¾åºå¸å­çå¤çä»¥ååç§
 [BanG Dreamï¼å°å¥³ä¹å¢æ´¾å¯¹](https://zh.moegirl.org.cn/
 BanG_Dream!_%E5%B0%91%E5%A5%B3%E4%B9%90%E5%9B%A2%E6%B4%BE%E5%AF%B9%EF%BC%81)
 æ¸¸æåèµæºçè·åã
```

### Comparing `bestdori-api-1.1.0/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-1.1.1/bestdori_api.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 bestdori/models/note.py
 bestdori/utils/__init__.py
 bestdori/utils/network.py
 bestdori/utils/utils.py
 bestdori_api.egg-info/PKG-INFO
 bestdori_api.egg-info/SOURCES.txt
 bestdori_api.egg-info/dependency_links.txt
+bestdori_api.egg-info/requires.txt
 bestdori_api.egg-info/top_level.txt
```

### Comparing `bestdori-api-1.1.0/setup.py` & `bestdori-api-1.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori-api',
-    version='1.1.0',
+    version='1.1.1',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
@@ -17,8 +17,12 @@
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.8',
+    install_requires=[
+        'httpx>=0.18.2',
+        'aiohttp>=3.7.4'
+    ]
 )
```

