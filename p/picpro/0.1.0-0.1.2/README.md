# Comparing `tmp/picpro-0.1.0.tar.gz` & `tmp/picpro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picpro-0.1.0.tar", last modified: Fri Nov 24 20:30:06 2023, max compression
+gzip compressed data, was "picpro-0.1.2.tar", last modified: Mon May 13 10:54:48 2024, max compression
```

## Comparing `picpro-0.1.0.tar` & `picpro-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.588192 picpro-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    17992 2023-11-24 20:28:46.000000 picpro-0.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-11-24 20:28:46.000000 picpro-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3899 2023-11-24 20:30:06.588192 picpro-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2878 2023-11-24 20:28:46.000000 picpro-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.584192 picpro-0.1.0/picpro/
--rw-rw-rw-   0 root         (0) root         (0)     7313 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/ChipInfoEntry.py
--rw-rw-rw-   0 root         (0) root         (0)     6482 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/ChipInfoReader.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/HexFileReader.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/IChipInfoEntry.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/ProgrammingVars.py
--rw-rw-rw-   0 root         (0) root         (0)    18738 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/ProtocolInterface.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.584192 picpro-0.1.0/picpro/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/bin/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    18756 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/bin/picpro.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2023-11-24 20:28:46.000000 picpro-0.1.0/picpro/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.584192 picpro-0.1.0/picpro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3899 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      603 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-11-24 20:30:06.000000 picpro-0.1.0/picpro.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-11-24 20:30:06.588192 picpro-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-11-24 20:28:46.000000 picpro-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.588192 picpro-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 20:28:46.000000 picpro-0.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4039 2023-11-24 20:28:46.000000 picpro-0.1.0/tests/test_ChipInfoReader.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-11-24 20:28:46.000000 picpro-0.1.0/tests/test_chip_data.cid
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.580192 picpro-0.1.0/usr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.584192 picpro-0.1.0/usr/share/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 20:30:06.588192 picpro-0.1.0/usr/share/picpro/
--rw-rw-rw-   0 root         (0) root         (0)   204311 2023-11-24 20:28:46.000000 picpro-0.1.0/usr/share/picpro/chipdata.cid
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    17992 2024-05-13 10:53:14.000000 picpro-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-13 10:53:14.000000 picpro-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-13 10:54:48.240746 picpro-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2024-05-13 10:53:14.000000 picpro-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/picpro/
+-rw-rw-rw-   0 root         (0) root         (0)     7313 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/ChipInfoEntry.py
+-rw-rw-rw-   0 root         (0) root         (0)     6482 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/ChipInfoReader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/HexFileReader.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/IChipInfoEntry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/ProgrammingVars.py
+-rw-rw-rw-   0 root         (0) root         (0)    18738 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/ProtocolInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/picpro/bin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/bin/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21602 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/bin/picpro.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3330 2024-05-13 10:53:14.000000 picpro-0.1.2/picpro/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/picpro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-13 10:54:48.000000 picpro-0.1.2/picpro.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-13 10:54:48.244746 picpro-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2024-05-13 10:53:14.000000 picpro-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 10:53:14.000000 picpro-0.1.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4039 2024-05-13 10:53:14.000000 picpro-0.1.2/tests/test_ChipInfoReader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-05-13 10:53:14.000000 picpro-0.1.2/tests/test_chip_data.cid
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.236746 picpro-0.1.2/usr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.236746 picpro-0.1.2/usr/share/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 10:54:48.240746 picpro-0.1.2/usr/share/picpro/
+-rw-rw-rw-   0 root         (0) root         (0)   204311 2024-05-13 10:53:14.000000 picpro-0.1.2/usr/share/picpro/chipdata.cid
```

### Comparing `picpro-0.1.0/LICENSE` & `picpro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/PKG-INFO` & `picpro-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picpro
-Version: 0.1.0
+Version: 0.1.2
 Summary: picpro a kitsrus PIC CLI programmer
 Home-page: https://github.com/Salamek/picpro
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: LGPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/picpro/releases
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `picpro-0.1.0/README.md` & `picpro-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/ChipInfoEntry.py` & `picpro-0.1.2/picpro/ChipInfoEntry.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/ChipInfoReader.py` & `picpro-0.1.2/picpro/ChipInfoReader.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/HexFileReader.py` & `picpro-0.1.2/picpro/HexFileReader.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/IChipInfoEntry.py` & `picpro-0.1.2/picpro/IChipInfoEntry.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/ProgrammingVars.py` & `picpro-0.1.2/picpro/ProgrammingVars.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/ProtocolInterface.py` & `picpro-0.1.2/picpro/ProtocolInterface.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/bin/picpro.py` & `picpro-0.1.2/picpro/bin/picpro.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 
 Command details:
     program             Program PIC chip.
     verify              Verify PIC flash.
     dump                Dump PIC data as binary.
     erase               Erase PIC.
     chipinfo            Prints chipinfo as JSON in terminal.
+    hexinfo             Prints information about hexfile.
 
 Usage:
     picpro program -p PORT -i HEX_FILE -t PIC_TYPE [--id=PIC_ID] [--fuse=FUSE_NAME:FUSE_VALUE...] [--icsp]
     picpro verify -p PORT -i HEX_FILE -t PIC_TYPE [--icsp]
     picpro erase -p PORT -t PIC_TYPE [--icsp]
     picpro dump <mem_type> -p PORT -o HEX_FILE -t PIC_TYPE [--icsp]
     picpro chipinfo [<PIC_TYPE>]
+    picpro hexinfo <HEX_FILE> <PIC_TYPE>
     picpro (-h | --help)
 
 
 Options:
     --icsp                           Enable ISCP programming.
     --fuse=FUSE_NAME:FUSE_VALUE      Set fuse value directly.
     --id=PIC_ID                      Set PIC id to be programmed in pic.
@@ -187,14 +189,81 @@
     if pic_type:
         data = chip_info_reader.get_chip(pic_type).to_dict()
     else:
         data = {chip_name: entry.to_dict() for chip_name, entry in chip_info_reader.chip_entries.items()}
 
     print(json.dumps(data))
 
+@command()
+def hexinfo() -> None:
+    pic_type = OPTIONS['<PIC_TYPE>']
+    hex_file_name = OPTIONS['<HEX_FILE>']
+
+    # Read hex file.
+    try:
+        hex_file = HexFileReader(hex_file_name)
+    except IOError:
+        print('Unable to find hex file "{}".'.format(hex_file_name))
+        print('Please verify that the file exists and that you have access to it.')
+        return None
+
+        # Get chip info
+    chip_info_filename = find_chip_data()
+    try:
+        chip_info_reader = ChipInfoReader(chip_info_filename)
+    except IOError:
+        print('Unable to locate chipinfo.cid file.')
+        print('Please verify that file is present in the same directory as this script, '
+              'and that the filename is in lowercase characters, and that you have access to read the file.')
+        return None
+
+    try:
+        chip_info = chip_info_reader.get_chip(pic_type)
+    except KeyError:
+        print('Unable to find chip type "{}" in data file.'.format(pic_type))
+        print('Please check that the spelling is correct and that data file is up to date.')
+        return None
+
+
+    try:
+        rom_data, eeprom_data, id_data, fuse_values = prepare_flash_data_from_hex_file(chip_info, hex_file)
+    except FuseError:
+        print('Invalid fuse setting.  Fuse names and valid settings for this chip are as follows:')
+        print(chip_info.fuse_doc())
+        return None
+
+    word_count_rom = (len(rom_data) // 2)
+    word_count_eeprom = (len(eeprom_data) // 2)
+    print('ROM {} words used, {} words free on chip'.format(word_count_rom, chip_info.programming_vars.rom_size - word_count_rom))
+    print('EEPROM {} words used, {} words free on chip'.format(word_count_eeprom, chip_info.programming_vars.eeprom_size - word_count_eeprom))
+
+    INDENT = '  '
+    INLIST = '- '
+    intel_hex = IntelHex(hex_file_name)
+    if intel_hex.start_addr:
+        keys = sorted(intel_hex.start_addr.keys())
+        if keys == ['CS', 'IP']:
+            entry = intel_hex.start_addr['CS'] * 16 + intel_hex.start_addr['IP']
+        elif keys == ['EIP']:
+            entry = intel_hex.start_addr['EIP']
+        else:
+            raise RuntimeError("unknown 'IntelHex.start_addr' found")
+        print("{:s}entry: 0x{:08X}".format(INDENT, entry))
+    segments = intel_hex.segments()
+    if segments:
+        print("{:s}data:".format(INDENT))
+        for s in segments:
+            print("{:s}{:s}{{ first: 0x{:08X}, last: 0x{:08X}, length: 0x{:08X} }}".format(INDENT, INLIST, s[0], s[1] - 1, s[1] - s[0]))
+    print("")
+
+    """
+    
+    if self.chip_info.programming_vars.rom_size < word_count:  # type: ignore
+        raise InvalidValueError('Data too large for PIC ROM {} > {}'.format(word_count, chip_info.programming_vars.rom_size))
+    """
 
 def find_chip_data() -> str:
     chip_data_files = [f for f in [
         os.path.join('/', 'usr', 'share', 'picpro', 'chipdata.cid'),
         os.path.abspath(os.path.join(APP_ROOT_FOLDER, '..', 'usr', 'share', 'picpro', 'chipdata.cid')),
         os.path.abspath(os.path.join(APP_ROOT_FOLDER, '..', 'usr', 'lib', 'picpro', 'chipdata.cid')),  # Legacy search path
         os.path.abspath(os.path.join(APP_ROOT_FOLDER, '..', 'lib', 'picpro', 'chipdata.cid')),  # Legacy search path
```

### Comparing `picpro-0.1.0/picpro/exceptions.py` & `picpro-0.1.2/picpro/exceptions.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro/tools.py` & `picpro-0.1.2/picpro/tools.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/picpro.egg-info/PKG-INFO` & `picpro-0.1.2/picpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picpro
-Version: 0.1.0
+Version: 0.1.2
 Summary: picpro a kitsrus PIC CLI programmer
 Home-page: https://github.com/Salamek/picpro
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: LGPL-3.0 
 Project-URL: Release notes, https://github.com/Salamek/picpro/releases
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `picpro-0.1.0/picpro.egg-info/SOURCES.txt` & `picpro-0.1.2/picpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/setup.py` & `picpro-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme() -> str:
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='picpro',
-    version='0.1.0',
+    version='0.1.2',
     packages=find_packages(exclude=['tests', 'tests.*']),
     package_data={'picpro': ['py.typed']},
     install_requires=[
         'pyserial',
         'docopt',
         'intelhex'
     ],
```

### Comparing `picpro-0.1.0/tests/test_ChipInfoReader.py` & `picpro-0.1.2/tests/test_ChipInfoReader.py`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/tests/test_chip_data.cid` & `picpro-0.1.2/tests/test_chip_data.cid`

 * *Files identical despite different names*

### Comparing `picpro-0.1.0/usr/share/picpro/chipdata.cid` & `picpro-0.1.2/usr/share/picpro/chipdata.cid`

 * *Files identical despite different names*

