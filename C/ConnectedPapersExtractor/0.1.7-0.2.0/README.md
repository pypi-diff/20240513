# Comparing `tmp/connectedpapersextractor-0.1.7.tar.gz` & `tmp/connectedpapersextractor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectedpapersextractor-0.1.7.tar", max compression
+gzip compressed data, was "connectedpapersextractor-0.2.0.tar", max compression
```

## Comparing `connectedpapersextractor-0.1.7.tar` & `connectedpapersextractor-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,35 @@
--rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.7/LICENSE
--rw-r--r--   0        0        0      661 2024-04-30 17:03:36.297583 connectedpapersextractor-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.7/src/connectedpapersextractor/ArticleFilter.py
--rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.7/src/connectedpapersextractor/Config.py
--rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.7/src/connectedpapersextractor/MainPartsExtractor.py
--rw-r--r--   0        0        0     2157 2024-04-29 13:12:12.624547 connectedpapersextractor-0.1.7/src/connectedpapersextractor/PdfSummary.py
--rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_AIExtractor.py
--rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.7/src/connectedpapersextractor/__init__.py
--rw-r--r--   0        0        0      531 2024-04-29 20:28:54.583294 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_add_docs.py
--rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_combine_summaries.py
--rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_get_pdf_summaries.py
--rw-r--r--   0        0        0     1405 2024-04-30 17:01:18.508897 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_huggingface_reduce.py
--rw-r--r--   0        0        0     1107 2024-04-30 09:00:32.674059 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_refine_documents.py
--rw-r--r--   0        0        0      786 2024-04-30 09:00:32.694059 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_stuff_documents.py
--rw-r--r--   0        0        0     1801 2024-04-30 16:56:21.564378 connectedpapersextractor-0.1.7/src/connectedpapersextractor/_summarize_documents.py
--rw-r--r--   0        0        0     1516 2024-04-29 20:28:54.595295 connectedpapersextractor-0.1.7/src/connectedpapersextractor/create_related_work.py
--rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.7/src/connectedpapersextractor/get_summaries.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.2.0/LICENSE
+-rw-r--r--   0        0        0      724 2024-05-13 15:54:27.824658 connectedpapersextractor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.2.0/src/connectedpapersextractor/Config.py
+-rw-r--r--   0        0        0      509 2024-05-12 20:55:22.805319 connectedpapersextractor-0.2.0/src/connectedpapersextractor/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-12 21:06:16.228124 connectedpapersextractor-0.2.0/src/connectedpapersextractor/article.py
+-rw-r--r--   0        0        0      780 2024-05-12 20:55:22.829347 connectedpapersextractor-0.2.0/src/connectedpapersextractor/create_related_work.py
+-rw-r--r--   0        0        0     1178 2024-05-12 21:03:28.591060 connectedpapersextractor-0.2.0/src/connectedpapersextractor/get_summaries_from_arxiv.py
+-rw-r--r--   0        0        0     1227 2024-05-12 21:03:28.607050 connectedpapersextractor-0.2.0/src/connectedpapersextractor/get_summaries_from_connected_papers.py
+-rw-r--r--   0        0        0        0 2024-05-12 12:02:19.941885 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-12 17:48:07.161135 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      816 2024-05-12 21:00:57.694734 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/article_filter.cpython-310.pyc
+-rw-r--r--   0        0        0     1902 2024-05-12 21:00:58.166847 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/convert_service.cpython-310.pyc
+-rw-r--r--   0        0        0      835 2024-05-12 21:00:58.162846 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/main_parts_extractor.cpython-310.pyc
+-rw-r--r--   0        0        0     1006 2024-05-12 21:00:58.166847 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/sumaries_combine.cpython-310.pyc
+-rw-r--r--   0        0        0     1035 2024-05-12 21:00:58.166847 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/summarizer.cpython-310.pyc
+-rw-r--r--   0        0        0     1081 2024-05-12 21:00:59.147082 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/__pycache__/text_splitter.cpython-310.pyc
+-rw-r--r--   0        0        0      253 2024-05-12 20:53:59.987562 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/article_filter.py
+-rw-r--r--   0        0        0     1792 2024-05-12 20:54:44.819163 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/convert_service.py
+-rw-r--r--   0        0        0      251 2024-05-12 21:00:57.386660 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/main_parts_extractor.py
+-rw-r--r--   0        0        0      519 2024-05-12 20:54:00.015561 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/sumaries_combine.py
+-rw-r--r--   0        0        0      460 2024-05-12 20:53:59.839564 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/summarizer.py
+-rw-r--r--   0        0        0      538 2024-05-12 20:58:37.132710 connectedpapersextractor-0.2.0/src/connectedpapersextractor/services/text_splitter.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:58:02.048594 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-12 17:48:07.889141 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1386 2024-05-12 21:00:58.150843 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/download_summaries.cpython-310.pyc
+-rw-r--r--   0        0        0     1219 2024-05-12 21:00:59.363134 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/download_summaries_from_arxiv.cpython-310.pyc
+-rw-r--r--   0        0        0     2312 2024-05-12 21:00:58.014811 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/download_summaries_from_connected_papers.cpython-310.pyc
+-rw-r--r--   0        0        0     1441 2024-05-12 21:00:58.162846 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/get_existing_summaries.cpython-310.pyc
+-rw-r--r--   0        0        0      718 2024-05-12 21:00:59.355131 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/__pycache__/summarize_documents.cpython-310.pyc
+-rw-r--r--   0        0        0      914 2024-05-12 21:04:07.835013 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/download_summaries.py
+-rw-r--r--   0        0        0      820 2024-05-12 20:54:53.319547 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/download_summaries_from_arxiv.py
+-rw-r--r--   0        0        0     2257 2024-05-12 21:04:22.905031 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/download_summaries_from_connected_papers.py
+-rw-r--r--   0        0        0      913 2024-05-12 20:54:53.327558 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/get_existing_summaries.py
+-rw-r--r--   0        0        0      440 2024-05-12 21:04:49.120460 connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/summarize_documents.py
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 connectedpapersextractor-0.2.0/PKG-INFO
```

### Comparing `connectedpapersextractor-0.1.7/LICENSE` & `connectedpapersextractor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.7/pyproject.toml` & `connectedpapersextractor-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ConnectedPapersExtractor"
-version = "0.1.7"
+version = "0.2.0"
 description = "A package for creating summaries based on https://www.connectedpapers.com/."
 authors = ["Tesla2000 <fratajczak124@gmail.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 langchain = "^0.1.16"
@@ -13,13 +13,16 @@
 download = "^0.3.5"
 chromedriver-autoinstaller = "^0.6.4"
 langchain-experimental = "^0.0.57"
 PyPDF2 = "^3.0.1"
 EnhancedWebdriver = "^0.1.6"
 langchain-openai = "^0.1.4"
 cffi = "^1.16.0"
+arxiv = "^2.1.0"
+python-dotenv = "^1.0.1"
+injector = "^0.21.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `connectedpapersextractor-0.1.7/src/connectedpapersextractor/_get_pdf_summaries.py` & `connectedpapersextractor-0.2.0/src/connectedpapersextractor/utils/download_summaries_from_connected_papers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,73 @@
-import json
-from dataclasses import asdict
+from __future__ import annotations
+
 from itertools import count
 from pathlib import Path
 from typing import Union
 
-from download import download
 from enhanced_webdriver import EnhancedWebdriver
 from undetected_chromedriver import ChromeOptions
 
-from . import PdfSummaries, PdfSummary
-from .Config import Config
+from .. import Article
+from .. import Articles
+from ..utils.download_summaries import download_summaries
+
+
+def _collect_article(driver: EnhancedWebdriver, dir_path: Path):
+    link = driver.get_attribute(
+        '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]',
+        "href",
+    )
+    if (
+        driver.get_text_of_element(
+            '//*[@id="desktop-app"]/div[2]/div[4]'
+            '/div[3]/div/div[2]/div[5]/a[1]/span'
+        ) != "PDF"
+    ):
+        return
+    title = driver.get_text_of_element(
+        '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[1]/div/a'
+    )
+    file_path = dir_path.joinpath(link.rpartition("/")[-1]).with_suffix(".pdf")
+    return Article(
+        file_path=file_path,
+        download_link=link,
+        year=int(
+            driver.get_text_of_element(
+                '//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]'
+                '/div/div[2]/div[2]/div[2]/div[2]'
+            )
+        ),
+        citations=int(
+            driver.get_text_of_element(
+                '//*[@id="desktop-app"]/div[2]/div[4]/'
+                'div[3]/div/div[2]/div[4]/div[1]'
+            ).split()[0]
+        ),
+        title=title,
+    )
+
+
+def _collect_articles(driver: EnhancedWebdriver, dir_path: Path) -> Articles:
+    articles = list()
+    for index in count(1):
+        if not driver.click(
+            '//*[@id="desktop-app"]/div[2]/div[4]/'
+            f'div[1]/div/div[2]/div/div[2]/div[{index}]'
+        ):
+            break
+        articles.append(_collect_article(driver, dir_path))
+    return articles
 
 
-def _get_pdf_summaries(
+def download_summaries_from_connected_papers(
     connected_papers_link: str,
-    dir_path: Union[str, Path] = Path("./"),
-) -> PdfSummaries:
+    dir_path: Union[str, Path] = Path("/"),
+) -> Articles:
     options = ChromeOptions()
     options.headless = True
     driver = EnhancedWebdriver.create(undetected=True, options=options)
     driver.get(connected_papers_link)
-    summaries = list()
-    downloads = list()
-    for index in count(1):
-        if not driver.click(
-            f'//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]/div/div[2]/div[{index}]'
-        ):
-            break
-        link = driver.get_attribute(
-            '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]',
-            "href",
-        )
-        if (
-            driver.get_text_of_element(
-                '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[5]/a[1]/span'
-            )
-            != "PDF"
-        ):
-            continue
-        title = driver.get_text_of_element(
-            '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[1]/div/a'
-        )
-        file_path = dir_path.joinpath(link.rpartition("/")[-1]).with_suffix(".pdf")
-        summary = PdfSummary(
-            file_path=file_path,
-            year=int(
-                driver.get_text_of_element(
-                    '//*[@id="desktop-app"]/div[2]/div[4]/div[1]/div/div[2]/div/div[2]/div[2]/div[2]/div[2]'
-                )
-            ),
-            citations=int(
-                driver.get_text_of_element(
-                    '//*[@id="desktop-app"]/div[2]/div[4]/div[3]/div/div[2]/div[4]/div[1]'
-                ).split()[0]
-            ),
-            title=title,
-        )
-        summaries.append(summary)
-        downloads.append(
-            (
-                link,
-                str(file_path),
-            )
-        )
+    summaries = _collect_articles(driver, Path(dir_path))
     driver.quit()
-    failed_download = set()
-    for link, file_path in downloads:
-        try:
-            download(link, file_path)
-        except RuntimeError:
-            failed_download.add(file_path)
-    summaries = list(
-        summary for summary in summaries if summary.is_valid())
-    dir_path.joinpath(Config.metadate_file_name).write_text(
-        json.dumps(
-            dict(
-                (str(summary_dict.pop("file_path")), summary_dict)
-                for summary_dict in map(asdict, summaries)
-            ),
-            indent=2,
-        )
-    )
+    download_summaries(summaries, Path(dir_path))
     return summaries
```

### Comparing `connectedpapersextractor-0.1.7/src/connectedpapersextractor/create_related_work.py` & `connectedpapersextractor-0.2.0/src/connectedpapersextractor/get_summaries_from_connected_papers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from operator import attrgetter
-from typing import Union, Optional
+from __future__ import annotations
 
-from langchain_core.language_models import LanguageModelInput
-from langchain_core.messages import BaseMessage
-from langchain_core.runnables import Runnable
-from langchain_text_splitters import TextSplitter
+import json
+import shutil
+from os import PathLike
+from typing import Optional
 
-from . import MainPartsExtractor
-from .MainPartsExtractor import _DefaultExtractor
-from .PdfSummary import PdfSummaries
-from ._combine_summaries import _combine_summaries
-from ._summarize_documents import _summarize_documents
+from . import ArticleFilterService
+from . import Articles
+from .Config import Config
+from .utils.download_summaries_from_connected_papers import (
+    download_summaries_from_connected_papers,
+)
+from .utils.get_existing_summaries import (
+    check_for_existing_summaries,
+)
 
 
-def create_related_work(
-    summaries: PdfSummaries,
-    llm: Union[
-        Runnable[LanguageModelInput, str],
-        Optional[Runnable[LanguageModelInput, BaseMessage]],
-    ] = None,
-    text_splitter: Optional[TextSplitter] = None,
-    main_parts_extractor: Optional[MainPartsExtractor] = None,
-    refine: bool = True,
-) -> str:
-    if not summaries:
-        raise ValueError("Summaries must be provided")
-    if main_parts_extractor is None:
-        main_parts_extractor = _DefaultExtractor()
-    if llm is None:
-        from langchain_openai import ChatOpenAI
-        llm = ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo-16k")
-    summaries_with_text = _summarize_documents(
-        summaries, main_parts_extractor, llm, text_splitter
-    )
-    combined_summaries = "\n\n".join(
-        map(": ".join, map(attrgetter("title", "text_summary"), summaries_with_text))
+def get_summaries_from_connected_papers(
+    connected_papers_url: str,
+    pdf_output: Optional[PathLike[str]] = None,
+    article_filter: Optional[ArticleFilterService] = None,
+) -> Articles:
+    article_filter, temp_pdf, summaries = check_for_existing_summaries(
+        pdf_output, article_filter
     )
-    if refine and len(summaries) != 1:
-        return _combine_summaries(combined_summaries, llm)
-    return combined_summaries
+    if not summaries:
+        summaries = download_summaries_from_connected_papers(
+            connected_papers_url,
+            temp_pdf,
+        )
+    else:
+        metadata = json.loads(
+            temp_pdf.joinpath(Config.metadate_file_name).read_text()
+        )
+        for summary in summaries:
+            for key, value in metadata[str(summary.file_path)].items():
+                setattr(summary, key, value)
+    if temp_pdf != pdf_output:
+        shutil.rmtree(temp_pdf)
+    return article_filter.filter(summaries)
```

### Comparing `connectedpapersextractor-0.1.7/PKG-INFO` & `connectedpapersextractor-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: ConnectedPapersExtractor
-Version: 0.1.7
+Version: 0.2.0
 Summary: A package for creating summaries based on https://www.connectedpapers.com/.
 License: MIT
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: EnhancedWebdriver (>=0.1.6,<0.2.0)
 Requires-Dist: PyPDF2 (>=3.0.1,<4.0.0)
+Requires-Dist: arxiv (>=2.1.0,<3.0.0)
 Requires-Dist: cffi (>=1.16.0,<2.0.0)
 Requires-Dist: chromedriver-autoinstaller (>=0.6.4,<0.7.0)
 Requires-Dist: download (>=0.3.5,<0.4.0)
+Requires-Dist: injector (>=0.21.0,<0.22.0)
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-experimental (>=0.0.57,<0.0.58)
 Requires-Dist: langchain-openai (>=0.1.4,<0.2.0)
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: undetected-chromedriver (>=3.5.5,<4.0.0)
```

