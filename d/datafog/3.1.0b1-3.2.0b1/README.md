# Comparing `tmp/datafog-3.1.0b1.tar.gz` & `tmp/datafog-3.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.1.0b1.tar", last modified: Tue May  7 23:49:31 2024, max compression
+gzip compressed data, was "datafog-3.2.0b1.tar", last modified: Mon May 13 18:39:53 2024, max compression
```

## Comparing `datafog-3.1.0b1.tar` & `datafog-3.2.0b1.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-07 23:49:31.418947 datafog-3.1.0b1/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-06 15:35:25.000000 datafog-3.1.0b1/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6034 2024-05-07 23:49:31.418827 datafog-3.1.0b1/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     4813 2024-05-06 18:39:55.000000 datafog-3.1.0b1/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-07 23:49:31.418620 datafog-3.1.0b1/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6034 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      180 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      165 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-07 23:49:31.418994 datafog-3.1.0b1/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1829 2024-05-07 23:33:52.000000 datafog-3.1.0b1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.152751 datafog-3.2.0b1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b1/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6916 2024-05-13 18:39:53.152484 datafog-3.2.0b1/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b1/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.150961 datafog-3.2.0b1/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 14:39:02.000000 datafog-3.2.0b1/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      150 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2969 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.152118 datafog-3.2.0b1/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6916 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      201 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 18:39:53.152807 datafog-3.2.0b1/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1935 2024-05-13 18:39:10.000000 datafog-3.2.0b1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.151863 datafog-3.2.0b1/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b1/tests/test_main.py
```

### Comparing `datafog-3.1.0b1/LICENSE` & `datafog-3.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.1.0b1/PKG-INFO` & `datafog-3.2.0b1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: datafog
-Version: 3.1.0b1
-Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
-Home-page: https://datafog.ai
-Author: DataFog
-Author-email: hi@datafog.ai
-Maintainer: DataFog
-Maintainer-email: hi@datafog.ai
-License: MIT
-Project-URL: Homepage, https://datafog.ai
-Project-URL: Documentation, https://docs.datafog.ai
-Project-URL: Discord, https://discord.gg/bzDth394R4
-Project-URL: Twitter, https://twitter.com/datafoginc
-Project-URL: GitHub, https://github.com/datafog/datafog-python
-Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: tox
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
 </p>
@@ -54,57 +23,104 @@
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
 ### Core Problem
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-How do you keep:
 
-- Customer PII
-- Employee PII
-- Sensitive company information pertaining to org changes or restructurings
-- Pending M&A activity
-- Conversations with external counsel on material corporate matters (i.e. product recall, etc)
-- and more
+### How it works
 
-from entering a Generative AI environment in the first place? What you need is a tool to scan and redact your RAG-bound documents based on your organization or team needs.
+![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
 
-**That's where DataFog comes in.**
 
-### How it works
+## Installation
 
-![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
+DataFog can be installed via pip:
 
-### There's lots of PII tools out there; why DataFog?
+```bash
+pip install datafog
+```
 
-If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
-In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
-are purpose-built for the problem that they are solving.
+## Examples - Updated for v3.1
 
-However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
+### Base case: PII annotation of text-files
 
-### Roadmap
+```
+from datafog import OCRPIIAnnotator, TextPIIAnnotator
+import json
+import requests
+
+response = requests.get('https://gist.githubusercontent.com/sidmohan0/1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/sotu_2023.txt')
+response.raise_for_status()  # Ensure the request was successful
+text = response.text
+# print(text)
+text_annotator = TextPIIAnnotator()
+annotated_text = text_annotator.run(text, output_path=f"sotu_2023_output.json")
+print("Annotated Text:", annotated_text)
+```
 
-DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT). Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
+### OCR Reference Set (Images)
 
-![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
+```
+image_set = {
+    "medical_invoice": "https://s3.amazonaws.com/thumbnails.venngage.com/template/dc377004-1c2d-49f2-8ddf-d63f11c8d9c2.png",
+    "sales_receipt": "https://templates.invoicehome.com/sales-receipt-template-us-classic-white-750px.png",
+    "press_release": "https://newsroom.cisco.com/c/dam/r/newsroom/en/us/assets/a/y2023/m09/cisco_splunk_1200x675_v3.png",
+    "insurance_claim_scanned_form": "https://www.pdffiller.com/preview/101/35/101035394.png",
+    "scanned_internal_record": "https://www.pdffiller.com/preview/435/972/435972694.png",
+    "executive_email": "https://pbs.twimg.com/media/GM3-wpeWkAAP-cX.jpg"
+}
 
-## Installation
+```
 
-DataFog can be installed via pip:
+### OCR text extraction from images + PII annotation
+
+with this, you can then run the following steps:
 
-```bash
-pip install datafog
 ```
+from datafog import OCRPIIAnnotator, TextPIIAnnotator
+import json
 
-## Examples - Updated for v3
+image_url = image_set["executive_email"]
 
-Check out for examples to get started with datafog v3: https://colab.research.google.com/drive/1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd
+annotator = OCRPIIAnnotator()
+annotated_text = annotator.run(image_url, output_path=f"executive_email_output.json")
+print("Annotated Text:", annotated_text)
 
+```
+
+and the output should look like this:
+
+```
+Annotated Text: {'DATE_TIME': ['Wednesday', 'June 12, 2019'], 'LOC': [], 'NRP': [], 'ORG': [], 'PER': ['Kevin Scott Sent', 'Satya Nadella', 'Bill Gates Subject', 'Thoughts']}
+
+```
+
+### With PySpark
+
+Note: as of 3.1.0, you'll need to start the Spark session by instancing the DataFog class as shown below
+
+```
+from datafog import DataFog
+from datafog.pii_annotation import ImageProcessor
+datafog = DataFog()
+
+# let's process the images that we shared above
+processed_images = [(name, ImageProcessor().download_image(url=image_url)) for name, image_url in image_set.items()]
+
+from datafog.pii_annotation import SparkService
+parsed_images = [(name, ImageProcessor().parse_image(img)) for name, img in processed_images]
+
+df = SparkService().spark.createDataFrame(parsed_images, ["image_name", "parsed_data"])
+
+# Display DataFrame
+df.show(truncate=False)
+
+```
 
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
@@ -122,9 +138,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### html2text {}

```diff
@@ -1,64 +1,54 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.1.0b1 Summary: Scan, redact, and
-manage PII in your documents before they get uploaded to a Retrieval Augmented
-Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
-email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
-License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
-Documentation, https://docs.datafog.ai Project-URL: Discord, https://
-discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
-Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
 DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
-How do you keep: - Customer PII - Employee PII - Sensitive company information
-pertaining to org changes or restructurings - Pending M&A activity -
-Conversations with external counsel on material corporate matters (i.e. product
-recall, etc) - and more from entering a Generative AI environment in the first
-place? What you need is a tool to scan and redact your RAG-bound documents
-based on your organization or team needs. **That's where DataFog comes in.**
 ### How it works ![image](https://github.com/DataFog/datafog-python/assets/
-61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ### There's lots of PII tools
-out there; why DataFog? If you look at the landscape of PII detection tools,
-their very existence was in many cases driven by regulatory requirements (i.e.
-'comply with CCPA/GDPR/HIPAA'). In this scenario, there's a very defined
-problem, a specific set of immutable entities to look for, and a relatively
-static universe of document schema to work with. What that means as an end-
-result is that the products are purpose-built for the problem that they are
-solving. However, Generative AI changes how we think about privacy. There's now
-a changing set of privacy requirements (new M&A deals, internal discussions
-means new terms to scan/redact) as well as different and varying document
-sources to contend with. PII detection is no longer just about compliance, it's
-an active - and for some, new - internal security threat for CISOs and Eng
-Leaders to contend with. We want DataFog to be built and driven to meet the
-needs of the open-source community as they tackle this challenge. ### Roadmap
-DataFog is an active project with regular weekly releases to production
-(typically on/around Monday evenings US PT). Here's a snapshot of our coming
-roadmap; if you have questions or would like to weigh in, join our discord and
-let us know what we can do to make the product better! ![image](https://
-github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
-0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
-install datafog ``` ## Examples - Updated for v3 Check out for examples to get
-started with datafog v3: https://colab.research.google.com/drive/
-1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd ## Contributing DataFog
-is a community-driven **open-source** platform and we've been fortunate to have
-a small and growing contributor base. We'd love to hear ideas, feedback,
-suggestions for improvement - anything on your mind about what you think can be
-done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
-and join our growing community. ### Dev Notes - Justfile commands: - `just
-format` to apply formatting. - `just lint` to check formatting and style. ###
-Testing To run the datafog unit tests, check out this repository and do ``` tox
-``` ## License This software is published under the [MIT license](https://
-en.wikipedia.org/wiki/MIT_License).
+61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ## Installation DataFog can be
+installed via pip: ```bash pip install datafog ``` ## Examples - Updated for
+v3.1 ### Base case: PII annotation of text-files ``` from datafog import
+OCRPIIAnnotator, TextPIIAnnotator import json import requests response =
+requests.get('https://gist.githubusercontent.com/sidmohan0/
+1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/
+sotu_2023.txt') response.raise_for_status() # Ensure the request was successful
+text = response.text # print(text) text_annotator = TextPIIAnnotator()
+annotated_text = text_annotator.run(text, output_path=f"sotu_2023_output.json")
+print("Annotated Text:", annotated_text) ``` ### OCR Reference Set (Images) ```
+image_set = { "medical_invoice": "https://s3.amazonaws.com/
+thumbnails.venngage.com/template/dc377004-1c2d-49f2-8ddf-d63f11c8d9c2.png",
+"sales_receipt": "https://templates.invoicehome.com/sales-receipt-template-us-
+classic-white-750px.png", "press_release": "https://newsroom.cisco.com/c/dam/r/
+newsroom/en/us/assets/a/y2023/m09/cisco_splunk_1200x675_v3.png",
+"insurance_claim_scanned_form": "https://www.pdffiller.com/preview/101/35/
+101035394.png", "scanned_internal_record": "https://www.pdffiller.com/preview/
+435/972/435972694.png", "executive_email": "https://pbs.twimg.com/media/GM3-
+wpeWkAAP-cX.jpg" } ``` ### OCR text extraction from images + PII annotation
+with this, you can then run the following steps: ``` from datafog import
+OCRPIIAnnotator, TextPIIAnnotator import json image_url = image_set
+["executive_email"] annotator = OCRPIIAnnotator() annotated_text =
+annotator.run(image_url, output_path=f"executive_email_output.json") print
+("Annotated Text:", annotated_text) ``` and the output should look like this:
+``` Annotated Text: {'DATE_TIME': ['Wednesday', 'June 12, 2019'], 'LOC': [],
+'NRP': [], 'ORG': [], 'PER': ['Kevin Scott Sent', 'Satya Nadella', 'Bill Gates
+Subject', 'Thoughts']} ``` ### With PySpark Note: as of 3.1.0, you'll need to
+start the Spark session by instancing the DataFog class as shown below ``` from
+datafog import DataFog from datafog.pii_annotation import ImageProcessor
+datafog = DataFog() # let's process the images that we shared above
+processed_images = [(name, ImageProcessor().download_image(url=image_url)) for
+name, image_url in image_set.items()] from datafog.pii_annotation import
+SparkService parsed_images = [(name, ImageProcessor().parse_image(img)) for
+name, img in processed_images] df = SparkService().spark.createDataFrame
+(parsed_images, ["image_name", "parsed_data"]) # Display DataFrame df.show
+(truncate=False) ``` ## Contributing DataFog is a community-driven **open-
+source** platform and we've been fortunate to have a small and growing
+contributor base. We'd love to hear ideas, feedback, suggestions for
+improvement - anything on your mind about what you think can be done to make
+DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
+growing community. ### Dev Notes - Justfile commands: - `just format` to apply
+formatting. - `just lint` to check formatting and style. ### Testing To run the
+datafog unit tests, check out this repository and do ``` tox ``` ## License
+This software is published under the [MIT license](https://en.wikipedia.org/
+wiki/MIT_License).
```

### Comparing `datafog-3.1.0b1/setup.py` & `datafog-3.2.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.1.0b1"
+    return "3.2.0b1"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -22,26 +22,31 @@
     name="datafog",
     version=__version__(),
     author="DataFog",
     author_email="hi@datafog.ai",
     description="Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    packages=["datafog"],
     install_requires=[
-        "pandas==2.2.2",
+        "pandas",
         "Requests==2.31.0",
         "spacy==3.4.4",
         "en_spacy_pii_fast==0.0.0",
         "transformers==4.40.1",
         "torch==2.2.2",
         "pyspark==3.4.1",
         "pydantic==1.10.8",
         "Pillow",
         "sentencepiece",
         "protobuf",
+        "pytesseract",
+        "aiohttp",
+        "asyncio",
+        "pytest-asyncio",
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

