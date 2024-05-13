# Comparing `tmp/mandown-1.8.0.tar.gz` & `tmp/mandown-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.8.0.tar", max compression
+gzip compressed data, was "mandown-1.8.1.tar", max compression
```

## Comparing `mandown-1.8.0.tar` & `mandown-1.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.8.0/LICENSE
--rw-r--r--   0        0        0     3885 2024-05-12 17:51:49.558004 mandown-1.8.0/README.md
--rw-r--r--   0        0        0      542 2024-05-12 17:53:03.014544 mandown-1.8.0/mandown/__init__.py
--rw-r--r--   0        0        0    11901 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/api.py
--rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.8.0/mandown/base.py
--rw-r--r--   0        0        0    17068 2024-05-12 16:28:10.003897 mandown-1.8.0/mandown/cli.py
--rw-r--r--   0        0        0     2562 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/comic.py
--rw-r--r--   0        0        0      700 2023-06-22 00:52:39.390941 mandown-1.8.0/mandown/convert_utils.py
--rw-r--r--   0        0        0     5543 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/io.py
--rw-r--r--   0        0        0     5095 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4064 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/processor/ops.py
--rw-r--r--   0        0        0     1597 2024-03-08 17:11:50.448985 mandown-1.8.0/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1505 2024-05-12 17:51:49.558004 mandown-1.8.0/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2016 2024-03-08 17:11:50.448985 mandown-1.8.0/mandown/sources/base_source.py
--rw-r--r--   0        0        0     3301 2024-05-12 16:09:43.070512 mandown-1.8.0/mandown/sources/source_blogtruyenmoi.py
--rw-r--r--   0        0        0     4476 2024-05-12 17:51:49.558004 mandown-1.8.0/mandown/sources/source_kuaikanmanhua.py
--rw-r--r--   0        0        0     5045 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2535 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2641 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3658 2024-03-08 17:11:50.450985 mandown-1.8.0/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3044 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/sources/source_manhuaes.py
--rw-r--r--   0        0        0     3567 2023-07-14 02:43:47.054901 mandown-1.8.0/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     5154 2024-03-08 17:11:50.451985 mandown-1.8.0/mandown/sources/source_thecomicseries.py
--rw-r--r--   0        0        0     4059 2024-03-08 17:11:50.449985 mandown-1.8.0/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.8.0/mandown/ui/form.ui
--rw-r--r--   0        0        0     7060 2024-03-08 17:14:31.384962 mandown-1.8.0/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.8.0/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     6954 2024-03-08 17:14:31.383962 mandown-1.8.0/mandown/ui/ui.py
--rw-r--r--   0        0        0     1603 2024-05-12 17:52:55.373592 mandown-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.8.1/LICENSE
+-rw-r--r--   0        0        0     3885 2024-05-12 17:51:49.558004 mandown-1.8.1/README.md
+-rw-r--r--   0        0        0      542 2024-05-13 20:11:19.729400 mandown-1.8.1/mandown/__init__.py
+-rw-r--r--   0        0        0    11781 2024-05-13 20:08:43.671607 mandown-1.8.1/mandown/api.py
+-rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.8.1/mandown/base.py
+-rw-r--r--   0        0        0    17083 2024-05-13 20:09:58.149495 mandown-1.8.1/mandown/cli.py
+-rw-r--r--   0        0        0     2562 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/comic.py
+-rw-r--r--   0        0        0      705 2024-05-13 20:10:08.695482 mandown-1.8.1/mandown/convert_utils.py
+-rw-r--r--   0        0        0     5543 2024-03-08 17:11:50.450985 mandown-1.8.1/mandown/io.py
+-rw-r--r--   0        0        0     5095 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4064 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1597 2024-03-08 17:11:50.448985 mandown-1.8.1/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1505 2024-05-12 17:51:49.558004 mandown-1.8.1/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2016 2024-03-08 17:11:50.448985 mandown-1.8.1/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     3301 2024-05-12 16:09:43.070512 mandown-1.8.1/mandown/sources/source_blogtruyenmoi.py
+-rw-r--r--   0        0        0     4476 2024-05-12 17:51:49.558004 mandown-1.8.1/mandown/sources/source_kuaikanmanhua.py
+-rw-r--r--   0        0        0     5045 2024-03-08 17:11:50.450985 mandown-1.8.1/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2535 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2641 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3658 2024-03-08 17:11:50.450985 mandown-1.8.1/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3044 2024-03-08 17:11:50.451985 mandown-1.8.1/mandown/sources/source_manhuaes.py
+-rw-r--r--   0        0        0     3567 2023-07-14 02:43:47.054901 mandown-1.8.1/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     5154 2024-03-08 17:11:50.451985 mandown-1.8.1/mandown/sources/source_thecomicseries.py
+-rw-r--r--   0        0        0     4059 2024-03-08 17:11:50.449985 mandown-1.8.1/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.8.1/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7060 2024-03-08 17:14:31.384962 mandown-1.8.1/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.8.1/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     6954 2024-03-08 17:14:31.383962 mandown-1.8.1/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1603 2024-05-13 20:11:14.885405 mandown-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 mandown-1.8.1/PKG-INFO
```

### Comparing `mandown-1.8.0/LICENSE` & `mandown-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/README.md` & `mandown-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/__init__.py` & `mandown-1.8.1/mandown/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     ProcessConfig,
     ProcessOps,
     ProcessOptionMismatchError,
     Processor,
 )
 from .processor.profiles import SupportedProfiles, all_profiles
 
-__version__ = (1, 8, 0)
+__version__ = (1, 8, 1)
 __version_str__ = ".".join(map(str, __version__))
```

### Comparing `mandown-1.8.0/mandown/api.py` & `mandown-1.8.1/mandown/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
             yield len(comicon_comics)
             existing_filenames = {file.name for file in dest_folder.iterdir() if file.is_file()}
             for comicomic in comicon_comics:
                 yield comicomic.metadata.title
 
                 # do not overwrite existing cache
-                if f"{comicomic.metadata.title}.{to.value}" in existing_filenames:
+                if f"{comicomic.metadata.title_slug}.{to.value}" in existing_filenames:
                     continue
                 for _ in convert_one(comicomic, comic_path, to, dest_folder):
                     ...
 
         else:
             comicon_comic = comicon.Comic(
                 comicon.Metadata(
@@ -248,20 +248,15 @@
     """
     path = Path(path)
 
     # make var comic a BaseComic
     if isinstance(comic, str):
         comic = query(comic)
 
-    # create dir
-    try:
-        full_path = path / comic.metadata.title
-    except IOError:
-        # invalid filename
-        full_path = path / comic.metadata.title_slug
+    full_path = path / comic.metadata.title_slug
     full_path.mkdir(exist_ok=True)
 
     # save metadata json
     comic.set_chapter_range(start=start, end=end)
     io.save_comic(comic, full_path)
 
     # cover
```

### Comparing `mandown-1.8.0/mandown/base.py` & `mandown-1.8.1/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/cli.py` & `mandown-1.8.1/mandown/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
     with typer.progressbar(
         api.download_progress(comic, dest, threads=maxthreads),
         length=len(comic.chapters),
     ) as progress:
         for title in progress:
             progress.label = title
 
-    full_dest_folder = dest.absolute() / comic.metadata.title
+    full_dest_folder = dest.absolute() / comic.metadata.title_slug
     typer.secho(
         f"Successfully downloaded {end_chapter - start_chapter} chapter(s) to {full_dest_folder}.",
         fg=typer.colors.GREEN,
     )
 
     # process
     if processing_options:
@@ -439,20 +439,20 @@
                 target_size=target_size,
                 output_profile=size_profile,
             )
         except Exception as err:
             typer.secho(f"Could not apply processing options: {err}", fg=typer.colors.RED)
             raise typer.Exit(1) from err
 
-        cli_process(dest / comic.metadata.title, processing_options, config)
+        cli_process(dest / comic.metadata.title_slug, processing_options, config)
 
     # convert
     if convert_to != ConvertFormats.NONE:
         cli_convert(
-            dest / comic.metadata.title,
+            dest / comic.metadata.title_slug,
             convert_to,
             dest,
             remove_after,
             split_by_chapters,
         )
```

### Comparing `mandown-1.8.0/mandown/comic.py` & `mandown-1.8.1/mandown/comic.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/convert_utils.py` & `mandown-1.8.1/mandown/convert_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 def convert_one(
     comic: comicon.Comic, comic_path: Path, to: ConvertFormats, dest_folder: Path
 ) -> Iterator[str | int]:
     # save comicon.json
     (comic_path / comicon.cirtools.IR_DATA_FILE).write_text(comic.to_json())
 
     yield from comicon.outputs.create_comic_progress(
-        comic_path, dest_folder / f"{comic.metadata.title}.{to.value}"
+        comic_path, dest_folder / f"{comic.metadata.title_slug}.{to.value}"
     )
```

### Comparing `mandown-1.8.0/mandown/io.py` & `mandown-1.8.1/mandown/io.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/processor/__init__.py` & `mandown-1.8.1/mandown/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/processor/ops.py` & `mandown-1.8.1/mandown/processor/ops.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/processor/profiles.py` & `mandown-1.8.1/mandown/processor/profiles.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/__init__.py` & `mandown-1.8.1/mandown/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/base_source.py` & `mandown-1.8.1/mandown/sources/base_source.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_blogtruyenmoi.py` & `mandown-1.8.1/mandown/sources/source_blogtruyenmoi.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_kuaikanmanhua.py` & `mandown-1.8.1/mandown/sources/source_kuaikanmanhua.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_mangadex.py` & `mandown-1.8.1/mandown/sources/source_mangadex.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_mangakakalot.py` & `mandown-1.8.1/mandown/sources/source_mangakakalot.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_manganato.py` & `mandown-1.8.1/mandown/sources/source_manganato.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_mangasee.py` & `mandown-1.8.1/mandown/sources/source_mangasee.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_manhuaes.py` & `mandown-1.8.1/mandown/sources/source_manhuaes.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_readcomiconline.py` & `mandown-1.8.1/mandown/sources/source_readcomiconline.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_thecomicseries.py` & `mandown-1.8.1/mandown/sources/source_thecomicseries.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/sources/source_webtoons.py` & `mandown-1.8.1/mandown/sources/source_webtoons.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/ui/form.ui` & `mandown-1.8.1/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/ui/mainwin.py` & `mandown-1.8.1/mandown/ui/mainwin.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/mandown/ui/ui.py` & `mandown-1.8.1/mandown/ui/ui.py`

 * *Files identical despite different names*

### Comparing `mandown-1.8.0/pyproject.toml` & `mandown-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mandown"
-version = "1.8.0"
+version = "1.8.1"
 description = "Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter"
 authors = ["potatoeggy <eggyrules@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
```

### Comparing `mandown-1.8.0/PKG-INFO` & `mandown-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.8.0
+Version: 1.8.1
 Summary: Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
 Author: potatoeggy
 Author-email: eggyrules@gmail.com
 Requires-Python: >=3.10,<3.13
```

