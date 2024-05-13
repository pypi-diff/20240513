# Comparing `tmp/gameyamlspiderandgenerator-1.7.6.tar.gz` & `tmp/gameyamlspiderandgenerator-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.7.6.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.7.7.tar", last modified: Mon May 13 15:13:53 2024, max compression
```

## Comparing `gameyamlspiderandgenerator-1.7.6.tar` & `gameyamlspiderandgenerator-1.7.7.tar`

### file list

```diff
@@ -1,19 +1,26 @@
--rwxr-xr-x   0        0        0     1090 2023-08-21 12:35:20.828865 gameyamlspiderandgenerator-1.7.6/LICENSE
--rwxr-xr-x   0        0        0     1528 2023-12-30 15:56:28.985964 gameyamlspiderandgenerator-1.7.6/README.md
--rwxr-xr-x   0        0        0      839 2023-12-30 15:17:36.324144 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     2140 2023-10-27 02:57:48.999956 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      584 2023-12-30 15:17:36.318839 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       55 2023-08-21 12:35:20.831751 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      250 2023-08-21 12:35:20.831751 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0       59 2023-08-21 12:35:20.832315 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2597 2023-12-30 15:44:10.564902 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7161 2023-12-30 15:46:27.513439 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-12-30 15:53:25.910333 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-08-21 12:35:20.833321 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1491 2023-10-27 02:29:29.498438 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1926 2023-08-29 11:31:52.004454 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     2102 2023-10-27 03:01:35.509137 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2594 2023-11-18 07:40:22.692317 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2546 2023-10-27 03:01:35.518206 gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      792 2023-12-30 15:59:01.084784 gameyamlspiderandgenerator-1.7.6/pyproject.toml
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.7.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2023-08-21 12:35:20.828865 gameyamlspiderandgenerator-1.7.7/LICENSE
+-rwxr-xr-x   0        0        0     1528 2023-12-30 15:56:28.985964 gameyamlspiderandgenerator-1.7.7/README.md
+-rwxr-xr-x   0        0        0      856 2024-05-13 15:05:23.463898 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     2142 2024-05-13 15:05:23.463689 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      758 2024-02-15 07:25:34.917548 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       55 2023-08-21 12:35:20.831751 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      250 2023-08-21 12:35:20.831751 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0       59 2023-08-21 12:35:20.832315 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2804 2024-05-13 14:58:21.929196 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7446 2024-05-13 15:07:11.652751 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     8298 2024-05-13 15:06:42.128527 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-08-21 12:35:20.833321 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1486 2024-05-13 15:05:23.463250 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1926 2023-08-29 11:31:52.004454 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     2102 2024-05-13 15:05:23.484772 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     3034 2024-05-13 15:05:23.485983 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2024-05-13 15:05:23.463448 gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0     1445 2024-05-13 15:13:53.419937 gameyamlspiderandgenerator-1.7.7/pyproject.toml
+-rwxr-xr-x   0        0        0    18046 2023-08-27 05:07:26.271399 gameyamlspiderandgenerator-1.7.7/tests/Atopes.zip
+-rwxr-xr-x   0        0        0   115913 2024-05-13 14:58:33.768149 gameyamlspiderandgenerator-1.7.7/tests/Fall_of_Porcupine.zip
+-rwxr-xr-x   0        0        0   780414 2024-05-13 14:58:29.380614 gameyamlspiderandgenerator-1.7.7/tests/Longest_Night.zip
+-rwxr-xr-x   0        0        0      307 2023-11-08 11:17:17.238268 gameyamlspiderandgenerator-1.7.7/tests/config.yaml
+-rwxr-xr-x   0        0        0     1074 2024-05-13 15:05:23.463644 gameyamlspiderandgenerator-1.7.7/tests/local_test.py
+-rwxr-xr-x   0        0        0      376 2023-08-29 11:24:14.876836 gameyamlspiderandgenerator-1.7.7/tests/test_config.yaml
+-rwxr-xr-x   0        0        0     1919 2023-12-30 15:56:29.046745 gameyamlspiderandgenerator-1.7.7/tests/unit_test.py
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.7.7/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.7.6/LICENSE` & `gameyamlspiderandgenerator-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.7.6/README.md` & `gameyamlspiderandgenerator-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+from collections.abc import Callable
 from inspect import signature
-from typing import Callable
-
-from loguru import logger
 
+from .exception import InvalidUrlError, PluginNotLoadedError
 from .plugin import BasePlugin
 from .util.fgi_yaml import YamlData
 from .util.plugin_manager import pkg
 
 
-def verify(url: str) -> Callable[..., BasePlugin]:
+def verify(url: str) -> Callable[..., BasePlugin] | None:
     if not pkg.plugin:
-        raise Exception("Plugin not yet loaded")
+        raise PluginNotLoadedError
     verify_list = [
         [
             pkg.plugin[n].verify,
             pkg.plugin[n],
         ]
         for n in pkg.plugin
     ]
     return next((cls for func, cls in verify_list if func(url)), None)
 
 
 def produce_yaml(url: str, lang: str = "en") -> YamlData | None:
     ret = verify(url)
     if ret is None:
-        logger.error("URL is invalid")
-        return
+        raise InvalidUrlError(url)
     if 'lang' in [i.name for i in signature(ret).parameters.values()]:
         return ret(url, lang).to_yaml()
     else:
         return ret(url).to_yaml()
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 
 from loguru import logger
 from yaml import safe_load
 
 from gameyamlspiderandgenerator import produce_yaml
+
 from .util.config import config
 from .util.fgi import default_config
 from .util.fgi_yaml import get_valid_filename
 from .util.plugin_manager import pkg
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,30 @@
-class ReadOrWriteConfigFailed(Exception):
+class GenerateError(Exception):
+    pass
+
+
+class PluginNotLoadedError(GenerateError):
+    pass
+
+
+class InvalidUrlError(GenerateError):
+    pass
+
+
+class ReadOrWriteConfigFailed(GenerateError):
     def __init__(self):
         super().__init__("Failed to read or write config")
 
 
-class InvalidTargetResourceError(Exception):
+class InvalidTargetResourceError(GenerateError):
     def __init__(self, code: int):
         super().__init__(f"The target resource is no longer valid.status code: {code}")
 
 
-class ResponseNotInitialized(Exception):
+class ResponseNotInitialized(GenerateError):
     def __init__(self, url: str):
         super().__init__(f"Response not initialized, url: {url}")
 
 
-class InvalidResponse(Exception):
+class InvalidResponse(GenerateError):
     def __init__(self, url: str):
         super().__init__(f"Invalid response, url: {url}")
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import abc
 import re
 
+from loguru import logger
+
 from ..util.fgi_yaml import YamlData
 
 
 class BasePlugin(abc.ABC):
     """插件基类"""
 
     _VERIFY_PATTERN: re.Pattern
@@ -16,28 +18,32 @@
 
         Args:
             url: URL
 
         Returns:
             是否符合要求
         """
-        return bool(cls._VERIFY_PATTERN.match(url))
+        return cls._VERIFY_PATTERN.match(url) is not None
 
     @staticmethod
     def _load_hook(data: dict):
         """
         加载钩子
 
         Args:
             data: 钩子数据
         """
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
 
-        for i in pkg.hook.values():
-            data = i().setup(data)
+        for i in pkg.hook:
+            try:
+                data = pkg.hook[i]().setup(data)
+            except Exception as e:
+                logger.warning(f'An error occurred while running the {i} hook')
+                logger.error(str(e))
         return data
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 from contextlib import suppress
 from json import loads
 
 from bs4 import BeautifulSoup
+from bs4.element import Tag
 from html2text import html2text
 from langcodes import find
 from py3langid import classify
 
-from ._base import BasePlugin
 from ..util.fgi import fgi_dict
 from ..util.fgi_yaml import YamlData
 from ..util.spider import get_text
+from . import BasePlugin
 
 
 class ItchIO(BasePlugin):
     _VERIFY_PATTERN = re.compile(r"https?://.+\.itch\.io/.+")
 
     @staticmethod
     def remove_query(s: str):
@@ -47,33 +48,47 @@
     def get_brief_desc(self):
         return self.soup.find("meta", {"name": "twitter:description"}).attrs["content"]
 
     def get_name(self):
         return self.data["name"]
 
     def get_screenshots(self):
-        temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
-        return [i.attrs['href'] for i in temp]
+        temp = self.soup.select_one(
+            "div.columns > div.right_col.column > div.screenshot_list"
+        ).select("a")
+        return [i.attrs["href"] for i in temp]
 
     def get_desc(self):
-        return self.remove_query(html2text(
-            str(self.soup.select_one("div.formatted_description.user_formatted")),
-            bodywidth=0,
-        )).replace("\n" * 3, "\n").strip()
+        return (
+            self.remove_query(
+                html2text(
+                    str(
+                        self.soup.select_one("div.formatted_description.user_formatted")
+                    ),
+                    bodywidth=0,
+                )
+            )
+            .replace("\n" * 3, "\n")
+            .strip()
+        )
 
     def get_platforms(self):
         repl = {
             "Windows": "windows",
             "macOS": "macos",
             "Linux": "linux",
             "Android": "android",
             "HTML5": "web",
             "iOS": "ios",
         }
-        platforms = self.more_info["Platforms"] if "Platforms" in self.more_info else ["Windows"]
+        platforms = (
+            self.more_info["Platforms"]
+            if "Platforms" in self.more_info
+            else ["Windows"]
+        )
         return [repl[i.strip()] for i in platforms]
 
     def get_authors(self):
         temp = []
         if "Authors" in self.more_info:
             temp = self.more_info["Authors"]
         elif "Author" in self.more_info:
@@ -113,20 +128,23 @@
 
     def get_langs(self):
         if "Languages" in self.more_info:
             temp = self.more_info["Languages"]
         else:
             return [classify(self.get_desc())[0]]
 
-        return list(set(find(i).language for i in temp))
+        return list({find(i).language for i in temp})
 
     def get_links(self):
-        link = [i.attrs["href"]
-                for i in self.soup.select_one("div.left_col.column > "
-                                              "div.formatted_description.user_formatted").select("a[href]")]
+        link = [
+            i.attrs["href"]
+            for i in self.soup.select_one(
+                "div.left_col.column > " "div.formatted_description.user_formatted"
+            ).select("a[href]")
+        ]
         data = [{"url": i, "processed": False} for i in list(set(link))]
         processed_data = []
         for i in data:
             for p in fgi_dict:
                 if re.match(p["match"], i["url"]):
                     processed_data.append(
                         {
@@ -139,19 +157,20 @@
             if not i["processed"]:
                 processed_data.append({"name": ".website", "uri": i["url"]})
         processed_data.append({"name": ".itchio", "uri": self.link})
         return processed_data
 
     def get_more_info(self):
         d = {}
-        for i in range(1, 18):
+        for _ in range(18):
             with suppress(Exception):
                 cache = self.soup.select_one(
-                    f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
+                    f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(_+1)})"
                 )
+                i: Tag
                 temp = [i.get_text() for i in list(cache.children)]
                 d[temp[0]] = temp[1:][0].split(",")
         return d
 
     def to_yaml(self):
         ret = {
             "name": self.get_name(),
@@ -164,15 +183,15 @@
                 "lang": self.get_langs(),
                 "platform": self.get_platforms(),
                 "publish": [".itchio"],
                 "misc": self.get_misc_tags(),
             },
             "links": self.get_links(),
             "thumbnail": self.get_thumbnail(),
-            "screenshots": self.get_screenshots()
+            "screenshots": self.get_screenshots(),
         }
         return YamlData(self._load_hook(ret))
 
     def get_type_tag(self):
         repl = {
             "Visual Novel": "visual-novel",
             "Real time strategy": "real-time-strategy",
@@ -192,14 +211,14 @@
             "Roguelike": "roguelike",
             "Sports": "Sports",
             "Bara": "bara",
             "Yuri": "yuri",
             "Gore": "gore",
             "Comedy": "comedy",
             "tragedy": "tragedy",
-            "Horror": "horror"
+            "Horror": "horror",
         }
 
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import concurrent.futures
 import re
 from urllib.parse import parse_qs, urlparse
 
 from bs4 import BeautifulSoup
 from html2text import html2text
-from langcodes import find, Language
+from langcodes import Language, find
 from yaml import dump
 
-from ._base import BasePlugin
 from ..util.fgi import fgi_dict
 from ..util.fgi_yaml import YamlData
 from ..util.spider import get_json, get_text
+from . import BasePlugin
 
 
 class Steam(BasePlugin):
     _VERIFY_PATTERN = re.compile(r"https?://store\.steampowered\.com/app/\d+/.+/?.+")
 
     @staticmethod
     def get_steam_id(link: str) -> int:
@@ -24,24 +24,34 @@
         return self.data[str(self.id)]["data"]["name"]
 
     @staticmethod
     def remove_query(s: str):
         s = re.sub(r"\?t=\d{6,12}", "", s)
         return s.replace("![]", "![img]")
 
-    def __init__(self, link: str, lang: str = 'en') -> None:
+    def __init__(self, link: str, lang: str = "en") -> None:
         self.id = self.get_steam_id(link)
-        if lang != 'en':
-            print(dump(get_json(
-                f'https://store.steampowered.com/api/appdetails?appids={self.id}&l={Language.get(lang).display_name("en").lower()}'),
-                allow_unicode=True))
+        if lang != "en":
+            print(
+                dump(
+                    get_json(
+                        f'https://store.steampowered.com/api/appdetails?appids='
+                        f'{self.id}&l={Language.get(lang).display_name("en").lower()}'
+                    ),
+                    allow_unicode=True,
+                )
+            )
         result = []
         with concurrent.futures.ThreadPoolExecutor() as executor:
             result.append(
-                executor.submit(get_json, f"https://store.steampowered.com/api/appdetails?appids={self.id}&l=english"))
+                executor.submit(
+                    get_json,
+                    f"https://store.steampowered.com/api/appdetails?appids={self.id}&l=english",
+                )
+            )
             result.append(executor.submit(get_text, link))
         self.data, self.data_html = (result[0].result(), result[1].result())
         self.soup = BeautifulSoup(self.data_html, "lxml")
         self.name = self.get_name()
         temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
         self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
 
@@ -66,30 +76,38 @@
         return YamlData(self._load_hook(ret))
 
     def get_langs(self):
         temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
         return list({find(i).language for i in temp})
 
     def get_desc(self):
-        return self.remove_query(
-            (
+        return (
+            self.remove_query(
                 html2text(
                     self.data[str(self.id)]["data"]["detailed_description"],
                     bodywidth=0,
                 )
             )
-        ).replace("\n" * 4, "\n").strip()
+            .replace("\n" * 4, "\n")
+            .strip()
+        )
 
     def get_brief_desc(self):
-        return html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
+        return html2text(
+            self.data[str(self.id)]["data"]["short_description"], bodywidth=0
+        )
 
     def get_authors(self):
         temp = self.data[str(self.id)]["data"]
-        developers = [{"name": i.strip(), "role": ["producer"]} for i in temp["developers"]]
-        publishers = [{"name": i.strip(), "role": ["publisher"]} for i in temp["publishers"]]
+        developers = [
+            {"name": i.strip(), "role": ["producer"]} for i in temp["developers"]
+        ]
+        publishers = [
+            {"name": i.strip(), "role": ["publisher"]} for i in temp["publishers"]
+        ]
         return developers + publishers
 
     def get_platforms(self):
         temp = self.data[str(self.id)]["data"]["platforms"]
         repl = {"windows": "windows", "mac": "macos", "linux": "linux"}
         return [repl[i] for i in temp if temp[i]]
 
@@ -142,16 +160,16 @@
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
 
     def get_if_nsfw(self):
         return (
-                self.soup.body.find_all("div", {"id": "game_area_content_descriptors"})
-                != []
+            self.soup.body.find_all("div", {"id": "game_area_content_descriptors"})
+            != []
         )
 
     def get_screenshots(self):
         return [
             self.remove_query(i["path_full"])
             for i in self.data[str(self.id)]["data"]["screenshots"]
         ]
@@ -164,17 +182,22 @@
         ]
         video_mp4 = [
             self.remove_query(i["mp4"]["max"]).replace("http", "https")
             for i in self.data[str(self.id)]["data"]["movies"]
         ]
         return [
             {
-                "video": [{"mime": "video/webm", "sensitive": is_nsfw, "uri": video_webm[i], },
-                          {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
-                          ]
+                "video": [
+                    {
+                        "mime": "video/webm",
+                        "sensitive": is_nsfw,
+                        "uri": video_webm[i],
+                    },
+                    {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
+                ]
                 if is_nsfw
                 else [
                     {"mime": "video/webm", "uri": video_webm[i]},
                     {"mime": "video/mp4", "uri": video_mp4[i]},
                 ],
             }
             for i in range(len(video_webm))
@@ -210,14 +233,14 @@
                             "uri": re.sub(p["match"], p["replace"], i["url"]),
                         }
                     )
                     i["processed"] = True
         for i in data:
             if not i["processed"]:
                 processed_data.append({"name": ".website", "uri": i["url"]})
-        processed_data.append({"name": ".steam", "uri": f'steam:{self.id}'})
+        processed_data.append({"name": ".steam", "uri": f"steam:{self.id}"})
         return processed_data
 
     def get_thumbnail(self):
         return self.remove_query(
             self.soup.body.find("img", {"class": "game_header_image_full"}).attrs["src"]
         )
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from ..exception import ReadOrWriteConfigFailed
 from .fgi import default_config
 from .fgi_yaml import fgi
-from ..exception import ReadOrWriteConfigFailed
 
 
 class Config:
     proxy = {}
     api = {}
     plugin = {}
     hook = {}
@@ -34,15 +34,15 @@
         Returns:
 
         """
         if type(file_data) is dict:
             self.__dict__.update(file_data)
             return
         try:
-            with open(file_data, "r", encoding="utf-8") as fp:
+            with open(file_data, encoding="utf-8") as fp:
                 self.__dict__.update(fgi.load(fp))
         except Exception as e:
             raise ReadOrWriteConfigFailed from e
 
     def update(self, data: dict):
         self.__dict__.update(data)
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import zipfile
 from io import BytesIO
 from textwrap import dedent
 
-from PIL import Image
 from loguru import logger
+from PIL import Image
 from ruamel.yaml import YAML
 from ruamel.yaml.scalarstring import PreservedScalarString
 
 
 def pss_dedent(x: str) -> PreservedScalarString:
     return PreservedScalarString(dedent(x))
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 import importlib
 from types import ModuleType
-from typing import Literal, Type
+from typing import Literal
 
 from loguru import logger
 
 from ..hook import BaseHook
 from ..plugin import BasePlugin
 from ..util.config import config
 
 
-def get_subclasses(module: ModuleType, base_class: Type) -> Type:
+def get_subclasses(module: ModuleType, base_class: type) -> type:
+    """
+    Get the subclasses of the specified base class from the given module.
+
+    Args:
+        module (ModuleType): The module to search for subclasses.
+        base_class (Type): The base class to find subclasses for.
+
+    Returns:
+        Type: The subclass of the specified base class.
+
+    Raises:
+        NotImplementedError: If the specified base class is not found in the module.
+    """
+
     class_dir = dir(module)
     if base_class.__name__ in class_dir:
         for i in class_dir:
             obj = getattr(module, i)
             if isinstance(obj, type) and issubclass(obj, base_class) and obj is not base_class:
                 return getattr(module, i)
-    raise NotImplementedError
+    raise NotImplementedError(base_class.__name__)
 
 
 class Package:
     plugin: dict[str, BasePlugin] = {}
     hook: dict[str, BaseHook] = {}
 
     def init(self):
@@ -34,15 +48,15 @@
     def __setitem__(self, key, value):
         # Compatibility with the old version
         self.__setattr__(key, value)
 
     def _load(
             self,
             _dir: Literal["plugin"],
-            _type: Type[BasePlugin],
+            _type: type[BasePlugin],
     ):
         base = __package__.split(".")[0] + "." + _dir
         for plugin in getattr(config, _dir, []):
             if plugin.startswith("_"):
                 logger.warning(f"Skip loading protected {_dir} {plugin}")
                 continue
             try:
@@ -57,21 +71,21 @@
                 logger.error(f"Imported {_dir} but no {_type.__name__} found: {plugin}")
 
     def load_plugins(self):
         self._load("plugin", BasePlugin)
 
     def load_hooks(self):
         if config["hook"] is None:
-            logger.warning(f"All hooks are disabled")
+            logger.warning("All hooks are disabled")
             return
         for plugin in getattr(config, "hook", []):
             try:
                 logger.info(f"Loading hook: {plugin}")
                 temp = importlib.import_module(f"yamlgenerator_hook_{plugin}")
-                self["hook"][plugin] = get_subclasses(temp, BaseHook)
+                self["hook"][f"yamlgenerator_hook_{plugin}"] = get_subclasses(temp, BaseHook)
             except ImportError as e:
                 logger.trace(e)
                 logger.error(f"Failed to import hook: {plugin}")
             except NotImplementedError:
                 logger.error(f"Imported hook but no BaseHook found: {plugin}")
```

### Comparing `gameyamlspiderandgenerator-1.7.6/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.7.7/gameyamlspiderandgenerator/util/spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import requests
 from requests import JSONDecodeError
 
 from ..exception import (
-    InvalidTargetResourceError,
     InvalidResponse,
+    InvalidTargetResourceError,
 )
 
 
 class GetResponse:
     """
-    Simple wrapper around requests.get, using context to ensure resources are released properly
+    Simple wrapper around `requests.get`, using context to ensure resources are released properly
 
     Instructions:
      with GetResponse("https://www.example.com/") as resp:
          print(resp.response) # response content
          response.to_disk("example.html") # write the response content to disk
     """
 
     def __init__(self, url: str, allow_redirects: bool = True, /, **kwargs):
         """
         get response
 
         Args:
              url: URL of the request
              allow_redirects: whether to allow redirection
-             kwargs: Other parameters that should be passed to requests.get, proxies will be added automatically
+             kwargs: Other parameters that should be passed to `requests.get`, proxies will be added automatically
         """
         from ..util.config import config
         if config.api['git_proxy'] and 'raw.githubusercontent.com' in url:
             self.url = config.api['git_proxy'] + url
         else:
             self.url = url
         self.args = {
```

### Comparing `gameyamlspiderandgenerator-1.7.6/PKG-INFO` & `gameyamlspiderandgenerator-1.7.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.7.6
+Version: 1.7.7
 Summary: A useful tool for generating Furrygameindex yaml files
-License: MIT
 Author: kaesinol
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: epicstore-api (>=0.1.7,<0.2.0)
-Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
-Requires-Dist: langcodes (>=3.3.0,<4.0.0)
-Requires-Dist: language-data (>=1.1,<2.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
-Requires-Dist: py3langid (>=0.2.2,<0.3.0)
-Requires-Dist: pysocks (>=1.7.1,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: ruamel.yaml.string (>=0.1.0,<0.2.0)
-Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
-Requires-Dist: yamlgenerator-hook-search (>=0.3.1,<0.4.0)
-Requires-Dist: yamlgenerator-hook-validate (>=0.1.0)
+License: MIT
+Requires-Python: <4.0,>=3.11
+Requires-Dist: langcodes<4.0.0,>=3.3.0
+Requires-Dist: language-data<2.0,>=1.1
+Requires-Dist: html2text<2021.0.0,>=2020.1.16
+Requires-Dist: ruamel-yaml<1.0.0,>=0.17.21
+Requires-Dist: ruamel-yaml-string<1.0.0,>=0.1.0
+Requires-Dist: urllib3<2.0.0,>=1.26.14
+Requires-Dist: beautifulsoup4<5.0.0,>=4.11.1
+Requires-Dist: pillow<10.0.0,>=9.4.0
+Requires-Dist: requests<3.0.0,>=2.28.2
+Requires-Dist: ruamel-base<2.0.0,>=1.0.0
+Requires-Dist: loguru<1.0.0,>=0.7.0
+Requires-Dist: pyyaml<7.0,>=6.0
+Requires-Dist: pysocks<2.0.0,>=1.7.1
+Requires-Dist: lxml<5.0.0,>=4.9.2
+Requires-Dist: py3langid<1.0.0,>=0.2.2
+Requires-Dist: yamlgenerator-hook-validate>=0.1.0
+Requires-Dist: yamlgenerator-hook-search<1.0.0,>=0.3.1
+Requires-Dist: epicstore-api<1.0.0,>=0.1.7
 Description-Content-Type: text/markdown
 
 # Quick Start
 
 ## Install
 
 ```commandline
@@ -81,8 +78,7 @@
 
 config.load("/home/user/desktop/config.yaml")
 pkg.init()
 print(produce_yaml("https://store.steampowered.com/app/1470120/Atopes/"))
 ```
 
 ### More: see [API Reference](https://github.com/FurryGamesIndex/GameYamlSpiderAndGenerator/wiki/Api-Reference)
-
```

