# Comparing `tmp/grabberlib-0.1.5.tar.gz` & `tmp/grabberlib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.5.tar", max compression
+gzip compressed data, was "grabberlib-0.1.7.tar", max compression
```

## Comparing `grabberlib-0.1.5.tar` & `grabberlib-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.5/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.5/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5270 2024-05-10 14:48:30.795989 grabberlib-0.1.5/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.5/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.5/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/exc.py
--rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.5/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.5/grabber/core/sources/common.py
--rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.5/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.5/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3218 2024-05-10 12:29:42.290554 grabberlib-0.1.5/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     2857 2024-05-10 12:22:23.770346 grabberlib-0.1.5/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.5/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.5/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    19128 2024-05-10 14:47:30.689591 grabberlib-0.1.5/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-10 14:59:26.762508 grabberlib-0.1.5/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-10 14:59:34.322306 grabberlib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.7/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.7/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5270 2024-05-10 14:48:30.795989 grabberlib-0.1.7/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.7/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.7/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.7/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.7/grabber/core/sources/common.py
+-rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.7/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.7/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3218 2024-05-10 12:29:42.290554 grabberlib-0.1.7/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3409 2024-05-13 15:57:32.514304 grabberlib-0.1.7/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.7/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.7/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19423 2024-05-13 16:21:26.079038 grabberlib-0.1.7/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-13 16:21:30.398921 grabberlib-0.1.7/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-13 16:21:33.986823 grabberlib-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.7/PKG-INFO
```

### Comparing `grabberlib-0.1.5/grabber/__main__.py` & `grabberlib-0.1.7/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/controllers/base.py` & `grabberlib-0.1.7/grabber/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/bot/core.py` & `grabberlib-0.1.7/grabber/core/bot/core.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/settings.py` & `grabberlib-0.1.7/grabber/core/settings.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/common.py` & `grabberlib-0.1.7/grabber/core/sources/common.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/everia.py` & `grabberlib-0.1.7/grabber/core/sources/everia.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/graph.py` & `grabberlib-0.1.7/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/khd.py` & `grabberlib-0.1.7/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/nudecosplay.py` & `grabberlib-0.1.7/grabber/core/sources/nudecosplay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import pathlib
-from typing import List
+from typing import List, Optional
 
 from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     downloader,
+    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
 def get_sources_for_nudecosplay(
     sources: List[str],
     entity: str,
     telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
-    **kwargs,
+    is_tag: Optional[bool] = False,
+    limit: Optional[int] = None,
 ) -> None:
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
@@ -44,14 +46,26 @@
         final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
+        if is_tag:
+            urls = get_pages_from_pagination(url=source_url, target="nudecosplay")
+            targets = urls[:limit] if limit else urls
+            return get_sources_for_nudecosplay(
+                sources=targets,
+                entity=entity,
+                telegraph_client=telegraph_client,
+                final_dest=final_dest,
+                save_to_telegraph=save_to_telegraph,
+                is_tag=False,
+            )
+
         image_tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
         if page_title is None:
             page_title = soup.find('title').get_text(strip=True).split(split_text_with)[0].strip().rstrip()
```

### Comparing `grabberlib-0.1.5/grabber/core/sources/xasiat.py` & `grabberlib-0.1.7/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/sources/xiuren.py` & `grabberlib-0.1.7/grabber/core/sources/xiuren.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.5/grabber/core/utils.py` & `grabberlib-0.1.7/grabber/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,15 @@
 POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
     "nudebird": ("div.thecontent a", "href"),
     "hotgirl": ("div.thecontent a", "href"),
-    "nudecosplay": (
-        "div.content-inner a[data-lbwps-srcsmall^='https://nudecosplay.biz'] img",
-        "src",
-    ),
+    "nudecosplay": ("div.content-inner a img", "src"),
     "v2ph": ("div.photos-list.text-center img", "src"),  # Needs to handle pagination
     "cgcosplay": ("div.gallery-icon.portrait img", "src"),
     "mitaku": ("img.msacwl-img", "data-lazy"),
     "xasiat": ("div.images a", "href"),
     "telegraph": ("img", "src"),
     "4khd": (
         "div.is-layout-constrained.entry-content.wp-block-post-content img",
@@ -82,14 +79,20 @@
         pages_count_query="span.page_info",
         pagination_base_url_query="div.jeg_navigation.jeg_pagination a.page_number",
         posts_query_xpath=(
             "/html/body/div[3]/div[4]/div/div[1]/div/div/div[2]/"
             "div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
         ),
     ),
+    "nudecosplay": PaginationXPath(
+        pagination_query="div.jeg_navigation.jeg_pagination",
+        pages_count_query="span.page_info",
+        pagination_base_url_query="div.jeg_navigation.jeg_pagination a.page_number",
+        posts_query_xpath="/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div/div/div/div/article/div/a",
+    ),
 }
 headers_mapping = {
     "nudebird": {
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
     },
     "nudecosplay": {
@@ -507,53 +510,53 @@
 
         content = "\n".join([f"{page_url}" for page_url in page_urls])
         print(content)
 
 
 def get_pages_from_pagination(url: str, target: str) -> List[str]:
     pagination_params = query_pagination_mapping[target]
-    source_urls = []
+    source_urls = set()
     soup = get_soup(url)
     dom = etree.HTML(str(soup))
     pagination_set = soup.select(pagination_params.pages_count_query)
 
     if not pagination_set:
         for a_tag in dom.xpath(pagination_params.posts_query_xpath):
             if a_tag is not None and a_tag.attrib["href"] not in source_urls:
-                source_urls.append(a_tag.attrib["href"])
+                source_urls.add(a_tag.attrib["href"])
         return source_urls
 
     pagination = pagination_set[0]
     pagination_text = pagination.text
     first, last = pagination_text.split("Page")[-1].strip().split("of")
     first_page, last_page = int(first), int(last)
 
     first_link_pagination = soup.select(pagination_params.pagination_base_url_query)[0]
     href = first_link_pagination.attrs["href"]
     base_pagination_url = href.rsplit("/", 2)[0]
 
     for a_tag in dom.xpath(pagination_params.posts_query_xpath):
-        source_urls.append(a_tag.attrib["href"])
+        source_urls.add(a_tag.attrib["href"])
 
     for index in range(first_page, last_page + 1):
         if index == 1:
             continue
 
         target_url = f"{base_pagination_url}/{index}/"
 
         soup = get_soup(target_url)
         dom = etree.HTML(str(soup))
-        source_urls.extend(
+        source_urls.update(
             [
                 a_tag.attrib["href"]
                 for a_tag in dom.xpath(pagination_params.posts_query_xpath)
             ]
         )
 
-    return source_urls
+    return list(source_urls)
 
 
 def print_albums_message(albums_links: List[str]) -> None:
     albums_message = ""
 
     for album in albums_links:
         albums_message += f"\t- {album}\n"
```

### Comparing `grabberlib-0.1.5/pyproject.toml` & `grabberlib-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.5"
+version = "0.1.7"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.1.5/PKG-INFO` & `grabberlib-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.5
+Version: 0.1.7
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

