# Comparing `tmp/ektools-0.1.tar.gz` & `tmp/ektools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ektools-0.1.tar", last modified: Fri Nov 24 08:22:58 2023, max compression
+gzip compressed data, was "ektools-0.1.1.tar", last modified: Mon May 13 10:38:39 2024, max compression
```

## Comparing `ektools-0.1.tar` & `ektools-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2023-11-24 08:22:58.528639 ektools-0.1/
--rw-r--r--   0 ketil     (1000) ketil     (1000)     1671 2023-11-24 08:22:58.528639 ektools-0.1/PKG-INFO
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     1390 2023-11-24 07:51:11.000000 ektools-0.1/README.md
-drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2023-11-24 08:22:58.528639 ektools-0.1/ektools/
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     2234 2023-11-24 07:51:11.000000 ektools-0.1/ektools/__init__.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     5039 2023-11-24 07:51:11.000000 ektools-0.1/ektools/actions.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)      466 2023-11-24 07:51:11.000000 ektools-0.1/ektools/annotations.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     2807 2023-11-24 07:51:11.000000 ektools-0.1/ektools/conversion.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     6567 2023-11-24 07:51:11.000000 ektools-0.1/ektools/date_conversion.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)     8158 2023-11-24 07:51:11.000000 ektools-0.1/ektools/korona_parsers.py
--rwxrwxr-x   0 ketil     (1000) ketil     (1000)      447 2023-11-24 07:51:11.000000 ektools-0.1/ektools/rawdecode.py
--rw-rw-r--   0 ketil     (1000) ketil     (1000)    83476 2023-11-24 07:51:11.000000 ektools-0.1/ektools/simrad_parsers.py
-drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2023-11-24 08:22:58.528639 ektools-0.1/ektools.egg-info/
--rw-r--r--   0 ketil     (1000) ketil     (1000)     1671 2023-11-24 08:22:58.000000 ektools-0.1/ektools.egg-info/PKG-INFO
--rw-rw-r--   0 ketil     (1000) ketil     (1000)      439 2023-11-24 08:22:58.000000 ektools-0.1/ektools.egg-info/SOURCES.txt
--rw-rw-r--   0 ketil     (1000) ketil     (1000)        1 2023-11-24 08:22:58.000000 ektools-0.1/ektools.egg-info/dependency_links.txt
--rw-rw-r--   0 ketil     (1000) ketil     (1000)        1 2023-11-22 12:12:43.000000 ektools-0.1/ektools.egg-info/not-zip-safe
--rw-rw-r--   0 ketil     (1000) ketil     (1000)        8 2023-11-24 08:22:58.000000 ektools-0.1/ektools.egg-info/requires.txt
--rw-rw-r--   0 ketil     (1000) ketil     (1000)        8 2023-11-24 08:22:58.000000 ektools-0.1/ektools.egg-info/top_level.txt
--rw-rw-r--   0 ketil     (1000) ketil     (1000)       38 2023-11-24 08:22:58.528639 ektools-0.1/setup.cfg
--rw-rw-r--   0 ketil     (1000) ketil     (1000)      546 2023-11-24 08:22:52.000000 ektools-0.1/setup.py
-drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2023-11-24 08:22:58.528639 ektools-0.1/tools/
--rwxrwxr-x   0 ketil     (1000) ketil     (1000)     2517 2023-11-24 07:51:11.000000 ektools-0.1/tools/eklist
--rwxrwxr-x   0 ketil     (1000) ketil     (1000)     5259 2023-11-24 07:51:11.000000 ektools-0.1/tools/ekmeta
--rwxrwxr-x   0 ketil     (1000) ketil     (1000)     1439 2023-11-24 07:51:11.000000 ektools-0.1/tools/ekplot
--rwxrwxr-x   0 ketil     (1000) ketil     (1000)     2064 2023-11-24 07:51:11.000000 ektools-0.1/tools/eksplit
+drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2024-05-13 10:38:39.395290 ektools-0.1.1/
+-rw-r--r--   0 ketil     (1000) ketil     (1000)     1821 2024-05-13 10:38:39.395290 ektools-0.1.1/PKG-INFO
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     1390 2023-11-24 07:51:11.000000 ektools-0.1.1/README.md
+drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2024-05-13 10:38:39.392290 ektools-0.1.1/ektools/
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     2360 2024-05-08 08:44:16.000000 ektools-0.1.1/ektools/__init__.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     5155 2023-11-26 09:31:24.000000 ektools-0.1.1/ektools/actions.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)      466 2023-11-24 07:51:11.000000 ektools-0.1.1/ektools/annotations.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     2807 2023-11-24 07:51:11.000000 ektools-0.1.1/ektools/conversion.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     6567 2023-11-24 07:51:11.000000 ektools-0.1.1/ektools/date_conversion.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)     8212 2024-04-23 07:02:11.000000 ektools-0.1.1/ektools/korona_parsers.py
+-rwxrwxr-x   0 ketil     (1000) ketil     (1000)      447 2023-11-24 07:51:11.000000 ektools-0.1.1/ektools/rawdecode.py
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)    83476 2023-11-24 07:51:11.000000 ektools-0.1.1/ektools/simrad_parsers.py
+drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2024-05-13 10:38:39.394290 ektools-0.1.1/ektools.egg-info/
+-rw-r--r--   0 ketil     (1000) ketil     (1000)     1821 2024-05-13 10:38:39.000000 ektools-0.1.1/ektools.egg-info/PKG-INFO
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)      419 2024-05-13 10:38:39.000000 ektools-0.1.1/ektools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)        1 2024-05-13 10:38:39.000000 ektools-0.1.1/ektools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)       24 2024-05-13 10:38:39.000000 ektools-0.1.1/ektools.egg-info/requires.txt
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)        8 2024-05-13 10:38:39.000000 ektools-0.1.1/ektools.egg-info/top_level.txt
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)      582 2024-05-13 10:38:39.395290 ektools-0.1.1/setup.cfg
+-rw-rw-r--   0 ketil     (1000) ketil     (1000)       38 2024-05-13 10:26:18.000000 ektools-0.1.1/setup.py
+drwxrwsr-x   0 ketil     (1000) ketil     (1000)        0 2024-05-13 10:38:39.394290 ektools-0.1.1/tools/
+-rwxrwxr-x   0 ketil     (1000) ketil     (1000)     2519 2024-05-08 08:45:43.000000 ektools-0.1.1/tools/eklist
+-rwxrwxr-x   0 ketil     (1000) ketil     (1000)     5251 2024-05-07 13:50:10.000000 ektools-0.1.1/tools/ekmeta
+-rwxrwxr-x   0 ketil     (1000) ketil     (1000)     1443 2024-05-07 13:42:59.000000 ektools-0.1.1/tools/ekplot
+-rwxrwxr-x   0 ketil     (1000) ketil     (1000)     2155 2024-05-07 16:05:45.000000 ektools-0.1.1/tools/eksplit
```

### Comparing `ektools-0.1/PKG-INFO` & `ektools-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: ektools
-Version: 0.1
-Summary: Utilities to read and process Simrad RAW files
+Version: 0.1.1
+Summary: Utilities to read and process Simrad RAW files.
 Home-page: http://github.com/ketil-malde/ektools
 Author: Ketil Malde
 Author-email: ketil@malde.org
 License: MIT
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Dist: pynmea2
+Requires-Dist: numpy
+Requires-Dist: lxml
+Requires-Dist: pytz
 
 Ektools is a small collection of utilities/library functions to work
 with Simrad EK60 and EK80 echo sounder data.  There are two executable
 programs which take a RAW file as their parameter:
 
 - ekplot - simple plot of the raw data from each channel
 - eklist - extracts various information from the RAW file
```

### Comparing `ektools-0.1/README.md` & `ektools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ektools-0.1/ektools/__init__.py` & `ektools-0.1.1/ektools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import struct
 import mmap
 
 # text colors: GREEN = '\033[92m', BLUE = '\033[94m', HEADER = '\033[95m', CYAN = '\033[96m', BOLD = '\033[1m', UNDERLINE = '\033[4m'
 #              CLEAR = '\033[0m', YELLOW = '\033[93m', RED = '\033[91m'
 
 def warn(*args, **kwargs):
-    print('\033[93mWarning\033[0m',*args, file=sys.stderr, **kwargs)
+    print('\033[93mWarning\033[0m', *args, file=sys.stderr, **kwargs)
 
 def error(*args, **kwargs):
-    print('\033[91mError:\033[0m',*args, file=sys.stderr, **kwargs)
+    print('\033[91mError:\033[0m', *args, file=sys.stderr, **kwargs)
 
 import ektools.simrad_parsers as sp
 import ektools.korona_parsers as kp
 
 def parse(str):
     '''Table for selecting the correct parser to use for datagrams.
        Throws an exception if the datagram isn't known.'''
     # duplicates the simrad_raw_file.DGRAM_TYPE_KEY, but with bytestring keys
     parsers = {
-          b'BOT' : sp.SimradBottomParser()
+        b'BOT' : sp.SimradBottomParser()
         , b'CON' : sp.SimradConfigParser()
         , b'DEP' : sp.SimradDepthParser()
         , b'FIL' : sp.SimradFILParser()
         , b'MRU' : sp.SimradMRUParser()
         , b'NME' : sp.SimradNMEAParser()
         , b'RAW' : sp.SimradRawParser()
         , b'TAG' : sp.SimradAnnotationParser()
@@ -33,26 +33,27 @@
         , b'TNF' : kp.SimradTrackInfoParser()
         , b'TBR' : kp.SimradTrackBorderParser()
         , b'TTC' : kp.SimradTrackContentsParser()
     }
 
     dgram_type = str[:3]
     p = parsers[dgram_type]
-    return(p.from_string(str, len(str)))
+    return p.from_string(str, len(str))
 
-def index(f):
+def index(f, maxcount=None):
     '''Build an index of datagrams in a Simrad RAW file.  This is a list of position, type, length, and (unparsed) contents.'''
     idx = []
     with open(f, "rb") as fh:
         with mmap.mmap(fh.fileno(), length=0, access=mmap.ACCESS_READ) as mf:
             pos = 0
-            while pos < len(mf):
-                l, m = struct.unpack('<l4s', mf[pos:pos+8])
-                if pos+l > len(mf):
+            count = 0
+            while pos < len(mf) and (maxcount is None or count < maxcount):
+                l, m = struct.unpack('<l4s', mf[pos:pos + 8])
+                if pos + l > len(mf):
                     raise Exception('Premature EOF, truncated RAW file?')
-                v = struct.unpack('<l', mf[pos+l+4:pos+l+8])
+                v = struct.unpack('<l', mf[pos + l + 4:pos + l + 8])
                 t = m.decode('latin-1')
-                if v[0]!=l: warn(f'Datagram at {pos}: control lenght mismatch ({l} vs {v[0]}) - endianness error or corrupt file?')
-                idx.append((pos,t,l,mf[pos+4:pos+4+l]))
-                pos += l+8
+                if v[0] != l: warn(f'Datagram at {pos}: control lenght mismatch ({l} vs {v[0]}) - endianness error or corrupt file?')
+                idx.append((pos, t, l, mf[pos + 4:pos + 4 + l]))
+                pos += l + 8
+                count += 1
     return idx
-
```

### Comparing `ektools-0.1/ektools/actions.py` & `ektools-0.1.1/ektools/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 def showdict(obj, indent=4):
     if obj is None: return
     for k in obj.keys():
         if type(obj[k]) == type({}):
             print(indent*' ',k,'{')
             showdict(obj[k], indent+4)
             print(indent*' ','}')
+        elif isinstance(obj[k], datetime):
+            print(indent*' ', k, obj[k].strftime("%Y-%m-%d %H:%M:%S%Z"))
         else:
             print(indent*' ', k, repr(obj[k])[:72])
 
 import pickle
 import sys
 
 def rawdump():
```

### Comparing `ektools-0.1/ektools/conversion.py` & `ektools-0.1.1/ektools/conversion.py`

 * *Files identical despite different names*

### Comparing `ektools-0.1/ektools/date_conversion.py` & `ektools-0.1.1/ektools/date_conversion.py`

 * *Files identical despite different names*

### Comparing `ektools-0.1/ektools/korona_parsers.py` & `ektools-0.1.1/ektools/korona_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from .simrad_parsers import _SimradDatagramParser
+import struct
+from .date_conversion import nt_to_unix
 
 """
 These parsers are similar to Simrad Parsers, but process datagrams 
 found in RAW files after processing with the Korona library.
 
 | Authors:
 |       Ingrid Utseth <utseth@nr.no>
```

### Comparing `ektools-0.1/ektools/simrad_parsers.py` & `ektools-0.1.1/ektools/simrad_parsers.py`

 * *Files identical despite different names*

### Comparing `ektools-0.1/ektools.egg-info/PKG-INFO` & `ektools-0.1.1/ektools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: ektools
-Version: 0.1
-Summary: Utilities to read and process Simrad RAW files
+Version: 0.1.1
+Summary: Utilities to read and process Simrad RAW files.
 Home-page: http://github.com/ketil-malde/ektools
 Author: Ketil Malde
 Author-email: ketil@malde.org
 License: MIT
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Requires-Dist: pynmea2
+Requires-Dist: numpy
+Requires-Dist: lxml
+Requires-Dist: pytz
 
 Ektools is a small collection of utilities/library functions to work
 with Simrad EK60 and EK80 echo sounder data.  There are two executable
 programs which take a RAW file as their parameter:
 
 - ekplot - simple plot of the raw data from each channel
 - eklist - extracts various information from the RAW file
```

### Comparing `ektools-0.1/tools/eklist` & `ektools-0.1.1/tools/eklist`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 
 # import cProfile
 
 from ektools import actions
 from ektools import warn, error, parse, index
 
 def process(df, verbose=False, filters=[], actions=[]):
     '''Process an indexed Simrad RAW file by applying a set of actions'''
     count = 0
     for pos, t, l, bstr in df:
         if verbose:
             print(f'Datagram {count}:\t{pos}\t{l}\t{t}')
         count += 1
         if actions:
-            if filters == [] or any(f(pos,t,l) for f in filters):
+            if filters == [] or any(f(pos, t, l) for f in filters):
                 try:
                     obj = parse(bstr)
                     for a in actions:
                         a(obj)
-                except IOError: # e.g., broken pipe
+                except IOError:  # e.g., broken pipe
                     exit(0)
                 except Exception as e:
                     warn(f'Don\'t know how/failure to parse datagram of type {t}\n   Exception: {e}')
 
     # signal end
     for a in actions:
         a(None)
 
 if __name__ == '__main__':
 
     import argparse
 
     p = argparse.ArgumentParser(description='Extract information from Simrad RAW files.')
-    p.add_argument('-t', '--type',  default=[], action='append', help='only apply to given datagram types')
-    p.add_argument('-l', '--list',  action='store_true', help='output datagram contents extensively')
+    p.add_argument('-t', '--type', default=[], action='append', help='only apply to given datagram types')
+    p.add_argument('-l', '--list', action='store_true', help='output datagram contents extensively')
     p.add_argument('-s', '--summarize', action='store_true', help='summarize datagrams')
     p.add_argument('-q', '--quiet', action='store_true', help='produce minimal output')
     p.add_argument('-c', '--check', action='store_true', help='check datagram contents for consistency')
     p.add_argument('-r', '--rawdump', action='store_true', help='dump pickled raw datagrams')
     p.add_argument('FILE', nargs='+', help='input files in RAW format.')
     args = p.parse_args()
     
@@ -46,22 +46,22 @@
     if args.list:
         if args.quiet:
             error('Please specify at most one of -l and -q')
             exit(-1)
         else:
             myactions.append(actions.showdict)
     if args.rawdump:
-        myactions = [actions.rawdump()] # override previous
+        myactions = [actions.rawdump()]  # override previous
         args.quiet = True
         if args.list: warn("Ignoring '-l' because '-r' was specified.")
 
     fs = []
     if args.type: fs.append(actions.filtertype(args.type))
 
     if args.check:     myactions.append(actions.checkdate())
     if args.summarize: myactions.append(actions.summarize())
-    
+
     for f in args.FILE:
         # print(f)
         d = index(f)
         # cProfile.run("process(d, verbose=not args.quiet, actions=actions, filters=fs)")
         process(d, verbose=not args.quiet, actions=myactions, filters=fs)
```

### Comparing `ektools-0.1/tools/ekmeta` & `ektools-0.1.1/tools/ekmeta`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 
 from ektools import parse, index, warn, error
 
 import datetime
 import hashlib
 import mmap
 import pynmea2 as nm
@@ -23,33 +23,33 @@
     timedeltas = []
     speeds = []
     starttime = None
     endtime = None
     heaves = []
     rolls = []
     pitch = []
-    # EK80 does these differently    
-    sound_speed = None  
+    # EK80 does these differently
+    sound_speed = None
     temperatures = []
-    
+
     for pos, typ, ln, bstr in index(f):
         try:
             obj = parse(bstr)
         except:
             warn(f'Couldn\'t parse datagram of type {typ}, position {pos}.')
             continue
         if starttime is None:
             starttime = obj['timestamp']
         endtime = obj['timestamp']  # last time standing
 
         if typ == 'CON0':
             for tspname in obj['configuration']:
                 tsp = obj['configuration'][tspname]
                 fq = int(tsp['frequency'])
-                rcounts[fq] = { 'transducer': tspname, 'pings': 0, 'ranges': [] }
+                rcounts[fq] = {'transducer': tspname, 'pings': 0, 'ranges': []}
 
                 snm = tsp['survey_name'].decode('latin-1')
                 if survey_name is None:
                     survey_name = snm
                 else:
                     assert survey_name == snm
```

### Comparing `ektools-0.1/tools/ekplot` & `ektools-0.1.1/tools/ekplot`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 
 import numpy as np
 import seaborn as sns
 import matplotlib.pylab as plt
 
 # https://stackoverflow.com/questions/33282368/plotting-a-2d-heatmap-with-matplotlib
 def heatmap(mx):
```

### Comparing `ektools-0.1/tools/eksplit` & `ektools-0.1.1/tools/eksplit`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 
 import struct
 from ektools import index, parse
 import sys
 import os.path
 
 fn = sys.argv[1]
 
 idx = index(fn)
 
 config = parse(idx[0][3])
-
 assert config['subtype'] == 'configuration'
-confs = set([ k.split('_')[-1] for k in config['configuration'].keys()])
+# config2 = parse(idx[1][3])
+# assert config2['subtype'] == 'initialparameter'
+
+confs = set([k.split('_')[-1] for k in config['configuration'].keys()])
 print('Configurations:', confs)
 
 def matches(predicate, msg):
     try:
         p = parse(msg)
     except:
         return False
@@ -25,15 +27,15 @@
     elif 'parameter' in p.keys():
         return predicate(p['parameter']['channel_id'])
     else:
         return True
 
 def dgram_write(f, dgram):
     """Write a datagram to a file"""
-    hdr = struct.pack('<l',len(dgram))
+    hdr = struct.pack('<l', len(dgram))
     f.write(hdr)
     f.write(dgram)
     f.write(hdr)
 
 import lxml.etree as et
 
 def edit_xml(predicate, xmlstr):
@@ -47,31 +49,29 @@
         if len(trans.findall('.//Channel')) == 0:
             trans.getparent().remove(trans)
 
     return xml
 
 split = {}
 for a in confs:
-    split[a] = [(p,t,l,m) for p,t,l,m in index(fn) if matches(lambda c : c.split('_')[-1] == a, m)]
+    split[a] = [(p, t, l, m) for p, t, l, m in index(fn) if matches(lambda c: c.split('_')[-1] == a, m)]
 
 for a in confs:
     print(f'Config {a}, count: {len(split[a])}')
     counts = {}
     for x in split[a]:
         if x[1] not in counts:
             counts[x[1]] = 1
         else:
-            counts[x[1]]+=1
+            counts[x[1]] += 1
     print(counts)
 
-    outname = os.path.splitext(os.path.basename(fn))[0]+'_'+a+'.raw'
+    outname = os.path.splitext(os.path.basename(fn))[0] + '_' + a + '.raw'
     with open(outname, 'wb') as f:
         # Output configuration datagram
         xmlconf = idx[0][3][12:-2]
-        x0 = et.tostring(edit_xml(lambda c: c.split('_')[-1]==a, xmlconf))
-        dgram_write(f,split[a][0][3][:12]+x0)
+        x0 = et.tostring(edit_xml(lambda c: c.split('_')[-1] == a, xmlconf))
+        dgram_write(f, split[a][0][3][:12] + x0)
 
-        for (pos,typ,length,dgram) in split[a][1:]:
+        for (pos, typ, length, dgram) in split[a][1:]:
             # write length (dgram already contains type)
-            dgram_write(f,dgram)
-        
-    
+            dgram_write(f, dgram)
```

