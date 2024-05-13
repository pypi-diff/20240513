# Comparing `tmp/datafog-3.2.0b1.tar.gz` & `tmp/datafog-3.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b1.tar", last modified: Mon May 13 18:39:53 2024, max compression
+gzip compressed data, was "datafog-3.2.0b2.tar", last modified: Mon May 13 18:57:19 2024, max compression
```

## Comparing `datafog-3.2.0b1.tar` & `datafog-3.2.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.152751 datafog-3.2.0b1/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b1/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6916 2024-05-13 18:39:53.152484 datafog-3.2.0b1/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b1/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.150961 datafog-3.2.0b1/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 14:39:02.000000 datafog-3.2.0b1/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      150 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2969 2024-05-13 18:39:10.000000 datafog-3.2.0b1/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.152118 datafog-3.2.0b1/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6916 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      201 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 18:39:53.000000 datafog-3.2.0b1/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 18:39:53.152807 datafog-3.2.0b1/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1935 2024-05-13 18:39:10.000000 datafog-3.2.0b1/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:39:53.151863 datafog-3.2.0b1/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b1/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153817 datafog-3.2.0b2/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b2/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 18:57:19.153695 datafog-3.2.0b2/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b2/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.152418 datafog-3.2.0b2/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 18:56:44.000000 datafog-3.2.0b2/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      150 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2969 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153202 datafog-3.2.0b2/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      167 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 18:57:19.153864 datafog-3.2.0b2/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1939 2024-05-13 18:57:03.000000 datafog-3.2.0b2/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153319 datafog-3.2.0b2/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b2/tests/test_main.py
```

### Comparing `datafog-3.2.0b1/LICENSE` & `datafog-3.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b1/PKG-INFO` & `datafog-3.2.0b2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b1
+Version: 3.2.0b2
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast==0.0.0
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: pyspark==3.4.1
-Requires-Dist: pydantic==1.10.8
-Requires-Dist: Pillow
-Requires-Dist: sentencepiece
-Requires-Dist: protobuf
-Requires-Dist: pytesseract
-Requires-Dist: aiohttp
-Requires-Dist: asyncio
-Requires-Dist: pytest-asyncio
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -183,7 +169,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b1 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b2 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
-Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: transformers==4.40.1 Requires-
-Dist: torch==2.2.2 Requires-Dist: pyspark==3.4.1 Requires-Dist:
-pydantic==1.10.8 Requires-Dist: Pillow Requires-Dist: sentencepiece Requires-
-Dist: protobuf Requires-Dist: pytesseract Requires-Dist: aiohttp Requires-Dist:
-asyncio Requires-Dist: pytest-asyncio
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.0b1/README.md` & `datafog-3.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b1/datafog/main.py` & `datafog-3.2.0b2/datafog/main.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b1/datafog.egg-info/PKG-INFO` & `datafog-3.2.0b2/datafog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b1
+Version: 3.2.0b2
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast==0.0.0
-Requires-Dist: transformers==4.40.1
-Requires-Dist: torch==2.2.2
-Requires-Dist: pyspark==3.4.1
-Requires-Dist: pydantic==1.10.8
-Requires-Dist: Pillow
-Requires-Dist: sentencepiece
-Requires-Dist: protobuf
-Requires-Dist: pytesseract
-Requires-Dist: aiohttp
-Requires-Dist: asyncio
-Requires-Dist: pytest-asyncio
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -183,7 +169,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b1 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b2 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
-Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: transformers==4.40.1 Requires-
-Dist: torch==2.2.2 Requires-Dist: pyspark==3.4.1 Requires-Dist:
-pydantic==1.10.8 Requires-Dist: Pillow Requires-Dist: sentencepiece Requires-
-Dist: protobuf Requires-Dist: pytesseract Requires-Dist: aiohttp Requires-Dist:
-asyncio Requires-Dist: pytest-asyncio
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.0b1/setup.py` & `datafog-3.2.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b1"
+    return "3.2.0b2"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -28,16 +28,16 @@
     long_description_content_type="text/markdown",
     packages=["datafog"],
     install_requires=[
         "pandas",
         "Requests==2.31.0",
         "spacy==3.4.4",
         "en_spacy_pii_fast==0.0.0",
-        "transformers==4.40.1",
-        "torch==2.2.2",
+        # "transformers==4.40.1",
+        # "torch==2.2.2",
         "pyspark==3.4.1",
         "pydantic==1.10.8",
         "Pillow",
         "sentencepiece",
         "protobuf",
         "pytesseract",
         "aiohttp",
```

### Comparing `datafog-3.2.0b1/tests/test_main.py` & `datafog-3.2.0b2/tests/test_main.py`

 * *Files identical despite different names*

