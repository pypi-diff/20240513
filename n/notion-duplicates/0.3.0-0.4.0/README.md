# Comparing `tmp/notion_duplicates-0.3.0.tar.gz` & `tmp/notion_duplicates-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion_duplicates-0.3.0.tar", max compression
+gzip compressed data, was "notion_duplicates-0.4.0.tar", max compression
```

## Comparing `notion_duplicates-0.3.0.tar` & `notion_duplicates-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5040 2024-05-12 16:08:50.588360 notion_duplicates-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 20:49:07.405044 notion_duplicates-0.3.0/notion_duplicates/__init__.py
--rw-r--r--   0        0        0     4148 2024-05-12 17:16:33.713280 notion_duplicates-0.3.0/notion_duplicates/notion_duplicates.py
--rw-r--r--   0        0        0      512 2024-05-12 17:13:11.308562 notion_duplicates-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5562 1970-01-01 00:00:00.000000 notion_duplicates-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5040 2024-05-12 16:08:50.588360 notion_duplicates-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 20:49:07.405044 notion_duplicates-0.4.0/notion_duplicates/__init__.py
+-rw-r--r--   0        0        0     4152 2024-05-12 23:11:39.897434 notion_duplicates-0.4.0/notion_duplicates/notion_duplicates.py
+-rw-r--r--   0        0        0      512 2024-05-12 23:12:53.467327 notion_duplicates-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5562 1970-01-01 00:00:00.000000 notion_duplicates-0.4.0/PKG-INFO
```

### Comparing `notion_duplicates-0.3.0/README.md` & `notion_duplicates-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `notion_duplicates-0.3.0/notion_duplicates/notion_duplicates.py` & `notion_duplicates-0.4.0/notion_duplicates/notion_duplicates.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             dupe_count += 1
             if cli_args.delete:
                 print(f"DELETING dupe page -> {page}")
                 response = notion.pages.update(page_id=page.page_id, in_trash=True)
                 delete_page_count += 1
                 if delete_page_count >= max_delete_page_count:
                     print("Reached max delete page count")
-                break
+                    break
             else:
                 print(f"This page is a dupe -> {page}")
 
         page_count += 1
         if page_count >= max_page_count:
             print("Reached max page count")
             break
```

### Comparing `notion_duplicates-0.3.0/pyproject.toml` & `notion_duplicates-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notion-duplicates"
-version = "0.3.0"
+version = "0.4.0"
 description = "Detect duplicated pages in a Notion database and optionallly delete them"
 authors = ["Jerome Provensal <jeromegit@provensal.com>"]
 readme = "README.md"
 packages = [{include = "notion_duplicates"}]
 
 [tool.poetry.scripts]
 notion_duplicates = 'notion_duplicates.notion_duplicates:main'
```

### Comparing `notion_duplicates-0.3.0/PKG-INFO` & `notion_duplicates-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-duplicates
-Version: 0.3.0
+Version: 0.4.0
 Summary: Detect duplicated pages in a Notion database and optionallly delete them
 Author: Jerome Provensal
 Author-email: jeromegit@provensal.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

