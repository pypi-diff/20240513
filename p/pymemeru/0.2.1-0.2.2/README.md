# Comparing `tmp/pymemeru-0.2.1.tar.gz` & `tmp/pymemeru-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemeru-0.2.1.tar", max compression
+gzip compressed data, was "pymemeru-0.2.2.tar", max compression
```

## Comparing `pymemeru-0.2.1.tar` & `pymemeru-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-09 18:45:18.470666 pymemeru-0.2.1/LICENSE
--rw-r--r--   0        0        0       42 2024-03-09 18:45:18.470666 pymemeru-0.2.1/README.md
--rw-r--r--   0        0        0      146 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/__init__.py
--rw-r--r--   0        0        0      195 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/aioget.py
--rw-r--r--   0        0        0       74 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/models/__init__.py
--rw-r--r--   0        0        0     1457 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/models/page.py
--rw-r--r--   0        0        0      145 2024-03-09 20:21:15.446505 pymemeru-0.2.1/pymemeru/models/search.py
--rw-r--r--   0        0        0     1607 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/page.py
--rw-r--r--   0        0        0      710 2024-03-09 18:45:18.470666 pymemeru-0.2.1/pymemeru/popular.py
--rw-r--r--   0        0        0      647 2024-03-09 20:21:37.562690 pymemeru-0.2.1/pymemeru/search.py
--rw-r--r--   0        0        0      505 2024-03-09 20:25:04.000343 pymemeru-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 pymemeru-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 21:54:38.182019 pymemeru-0.2.2/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-12 21:54:38.182019 pymemeru-0.2.2/README.md
+-rw-r--r--   0        0        0      146 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/aioget.py
+-rw-r--r--   0        0        0       74 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/models/__init__.py
+-rw-r--r--   0        0        0     2207 2024-05-12 22:02:25.236589 pymemeru-0.2.2/pymemeru/models/page.py
+-rw-r--r--   0        0        0      145 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/models/search.py
+-rw-r--r--   0        0        0     1738 2024-05-12 22:01:51.704476 pymemeru-0.2.2/pymemeru/page.py
+-rw-r--r--   0        0        0      710 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/popular.py
+-rw-r--r--   0        0        0      647 2024-05-12 21:54:38.182019 pymemeru-0.2.2/pymemeru/search.py
+-rw-r--r--   0        0        0      505 2024-05-12 22:05:15.761162 pymemeru-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 pymemeru-0.2.2/PKG-INFO
```

### Comparing `pymemeru-0.2.1/LICENSE` & `pymemeru-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemeru-0.2.1/pymemeru/models/page.py` & `pymemeru-0.2.2/pymemeru/models/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class Trending(BaseModel):
     preview: str
     title: str
     url: str
 
-    views: str = 0
+    views: str = "0"
 
 
 class Page(BaseModel):
     title: str
     published_at: str
 
     views: str
@@ -21,36 +21,56 @@
 
     main_image: str
     text: str
     trending: list[Trending]
 
     @property
     def cleared_text(self) -> BeautifulSoup:
-        soup = BeautifulSoup(self.text)
+        soup = BeautifulSoup(self.text, features="lxml")
 
         for tag in [
             *soup.find_all("time"),
             *soup.find_all("img", class_=["avatar"]),
             *soup.find_all("span", class_=["count"]),
             *soup.find_all("span", itemprop="name"),
             *soup.find_all("div", class_=["mistape_caption", "share-box"]),
             *soup.find_all("h1"),
             *soup.find_all("hr"),
-            *soup.find_all("figure", class_="bb-mb-el")
+            *soup.find_all("figure", class_="bb-mb-el"),
+            *soup.find_all("div", class_="tds-message-box"),
         ]:
             tag.replace_with("")
 
         for tag in soup.find_all("div", class_="su-quote-inner"):
             tag.name = "blockquote"
 
         for tag in soup.find_all("span", class_="su-quote-cite"):
             tag.name = "cite"
 
+        for tag in soup.find_all("h2"):
+            if tag.text in ("Галерея", "Читайте также"):
+                tag.replace_with("")
+
         for tag in soup.find_all("a"):
             if tag["href"] == "https://t.me/memepedia_Ru":
                 tag.replace_with("")
 
+        for tag in soup.find_all("div", class_="wc-comment-text"):
+            tag.replace_with(
+                "\n\n".join(
+                    map(
+                        lambda x: f"<blockquote>{x}</blockquote>JDAN_EXTRA_SPACE",
+                        tag.stripped_strings,
+                    )
+                )
+            )
+
+        for tag in soup.find_all("em", recursive=True):
+            tag.replace_with(f"<blockquote>{tag.text}</blockquote>JDAN_EXTRA_SPACE")
+
         for tag in soup.find_all("a"):
             if tag["href"].startswith("https://memepedia.ru/"):
-                tag["href"] = "/memepedia/" + tag["href"].removeprefix("https://memepedia.ru/")
+                tag["href"] = "/memepedia/" + tag["href"].removeprefix(
+                    "https://memepedia.ru/"
+                )
 
         return soup
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymemeru-0.2.1/pymemeru/page.py` & `pymemeru-0.2.2/pymemeru/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,50 +7,55 @@
 async def page(name: str) -> Page:
     page = await aioget(f"https://memepedia.ru/{name}/")
 
     soup = BeautifulSoup(page, "lxml")
     post = soup.find_all(class_="s-post-main")[0]
 
     try:
-        image = post.find_all("figure", class_="post-thumbnail", recursive=True)[0].img["src"]
+        image = post.find_all("figure", class_="post-thumbnail", recursive=True)[0].img[
+            "src"
+        ]
     except:
         image = post.find_all("div", class_="bb-media-placeholder")[0].img["src"]
 
     try:
         trending_ = soup.find_all(class_="widget_trending_entries")[0].ul
     except:
         trending_ = []
 
     try:
         comments = (
             soup.find_all("a", class_="post-comments")[0]
-                .find_all("span", class_="count")[0].text
+            .find_all("span", class_="count")[0]
+            .text
         )
     except:
-        comments = 0
+        comments = "0"
 
     return Page(
         title=post.h1.text,
         published_at=post.find_all("time", class_="published")[0].text,
-
         author_name=(
             soup.find_all("div", class_="author-info")[0]
-                .find_all("a", class_="auth-url")[0]
-                .span.text
+            .find_all("a", class_="auth-url")[0]
+            .span.text
         ),
-
         views=(
             soup.find_all("span", class_="post-views")[0]
-                .find_all("span", class_="count")[0].text
+            .find_all("span", class_="count")[0]
+            .text
         ),
         comments=comments,
-
         main_image=image,
-
         text=str(post),
-        trending=[Trending(
-            preview=trending.find_all("img")[0]["src"],
-            title=trending.find_all(class_="content")[0].find_all("a")[0].text,
-            url="/" + trending.find_all(class_="content")[0].find_all("a")[0]["href"].split("/")[-2]
-        ) for trending in trending_]
+        trending=[
+            Trending(
+                preview=trending.find_all("img")[0]["src"],
+                title=trending.find_all(class_="content")[0].find_all("a")[0].text,
+                url="/"
+                + trending.find_all(class_="content")[0]
+                .find_all("a")[0]["href"]
+                .split("/")[-2],
+            )
+            for trending in trending_
+        ],
     )
-
```

### Comparing `pymemeru-0.2.1/pymemeru/popular.py` & `pymemeru-0.2.2/pymemeru/popular.py`

 * *Files identical despite different names*

### Comparing `pymemeru-0.2.1/pymemeru/search.py` & `pymemeru-0.2.2/pymemeru/search.py`

 * *Files identical despite different names*

### Comparing `pymemeru-0.2.1/PKG-INFO` & `pymemeru-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pymemeru
-Version: 0.2.1
+Version: 0.2.2
 Summary: memepedia.ru parser for python
 License: MIT
 Keywords: memepedia
 Author: Daniel Zakharov
 Author-email: gzdan734@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: httpx (>=0.21.0,<0.22.0)
-Requires-Dist: lxml (>=4.8.0,<5.0.0)
-Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pymemeru
 memepedia.ru parser for python
```

