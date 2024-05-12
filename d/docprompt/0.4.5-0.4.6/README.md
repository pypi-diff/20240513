# Comparing `tmp/docprompt-0.4.5.tar.gz` & `tmp/docprompt-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.5.tar", last modified: Sat May 11 02:46:12 2024, max compression
+gzip compressed data, was "docprompt-0.4.6.tar", last modified: Sun May 12 22:46:44 2024, max compression
```

## Comparing `docprompt-0.4.5.tar` & `docprompt-0.4.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.5/LICENSE
--rw-r--r--   0        0        0     5174 2024-05-10 05:55:50.188361 docprompt-0.4.5/README.md
--rw-r--r--   0        0        0      752 2024-05-11 02:46:08.414792 docprompt-0.4.5/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.5/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.5/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0     1541 2024-05-07 01:14:14.543427 docprompt-0.4.5/docprompt/_pdfium.py
--rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.5/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9861 2024-05-10 22:04:25.589467 docprompt-0.4.5/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1425 2024-05-10 22:19:31.977780 docprompt-0.4.5/docprompt/provenance/source.py
--rw-r--r--   0        0        0     5771 2024-05-10 22:19:31.977780 docprompt-0.4.5/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.4.5/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.5/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9402 2024-05-07 01:14:14.547427 docprompt-0.4.5/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.5/docprompt/schema/layout.py
--rw-r--r--   0        0        0    12026 2024-05-07 01:27:16.164027 docprompt-0.4.5/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.5/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.5/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.5/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.5/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.5/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.5/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.5/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.5/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.5/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.5/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.5/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.5/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.5/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.5/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.5/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.5/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.5/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.5/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.5/docprompt/utils/util.py
--rw-r--r--   0        0        0     2717 2024-05-11 02:46:12.886829 docprompt-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.5/tests/fixtures.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.5/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.5/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.5/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.5/tests/test_document.py
--rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.4.5/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.5/tests/test_layout_models.py
--rw-r--r--   0        0        0     2868 2024-05-10 22:19:31.977780 docprompt-0.4.5/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.5/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.5/tests/util.py
--rw-r--r--   0        0        0     6689 1970-01-01 00:00:00.000000 docprompt-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.6/LICENSE
+-rw-r--r--   0        0        0     5174 2024-05-10 05:55:50.188361 docprompt-0.4.6/README.md
+-rw-r--r--   0        0        0      752 2024-05-12 22:46:23.635955 docprompt-0.4.6/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.6/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.6/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0     1545 2024-05-12 22:42:37.149558 docprompt-0.4.6/docprompt/_pdfium.py
+-rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.6/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9861 2024-05-10 22:04:25.589467 docprompt-0.4.6/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1425 2024-05-10 22:19:31.977780 docprompt-0.4.6/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     5771 2024-05-10 22:19:31.977780 docprompt-0.4.6/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.4.6/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.6/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9548 2024-05-12 22:44:37.214627 docprompt-0.4.6/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.6/docprompt/schema/layout.py
+-rw-r--r--   0        0        0    12026 2024-05-07 01:27:16.164027 docprompt-0.4.6/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.6/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.6/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.6/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.6/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.6/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.6/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.6/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.6/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.6/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.6/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.6/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.6/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.6/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.6/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.6/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.6/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.6/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.6/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.6/docprompt/utils/util.py
+-rw-r--r--   0        0        0     2717 2024-05-12 22:46:44.480225 docprompt-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.6/tests/fixtures.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.6/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.6/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.6/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5545 2024-05-12 22:45:37.195345 docprompt-0.4.6/tests/test_document.py
+-rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.4.6/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.6/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2868 2024-05-10 22:19:31.977780 docprompt-0.4.6/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.6/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.6/tests/util.py
+-rw-r--r--   0        0        0     6689 1970-01-01 00:00:00.000000 docprompt-0.4.6/PKG-INFO
```

### Comparing `docprompt-0.4.5/LICENSE` & `docprompt-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/README.md` & `docprompt-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/__init__.py` & `docprompt-0.4.6/docprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.5/docprompt/_exec/ghostscript.py` & `docprompt-0.4.6/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/_pdfium.py` & `docprompt-0.4.6/docprompt/_pdfium.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     page_number: int,
     **kwargs,
 ):
     """
     Rasterizes a page of a PDF document
     """
     with get_pdfium_document(fp) as pdf:
-        page = pdf.get_page(page_number)
+        page = pdf.get_page(page_number - 1)
         return page.render(**kwargs)
 
 
 def rasterize_pdf_with_pdfium(
     fp: Union[PathLike, Path, bytes],
     **kwargs,
 ):
```

### Comparing `docprompt-0.4.5/docprompt/provenance/search.py` & `docprompt-0.4.6/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/provenance/source.py` & `docprompt-0.4.6/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/provenance/util.py` & `docprompt-0.4.6/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/rasterize.py` & `docprompt-0.4.6/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/schema/document.py` & `docprompt-0.4.6/docprompt/schema/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,17 @@
         """
         Compresses the document using Ghostscript
         """
         with self.as_tempfile() as temp_path:
             return compress_pdf_to_bytes(temp_path, **compression_kwargs)
 
     def render_page_to_bytes(self, page_number: int, dpi: int = DEFAULT_DPI) -> bytes:
+        if page_number <= 0 or page_number > self.num_pages:
+            raise ValueError(f"Page number must be between 0 and {self.num_pages}")
+
         bitmap = rasterize_page_with_pdfium(
             self.file_bytes, page_number, scale=(1 / 72) * dpi
         )
         pil = bitmap.to_pil().convert("RGB")
 
         img_bytes = BytesIO()
         pil.save(img_bytes, format="PNG")
```

### Comparing `docprompt-0.4.5/docprompt/schema/layout.py` & `docprompt-0.4.6/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/schema/pipeline.py` & `docprompt-0.4.6/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/base.py` & `docprompt-0.4.6/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/message.py` & `docprompt-0.4.6/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.6/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/ocr/result.py` & `docprompt-0.4.6/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.6/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.6/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.6/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/utils/date_extraction.py` & `docprompt-0.4.6/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/utils/masking/image.py` & `docprompt-0.4.6/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/utils/splitter.py` & `docprompt-0.4.6/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/docprompt/utils/util.py` & `docprompt-0.4.6/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/pyproject.toml` & `docprompt-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "docprompt"
-version = "0.4.5"
+version = "0.4.6"
 description = "Documents and large language models."
 authors = [
     { name = "Frank Colson", email = "frank@pageleaf.io" },
 ]
 dependencies = [
     "python-dateutil<3.0.0,>=2.8.2",
     "pillow>=9.0.1",
```

### Comparing `docprompt-0.4.5/tests/fixtures/1.pdf` & `docprompt-0.4.6/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/fixtures/1_ocr.json` & `docprompt-0.4.6/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/test_date_extraction.py` & `docprompt-0.4.6/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/test_document.py` & `docprompt-0.4.6/tests/test_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,26 @@
     # Fow now just test PIL can open the image
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
         img_bytes = doc.rasterize_page(1)
         Image.open(io.BytesIO(img_bytes))
 
 
+def test_rasterize_invalid_page():
+    document = load_document(PDF_FIXTURES[0].get_full_path())
+
+    with pytest.raises(ValueError):
+        document.rasterize_page(0)
+
+    with pytest.raises(ValueError):
+        document.rasterize_page(1000)
+
+    document.rasterize_page(len(document))  # Should rasterize last page
+
+
 def test_rasterize_convert_and_quantize():
     # Fow now just test PIL can open the image
     convert_mode = "L"
     quantize_color_count = 8
 
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
```

### Comparing `docprompt-0.4.5/tests/test_documentnode.py` & `docprompt-0.4.6/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/test_layout_models.py` & `docprompt-0.4.6/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/test_search.py` & `docprompt-0.4.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/test_threadpool.py` & `docprompt-0.4.6/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/tests/util.py` & `docprompt-0.4.6/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.5/PKG-INFO` & `docprompt-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.4.5
+Version: 0.4.6
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 Author-Email: Frank Colson <frank@pageleaf.io>
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.4.5 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.4.6 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 Author-Email: Frank Colson
 pageleaf.io> License: Apache-2.0 Classifier: Development Status :: 2 - Pre-
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

