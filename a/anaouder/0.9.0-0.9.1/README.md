# Comparing `tmp/anaouder-0.9.0.tar.gz` & `tmp/anaouder-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaouder-0.9.0.tar", last modified: Sat Mar  9 17:15:28 2024, max compression
+gzip compressed data, was "anaouder-0.9.1.tar", last modified: Mon May 13 11:55:17 2024, max compression
```

## Comparing `anaouder-0.9.0.tar` & `anaouder-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.472843 anaouder-0.9.0/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     1468 2024-03-09 16:54:14.000000 anaouder-0.9.0/CHANGELOG.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7001 2024-03-09 17:15:28.472843 anaouder-0.9.0/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5814 2024-01-04 10:16:16.000000 anaouder-0.9.0/README-fr.md
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5274 2024-01-04 10:16:16.000000 anaouder-0.9.0/README.md
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.464843 anaouder-0.9.0/anaouder/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.0/anaouder/__init__.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     9538 2024-03-09 15:01:47.000000 anaouder-0.9.0/anaouder/adskrivan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.468843 anaouder-0.9.0/anaouder/asr/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.0/anaouder/asr/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.0/anaouder/asr/inorm_units.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3698 2024-03-09 16:05:14.000000 anaouder-0.9.0/anaouder/asr/models.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6126 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/asr/post_processing.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/asr/postproc_sub.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5097 2024-03-09 16:07:09.000000 anaouder-0.9.0/anaouder/asr/recognizer.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.468843 anaouder-0.9.0/anaouder/audio/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5482 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/audio/__init__.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.468843 anaouder-0.9.0/anaouder/dicts/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.0/anaouder/dicts/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/acronyms.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/corrected_tokens.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/noun_f.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/noun_m.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/proper_nouns_phon.tsv
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.0/anaouder/dicts/standard_tokens.tsv
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.0/anaouder/istitlan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.0/anaouder/linennan.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.0/anaouder/mikro.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.0/anaouder/normalizan.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.468843 anaouder-0.9.0/anaouder/text/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.0/anaouder/text/__init__.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.0/anaouder/text/definitions.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.0/anaouder/text/inverse_normalizer.py
--rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.0/anaouder/text/normalizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.0/anaouder/text/tokenizer.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.0/anaouder/text/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5442 2023-11-10 20:39:34.000000 anaouder-0.9.0/anaouder/utils.py
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-03-05 10:58:23.000000 anaouder-0.9.0/anaouder/version.py
-drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-03-09 17:15:28.468843 anaouder-0.9.0/anaouder.egg-info/
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     7001 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/PKG-INFO
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      979 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/SOURCES.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/dependency_links.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      189 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/entry_points.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/requires.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-03-09 17:15:28.000000 anaouder-0.9.0/anaouder.egg-info/top_level.txt
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-03-09 17:15:28.472843 anaouder-0.9.0/setup.cfg
--rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2080 2024-03-09 17:01:43.000000 anaouder-0.9.0/setup.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2018 2024-05-13 11:38:08.000000 anaouder-0.9.1/CHANGELOG.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6754 2024-05-13 11:55:17.480837 anaouder-0.9.1/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5609 2024-05-13 11:51:35.000000 anaouder-0.9.1/README-fr.md
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5083 2024-05-13 11:52:12.000000 anaouder-0.9.1/README.md
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.476836 anaouder-0.9.1/anaouder/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      180 2023-10-21 14:25:36.000000 anaouder-0.9.1/anaouder/__init__.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11650 2024-05-13 11:54:43.000000 anaouder-0.9.1/anaouder/adskrivan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/asr/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        0 2023-05-20 06:43:27.000000 anaouder-0.9.1/anaouder/asr/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       74 2023-05-20 06:43:27.000000 anaouder-0.9.1/anaouder/asr/inorm_units.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3698 2024-03-09 16:05:14.000000 anaouder-0.9.1/anaouder/asr/models.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6255 2024-05-13 10:09:57.000000 anaouder-0.9.1/anaouder/asr/post_processing.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2797 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/asr/postproc_sub.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4993 2024-05-13 10:13:05.000000 anaouder-0.9.1/anaouder/asr/recognizer.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/audio/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5482 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/audio/__init__.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/dicts/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2769 2023-10-21 14:25:36.000000 anaouder-0.9.1/anaouder/dicts/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3263 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/acronyms.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5601 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/corrected_tokens.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3328 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/noun_f.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4439 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/noun_m.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18304 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/proper_nouns_phon.tsv
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3415 2024-03-05 10:58:22.000000 anaouder-0.9.1/anaouder/dicts/standard_tokens.tsv
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)      206 2023-11-30 08:14:18.000000 anaouder-0.9.1/anaouder/istitlan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    11135 2024-03-09 15:05:10.000000 anaouder-0.9.1/anaouder/linennan.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     3688 2024-03-09 16:46:02.000000 anaouder-0.9.1/anaouder/mikro.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)     1185 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/normalizan.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder/text/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3446 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/text/__init__.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     4275 2023-05-23 13:01:08.000000 anaouder-0.9.1/anaouder/text/definitions.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    13824 2023-11-10 20:39:34.000000 anaouder-0.9.1/anaouder/text/inverse_normalizer.py
+-rwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)    10825 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/normalizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)    18371 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/tokenizer.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     3687 2023-10-21 14:25:37.000000 anaouder-0.9.1/anaouder/text/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     5396 2024-05-13 08:15:45.000000 anaouder-0.9.1/anaouder/utils.py
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       17 2024-05-13 09:34:17.000000 anaouder-0.9.1/anaouder/version.py
+drwxrwxr-x   0 gweltaz   (1000) gweltaz   (1000)        0 2024-05-13 11:55:17.480837 anaouder-0.9.1/anaouder.egg-info/
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     6754 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/PKG-INFO
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      979 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        1 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)      189 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/entry_points.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       73 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/requires.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)        9 2024-05-13 11:55:17.000000 anaouder-0.9.1/anaouder.egg-info/top_level.txt
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)       38 2024-05-13 11:55:17.480837 anaouder-0.9.1/setup.cfg
+-rw-rw-r--   0 gweltaz   (1000) gweltaz   (1000)     2080 2024-03-09 17:01:43.000000 anaouder-0.9.1/setup.py
```

### Comparing `anaouder-0.9.0/PKG-INFO` & `anaouder-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.0
+Version: 0.9.1
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
 Description: [![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
         
         # Anaouder mouezh e brezhoneg gant Vosk
         
         [Version française](https://github.com/gweltou/vosk-br/blob/main/README-fr.md)
         
-        Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant un donezon :
+        Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant ur roadenn :
         [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
         
-        Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://abp.fritzsch.net/), savet gant Philippe Argouarch.
+        Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://translate.bzh/), savet gant Philippe Argouarch.
         
         ## Petra eo ?
         
         Un anaouder mouezh emgefre, diazezet war [Vosk](https://github.com/alphacep/vosk-api).\
         Gantañ e c'heller adskrivañ komzoù e brezhoneg (**Son -> Skrid**) dre ur mikro e amzer real pe diouzh restroù son.
         
         Un nebeut perzhioù dedennus :
         
         * **Skañv**. Pouezh ar model a zo dindan 100 Mo ha treiñ a ra war ur bern mekanikoù : urzhiataerioù **hep GPU**, RaspberryPi, hezoug Android...
         * **Prim**. Gallout a reer adskrivañ ar son e **amzer real**, memes gant un urzhiataer kozh, pe primoc'h c'hoazh gant dafar nevesoc'h.
         * **Lec'hel**. Ezhomm ebet eus an Internet. Ho mouezh hag **ho data a chomo war ho penveg**, ha tretet e vint gant ho penveg nemetken. Kudenn surentez ebet liammet d'an treuzkas dre rouedad ha gwelloc'h a-fed ekologel.
         * **Digoust ha dieub**. Gellout a reoc'h azasaat ar meziant d'hoc'h ezhommoù pe enframmañ anezhañ e meziantoù all.
         
-        Dalc'hoù 'zo siwazh :
-        
-        * Poentadur ebet.
-        * Kizidig d'an trouzioù endro.
-        * Fall war ur bern pouezioù-mouezh c'hoazh.
-        * Ret eo komz sklaer ha goustadik.
-        
         Gwellaet e vo efedusted an anaouder tamm-ha-tamm, gant ma vo kavet roadennoù mouezh adskrivet.\
         Ul lisañs dieub (doare [Creative Commons](https://creativecommons.org/licenses/)) a aotrefe eskemm ar roadennoù-se en un doare aes.
         
+        Deuit e darempred ganin m'ho peus c'hoant kemer perzh !
+        
         ## Staliañ
         
         Goude bezañ bet staliet [Python3](https://www.python.org/downloads/) e c'heller staliañ an anaouder dre an terminal :
         
         ```bash
         pip install anaouder
         ```
@@ -102,19 +97,17 @@
         istitlan RESTR_SON_PE_VIDEO -o istitloù.srt
         ```
         
         An oberiadur-se a gemero kalzig a amzer (hervez padelezh an teuliad son). Klaskit gant un teul film berr da gentañ !
         
         https://user-images.githubusercontent.com/10166907/213805292-63becbe2-ffb5-492f-9bac-1330c4b2d07d.mp4
         
-        *Setu disoc'h an istitloù emgefre, hep cheñch netra. Kollet eo buan pa vez sonnerez...*
-        
         ## Implijout gant meziantoù all
         
-        *N'eo ket aliet dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
+        *N'eo ket aliet, dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
         
         Ar model noazh a c'hellit kavout en dosser `anaouder/models` pe dre al liamm [releases](https://github.com/gweltou/vosk-br/releases).
         
         ### Audapolis
         
         M'ho peus c'hoant implijout ar model gant ur etrefas grafikel e c'hellit mont da sellet ar raktres [Audapolis](https://github.com/bugbakery/audapolis).
```

### Comparing `anaouder-0.9.0/README-fr.md` & `anaouder-0.9.1/README-fr.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,28 @@
 [E brezhoneg](./README.md)
 
 Reconnaissance vocale pour le breton avec Vosk.
 
 Ce projet est développé bénévolement. Vous pouvez le soutenir par un don :
 [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
 
-Une [version en ligne](https://abp.fritzsch.net/), développée par Philippe Argouarch, est également disponible.
+Une [version en ligne](https://translate.bzh/), développée par Philippe Argouarch, est également disponible.
 
 ## Présentation
 
 Modèle de reconnaissance vocale (*speech-to-text*) entraîné avec le framework [Kaldi](https://www.kaldi-asr.org/), au format [Vosk](https://github.com/alphacep/vosk-api).\
 Il est accompagné de scripts permettant la retranscription automatique de fichiers audio et video, l'alignement texte/son pour la création de sous-titres, ou encore l'inférence en temps réel à l'aide d'un microphone.
 
 Principaux avantages :
 
 * **Léger**. Les modèles Vosk pèsent moins de 100 Mo et peuvent tourner sur une large gamme d'appareils : ordinateurs **sans GPU**, RaspberryPi, smartphone Android...
 * **Rapide**. L'inférence se fait en **temps réel**, même sur une machine un peu datée.
 * **Local**. Fonctionne sans connexion internet. Vos données restent donc sur votre appareil.
 * **Libre et gratuit**. La licence MIT vous permet de modifier le logiciel et de l'intégrer dans d'autres applications.
 
-Il y a toutefois des inconvénients :
-
-* Sensible au bruit ambiant.
-* Certains accents régionaux sont encore mal reconnus.
-* Nécessite de parler lentement et distinctement.
-* Absence de ponctuation.
-
 Le nombre d'heures d'enregistrement audio utilisé pour entraîner le modèle est relativement faible mais progresse peu à peu.
 En dehors du projet [Common Voice](https://commonvoice.mozilla.org/br) de Mozilla, les enregistrements retranscrits [libres de droit](https://creativecommons.org/licenses/) sont rares pour le breton. Toute aide sur ce terrain sera la bienvenue !
 
 ## Installation
 
 Les scripts nécessitent l'installation de [Python3](https://www.python.org/downloads/). L'installation du module de reconnaissance vocale se fera ensuite dans un terminal, en exécutant la commande suivante :
```

### Comparing `anaouder-0.9.0/README.md` & `anaouder-0.9.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 [![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
 
 # Anaouder mouezh e brezhoneg gant Vosk
 
 [Version française](https://github.com/gweltou/vosk-br/blob/main/README-fr.md)
 
-Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant un donezon :
+Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant ur roadenn :
 [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
 
-Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://abp.fritzsch.net/), savet gant Philippe Argouarch.
+Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://translate.bzh/), savet gant Philippe Argouarch.
 
 ## Petra eo ?
 
 Un anaouder mouezh emgefre, diazezet war [Vosk](https://github.com/alphacep/vosk-api).\
 Gantañ e c'heller adskrivañ komzoù e brezhoneg (**Son -> Skrid**) dre ur mikro e amzer real pe diouzh restroù son.
 
 Un nebeut perzhioù dedennus :
 
 * **Skañv**. Pouezh ar model a zo dindan 100 Mo ha treiñ a ra war ur bern mekanikoù : urzhiataerioù **hep GPU**, RaspberryPi, hezoug Android...
 * **Prim**. Gallout a reer adskrivañ ar son e **amzer real**, memes gant un urzhiataer kozh, pe primoc'h c'hoazh gant dafar nevesoc'h.
 * **Lec'hel**. Ezhomm ebet eus an Internet. Ho mouezh hag **ho data a chomo war ho penveg**, ha tretet e vint gant ho penveg nemetken. Kudenn surentez ebet liammet d'an treuzkas dre rouedad ha gwelloc'h a-fed ekologel.
 * **Digoust ha dieub**. Gellout a reoc'h azasaat ar meziant d'hoc'h ezhommoù pe enframmañ anezhañ e meziantoù all.
 
-Dalc'hoù 'zo siwazh :
-
-* Poentadur ebet.
-* Kizidig d'an trouzioù endro.
-* Fall war ur bern pouezioù-mouezh c'hoazh.
-* Ret eo komz sklaer ha goustadik.
-
 Gwellaet e vo efedusted an anaouder tamm-ha-tamm, gant ma vo kavet roadennoù mouezh adskrivet.\
 Ul lisañs dieub (doare [Creative Commons](https://creativecommons.org/licenses/)) a aotrefe eskemm ar roadennoù-se en un doare aes.
 
+Deuit e darempred ganin m'ho peus c'hoant kemer perzh !
+
 ## Staliañ
 
 Goude bezañ bet staliet [Python3](https://www.python.org/downloads/) e c'heller staliañ an anaouder dre an terminal :
 
 ```bash
 pip install anaouder
 ```
@@ -94,19 +89,17 @@
 istitlan RESTR_SON_PE_VIDEO -o istitloù.srt
 ```
 
 An oberiadur-se a gemero kalzig a amzer (hervez padelezh an teuliad son). Klaskit gant un teul film berr da gentañ !
 
 https://user-images.githubusercontent.com/10166907/213805292-63becbe2-ffb5-492f-9bac-1330c4b2d07d.mp4
 
-*Setu disoc'h an istitloù emgefre, hep cheñch netra. Kollet eo buan pa vez sonnerez...*
-
 ## Implijout gant meziantoù all
 
-*N'eo ket aliet dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
+*N'eo ket aliet, dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
 
 Ar model noazh a c'hellit kavout en dosser `anaouder/models` pe dre al liamm [releases](https://github.com/gweltou/vosk-br/releases).
 
 ### Audapolis
 
 M'ho peus c'hoant implijout ar model gant ur etrefas grafikel e c'hellit mont da sellet ar raktres [Audapolis](https://github.com/bugbakery/audapolis).
```

### Comparing `anaouder-0.9.0/anaouder/asr/models.py` & `anaouder-0.9.1/anaouder/asr/models.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/asr/post_processing.py` & `anaouder-0.9.1/anaouder/asr/post_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,20 @@
 
 
 
 def post_process_timecoded(
         tokens: List[dict],
         normalize=False,
         keep_fillers=True) -> List[dict]:
-    """ Apply post-processing on Vosk formatted result (keeping timecodes) """
+    """ Apply post-processing on Vosk formatted result (keeping timecodes)
+
+        Add hypens (-se, -mañ)
+        Common words substitution  (optional)
+        Inverse-normalization      (optional)
+    """
     
     # Verbal fillers removal
     if not keep_fillers:
         parsed = []
         for idx, tok in enumerate(tokens):
             if not tok["word"].lower() in verbal_fillers:
                 parsed.append(tok)
```

### Comparing `anaouder-0.9.0/anaouder/asr/postproc_sub.tsv` & `anaouder-0.9.1/anaouder/asr/postproc_sub.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/asr/recognizer.py` & `anaouder-0.9.1/anaouder/asr/recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             if "result" in result:
                 timecoded_text.extend(result["result"])
         i += 4000
     recognizer.AcceptWaveform(data[i:])
     result = json.loads(recognizer.FinalResult())
     if "result" in result:
         timecoded_text.extend(result["result"])
+    
     return timecoded_text
 
 
 
 def transcribe_file(filepath: str, normalize=False) -> List[str]:
     def format_output(sentence, normalize=False):
         sentence = post_process_text(sentence, normalize)
@@ -113,26 +114,24 @@
             {'word': str, 'start': float, 'end': float, 'conf': float}
         'start' and 'end' keys are in seconds
         'conf' is a normalized confidence score
     """
 
     def format_output(result, normalize=False) -> List[dict]:
         jres = json.loads(result)
+        return jres.get("result", [])
         if not "result" in jres:
             return []
-        words = jres["result"]
-        words = post_process_timecoded(words, normalize)
-        return words
+        return jres["result"]
 
     model = load_model()
     recognizer = KaldiRecognizer(model, 16000)
     recognizer.SetWords(True)
     
     total_duration = get_audiofile_length(filepath)
-    #print(f"Audio file duration: {round(total_duration)} seconds")
     progress_bar = tqdm(total=ceil(total_duration))
     i = 0
     cumul_frames = 0
 
     tokens = []
     with subprocess.Popen(["ffmpeg", "-loglevel", "quiet", "-i",
                                 filepath,
```

### Comparing `anaouder-0.9.0/anaouder/audio/__init__.py` & `anaouder-0.9.1/anaouder/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/__init__.py` & `anaouder-0.9.1/anaouder/dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/acronyms.tsv` & `anaouder-0.9.1/anaouder/dicts/acronyms.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/corrected_tokens.tsv` & `anaouder-0.9.1/anaouder/dicts/corrected_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/noun_f.tsv` & `anaouder-0.9.1/anaouder/dicts/noun_f.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/noun_m.tsv` & `anaouder-0.9.1/anaouder/dicts/noun_m.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/proper_nouns_phon.tsv` & `anaouder-0.9.1/anaouder/dicts/proper_nouns_phon.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/dicts/standard_tokens.tsv` & `anaouder-0.9.1/anaouder/dicts/standard_tokens.tsv`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/linennan.py` & `anaouder-0.9.1/anaouder/linennan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/mikro.py` & `anaouder-0.9.1/anaouder/mikro.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/normalizan.py` & `anaouder-0.9.1/anaouder/normalizan.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/__init__.py` & `anaouder-0.9.1/anaouder/text/__init__.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/definitions.py` & `anaouder-0.9.1/anaouder/text/definitions.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/inverse_normalizer.py` & `anaouder-0.9.1/anaouder/text/inverse_normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/normalizer.py` & `anaouder-0.9.1/anaouder/text/normalizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/tokenizer.py` & `anaouder-0.9.1/anaouder/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/text/utils.py` & `anaouder-0.9.1/anaouder/text/utils.py`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/anaouder/utils.py` & `anaouder-0.9.1/anaouder/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List
 import os
 
 # For eaf (Elan) file conversion
 import datetime, pytz
 from xml.dom import minidom
+
 from anaouder.audio import convert_to_mp3
+from anaouder.version import VERSION
 
 
 
 def list_files_with_extension(ext, rep, recursive=True) -> List[str]:
     file_list = []
     if os.path.isdir(rep):
         for filename in os.listdir(rep):
@@ -32,26 +34,24 @@
 
 
 
 def write_eaf(segments, sentences, audiofile, type="wav"):
     """ Export to eaf (Elan) file """
 
     record_id = os.path.splitext(os.path.abspath(audiofile))[0]
-    #audio_filename = os.path.extsep.join((record_id, 'wav'))
-    # audio_filename = audiofile
     if type == "mp3":
         mp3_file = os.path.extsep.join((record_id, 'mp3'))
         if not os.path.exists(mp3_file):
             convert_to_mp3(audiofile, mp3_file)
         audiofile = mp3_file
 
     doc = minidom.Document()
 
     root = doc.createElement('ANNOTATION_DOCUMENT')
-    root.setAttribute('AUTHOR', 'anaouder (Gweltaz DG)')
+    root.setAttribute('AUTHOR', f'Anaouder {VERSION} (Gweltaz DG)')
     root.setAttribute('DATE', datetime.datetime.now(pytz.timezone('Europe/Paris')).isoformat(timespec='seconds'))
     root.setAttribute('FORMAT', '3.0')
     root.setAttribute('VERSION', '3.0')
     root.setAttribute('xmlns:xsi', 'http://www.w3.org/2001/XMLSchema-instance')
     root.setAttribute('xsi:noNamespaceSchemaLocation', 'http://www.mpi.nl/tools/elan/EAFv3.0.xsd')
     doc.appendChild(root)
```

### Comparing `anaouder-0.9.0/anaouder.egg-info/PKG-INFO` & `anaouder-0.9.1/anaouder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 Metadata-Version: 2.1
 Name: anaouder
-Version: 0.9.0
+Version: 0.9.1
 Summary: Breton language speech-to-text tools
 Home-page: https://github.com/gweltou/vosk-br
 Author: Gweltaz Duval-Guennoc
 Author-email: gweltou@hotmail.com
 License: MIT
 Description: [![pypi version](https://img.shields.io/pypi/v/anaouder)](https://pypi.org/project/anaouder/)
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
         
         # Anaouder mouezh e brezhoneg gant Vosk
         
         [Version française](https://github.com/gweltou/vosk-br/blob/main/README-fr.md)
         
-        Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant un donezon :
+        Diorroet eo ar raktres-se a youl vat. Gallout a rit souten ar raktres gant ur roadenn :
         [![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/gweltou/donate)
         
-        Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://abp.fritzsch.net/), savet gant Philippe Argouarch.
+        Gallout a reer ivez implij ar meziant dre ur [c'hetal Web](https://translate.bzh/), savet gant Philippe Argouarch.
         
         ## Petra eo ?
         
         Un anaouder mouezh emgefre, diazezet war [Vosk](https://github.com/alphacep/vosk-api).\
         Gantañ e c'heller adskrivañ komzoù e brezhoneg (**Son -> Skrid**) dre ur mikro e amzer real pe diouzh restroù son.
         
         Un nebeut perzhioù dedennus :
         
         * **Skañv**. Pouezh ar model a zo dindan 100 Mo ha treiñ a ra war ur bern mekanikoù : urzhiataerioù **hep GPU**, RaspberryPi, hezoug Android...
         * **Prim**. Gallout a reer adskrivañ ar son e **amzer real**, memes gant un urzhiataer kozh, pe primoc'h c'hoazh gant dafar nevesoc'h.
         * **Lec'hel**. Ezhomm ebet eus an Internet. Ho mouezh hag **ho data a chomo war ho penveg**, ha tretet e vint gant ho penveg nemetken. Kudenn surentez ebet liammet d'an treuzkas dre rouedad ha gwelloc'h a-fed ekologel.
         * **Digoust ha dieub**. Gellout a reoc'h azasaat ar meziant d'hoc'h ezhommoù pe enframmañ anezhañ e meziantoù all.
         
-        Dalc'hoù 'zo siwazh :
-        
-        * Poentadur ebet.
-        * Kizidig d'an trouzioù endro.
-        * Fall war ur bern pouezioù-mouezh c'hoazh.
-        * Ret eo komz sklaer ha goustadik.
-        
         Gwellaet e vo efedusted an anaouder tamm-ha-tamm, gant ma vo kavet roadennoù mouezh adskrivet.\
         Ul lisañs dieub (doare [Creative Commons](https://creativecommons.org/licenses/)) a aotrefe eskemm ar roadennoù-se en un doare aes.
         
+        Deuit e darempred ganin m'ho peus c'hoant kemer perzh !
+        
         ## Staliañ
         
         Goude bezañ bet staliet [Python3](https://www.python.org/downloads/) e c'heller staliañ an anaouder dre an terminal :
         
         ```bash
         pip install anaouder
         ```
@@ -102,19 +97,17 @@
         istitlan RESTR_SON_PE_VIDEO -o istitloù.srt
         ```
         
         An oberiadur-se a gemero kalzig a amzer (hervez padelezh an teuliad son). Klaskit gant un teul film berr da gentañ !
         
         https://user-images.githubusercontent.com/10166907/213805292-63becbe2-ffb5-492f-9bac-1330c4b2d07d.mp4
         
-        *Setu disoc'h an istitloù emgefre, hep cheñch netra. Kollet eo buan pa vez sonnerez...*
-        
         ## Implijout gant meziantoù all
         
-        *N'eo ket aliet dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
+        *N'eo ket aliet, dre ma vez kollet un nebeut perzhioù e-keñver ar pezh vez graet gant ar modul `anaouder` : adlakaat ar varennigoù-stag hag amdreiñ an niverennoù da skouer.*
         
         Ar model noazh a c'hellit kavout en dosser `anaouder/models` pe dre al liamm [releases](https://github.com/gweltou/vosk-br/releases).
         
         ### Audapolis
         
         M'ho peus c'hoant implijout ar model gant ur etrefas grafikel e c'hellit mont da sellet ar raktres [Audapolis](https://github.com/bugbakery/audapolis).
```

### Comparing `anaouder-0.9.0/anaouder.egg-info/SOURCES.txt` & `anaouder-0.9.1/anaouder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anaouder-0.9.0/setup.py` & `anaouder-0.9.1/setup.py`

 * *Files identical despite different names*

