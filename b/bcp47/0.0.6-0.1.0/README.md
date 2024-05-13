# Comparing `tmp/bcp47-0.0.6.tar.gz` & `tmp/bcp47-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcp47-0.0.6.tar", last modified: Sat May 11 16:11:07 2024, max compression
+gzip compressed data, was "bcp47-0.1.0.tar", last modified: Mon May 13 11:48:52 2024, max compression
```

## Comparing `bcp47-0.0.6.tar` & `bcp47-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 16:11:07.670330 bcp47-0.0.6/
--rw-rw-rw-   0        0        0     1092 2019-09-27 15:01:21.000000 bcp47-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1971 2024-05-11 16:11:07.669329 bcp47-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1553 2020-11-13 13:47:41.000000 bcp47-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 16:11:07.663329 bcp47-0.0.6/bcp47/
--rw-rw-rw-   0        0        0       21 2019-09-27 15:05:49.000000 bcp47-0.0.6/bcp47/__init__.py
--rw-rw-rw-   0        0        0    29094 2024-05-11 16:10:01.000000 bcp47-0.0.6/bcp47/bcp47.py
--rw-rw-rw-   0        0        0     5149 2024-05-11 16:10:01.000000 bcp47-0.0.6/bcp47/generate-bcp47.py
-drwxrwxrwx   0        0        0        0 2024-05-11 16:11:07.668329 bcp47-0.0.6/bcp47.egg-info/
--rw-rw-rw-   0        0        0     1971 2024-05-11 16:11:07.000000 bcp47-0.0.6/bcp47.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-11 16:11:07.000000 bcp47-0.0.6/bcp47.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 16:11:07.000000 bcp47-0.0.6/bcp47.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 16:11:07.000000 bcp47-0.0.6/bcp47.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 16:11:07.670330 bcp47-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-05-11 16:10:25.000000 bcp47-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:48:52.191531 bcp47-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2019-09-27 15:01:21.000000 bcp47-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1971 2024-05-13 11:48:52.190531 bcp47-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1553 2020-11-13 13:47:41.000000 bcp47-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 11:48:52.186531 bcp47-0.1.0/bcp47/
+-rw-rw-rw-   0        0        0       21 2019-09-27 15:05:49.000000 bcp47-0.1.0/bcp47/__init__.py
+-rw-rw-rw-   0        0        0    30150 2024-05-13 11:45:31.000000 bcp47-0.1.0/bcp47/bcp47.py
+-rw-rw-rw-   0        0        0     5278 2024-05-13 11:43:16.000000 bcp47-0.1.0/bcp47/generate-bcp47.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:48:52.189530 bcp47-0.1.0/bcp47.egg-info/
+-rw-rw-rw-   0        0        0     1971 2024-05-13 11:48:51.000000 bcp47-0.1.0/bcp47.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-13 11:48:51.000000 bcp47-0.1.0/bcp47.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:48:51.000000 bcp47-0.1.0/bcp47.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 11:48:51.000000 bcp47-0.1.0/bcp47.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:48:52.191531 bcp47-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-05-13 11:46:13.000000 bcp47-0.1.0/setup.py
```

### Comparing `bcp47-0.0.6/LICENSE.txt` & `bcp47-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcp47-0.0.6/PKG-INFO` & `bcp47-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcp47
-Version: 0.0.6
+Version: 0.1.0
 Summary: Language tags made easy
 Home-page: https://github.com/highfestiva/bcp47.py
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bcp47-0.0.6/README.md` & `bcp47-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bcp47-0.0.6/bcp47/bcp47.py` & `bcp47-0.1.0/bcp47/bcp47.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
     "Basque - Spain": "eu-ES",
     "Belarusian": "be",
     "Belarusian - Belarus": "be-BY",
     "Bemba": "bem",
     "Bemba - Zambia": "bem-ZM",
     "Bena": "bez",
     "Bena - Tanzania": "bez-TZ",
+    "Bhojpuri": "bho",
+    "Bhojpuri (Devanagari)": "bho-Deva",
+    "Bhojpuri (Devanagari) - India": "bho-Deva-IN",
     "Blin": "byn",
     "Blin - Eritrea": "byn-ER",
     "Bodo": "brx",
     "Bodo - India": "brx-IN",
     "Bosnian (Cyrillic)": "bs-Cyrl",
     "Bosnian (Cyrillic) - Bosnia and Herzegovina": "bs-Cyrl-BA",
     "Bosnian (Latin)": "bs",
@@ -124,14 +127,17 @@
     "Chinese (Simplified) - People's Republic of China": "zh-CN",
     "Chinese (Simplified) - Singapore": "zh-SG",
     "Chinese (Traditional)": "zh-Hant",
     "Chinese (Traditional) - Hong Kong S.A.R.": "zh-HK",
     "Chinese (Traditional) - Macao S.A.R.": "zh-MO",
     "Chinese (Traditional) - Taiwan": "zh-TW",
     "Church Slavic - Russia": "cu-RU",
+    "Chuvash": "cv",
+    "Chuvash (Cyrillic)": "cv-Cyrl",
+    "Chuvash (Cyrillic) - Russia": "cv-Cyrl-RU",
     "Congo Swahili": "swc",
     "Congo Swahili - Congo DRC": "swc-CD",
     "Cornish": "kw",
     "Cornish - United Kingdom": "kw-GB",
     "Corsican": "co",
     "Corsican - France": "co-FR",
     "Croatian": "hr",
@@ -209,14 +215,15 @@
     "English - Kiribati": "en-KI",
     "English - Lesotho": "en-LS",
     "English - Liberia": "en-LR",
     "English - Macao SAR": "en-MO",
     "English - Madagascar": "en-MG",
     "English - Malawi": "en-MW",
     "English - Malaysia": "en-MY",
+    "English - Maldives": "en-MV",
     "English - Malta": "en-MT",
     "English - Marshall Islands": "en-MH",
     "English - Mauritius": "en-MU",
     "English - Micronesia": "en-FM",
     "English - Montserrat": "en-MS",
     "English - Namibia": "en-NA",
     "English - Nauru": "en-NR",
@@ -373,25 +380,30 @@
     "Greenlandic - Greenland": "kl-GL",
     "Guarani": "gn",
     "Guarani - Paraguay": "gn-PY",
     "Gujarati": "gu",
     "Gujarati - India": "gu-IN",
     "Gusii": "guz",
     "Gusii - Kenya": "guz-KE",
+    "Haryanvi": "bgc",
+    "Haryanvi (Devanagari)": "bgc-Deva",
+    "Haryanvi (Devanagari) - India": "bgc-Deva-IN",
     "Hausa (Latin)": "ha",
     "Hausa (Latin), Latn": "ha-Latn",
     "Hausa (Latin) - Ghana": "ha-Latn-GH",
     "Hausa (Latin) - Niger": "ha-Latn-NE",
     "Hausa (Latin) - Nigeria": "ha-Latn-NG",
     "Hawaiian": "haw",
     "Hawaiian - United States": "haw-US",
     "Hebrew": "he",
     "Hebrew - Israel": "he-IL",
     "Hindi": "hi",
     "Hindi - India": "hi-IN",
+    "Hindi (Latin)": "hi-Latn",
+    "Hindi (Latin) - India": "hi-Latn-IN",
     "Hungarian": "hu",
     "Hungarian - Hungary": "hu-HU",
     "Icelandic": "is",
     "Icelandic - Iceland": "is-IS",
     "Igbo": "ig",
     "Igbo - Nigeria": "ig-NG",
     "Indonesian": "id",
@@ -418,14 +430,17 @@
     "Javanese (Latin) - Indonesia": "jv-Latn-ID",
     "Jola-Fonyi": "dyo",
     "Jola-Fonyi - Senegal": "dyo-SN",
     "Kabuverdianu": "kea",
     "Kabuverdianu - Cabo Verde": "kea-CV",
     "Kabyle": "kab",
     "Kabyle - Algeria": "kab-DZ",
+    "Kaingang": "kgp",
+    "Kaingang (Latin)": "kgp-Latn",
+    "Kaingang (Latin) - Brazil": "kgp-Latn-BR",
     "Kako": "kkj",
     "Kako - Cameroon": "kkj-CM",
     "Kalenjin": "kln",
     "Kalenjin - Kenya": "kln-KE",
     "Kamba": "kam",
     "Kamba - Kenya": "kam-KE",
     "Kannada": "kn",
@@ -544,14 +559,19 @@
     "Nepali": "ne",
     "Nepali - India": "ne-IN",
     "Nepali - Nepal": "ne-NP",
     "Ngiemboon": "nnh",
     "Ngiemboon - Cameroon": "nnh-CM",
     "Ngomba": "jgo",
     "Ngomba - Cameroon": "jgo-CM",
+    "Nheengatu": "yrl",
+    "Nheengatu (Latin)": "yrl-Latn",
+    "Nheengatu (Latin) - Brazil": "yrl-Latn-BR",
+    "Nheengatu (Latin) - Colombia": "yrl-Latn-CO",
+    "Nheengatu (Latin) - Venezuela": "yrl-Latn-VE",
     "Northern Luri - Iraq": "lrc-IQ",
     "Northern Luri - Iran": "lrc-IR",
     "North Ndebele": "nd",
     "North Ndebele - Zimbabwe": "nd-ZW",
     "Norwegian (Bokmal)": "no",
     "Norwegian (Bokmal), nb": "nb",
     "Norwegian (Bokmal) - Norway": "nb-NO",
@@ -561,14 +581,15 @@
     "Nuer": "nus",
     "Nuer - Sudan": "nus-SD",
     "Nuer - South Sudan": "nus-SS",
     "Nyankole": "nyn",
     "Nyankole - Uganda": "nyn-UG",
     "Occitan": "oc",
     "Occitan - France": "oc-FR",
+    "Occitan - Spain": "oc-ES",
     "Odia": "or",
     "Odia - India": "or-IN",
     "Oromo": "om",
     "Oromo - Ethiopia": "om-ET",
     "Oromo - Kenya": "om-KE",
     "Ossetian": "os",
     "Ossetian - Cyrillic, Georgia": "os-GE",
@@ -602,14 +623,17 @@
     "Punjabi, Arab": "pa-Arab",
     "Punjabi - India": "pa-IN",
     "Punjabi - Islamic Republic of Pakistan": "pa-Arab-PK",
     "Quechua": "quz",
     "Quechua - Bolivia": "quz-BO",
     "Quechua - Ecuador": "quz-EC",
     "Quechua - Peru": "quz-PE",
+    "Rajasthani": "raj",
+    "Rajasthani (Devanagari)": "raj-Deva",
+    "Rajasthani (Devanagari) - India": "raj-Deva-IN",
     "Ripuarian": "ksh",
     "Ripuarian - Germany": "ksh-DE",
     "Romanian": "ro",
     "Romanian - Moldova": "ro-MD",
     "Romanian - Romania": "ro-RO",
     "Romansh": "rm",
     "Romansh - Switzerland": "rm-CH",
@@ -648,14 +672,17 @@
     "Sami (Southern) - Sweden": "sma-SE",
     "Sango": "sg",
     "Sango - Central African Republic": "sg-CF",
     "Sangu": "sbp",
     "Sangu - Tanzania": "sbp-TZ",
     "Sanskrit": "sa",
     "Sanskrit - India": "sa-IN",
+    "Sardinian": "sc",
+    "Sardinian (Latin)": "sc-Latn",
+    "Sardinian (Latin) - Italy": "sc-Latn-IT",
     "Scottish Gaelic": "gd",
     "Scottish Gaelic - United Kingdom": "gd-GB",
     "Sena": "seh",
     "Sena - Mozambique": "seh-MZ",
     "Serbian (Cyrillic)": "sr-Cyrl",
     "Serbian (Cyrillic) - Bosnia and Herzegovina": "sr-Cyrl-BA",
     "Serbian (Cyrillic) - Montenegro": "sr-Cyrl-ME",
```

### Comparing `bcp47-0.0.6/bcp47/generate-bcp47.py` & `bcp47-0.1.0/bcp47/generate-bcp47.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 # coding=utf-8
 
+import bisect
+import json
 from PyPDF2 import PdfReader
 import os
 import requests
 
 
 url = 'https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-LCID/[MS-LCID].pdf'
 language_markers = [' Windows ', ' Release ']
-bad_markers = ['release:', 'operating', 'server', 'first', 'supported']
+bad_markers = ['release:', 'operating', 'server', 'first', 'supported', ' elk ', 'LCID support']
 join_markers = ['Pseudo', 'Standard']
 languages = set()
 countries = set()
 
 
 def is_language_line(phrase):
     return any(lm in phrase for lm in language_markers) and not any(bm in phrase.lower() for bm in bad_markers)
@@ -60,14 +62,16 @@
         country = words[1].replace(' -', '-')
         tag = words[3]
     else:
         assert False, f'unknown phrase "{phrase}", {words}'
     lang,country = cleanup(lang),cleanup(country)
     if tag:
         tag = tag.replace(' ', '')
+        if tag.endswith(','):
+            tag = tag[:-1]
     # print(f'"{phrase}", {words}') # debug
     languages.add(lang)
     countries.add(country)
     name = f'{lang} - {country}' if country else lang
     return name,tag
 
 
@@ -129,9 +133,10 @@
 name_tag = [] # keeps name+tag tuples
 with open('.buffer.pdf', 'rb') as r:
     reader = PdfReader(r)
     for page in reader.pages:
         phrases = page.extract_text().splitlines()
         phrases = join_phrases(phrases)
         name_tag += generate_page(phrases)
+assert name_tag
 write_output(name_tag)
 print('file generation complete')
```

### Comparing `bcp47-0.0.6/bcp47.egg-info/PKG-INFO` & `bcp47-0.1.0/bcp47.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcp47
-Version: 0.0.6
+Version: 0.1.0
 Summary: Language tags made easy
 Home-page: https://github.com/highfestiva/bcp47.py
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bcp47-0.0.6/setup.py` & `bcp47-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='bcp47',
-    version='0.0.6',
+    version='0.1.0',
     author='Jonas Byström',
     author_email='highfestiva@gmail.com',
     description='Language tags made easy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/highfestiva/bcp47.py',
     packages=['bcp47'],
```

