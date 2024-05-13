# Comparing `tmp/payconpy-2.1.1.tar.gz` & `tmp/payconpy-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.1.1.tar", last modified: Mon Apr 22 17:45:51 2024, max compression
+gzip compressed data, was "payconpy-2.1.2.tar", last modified: Mon May 13 20:37:10 2024, max compression
```

## Comparing `payconpy-2.1.1.tar` & `payconpy-2.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.545956 payconpy-2.1.1/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      899 2024-04-22 17:45:51.537295 payconpy-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:50.761731 payconpy-2.1.1/payconpy/
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:50.946373 payconpy-2.1.1/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.1.1/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.1.1/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:50.976784 payconpy-2.1.1/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:50.989069 payconpy-2.1.1/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.031936 payconpy-2.1.1/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.1.1/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-2.1.1/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.072198 payconpy-2.1.1/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.1.1/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.105039 payconpy-2.1.1/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.1.1/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.143413 payconpy-2.1.1/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.1.1/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.170662 payconpy-2.1.1/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.1.1/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.206256 payconpy-2.1.1/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.1.1/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.1.1/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.231486 payconpy-2.1.1/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.1.1/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11710 2024-04-21 21:00:14.000000 payconpy-2.1.1/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.274363 payconpy-2.1.1/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.1/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.294615 payconpy-2.1.1/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.1.1/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.1.1/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.336742 payconpy-2.1.1/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.1/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.1.1/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.1.1/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:51.499446 payconpy-2.1.1/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.1/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   147726 2024-04-22 17:45:30.000000 payconpy-2.1.1/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:45:50.925290 payconpy-2.1.1/payconpy.egg-info/
--rw-rw-rw-   0        0        0      899 2024-04-22 17:45:50.000000 payconpy-2.1.1/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-04-22 17:45:50.000000 payconpy-2.1.1/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 17:45:50.000000 payconpy-2.1.1/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2024-04-22 17:45:50.000000 payconpy-2.1.1/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-04-22 17:45:50.000000 payconpy-2.1.1/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 17:45:51.545956 payconpy-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2049 2024-04-22 17:45:36.000000 payconpy-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.126229 payconpy-2.1.2/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0      899 2024-05-13 20:37:10.121486 payconpy-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.794518 payconpy-2.1.2/payconpy/
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.887333 payconpy-2.1.2/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.1.2/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.1.2/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.910264 payconpy-2.1.2/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.918010 payconpy-2.1.2/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.934283 payconpy-2.1.2/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.1.2/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    11597 2024-05-09 12:27:06.000000 payconpy-2.1.2/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.952263 payconpy-2.1.2/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.1.2/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.970352 payconpy-2.1.2/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.1.2/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.984990 payconpy-2.1.2/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.1.2/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.002048 payconpy-2.1.2/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.1.2/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.015445 payconpy-2.1.2/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.1.2/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.031048 payconpy-2.1.2/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.1.2/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.1.2/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.054770 payconpy-2.1.2/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.067902 payconpy-2.1.2/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.1.2/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.1.2/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.087158 payconpy-2.1.2/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.1.2/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.1.2/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.109961 payconpy-2.1.2/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   147726 2024-04-22 17:45:30.000000 payconpy-2.1.2/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.866217 payconpy-2.1.2/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      899 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 20:37:10.126229 payconpy-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2049 2024-05-13 20:36:54.000000 payconpy-2.1.2/setup.py
```

### Comparing `payconpy-2.1.1/LICENSE` & `payconpy-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/PKG-INFO` & `payconpy-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.1.1
+Version: 2.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.1.1/payconpy/femails/femails.py` & `payconpy-2.1.2/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fexceptions/exceptions.py` & `payconpy-2.1.2/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fpdf/focr/orc.py` & `payconpy-2.1.2/payconpy/fpdf/focr/orc.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     if export_from_file_txt:
         with open(export_from_file_txt, 'w', encoding='utf-8') as f:
             f.write(text)
     
     # Retorna o texto extraído
     return text
 
-def ocr_google_vision(pdf, api_key, dpi=300, file_output=uuid.uuid4(), return_text=True, limit_pages=None):
+def ocr_google_vision(pdf, api_key, dpi=300, file_output=uuid.uuid4(), return_text=True, limit_pages=None, is_image=False):
     def detect_text(files_png: list[str], api_key) -> str:
         """Recupera o texto das imagens
 
         Args:
             files_png (list[str]): Lista de imagens do pdf
 
         Raises:
@@ -91,41 +91,52 @@
                     else:
                         contador = len(files_png)
                 else:
                     raise Exception(r.json()['error']['message'])
 
         return remover_acentos(result.lower().strip())
     
-    with fitz.open(pdf) as pdf_fitz:
-        cria_dir_no_dir_de_trabalho_atual('pages')
+    if is_image == False:
+        with fitz.open(pdf) as pdf_fitz:
+            cria_dir_no_dir_de_trabalho_atual('pages')
+            limpa_diretorio('pages')
+            faz_log(f'Convertendo PDF para páginas...')
+            number_of_pages = len(pdf_fitz) if limit_pages is None else min(limit_pages, len(pdf_fitz))
+            with tqdm(total=number_of_pages, desc='EXTRACT PAGES') as bar:
+                for i, page in enumerate(pdf_fitz):
+                    if i >= number_of_pages:
+                        break
+                    page = pdf_fitz.load_page(i)
+                    mat = fitz.Matrix(dpi/72, dpi/72)  # Matriz de transformação usando DPI
+                    pix = page.get_pixmap(matrix=mat)
+                    image = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
+                    image.save(f'pages/{i}.png')
+                    bar.update(1)
+            
+        faz_log('Enviando para Google Vision...')
+        files = list(arquivos_com_caminho_absoluto_do_arquivo('pages'))
+        text_ocr = detect_text(files, api_key)
         limpa_diretorio('pages')
-        faz_log(f'Convertendo PDF para páginas...')
-        number_of_pages = len(pdf_fitz) if limit_pages is None else min(limit_pages, len(pdf_fitz))
-        with tqdm(total=number_of_pages, desc='EXTRACT PAGES') as bar:
-            for i, page in enumerate(pdf_fitz):
-                if i >= number_of_pages:
-                    break
-                page = pdf_fitz.load_page(i)
-                mat = fitz.Matrix(dpi/72, dpi/72)  # Matriz de transformação usando DPI
-                pix = page.get_pixmap(matrix=mat)
-                image = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
-                image.save(f'pages/{i}.png')
-                bar.update(1)
-        
-    faz_log('Enviando para Google Vision...')
-    files = list(arquivos_com_caminho_absoluto_do_arquivo('pages'))
-    text_ocr = detect_text(files, api_key)
-    limpa_diretorio('pages')
-    if return_text:
-        return text_ocr
+        if return_text:
+            return text_ocr
+        else:
+            file_path = arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt')
+            with open(file_path, 'w') as f:
+                text_ocr.write(f)
+            return file_path
     else:
-        file_path = arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt')
-        with open(file_path, 'w') as f:
-            text_ocr.write(f)
-        return file_path
+        files = [pdf]
+        text_ocr = detect_text(files, api_key)
+        if return_text:
+            return text_ocr
+        else:
+            file_path = arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt')
+            with open(file_path, 'w') as f:
+                text_ocr.write(f)
+            return file_path
     
     
     
 def ocr_tesseract_v2(pdf, dpi=300, file_output=uuid.uuid4(), return_text=True, config_tesseract='', limit_pages=None, lang='por', timeout=120, download_tesseract=False):
     """Realiza OCR em um arquivo PDF usando Tesseract, com opções de customização avançadas.
 
     Esta função avançada permite a personalização de diversos parâmetros do OCR, como DPI, linguagem, limitação de páginas e timeout. Caso os binários do Tesseract não estejam presentes, ela executa uma única requisição para o GitHub da organização Paycon para baixar os binários necessários. Esta requisição é crucial para a funcionalidade da função mas levanta questões importantes sobre segurança de dados.
```

### Comparing `payconpy-2.1.1/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.1.2/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.1.2/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fpython/fpython.py` & `payconpy-2.1.2/payconpy/fpython/fpython.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fregex/fregex.py` & `payconpy-2.1.2/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/fselenium/fselenium.py` & `payconpy-2.1.2/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.1.2/payconpy/odoo/odoo_xmlrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,41 +152,41 @@
         models.execute_kw(DB_RPC, uid, PASSWORD_RPC, model, 'write', [[record_id], data])
         faz_log(f'Record updated with ID: {record_id} on model: {model}')
         return record_id
     else:
         faz_log(f'Record with ID {record_id} does not exist on model: {model}')
         return None
 
-def get_odoo(model: str, data: dict, auth: dict, domain: list = [], uid: int = None, limit: int = None) -> list[dict]:
+def get_odoo(model: str, data: dict, auth: dict, domains: list = [], uid: int = None, limit: int = None) -> list[dict]:
     """
     Retrieves data from an Odoo model using XML-RPC, applying domains.
 
     Args:
         model (str): The name of the Odoo model to retrieve data from.
         data (dict): A dictionary containing additional arguments to pass to the XML-RPC call.
         auth (dict): A dictionary containing authentication information including URL, database name, username, and password
-        domain (list): A list of tuples representing the domains to apply. Each tuple should contain
+        domains (list): A list of tuples representing the domains to apply. Each tuple should contain
                         the field name, the operator, and the value to domain by.
         uid (int): UID from a retrieved auth
         limit (int): Limit of records to retrieve.
     Returns:
         list[dict]: A list of dictionaries containing the retrieved data.
 
     Example:
     ```
     model = 'res.partner'
     data = {'fields': ['name', 'email']}  # or without values into list for get all fields
-    domain = [('email', '=', 'example@domain.com')]
+    domains = [('email', '=', 'example@domain.com')]
     auth = {
         "URL_RPC": "http://example.com/",
         "DB_RPC": "mydb",
         "USERNAME_RPC": "admin",
         "PASSWORD_RPC": "admin_password"
     }
-    get_odoo(model, data, auth, domain, limit=10) 
+    get_odoo(model, data, auth, domains, limit=10) 
     [{'name': 'John Doe', 'email': 'example@domain.com'}]
     
     ```
     """
     URL_RPC = auth['URL_RPC']
     DB_RPC = auth['DB_RPC']
     USERNAME_RPC = auth['USERNAME_RPC']
@@ -194,30 +194,31 @@
     context = ssl._create_unverified_context()
 
     common = client.ServerProxy(f'{URL_RPC}xmlrpc/2/common', context=context)
     if uid is None:
         uid = common.authenticate(DB_RPC, USERNAME_RPC, PASSWORD_RPC, {})
     models = client.ServerProxy('{}/xmlrpc/2/object'.format(URL_RPC), context=context)
 
-    # Apply domains to the search call
+    # Apply filters to the search call
     domain = []
-    for dom in domain:
+    for dom in domains:
         domain.append(dom)
     
     # If a limit is provided, use it in the data argument for search_read
     if limit is not None:
         if 'limit' in data:
             # Respect the lower of the two limits if 'limit' was already in 'data'
             data['limit'] = min(data['limit'], limit)
         else:
             data['limit'] = limit
 
     values = models.execute_kw(DB_RPC, uid, PASSWORD_RPC, model, 'search_read', [domain], data)
     return values
 
+
 def insert_odoo_lots(model, data, auth, uid=None):
     """
     ### Alert! No verify if records exists
     Inserts a batch of records into a specified Odoo model using XML-RPC and returns the IDs of the newly created records. This function is 
     particularly useful for inserting multiple records in a single call, enhancing performance when dealing with large datasets.
 
     Args:
```

### Comparing `payconpy-2.1.1/payconpy/openai/apis/apis.py` & `payconpy-2.1.2/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/openai/assistants/assistants.py` & `payconpy-2.1.2/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/openai/get_cost.py` & `payconpy-2.1.2/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy/utils/utils.py` & `payconpy-2.1.2/payconpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/payconpy.egg-info/PKG-INFO` & `payconpy-2.1.2/payconpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.1.1
+Version: 2.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.1.1/payconpy.egg-info/SOURCES.txt` & `payconpy-2.1.2/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.1/setup.py` & `payconpy-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.1.1'
+version = '2.1.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
```

