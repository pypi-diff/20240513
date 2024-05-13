# Comparing `tmp/anemone_daisy_maker-1.55.6.tar.gz` & `tmp/anemone_daisy_maker-1.55.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.55.6.tar", last modified: Sun May 12 18:45:11 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.55.7.tar", last modified: Sun May 12 19:02:46 2024, max compression
```

## Comparing `anemone_daisy_maker-1.55.6.tar` & `anemone_daisy_maker-1.55.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 18:45:11.524939 anemone_daisy_maker-1.55.6/
--rw-r--r--   0 silbrown   (501) staff       (20)     6808 2024-05-12 18:45:11.524431 anemone_daisy_maker-1.55.6/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 18:45:11.520429 anemone_daisy_maker-1.55.6/anemone/
--rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 18:45:11.523701 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)     6808 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      308 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/requires.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 18:45:11.000000 anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 18:45:11.525041 anemone_daisy_maker-1.55.6/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)     7184 2024-05-12 18:44:25.000000 anemone_daisy_maker-1.55.6/setup.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 19:02:46.777600 anemone_daisy_maker-1.55.7/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6915 2024-05-12 19:02:46.777149 anemone_daisy_maker-1.55.7/PKG-INFO
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 19:02:46.772558 anemone_daisy_maker-1.55.7/anemone/
+-rw-r--r--   0 silbrown   (501) staff       (20)    70142 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone/__init__.py
+-rw-r--r--   0 silbrown   (501) staff       (20)       33 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone/__main__.py
+drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-12 19:02:46.776250 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/
+-rw-r--r--   0 silbrown   (501) staff       (20)     6915 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-r--r--   0 silbrown   (501) staff       (20)      308 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/requires.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-12 19:02:46.000000 anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/top_level.txt
+-rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-12 19:02:46.777698 anemone_daisy_maker-1.55.7/setup.cfg
+-rw-r--r--   0 silbrown   (501) staff       (20)     1073 2024-05-12 19:02:39.000000 anemone_daisy_maker-1.55.7/setup.py
```

### Comparing `anemone_daisy_maker-1.55.6/PKG-INFO` & `anemone_daisy_maker-1.55.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.55.6
+Version: 1.55.7
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: mutagen
 
 
+Anemone DAISY maker
+-----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
+(also mirrored at http://ssb22.gitlab.io/indexer/anemone.html just in case)
 
-Anemone is a Python 3 module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
-All files are placed on the command line if running with -m, or in parameters if you're calling Anemone as a module, and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
+All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
-## Behaviour of DAISY readers in 2024
+### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
 
 * EDRLab Thorium Reader (Windows, Mac and GNU/Linux): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  Still works in very large books but loading is slow.
 
 * Dolphin EasyReader 10 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened.  Very large (1 GB+) books can cause the program to crash when Search is used.
 
-* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `--mp3-recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
+* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `mp3-recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
 
 * HumanWare Brailliant: does not show text if there is audio (hopefully it can still be used for navigation) in both Daisy 2 and Daisy 3
 
 * Pronto Notetaker: ZIP needs to be unpacked to a “Daisy” folder on SD or USB, and the device just plays the audio; tested only with Daisy 2
 
-* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use `--mp3-recode`; tested only with Daisy 2 but the documentation says Daisy 3 should work
+* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use mp3-recode; tested only with Daisy 2 but the documentation says Daisy 3 should work
 
 * HumanWare Victor Reader Stream: ZIP needs to be unpacked, either to the top level of a USB device, or into a subfolder of a `$VRDTB` folder on the SD card (different books will be listed alphabetically).  If it's unpacked at the top level of the SD card, the device can still play the MP3s and allow track or time based navigation but not section navigation, so you should use either the folder structure of the SD card or else a USB device.  If correctly set up then audio plays and device can navigate by section.  Tested with both Daisy 2 and Daisy 3.
 
 * HumanWare Victor Reader Stratus4: When unpacking the ZIP to CD, please ensure that your CD writer does *not* create a *folder* with the same name as the ZIP: this default behaviour of Microsoft Windows does *not* result in a valid Daisy CD.  The individual *files* of the ZIP need to be written to the *top level* of the CD, *not* to a folder on it.  Otherwise, the Stratus4 will not recognise the CD as a Daisy CD and will just play the MP3s, resulting in only time and track based navigation being available.  Tested with both Daisy 2 and Daisy 3.
 
 * HIMS QBraille XL: can display the text (after opening with Space and Enter); does not play audio; tested only with Daisy 2
 
 * Daisy Consortium Simply Reading 3 (app available for Android 7 and below): is able to open the ZIP and play the audio while highlighting the paragraphs in a 'full audio plus full text' book, although fonts for some languages might be missing on earlier Android devices
 
-* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `--daisy3` option to produce it directly.
+* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `daisy3` option to produce it directly.
 
-# Copyright and Trademarks
+Copyright and Trademarks
+----------------------
 
 © Silas S. Brown, licensed under Apache 2.
 
+
 * Apache is a registered trademark of The Apache Software Foundation.
 
+
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
+
 * Windows is a registered trademark of Microsoft Corp.
 
 * Any other trademarks I mentioned without realising are trademarks of their respective holders.
```

### Comparing `anemone_daisy_maker-1.55.6/anemone/__init__.py` & `anemone_daisy_maker-1.55.7/anemone/__init__.py`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.55.6/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.55.7/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 Metadata-Version: 2.1
 Name: anemone_daisy_maker
-Version: 1.55.6
+Version: 1.55.7
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: mutagen
 
 
+Anemone DAISY maker
+-----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
+(also mirrored at http://ssb22.gitlab.io/indexer/anemone.html just in case)
 
-Anemone is a Python 3 module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce one of two different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
-All files are placed on the command line if running with -m, or in parameters if you're calling Anemone as a module, and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
+All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
-## Behaviour of DAISY readers in 2024
+### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
 
 * EDRLab Thorium Reader (Windows, Mac and GNU/Linux): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  Still works in very large books but loading is slow.
 
 * Dolphin EasyReader 10 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened.  Very large (1 GB+) books can cause the program to crash when Search is used.
 
-* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `--mp3-recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
+* JAWS FSReader 3 (Windows): is able to play audio while highlighting paragraphs in both Daisy 2 and Daisy 3, but ZIP needs to be unpacked separately and NCC or OPF file opened; may work better without JAWS running; synchronisation with audio seems to require `mp3-recode`; images are not scaled to fit; tested working with a Braille display and audio speed changes; not tested with very large books (1GB+)
 
 * HumanWare Brailliant: does not show text if there is audio (hopefully it can still be used for navigation) in both Daisy 2 and Daisy 3
 
 * Pronto Notetaker: ZIP needs to be unpacked to a “Daisy” folder on SD or USB, and the device just plays the audio; tested only with Daisy 2
 
-* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use `--mp3-recode`; tested only with Daisy 2 but the documentation says Daisy 3 should work
+* US Library of Congress NLS Player: unpack the ZIP onto a blank USB stick of capacity 4 GB or less—plays; navigation works if you use mp3-recode; tested only with Daisy 2 but the documentation says Daisy 3 should work
 
 * HumanWare Victor Reader Stream: ZIP needs to be unpacked, either to the top level of a USB device, or into a subfolder of a `$VRDTB` folder on the SD card (different books will be listed alphabetically).  If it's unpacked at the top level of the SD card, the device can still play the MP3s and allow track or time based navigation but not section navigation, so you should use either the folder structure of the SD card or else a USB device.  If correctly set up then audio plays and device can navigate by section.  Tested with both Daisy 2 and Daisy 3.
 
 * HumanWare Victor Reader Stratus4: When unpacking the ZIP to CD, please ensure that your CD writer does *not* create a *folder* with the same name as the ZIP: this default behaviour of Microsoft Windows does *not* result in a valid Daisy CD.  The individual *files* of the ZIP need to be written to the *top level* of the CD, *not* to a folder on it.  Otherwise, the Stratus4 will not recognise the CD as a Daisy CD and will just play the MP3s, resulting in only time and track based navigation being available.  Tested with both Daisy 2 and Daisy 3.
 
 * HIMS QBraille XL: can display the text (after opening with Space and Enter); does not play audio; tested only with Daisy 2
 
 * Daisy Consortium Simply Reading 3 (app available for Android 7 and below): is able to open the ZIP and play the audio while highlighting the paragraphs in a 'full audio plus full text' book, although fonts for some languages might be missing on earlier Android devices
 
-* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `--daisy3` option to produce it directly.
+* DAISY Pipeline (2023): Please do not use this to convert an Anemone-produced Daisy 2 book to Daisy 3.  The resulting Daisy 3 is not likely to play on anything.  If Daisy 3 is required, use Anemone's `daisy3` option to produce it directly.
 
-# Copyright and Trademarks
+Copyright and Trademarks
+----------------------
 
 © Silas S. Brown, licensed under Apache 2.
 
+
 * Apache is a registered trademark of The Apache Software Foundation.
 
+
 * MP3 is a trademark that was registered in Europe to Hypermedia GmbH Webcasting but I was unable to confirm its current holder.
 
 * Python is a trademark of the Python Software Foundation.
 
+
 * Windows is a registered trademark of Microsoft Corp.
 
 * Any other trademarks I mentioned without realising are trademarks of their respective holders.
```

