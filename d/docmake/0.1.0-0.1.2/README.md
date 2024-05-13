# Comparing `tmp/docmake-0.1.0.tar.gz` & `tmp/docmake-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmake-0.1.0.tar", max compression
+gzip compressed data, was "docmake-0.1.2.tar", max compression
```

## Comparing `docmake-0.1.0.tar` & `docmake-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     4002 2023-10-04 22:00:52.563218 docmake-0.1.0/README.md
--rwxr-xr-x   0        0        0      374 2024-05-13 15:22:48.462921 docmake-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.0/src/__init__.py
--rwxr-xr-x   0        0        0    31507 2024-05-13 04:44:25.185511 docmake-0.1.0/src/app.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 docmake-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2024-05-13 15:11:36.044304 docmake-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     3953 2024-05-13 16:01:03.066258 docmake-0.1.2/README.md
+-rwxr-xr-x   0        0        0      421 2024-05-13 15:59:16.035705 docmake-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-13 15:24:15.859574 docmake-0.1.2/src/__init__.py
+-rwxr-xr-x   0        0        0    31507 2024-05-13 04:44:25.185511 docmake-0.1.2/src/app.py
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 docmake-0.1.2/PKG-INFO
```

### Comparing `docmake-0.1.0/LICENSE` & `docmake-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docmake-0.1.0/README.md` & `docmake-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,46 +11,46 @@
 ## Installation
 
 1. Install Python.
 
 2. Clone this repository:
 
    ```bash
-   git clone https://github.com/your-username/docmaker-web-ui.git
+   git clone https://github.com/morisono/docmaker_webui.git
    ```
 
 3. Navigate to the project directory:
 
    ```bash
-   cd docmaker-web-ui
+   cd docmaker_webui
    ```
 
 4. Install dependencies:
 
    ```bash
    pip install -r requirements.txt
    ```
 
 ## CLI Usage
 
 ```sh
 usage: 
     [Examples]
         - Generate a PDF:
-            python app.py -i in_*.[html|pdf] -o out.pdf [options]
+            docmake -i in_*.[html|pdf] -o out.pdf [options]
 
             For example:
-                python app.py -i in_*.html -o out.pdf --scale 0.8 --css ' h1 { color: red }'
+                docmake -i in_*.html -o out.pdf --scale 0.8 --css ' h1 { color: red }'
 
         - Encrypt/Decrypto a PDF:
-            python app.py -i in.[html|pdf] -o out.pdf [options]
+            docmake -i in.[html|pdf] -o out.pdf [options]
 
             For example:
-                python app.py -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
-                python app.py -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
+                docmake -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
+                docmake -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
 
     [Units]
         You can use the following units for width, height, and margin options:
         - px (pixels) - Default unit., in (inches)., cm (centimeters)., mm (millimeters).
 
     [Formats]
         The following paper formats are available for the format option:
@@ -101,23 +101,23 @@
 
 This section provides instructions on how to use the web user interface (Web UI) of DocMaker Web UI.
 
 
 1. Start the app in the project directory:
 
    ```bash
-   python app.py --webui
+   docmake --webui
    ```
 
 2. Access it in your web browser at http://127.0.0.1:7860.
 
 3. Use the web interface to configure input files and options.
 
 4. Click the "▶" button to generate a PDF.
 
 ## License
 
 This project is provided under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Support
 
-For inquiries regarding support, including questions and bug reports, please use [GitHub Issues](https://github.com/your-username/docmaker-web-ui/issues).
+For inquiries regarding support, including questions and bug reports, please use [GitHub Issues](https://github.com/morisono/docmaker_webui/issues).
```

### Comparing `docmake-0.1.0/src/app.py` & `docmake-0.1.2/src/app.py`

 * *Files identical despite different names*

### Comparing `docmake-0.1.0/PKG-INFO` & `docmake-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: docmake
-Version: 0.1.0
-Summary: 
-Home-page: https://github.com/morisono/docmaker-webui
+Version: 0.1.2
+Summary: Generate pdf files from other format documents.
+Home-page: https://github.com/morisono/docmaker_webui
 Author: admin
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Project-URL: Repository, https://github.com/morisono/docmaker-webui
+Project-URL: Repository, https://github.com/morisono/docmaker_webui
 Description-Content-Type: text/markdown
 
 # DocMaker Web UI
 
 DocMaker Web UI is for converting various document formats to PDF format. Generate PDF documents from files such as Markdown, HTML, and CSS by combining them.
 
 ## Key Features
@@ -25,46 +25,46 @@
 ## Installation
 
 1. Install Python.
 
 2. Clone this repository:
 
    ```bash
-   git clone https://github.com/your-username/docmaker-web-ui.git
+   git clone https://github.com/morisono/docmaker_webui.git
    ```
 
 3. Navigate to the project directory:
 
    ```bash
-   cd docmaker-web-ui
+   cd docmaker_webui
    ```
 
 4. Install dependencies:
 
    ```bash
    pip install -r requirements.txt
    ```
 
 ## CLI Usage
 
 ```sh
 usage: 
     [Examples]
         - Generate a PDF:
-            python app.py -i in_*.[html|pdf] -o out.pdf [options]
+            docmake -i in_*.[html|pdf] -o out.pdf [options]
 
             For example:
-                python app.py -i in_*.html -o out.pdf --scale 0.8 --css ' h1 { color: red }'
+                docmake -i in_*.html -o out.pdf --scale 0.8 --css ' h1 { color: red }'
 
         - Encrypt/Decrypto a PDF:
-            python app.py -i in.[html|pdf] -o out.pdf [options]
+            docmake -i in.[html|pdf] -o out.pdf [options]
 
             For example:
-                python app.py -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
-                python app.py -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
+                docmake -i demo.pdf -o demo.encrypted.pdf --encrypto --autogen
+                docmake -i demo.encrypted.pdf -o demo.decrypted.pdf --decrypto
 
     [Units]
         You can use the following units for width, height, and margin options:
         - px (pixels) - Default unit., in (inches)., cm (centimeters)., mm (millimeters).
 
     [Formats]
         The following paper formats are available for the format option:
@@ -115,24 +115,24 @@
 
 This section provides instructions on how to use the web user interface (Web UI) of DocMaker Web UI.
 
 
 1. Start the app in the project directory:
 
    ```bash
-   python app.py --webui
+   docmake --webui
    ```
 
 2. Access it in your web browser at http://127.0.0.1:7860.
 
 3. Use the web interface to configure input files and options.
 
 4. Click the "▶" button to generate a PDF.
 
 ## License
 
 This project is provided under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Support
 
-For inquiries regarding support, including questions and bug reports, please use [GitHub Issues](https://github.com/your-username/docmaker-web-ui/issues).
+For inquiries regarding support, including questions and bug reports, please use [GitHub Issues](https://github.com/morisono/docmaker_webui/issues).
```

