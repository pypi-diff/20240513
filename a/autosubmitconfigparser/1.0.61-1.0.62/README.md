# Comparing `tmp/autosubmitconfigparser-1.0.61-py3-none-any.whl.zip` & `tmp/autosubmitconfigparser-1.0.62-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 35646 bytes, number of entries: 22
+Zip file size: 35785 bytes, number of entries: 22
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-07 13:48 autosubmitconfigparser/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-07 13:49 autosubmitconfigparser/config/__init__.py
 -rw-rw-r--  2.0 unx     8601 b- defN 24-Feb-14 14:23 autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--  2.0 unx   111794 b- defN 24-Apr-15 15:30 autosubmitconfigparser/config/configcommon.py
+-rw-rw-r--  2.0 unx   112443 b- defN 24-May-08 12:16 autosubmitconfigparser/config/configcommon.py
 -rw-rw-r--  2.0 unx      275 b- defN 23-Jun-07 12:06 autosubmitconfigparser/config/yamlparser.py
 -rwxrwxr-x  2.0 unx      269 b- defN 23-Feb-14 09:38 autosubmitconfigparser/config/files/autosubmit-dummy.yml
 -rwxrwxr-x  2.0 unx      269 b- defN 23-Feb-14 09:38 autosubmitconfigparser/config/files/autosubmit.yml
 -rwxrwxr-x  2.0 unx      562 b- defN 23-Feb-14 09:24 autosubmitconfigparser/config/files/expdef-dummy.yml
 -rwxrwxr-x  2.0 unx      557 b- defN 23-Feb-14 10:53 autosubmitconfigparser/config/files/expdef.yml
 -rwxrwxr-x  2.0 unx      401 b- defN 23-Mar-03 11:06 autosubmitconfigparser/config/files/git-minimal.yml
 -rwxrwxr-x  2.0 unx      669 b- defN 22-Oct-26 08:50 autosubmitconfigparser/config/files/jobs-dummy.yml
 -rwxrwxr-x  2.0 unx      669 b- defN 22-Oct-26 08:50 autosubmitconfigparser/config/files/jobs.yml
 -rwxrwxr-x  2.0 unx      321 b- defN 23-Mar-03 12:26 autosubmitconfigparser/config/files/local-minimal.yml
 -rwxrwxr-x  2.0 unx     1247 b- defN 23-Feb-14 10:53 autosubmitconfigparser/config/files/platforms-dummy.yml
 -rwxrwxr-x  2.0 unx     1247 b- defN 23-Feb-14 10:53 autosubmitconfigparser/config/files/platforms.yml
 -rw-rw-r--  2.0 unx        0 b- defN 22-Oct-26 08:51 log/__init__.py
 -rw-rw-r--  2.0 unx      871 b- defN 22-Oct-26 08:51 log/fd_show.py
 -rw-rw-r--  2.0 unx    13106 b- defN 22-Oct-26 08:51 log/log.py
--rw-rw-r--  2.0 unx     2928 b- defN 24-Apr-18 07:42 autosubmitconfigparser-1.0.61.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 07:42 autosubmitconfigparser-1.0.61.dist-info/WHEEL
--rw-rw-r--  2.0 unx       27 b- defN 24-Apr-18 07:42 autosubmitconfigparser-1.0.61.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2124 b- defN 24-Apr-18 07:42 autosubmitconfigparser-1.0.61.dist-info/RECORD
-22 files, 146029 bytes uncompressed, 32064 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx     2969 b- defN 24-May-13 13:48 autosubmitconfigparser-1.0.62.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-13 13:48 autosubmitconfigparser-1.0.62.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       27 b- defN 24-May-13 13:48 autosubmitconfigparser-1.0.62.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2124 b- defN 24-May-13 13:48 autosubmitconfigparser-1.0.62.dist-info/RECORD
+22 files, 146719 bytes uncompressed, 32203 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: log/fd_show.py
 Comment: 
 
 Filename: log/log.py
 Comment: 
 
-Filename: autosubmitconfigparser-1.0.61.dist-info/METADATA
+Filename: autosubmitconfigparser-1.0.62.dist-info/METADATA
 Comment: 
 
-Filename: autosubmitconfigparser-1.0.61.dist-info/WHEEL
+Filename: autosubmitconfigparser-1.0.62.dist-info/WHEEL
 Comment: 
 
-Filename: autosubmitconfigparser-1.0.61.dist-info/top_level.txt
+Filename: autosubmitconfigparser-1.0.62.dist-info/top_level.txt
 Comment: 
 
-Filename: autosubmitconfigparser-1.0.61.dist-info/RECORD
+Filename: autosubmitconfigparser-1.0.62.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autosubmitconfigparser/config/configcommon.py

```diff
@@ -2048,14 +2048,30 @@
         """
         content = open(self._exp_parser_file).read()
         if re.search('HPCARCH:.*', content):
             content = content.replace(
                 re.search('HPCARCH:.*', content).group(0), "HPCARCH: " + hpc)
         open(self._exp_parser_file, 'w').write(content)
 
+    def set_last_as_command(self, command):
+        """
+        Set the last autosubmit command used in the experiment's config file
+        :param command: current autosubmit command
+        :return:
+        """
+        misc = os.path.join(self.conf_folder_yaml,"as_misc.yml")
+        try:
+            content = open(misc, 'r').read()
+            if re.search('COMMAND:.*', content):
+                content = content.replace(re.search('COMMAND:.*', content).group(0),"COMMAND: {0}".format(command) )
+        except:
+            content = "ASMISC:\n  COMMAND: " + command + "\n"
+        open(misc,'w').write(content)
+        os.chmod(misc, 0o755)
+
     def set_version(self, autosubmit_version):
         """
         Sets autosubmit's version in autosubmit's config file
 
         :param autosubmit_version: autosubmit's version
         :type autosubmit_version: str
         """
```

## Comparing `autosubmitconfigparser-1.0.61.dist-info/METADATA` & `autosubmitconfigparser-1.0.62.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.61
+Version: 1.0.62
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
+License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-Requires-Dist: ruamel.yaml ==0.17.21
+Requires-Dist: ruamel.yaml (==0.17.21)
 Requires-Dist: mock
 Requires-Dist: pathlib
 Requires-Dist: bscearth.utils
 Requires-Dist: configobj
 Requires-Dist: pyparsing
 Requires-Dist: configparser
 Provides-Extra: all
-Requires-Dist: ruamel.yaml ==0.17.21 ; extra == 'all'
+Requires-Dist: ruamel.yaml (==0.17.21) ; extra == 'all'
 Requires-Dist: mock ; extra == 'all'
 Requires-Dist: pathlib ; extra == 'all'
 Requires-Dist: bscearth.utils ; extra == 'all'
 Requires-Dist: configobj ; extra == 'all'
 Requires-Dist: pyparsing ; extra == 'all'
 Requires-Dist: configparser ; extra == 'all'
 Requires-Dist: pytest ; extra == 'all'
@@ -79,7 +81,9 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
+
+
```

## Comparing `autosubmitconfigparser-1.0.61.dist-info/RECORD` & `autosubmitconfigparser-1.0.62.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 autosubmitconfigparser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autosubmitconfigparser/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autosubmitconfigparser/config/basicconfig.py,sha256=sS2ssdHQbogqdyS_x6K3BPa-4FP6Unx6FgNRBaMuv4Y,8601
-autosubmitconfigparser/config/configcommon.py,sha256=dJAck5p6QFAwLBWqBj1ttDBaylGt2__sj8OABjA7ffg,111794
+autosubmitconfigparser/config/configcommon.py,sha256=JgSOA5LuW9hXKNGwb3WoYRG9QHYwwaT7b3aE5TjEPQY,112443
 autosubmitconfigparser/config/yamlparser.py,sha256=x8p6YRjBVKw8BQxazWVOTJ2Lchs0OPrbZjsPg81y4Xg,275
 autosubmitconfigparser/config/files/autosubmit-dummy.yml,sha256=JFGQbOXG1J2Bxa15dOu9eeHGlSldd3doARR0ktkvtJw,269
 autosubmitconfigparser/config/files/autosubmit.yml,sha256=JFGQbOXG1J2Bxa15dOu9eeHGlSldd3doARR0ktkvtJw,269
 autosubmitconfigparser/config/files/expdef-dummy.yml,sha256=7eLrWcXjx-BTozLFt1GY5dlJHd-KVEmVASzJZ1eenag,562
 autosubmitconfigparser/config/files/expdef.yml,sha256=wbR8uLgBCrNZnu07XPFvYPQMi-I7FLNM48DhVoSP90E,557
 autosubmitconfigparser/config/files/git-minimal.yml,sha256=AMjAOdWFX62nFQ8FdlHUUJf_qe27Oakey_qYsilA8so,401
 autosubmitconfigparser/config/files/jobs-dummy.yml,sha256=NsGS1wT2j_S_FuVVTSs1J4D-EoA7IsFxgUunyvaJv7o,669
 autosubmitconfigparser/config/files/jobs.yml,sha256=NsGS1wT2j_S_FuVVTSs1J4D-EoA7IsFxgUunyvaJv7o,669
 autosubmitconfigparser/config/files/local-minimal.yml,sha256=WWP5dmVcZzVpw3j4SYenc54AuFn55632TrwmZjEkBWY,321
 autosubmitconfigparser/config/files/platforms-dummy.yml,sha256=rMOEf1XdTjiBmTIeR_RuehasRY4Y-s8DpkL8VFm03gI,1247
 autosubmitconfigparser/config/files/platforms.yml,sha256=rMOEf1XdTjiBmTIeR_RuehasRY4Y-s8DpkL8VFm03gI,1247
 log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 log/fd_show.py,sha256=M57TjTKtG0MEG_9wLBP1fr3c6itOUWWmbljXYq59O4c,871
 log/log.py,sha256=BKs2xyUp2EKCb8lpwmp5JdBsK6T1Zq6smsXeAOIO1QI,13106
-autosubmitconfigparser-1.0.61.dist-info/METADATA,sha256=ATAQ-aEXsveYIMIve8a9b5nNnOnbTTMTMNoMpkqdfyo,2928
-autosubmitconfigparser-1.0.61.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-autosubmitconfigparser-1.0.61.dist-info/top_level.txt,sha256=Ej_WBPxoZcqlpMWOdVVnaCm24XMTYfQdOrrOyRwL9o0,27
-autosubmitconfigparser-1.0.61.dist-info/RECORD,,
+autosubmitconfigparser-1.0.62.dist-info/METADATA,sha256=ZX_HECKqSesce6zO6HIhwQTS3sFR1LfeNoT54zDRs8s,2969
+autosubmitconfigparser-1.0.62.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+autosubmitconfigparser-1.0.62.dist-info/top_level.txt,sha256=Ej_WBPxoZcqlpMWOdVVnaCm24XMTYfQdOrrOyRwL9o0,27
+autosubmitconfigparser-1.0.62.dist-info/RECORD,,
```

