# Comparing `tmp/rdf_doctor-1.1.5-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,14 @@
-Zip file size: 75912 bytes, number of entries: 15
--rw-r--r--  2.0 unx       22 b- defN 24-May-10 00:14 dc/__init__.py
--rw-r--r--  2.0 unx     1754 b- defN 24-May-07 05:38 dc/consts.py
--rw-r--r--  2.0 unx    81131 b- defN 24-May-11 00:18 dc/doctor.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-11 08:06 doctor/__init__.py
--rw-r--r--  2.0 unx     2092 b- defN 24-May-11 08:06 doctor/consts.py
--rw-r--r--  2.0 unx    92088 b- defN 24-May-11 08:06 doctor/doctor.py
--rw-r--r--  2.0 unx   134314 b- defN 24-May-07 05:38 doctor/reference/prefixes.tsv
--rw-r--r--  2.0 unx       90 b- defN 24-May-07 05:38 doctor/reference/refine-class-uris.tsv
--rw-r--r--  2.0 unx      577 b- defN 24-May-07 05:38 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    10727 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1204 b- defN 24-May-11 08:30 rdf_doctor-1.1.5.dist-info/RECORD
-15 files, 325236 bytes uncompressed, 73928 bytes compressed:  77.3%
+Zip file size: 61422 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 24-May-13 03:41 doctor/__init__.py
+-rw-r--r--  2.0 unx     2491 b- defN 24-May-13 07:23 doctor/consts.py
+-rw-r--r--  2.0 unx   100741 b- defN 24-May-13 12:47 doctor/doctor.py
+-rw-r--r--  2.0 unx   134314 b- defN 24-May-09 12:17 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx       90 b- defN 24-May-09 12:17 doctor/reference/refine-class-uris.tsv
+-rw-r--r--  2.0 unx      577 b- defN 24-May-09 12:17 doctor/reference/refine-prefix-uris.tsv
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10676 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      996 b- defN 24-May-13 12:54 rdf_doctor-1.1.6.dist-info/RECORD
+12 files, 251119 bytes uncompressed, 59742 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -1,16 +1,7 @@
-Filename: dc/__init__.py
-Comment: 
-
-Filename: dc/consts.py
-Comment: 
-
-Filename: dc/doctor.py
-Comment: 
-
 Filename: doctor/__init__.py
 Comment: 
 
 Filename: doctor/consts.py
 Comment: 
 
 Filename: doctor/doctor.py
@@ -21,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/LICENSE
+Filename: rdf_doctor-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/METADATA
+Filename: rdf_doctor-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/WHEEL
+Filename: rdf_doctor-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.5.dist-info/RECORD
+Filename: rdf_doctor-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.5"
+__version__ = "1.1.6"
```

## doctor/consts.py

```diff
@@ -7,51 +7,60 @@
 
 # Target classes
 TARGET_CLASS_ALL = "all"
 
 # Input file extensions
 EXTENSION_NT = ".nt"
 EXTENSION_TTL = ".ttl"
+EXTENSION_JSON_LD = ".jsonld"
 EXTENSION_RDF = ".rdf"
 EXTENSION_XML = ".xml"
 EXTENSION_OWL = ".owl"
 EXTENSION_GZ = ".gz"
 EXTENSION_TAR_GZ = ".tar.gz"
 EXTENSION_XZ = ".xz"
 EXTENSION_TAR_XZ = ".tar.xz"
 EXTENSION_ZIP = ".zip"
 
 # Input file type
 FILE_TYPE_TTL = "ttl"
 FILE_TYPE_NT = "nt"
+FILE_TYPE_JSON_LD = "json-ld"
 FILE_TYPE_RDF_XML = "rdf_xml"
 FILE_TYPE_TTL_GZ = "ttl_gz"
+FILE_TYPE_JSON_LD_GZ = "json-ld_gz"
 FILE_TYPE_NT_GZ = "nt_gz"
 FILE_TYPE_RDF_XML_GZ = "rdf_xml_gz"
 FILE_TYPE_TTL_XZ = "ttl_xz"
+FILE_TYPE_JSON_LD_XZ = "json-ld_xz"
 FILE_TYPE_NT_XZ = "nt_xz"
 FILE_TYPE_RDF_XML_XZ = "rdf_xml_xz"
 FILE_TYPE_TTL_ZIP = "ttl_zip"
+FILE_TYPE_JSON_LD_ZIP = "json-ld_zip"
 FILE_TYPE_NT_ZIP = "nt_zip"
 FILE_TYPE_RDF_XML_ZIP = "rdf_xml_zip"
 
 FILE_TYPE_ALL = "all"
 
 # Dictionary of file type IDs and names
 FILE_TYPE_DICT = {
     FILE_TYPE_TTL: "Turtle(.ttl)",
     FILE_TYPE_NT: "N-Triples(.nt)",
+    FILE_TYPE_JSON_LD: "JSON-LD(.jsonld)",
     FILE_TYPE_RDF_XML: "RDF/XML(.rdf or .xml or .owl)",
-    FILE_TYPE_TTL_GZ: "tar compressed Turtle(.ttl.gz)",
-    FILE_TYPE_NT_GZ: "tar compressed N-Triples(.nt.gz)",
-    FILE_TYPE_RDF_XML_GZ: "tar compressed RDF/XML(.rdf.gz and .xml.gz and .owl.gz)",
-    FILE_TYPE_TTL_XZ: "tar compressed Turtle(.ttl.xz)",
-    FILE_TYPE_NT_XZ: "tar compressed N-Triples(.nt.xz)",
-    FILE_TYPE_RDF_XML_XZ: "tar compressed RDF/XML(.rdf.xz and .xml.xz and .owl.xz)",
+    FILE_TYPE_TTL_GZ: "gz compressed Turtle(.ttl.gz)",
+    FILE_TYPE_JSON_LD_GZ: "gz compressed JSON-LD(.jsonld.gz)",
+    FILE_TYPE_NT_GZ: "gz compressed N-Triples(.nt.gz)",
+    FILE_TYPE_RDF_XML_GZ: "gz compressed RDF/XML(.rdf.gz and .xml.gz and .owl.gz)",
+    FILE_TYPE_TTL_XZ: "xz compressed Turtle(.ttl.xz)",
+    FILE_TYPE_JSON_LD_XZ: "xz compressed JSON-LD(.jsonld.xz)",
+    FILE_TYPE_NT_XZ: "xz compressed N-Triples(.nt.xz)",
+    FILE_TYPE_RDF_XML_XZ: "xz compressed RDF/XML(.rdf.xz and .xml.xz and .owl.xz)",
     FILE_TYPE_TTL_ZIP: "zip compressed Turtle(.ttl.zip)",
+    FILE_TYPE_JSON_LD_ZIP: "zip compressed JSON-LD(.jsonld.zip)",
     FILE_TYPE_NT_ZIP: "zip compressed N-Triples(.nt.zip)",
     FILE_TYPE_RDF_XML_ZIP: "zip compressed RDF/XML(.rdf.zip and .xml.zip and .owl.zip)"
 }
 
 # Correct prefix list file path
 PREFIXES_FILE_PATH = "reference/prefixes.tsv"
```

## doctor/doctor.py

```diff
@@ -16,23 +16,24 @@
 import shutil
 from unidecode import unidecode
 from collections import defaultdict
 from pathlib import Path
 import tempfile
 import uuid
 import xz
-from doctor.consts import VERSION_FILE, TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, \
+from doctor.consts import VERSION_FILE, TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_JSON_LD, \
                             EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL, EXTENSION_GZ, EXTENSION_ZIP, EXTENSION_TAR_GZ, \
                             EXTENSION_XZ, EXTENSION_TAR_XZ, FILE_TYPE_TTL_XZ, FILE_TYPE_NT_XZ, FILE_TYPE_RDF_XML_XZ, \
                             PREFIXES_FILE_PATH, REFINE_CLASS_URIS_FILE_PATH, REFINE_PREFIX_URIS_FILE_PATH, HELP_LINK_URL, \
                             FILE_TYPE_TTL, FILE_TYPE_NT, FILE_TYPE_RDF_XML, FILE_TYPE_TTL_GZ, FILE_TYPE_NT_GZ, FILE_TYPE_RDF_XML_GZ, \
+                            FILE_TYPE_JSON_LD, FILE_TYPE_JSON_LD_GZ, FILE_TYPE_JSON_LD_XZ, FILE_TYPE_JSON_LD_ZIP, \
                             FILE_TYPE_TTL_ZIP, FILE_TYPE_NT_ZIP, FILE_TYPE_RDF_XML_ZIP, FILE_TYPE_ALL, FILE_TYPE_DICT, TMP_DISK_USAGE_LIMIT_DEFAULT
 
 from shexer.shaper import Shaper
-from shexer.consts import NT, TURTLE, TURTLE_ITER, RDF_XML, GZ, ZIP, XZ, MIXED_INSTANCES, ALL_EXAMPLES
+from shexer.consts import NT, TURTLE, TURTLE_ITER, RDF_XML, GZ, ZIP, XZ, MIXED_INSTANCES, ALL_EXAMPLES, JSON_LD
 
 is_displaying_spinner = False
 in_progress_rdflib_query = False
 
 # Main processing of rdf-doctor
 def doctor():
     args = get_command_line_args(sys.argv[1:])
@@ -107,15 +108,15 @@
                 else:
                     input_format = input_file_list[2]
 
                 if args.verbose:
                     print_overwrite(get_dt_now() + " -- Start processing [" + ", ".join(str(input_file) for input_file in input_file_list[0]) + "]")
 
                 # Get and output result. If an error occurs, store it in a queue
-                #print_overwrite(get_dt_now() + " -- " + input_format + ":" + compression_mode)
+                print_overwrite(get_dt_now() + " -- " + input_format + ":" + compression_mode)
                 executor_calc.submit(get_and_output_result, args, input_file_list[0], input_format, compression_mode, widely_used_prefixes_dict, refine_prefix_uris, refine_class_uris, error_queue)
 
             executor_calc.shutdown()
             if args.verbose:
                 is_displaying_spinner = False
                 executor_spinner.shutdown()
 
@@ -194,20 +195,20 @@
                         action="store_true",
                         help="show progress while processing")
 
     # Input RDF file (-i、--input [RDF-FILE]、required)
     parser.add_argument("-i","--input", type=str,
                         required=True,
                         nargs="+",
-                        help='input RDF file or directory (Turtle(.ttl), N-Triples(.nt), RDF/XML(.rdf, .xml, .owl) and their compressed versions are supported)',
+                        help='input RDF file or directory (Turtle(.ttl), N-Triples(.nt), RDF/XML(.rdf, .xml, .owl), JSON-LD(.jsonld) and their compressed versions are supported)',
                         metavar="RDF-FILE or DIRECTORY")
 
     # Input file type (-t、--type)
     parser.add_argument("-t","--type",
-                        help='specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, ttl_gz, nt_gz, rdf_xml_gz, ttl_xz, nt_xz, rdf_xml_xz, ttl_zip, nt_zip, rdf_xml_zip)')
+                        help='specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, jsonld, or one of these followed by gz, xz, or zip concatenated with _ such as ttl_gz)')
 
     # Add report to results (-r、--report)
     parser.add_argument("-r","--report",
                         action="store_true",
                         help="add report to results")
 
     # Output directory (-o、--output [DIRECTORY]、default: Standard output)
@@ -278,23 +279,27 @@
 #     [["test19.ttl.zip", "test20.ttl.zip", "test21.ttl.zip"], "zip", "turtle"]
 #     [["test22.nt.zip", "test23.nt.zip", "test24.nt.zip"], "zip", "nt"],
 #     [["test25.rdf.zip", "test26.xml.zip", "test27.owl.zip"], "zip", "xml"]
 # ]
 def get_input_files_by_type(input_files, temp_dir, tmp_dir_disk_usage_limit):
 
     input_file_list_ttl = []            # Turtle(.ttl)
+    input_file_list_jsonld = []         # JSON-LD(.jsonld)
     input_file_list_nt = []             # N-Triples(.nt)
     input_file_list_rdf_xml = []        # RDF/XML(.rdf, .xml, .owl)
     input_file_list_ttl_gz = []         # GZ compressed Turtle(.ttl.gz)
+    input_file_list_jsonld_gz = []      # GZ compressed JSON-LD(.jsonld.gz)
     input_file_list_nt_gz = []          # GZ compressed N-Triples(.nt.gz)
     input_file_list_rdf_xml_gz = []     # GZ compressed RDF/XML(.rdf.gz, .xml.gz, .owl.gz)
     input_file_list_ttl_xz = []         # XZ compressed Turtle(.ttl.xz)
+    input_file_list_jsonld_xz = []      # XZ compressed JSON-LD(.jsonld.xz)
     input_file_list_nt_xz = []          # XZ compressed N-Triples(.nt.xz)
     input_file_list_rdf_xml_xz = []     # XZ compressed RDF/XML(.rdf.xz, .xml.xz, .owl.xz)
     input_file_list_ttl_zip = []        # ZIP compressed Turtle(.ttl.zip)
+    input_file_list_jsonld_zip = []     # ZIP compressed JSON-LD(.jsonld.zip)
     input_file_list_nt_zip = []         # ZIP compressed N-Triples(.nt.zip)
     input_file_list_rdf_xml_zip = []    # ZIP compressed RDF/XML(.rdf.zip, .xml.zip, .owl.zip)
     input_file_2d_list = []             # For storing final results
     exists_file_types = []
 
     # input_file_list_other = []        # Other than those above
     for input_file in input_files:
@@ -311,62 +316,72 @@
                     compression_mode = get_compression_mode(file_path)
                     input_format = get_input_format(file_path, compression_mode)
 
                     # Determine file type and add to array
                     if compression_mode == GZ:
                         if input_format == TURTLE:
                             input_file_list_ttl_gz.append(file_path)
+                        elif input_format == JSON_LD:
+                            input_file_list_jsonld_gz.append(file_path)
                         elif input_format == NT:
                             input_file_list_nt_gz.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml_gz.append(file_path)
                         else:
-                            # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                            # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                             pass
 
                     elif compression_mode == XZ:
                         if input_format == TURTLE:
                             input_file_list_ttl_xz.append(file_path)
+                        elif input_format == JSON_LD:
+                            input_file_list_jsonld_xz.append(file_path)
                         elif input_format == NT:
                             input_file_list_nt_xz.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml_xz.append(file_path)
                         else:
-                            # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                            # No processing except for .ttl, ,jsonld, .nt, .rdf, .xml, .owl compressed
                             pass
 
                     elif compression_mode == ZIP:
                         if input_format == TURTLE:
                             input_file_list_ttl_zip.append(file_path)
+                        elif input_format == JSON_LD:
+                            input_file_list_jsonld_zip.append(file_path)
                         elif input_format == NT:
                             input_file_list_nt_zip.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml_zip.append(file_path)
                         else:
-                            # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                            # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                             pass
 
                     elif compression_mode is None:
                         if input_format == TURTLE:
                             input_file_list_ttl.append(file_path)
+                        elif input_format == JSON_LD:
+                            input_file_list_jsonld.append(file_path)
                         elif input_format == NT:
                             input_file_list_nt.append(file_path)
                         elif input_format == RDF_XML:
                             input_file_list_rdf_xml.append(file_path)
                         else:
-                            # No processing except for .ttl, .nt, .rdf, .xml, .owl
+                            # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl
                             pass
 
         else:
             compression_mode = get_compression_mode(input_file)
             input_format = get_input_format(input_file, compression_mode)
 
             if compression_mode == GZ:
                 if input_format == TURTLE:
                     input_file_list_ttl_gz.append(input_file)
+                elif input_format == JSON_LD:
+                    input_file_list_jsonld_gz.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt_gz.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml_gz.append(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
 
@@ -387,59 +402,69 @@
                                 file_path = Path(root) / file
 
                                 compression_mode = get_compression_mode(file_path)
                                 input_format = get_input_format(file_path, compression_mode)
                                 if compression_mode == GZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_gz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_gz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_gz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_gz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
                                 if compression_mode == XZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_xz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_xz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_xz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
                                 elif compression_mode == ZIP:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_zip.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_zip.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_zip.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_zip.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
 
                                 elif compression_mode is None:
                                     if input_format == TURTLE:
                                         input_file_list_ttl.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl
                                         pass
                     else:
-                        error_msg = '1:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        error_msg = '1:"' + extension + '" is an unsupported extension. ".ttl", ".jsonld", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                         return None, None, error_msg
 
             elif compression_mode == XZ:
                 if input_format == TURTLE:
                     input_file_list_ttl_xz.append(input_file)
+                elif input_format == JSON_LD:
+                    input_file_list_jsonld_xz.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt_xz.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml_xz.append(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
 
@@ -460,59 +485,69 @@
                                 file_path = Path(root) / file
 
                                 compression_mode = get_compression_mode(file_path)
                                 input_format = get_input_format(file_path, compression_mode)
                                 if compression_mode == GZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_gz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_gz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_gz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_gz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
                                 elif compression_mode == XZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_xz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_xz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_xz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
                                 elif compression_mode == ZIP:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_zip.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_zip.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_zip.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_zip.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
 
                                 elif compression_mode is None:
                                     if input_format == TURTLE:
                                         input_file_list_ttl.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl
                                         pass
                     else:
-                        error_msg = '2:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        error_msg = '2:"' + extension + '" is an unsupported extension. ".ttl", ".jsonld", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                         return None, None, error_msg
 
             elif compression_mode == ZIP:
                 if input_format == TURTLE:
                     input_file_list_ttl_zip.append(input_file)
+                elif input_format == JSON_LD:
+                    input_file_list_jsonld_zip.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt_zip.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml_zip.append(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
                     if extension == EXTENSION_ZIP:
@@ -532,89 +567,111 @@
                                 file_path = Path(root) / file
 
                                 compression_mode = get_compression_mode(file_path)
                                 input_format = get_input_format(file_path, compression_mode)
                                 if compression_mode == GZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_gz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_gz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_gz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_gz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
 
                                 elif compression_mode == XZ:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_xz.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_xz.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_xz.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_xz.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
 
                                 elif compression_mode == ZIP:
                                     if input_format == TURTLE:
                                         input_file_list_ttl_zip.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld_zip.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt_zip.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml_zip.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                                         pass
 
                                 elif compression_mode is None:
                                     if input_format == TURTLE:
                                         input_file_list_ttl.append(file_path)
+                                    elif input_format == JSON_LD:
+                                        input_file_list_jsonld.append(file_path)
                                     elif input_format == NT:
                                         input_file_list_nt.append(file_path)
                                     elif input_format == RDF_XML:
                                         input_file_list_rdf_xml.append(file_path)
                                     else:
-                                        # No processing except for .ttl, .nt, .rdf, .xml, .owl
+                                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl
                                         pass
                     else:
-                        error_msg = '3:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                        error_msg = '3:"' + extension + '" is an unsupported extension. ".ttl", ".jsonld", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                         return None, None, error_msg
 
             elif compression_mode is None:
                 if input_format == TURTLE:
                     input_file_list_ttl.append(input_file)
+                elif input_format == JSON_LD:
+                    input_file_list_jsonld.append(input_file)
                 elif input_format == NT:
                     input_file_list_nt.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml.append(input_file)
                 else:
-                    error_msg = '4:"' + get_extension(input_file) + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                    error_msg = '4:"' + get_extension(input_file) + '" is an unsupported extension. ".ttl", ".jsonld", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                     return None, None, error_msg
 
     if len(input_file_list_ttl) != 0:
         # input_file_dict[FILE_TYPE_TTL] = [input_file_list_ttl, None, TURTLE]
         input_file_2d_list.append([input_file_list_ttl, None, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL)
+    if len(input_file_list_jsonld) != 0:
+        # input_file_dict[FILE_TYPE_JSON_LD] = [input_file_list_jsonld, None, JSON_LD]
+        input_file_2d_list.append([input_file_list_jsonld, None, JSON_LD])
+        exists_file_types.append(FILE_TYPE_JSON_LD)
     if len(input_file_list_nt) != 0:
         # input_file_dict[FILE_TYPE_NT] = [input_file_list_nt, None, NT]
         input_file_2d_list.append([input_file_list_nt, None, NT])
         exists_file_types.append(FILE_TYPE_NT)
     if len(input_file_list_rdf_xml) != 0:
         # input_file_dict[FILE_TYPE_RDF_XML] = [input_file_list_rdf_xml, None, RDF_XML]
         input_file_2d_list.append([input_file_list_rdf_xml, None, RDF_XML])
         exists_file_types.append(FILE_TYPE_RDF_XML)
     if len(input_file_list_ttl_gz) != 0:
         # input_file_dict[FILE_TYPE_TTL_GZ] = [input_file_list_ttl_gz, GZ, TURTLE]
         input_file_2d_list.append([input_file_list_ttl_gz, GZ, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL_GZ)
+    if len(input_file_list_jsonld_gz) != 0:
+        # input_file_dict[FILE_TYPE_JSON_LD_GZ] = [input_file_list_jsonld_gz, GZ, JSON_LD]
+        input_file_2d_list.append([input_file_list_jsonld_gz, GZ, JSON_LD])
+        exists_file_types.append(FILE_TYPE_JSON_LD_GZ)
     if len(input_file_list_ttl_xz) != 0:
         # input_file_dict[FILE_TYPE_TTL_XZ] = [input_file_list_ttl_xz, XZ, TURTLE]
         input_file_2d_list.append([input_file_list_ttl_xz, XZ, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL_XZ)
+    if len(input_file_list_jsonld_xz) != 0:
+        # input_file_dict[FILE_TYPE_JSON_LD_XZ] = [input_file_list_jsonld_xz, XZ, JSON_LD]
+        input_file_2d_list.append([input_file_list_jsonld_xz, XZ, JSON_LD])
+        exists_file_types.append(FILE_TYPE_JSON_LD_XZ)
     if len(input_file_list_nt_gz) != 0:
         # input_file_dict[FILE_TYPE_NT_GZ] = [input_file_list_nt_gz, GZ, NT]
         input_file_2d_list.append([input_file_list_nt_gz, GZ, NT])
         exists_file_types.append(FILE_TYPE_NT_GZ)
     if len(input_file_list_nt_xz) != 0:
         # input_file_dict[FILE_TYPE_NT_XZ] = [input_file_list_nt_xz, XZ, NT]
         input_file_2d_list.append([input_file_list_nt_xz, XZ, NT])
@@ -627,14 +684,18 @@
         # input_file_dict[FILE_TYPE_RDF_XML_XZ] = [input_file_list_rdf_xml_xz, XZ, RDF_XML]
         input_file_2d_list.append([input_file_list_rdf_xml_xz, XZ, RDF_XML])
         exists_file_types.append(FILE_TYPE_RDF_XML_XZ)
     if len(input_file_list_ttl_zip) != 0:
         # input_file_dict[FILE_TYPE_TTL_ZIP] = [input_file_list_ttl_zip, ZIP, TURTLE]
         input_file_2d_list.append([input_file_list_ttl_zip, ZIP, TURTLE])
         exists_file_types.append(FILE_TYPE_TTL_ZIP)
+    if len(input_file_list_jsonld_zip) != 0:
+        # input_file_dict[FILE_TYPE_JSON_LD_ZIP] = [input_file_list_jsonld_zip, ZIP, JSON_LD]
+        input_file_2d_list.append([input_file_list_jsonld_zip, ZIP, JSON_LD])
+        exists_file_types.append(FILE_TYPE_JSON_LD_ZIP)
     if len(input_file_list_nt_zip) != 0:
         # input_file_dict[FILE_TYPE_NT_ZIP] = [input_file_list_nt_zip, ZIP, NT]
         input_file_2d_list.append([input_file_list_nt_zip, ZIP, NT])
         exists_file_types.append(FILE_TYPE_NT_ZIP)
     if len(input_file_list_rdf_xml_zip) != 0:
         # input_file_dict[FILE_TYPE_RDF_XML_ZIP] = [input_file_list_rdf_xml_zip, ZIP, RDF_XML]
         input_file_2d_list.append([input_file_list_rdf_xml_zip, ZIP, RDF_XML])
@@ -676,27 +737,27 @@
             for root, _, files in os.walk(top=input_file):
                 for file in files:
                     file_path = Path(root) / file
                     compression_mode = get_compression_mode(file_path)
                     input_format = get_input_format(file_path, compression_mode)
 
                     # Determine file type and add to array
-                    if input_format in (TURTLE, NT, RDF_XML):
+                    if input_format in (TURTLE, JSON_LD, NT, RDF_XML):
                         input_file_2d_list.append([[file_path], compression_mode, input_format])
                     else:
-                        # No processing except for .ttl, .nt, .rdf, .xml, .owl compressed
+                        # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl compressed
                         pass
 
         else:
-            # Files with the following extensions are supported: .ttl, .nt, .rdf, .xml, and .owl.
+            # Files with the following extensions are supported: .ttl, .jsonld, .nt, .rdf, .xml, and .owl.
             # However, other files are also added to the list for input checking.
             compression_mode = get_compression_mode(input_file)
             input_format = get_input_format(input_file, compression_mode)
 
-            if input_format in (TURTLE, NT, RDF_XML):
+            if input_format in (TURTLE, JSON_LD, NT, RDF_XML):
                 input_file_2d_list.append([[input_file], compression_mode, input_format])
             else:
                 # Case None
                 if compression_mode is None:
                     extension = get_extension(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
@@ -715,18 +776,18 @@
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
                         for file in files:
                             file_path = Path(root) / file
                             # Determine file type and add to array
                             compression_mode = get_compression_mode(file_path)
                             input_format = get_input_format(file_path, compression_mode)
-                            if input_format in (TURTLE, NT, RDF_XML):
+                            if input_format in (TURTLE, JSON_LD, NT, RDF_XML):
                                 input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
-                                # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
+                                # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl and their compressed
                                 pass
 
                 elif extension == EXTENSION_TAR_XZ:
                     # Check disk usage percentage
                     if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
                         error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
                         return None, None, error_msg
@@ -739,18 +800,18 @@
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
                         for file in files:
                             file_path = Path(root) / file
                             # Determine file type and add to array
                             compression_mode = get_compression_mode(file_path)
                             input_format = get_input_format(file_path, compression_mode)
-                            if input_format in (TURTLE, NT, RDF_XML):
+                            if input_format in (TURTLE, JSON_LD, NT, RDF_XML):
                                 input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
-                                # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
+                                # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl and their compressed
                                 pass
 
                 elif extension == EXTENSION_ZIP:
                     # Check disk usage percentage
                     if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
                         error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
                         return None, None, error_msg
@@ -762,48 +823,56 @@
 
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
                         for file in files:
                             file_path = Path(root) / file
                             compression_mode = get_compression_mode(file_path)
                             input_format = get_input_format(file_path, compression_mode)
-                            if input_format in (TURTLE, NT, RDF_XML):
+                            if input_format in (TURTLE, JSON_LD, NT, RDF_XML):
                                 input_file_2d_list.append([[file_path], compression_mode, input_format])
                             else:
-                                # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
+                                # No processing except for .ttl, .jsonld, .nt, .rdf, .xml, .owl and their compressed
                                 pass
                 else:
-                    error_msg = '5:"' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+                    error_msg = '5:"' + extension + '" is an unsupported extension. ".ttl", ".jsonld", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                     return None, None, error_msg
 
     for input_file_list in input_file_2d_list:
         if input_file_list[1] is None:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL)
+            elif input_file_list[2] == JSON_LD and FILE_TYPE_JSON_LD not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_JSON_LD)
             elif input_file_list[2] == NT and FILE_TYPE_NT not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML)
         elif input_file_list[1] == GZ:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL_GZ)
+            elif input_file_list[2] == JSON_LD and FILE_TYPE_JSON_LD_GZ not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_JSON_LD_GZ)
             elif input_file_list[2] == NT and FILE_TYPE_NT_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT_GZ)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_GZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML_GZ)
         elif input_file_list[1] == XZ:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL_XZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL_XZ)
+            elif input_file_list[2] == JSON_LD and FILE_TYPE_JSON_LD_XZ not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_JSON_LD_XZ)
             elif input_file_list[2] == NT and FILE_TYPE_NT_XZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT_XZ)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_XZ not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML_XZ)
         elif input_file_list[1] == ZIP:
             if input_file_list[2] == TURTLE and FILE_TYPE_TTL_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_TTL_ZIP)
+            elif input_file_list[2] == JSON_LD and FILE_TYPE_JSON_LD_ZIP not in exists_file_types:
+                exists_file_types.append(FILE_TYPE_JSON_LD_ZIP)
             elif input_file_list[2] == NT and FILE_TYPE_NT_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_NT_ZIP)
             elif input_file_list[2] == RDF_XML and FILE_TYPE_RDF_XML_ZIP not in exists_file_types:
                 exists_file_types.append(FILE_TYPE_RDF_XML_ZIP)
 
     return input_file_2d_list, exists_file_types, None
 
@@ -829,14 +898,17 @@
 
     if extension == EXTENSION_NT:
         # N-Triples
         return NT
     elif extension == EXTENSION_TTL:
         # Turtle
         return TURTLE
+    elif extension == EXTENSION_JSON_LD:
+        # JSON-LD
+        return JSON_LD
     elif extension in [EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
         # RDF/XML(.owl、.rdf、.xml)
         return RDF_XML
     else:
         return None
 
 
@@ -855,26 +927,26 @@
             return error_msg
 
         # Check if the file has read permission
         if os.access(input_file, os.R_OK) == False:
             error_msg = "Input file error: you don't have permission to read the input file."
             return error_msg
 
-        # Allow only ".nt", ".ttl", ".rdf", ".xml", ".owl" (and their compressed versions) extensions
+        # Allow only ".nt", ".ttl", ".jsonld", ".rdf", ".xml", ".owl" (and their compressed versions) extensions
         extension = get_extension(input_file)
         if extension in [EXTENSION_GZ, EXTENSION_XZ, EXTENSION_ZIP]:
             org_extension = get_extension_before_compression(input_file)
             # gz
             # if org_extension != EXTENSION_NT and org_extension != EXTENSION_TTL and org_extension != EXTENSION_RDF and org_extension != EXTENSION_XML and org_extension != EXTENSION_OWL:
-            if org_extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
-                error_msg = '6:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+            if org_extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_JSON_LD, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
+                error_msg = '6:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".jsonld", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
                 return error_msg
         #elif extension != EXTENSION_NT and extension != EXTENSION_TTL and extension != EXTENSION_RDF and extension != EXTENSION_XML and extension != EXTENSION_OWL:
-        elif extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
-            error_msg = '7:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
+        elif extension not in [EXTENSION_NT, EXTENSION_TTL, EXTENSION_JSON_LD, EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL]:
+            error_msg = '7:Input file error: "' + extension + '" is an unsupported extension. ".ttl", ".nt", ".jsonld", ".rdf", ".xml", ".owl" and their compressed versions are supported.'
             return error_msg
 
         if compression_mode == "":
             compression_mode = get_compression_mode(input_file)
         else:
             # This case usually does not occur because input files are classified by compression mode and input format at the start of processing.
             if compression_mode != get_compression_mode(input_file):
@@ -956,15 +1028,19 @@
         if FILE_TYPE_ALL in types:
             if len(types) != 1:
                 error_msg = 'Type error: If "all" is specified, other types cannot be specified.'
                 return error_msg
         else:
             for type in types:
                 if type not in FILE_TYPE_DICT:
-                    error_msg = 'Type error: "' + type + '" is an unsupported input file format. "' + FILE_TYPE_TTL + '", "' + FILE_TYPE_NT + '", "' + FILE_TYPE_RDF_XML + '", "' + FILE_TYPE_TTL_GZ + '", "' + FILE_TYPE_NT_GZ + '", "' + FILE_TYPE_RDF_XML_GZ + '", "' + FILE_TYPE_TTL_XZ + '", "' + FILE_TYPE_NT_XZ + '", "' + FILE_TYPE_RDF_XML_XZ + '", "' + FILE_TYPE_TTL_ZIP + '", "' + FILE_TYPE_NT_ZIP + '" and "' + FILE_TYPE_RDF_XML_ZIP + '" are supported.'
+                    error_msg = 'Type error: "' + type + '" is an unsupported input file format. "' \
+                        + FILE_TYPE_TTL + '", "' + FILE_TYPE_JSON_LD + '", "' + FILE_TYPE_NT + '", "' + FILE_TYPE_RDF_XML + '", "' \
+                        + FILE_TYPE_TTL_GZ + '", "' + FILE_TYPE_JSON_LD_GZ + '", "' + FILE_TYPE_NT_GZ + '", "' + FILE_TYPE_RDF_XML_GZ + '", "' \
+                        + FILE_TYPE_TTL_XZ + '", "' + FILE_TYPE_JSON_LD_XZ + '", "' + FILE_TYPE_NT_XZ + '", "' + FILE_TYPE_RDF_XML_XZ + '", "' \
+                        + FILE_TYPE_TTL_ZIP + '", "' + FILE_TYPE_JSON_LD_ZIP + '", "' + FILE_TYPE_NT_ZIP + '" and "' + FILE_TYPE_RDF_XML_ZIP + '" are supported.'
                     return error_msg
 
     # Check temporary directory
     if args.tmp_dir is not None:
         # Existence check of file temporary directory destination directory
         if Path(args.tmp_dir).is_file():
             error_msg = "Temporary directory error: A directory must be specified as the temporary directory destination. Files cannot be specified."
@@ -1000,21 +1076,26 @@
             namespaces_dict = get_default_namespaces_dict()
         else:
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Getting prefixes from input file... [" + ", ".join(str(input_file) for input_file in input_file_list) + "]")
 
             if input_format in (TURTLE, TURTLE_ITER):
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_turtle(input_file_list, compression_mode)
+            elif input_format == JSON_LD:
+                input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_json_ld(input_file_list, compression_mode)
             elif input_format == RDF_XML:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_rdf_xml(input_file_list, compression_mode)
             else:
                 raise ValueError("Invalid input format: " + str(input_format))
 
+            print_overwrite(get_dt_now() + " --- [" + str(input_prefixes) + "|" + str(duplicated_prefixes_dict) + "]")
             namespaces_dict = get_namespaces_dict(input_prefixes, duplicated_prefixes_dict, widely_used_prefixes_dict)
 
+        if args.verbose:
+            print_overwrite(get_dt_now() + " -- [" + str(namespaces_dict) + "]")
         shaper_result = get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict)
 
         report_result = []
         # Output only if report output option is specified
         if args.report:
             # Prefixes with the same Namespace but different URIs at the same time
             if args.verbose:
@@ -1155,14 +1236,16 @@
         else:
             # Output to file
             if args.merge:
                 # Output one result file for each type of file processed(Turtle, N-triples, and RDF/XML)
                 # turtle.shex, nt.shex, rdf.shex
                 if input_format in (TURTLE, TURTLE_ITER):
                     output_file_name = TURTLE
+                elif input_format == JSON_LD:
+                    output_file_name = "json-ld"
                 elif input_format == NT:
                     output_file_name = "n-triples"
                 elif input_format == RDF_XML:
                     output_file_name = "rdf_xml"
 
                 if compression_mode is None:
                     compression_exetention = ""
@@ -1345,15 +1428,14 @@
                 if len(fingerprint_comparison_result) == 0:
                     fingerprint_comparison_result.append(v)
                 else:
                     fingerprint_comparison_result.append("\n# "+v)
 
     return fingerprint_comparison_result
 
-
 # Get the prefixes contained within the Turtle file(s)
 # And get prefixes with the same Namespace but different URIs at the same time.
 def get_input_prefixes_turtle(input_files, compression_mode):
     input_prefixes = []
     duplicated_namespaces = []
     duplicated_prefixes_dict = defaultdict(list) # Used for processing Namespace collision prevention when generating namespaces_dict to be passed to sheXer. ex. {'foaf:': ['http://xmlns.com/foaf/0.1/', 'http://xmlns.com/foaf/spec/#']}
     for input_file in input_files:
@@ -1389,14 +1471,55 @@
     for key, values in duplicated_prefixes_dict.items():
         for value in values:
             duplicated_prefixes_list.append(key + "\t" + value + "\n")
 
     return input_prefixes, duplicated_prefixes_list, duplicated_prefixes_dict
 
 
+# Get the prefixes contained within the JSON-LD file(s)
+# And get prefixes with the same Namespace but different URIs at the same time.
+def get_input_prefixes_json_ld(input_files, compression_mode):
+    input_prefixes = []
+    duplicated_namespaces = []
+    duplicated_prefixes_dict = defaultdict(list) # Used for processing Namespace collision prevention when generating namespaces_dict to be passed to sheXer. ex. {'foaf:': ['http://xmlns.com/foaf/0.1/', 'http://xmlns.com/foaf/spec/#']}
+    for input_file in input_files:
+        if compression_mode == GZ:
+            with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
+                data = f.read()
+        elif compression_mode == XZ:
+            with xz.open(input_file, mode="rt", encoding="utf-8") as f:
+                data = f.read()
+        elif compression_mode == ZIP:
+            with ZipFile(input_file, "r") as f:
+                data = f.read(Path(input_file).name.replace(".zip", "")).decode()
+        else:
+            with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
+                data = f.read()
+    # using RDFLib to parse JSON-LD files and extract prefixes
+    g = rdflib.Graph()
+    g.parse(data=data, format="json-ld")
+    for prefix, uri in g.namespace_manager.namespaces():
+        uri = str(uri)
+        if [prefix, uri] not in input_prefixes:
+            input_prefixes.append([prefix, uri])
+            for input_prefix in input_prefixes:
+                if input_prefix[0] == prefix and input_prefix[1] != uri and prefix not in duplicated_namespaces:
+                    duplicated_namespaces.append(prefix)
+
+    for input_prefix in input_prefixes:
+        if input_prefix[0] in duplicated_namespaces:
+            duplicated_prefixes_dict[input_prefix[0]].append(input_prefix[1])
+
+    duplicated_prefixes_list = []
+    for key, values in duplicated_prefixes_dict.items():
+        for value in values:
+            duplicated_prefixes_list.append(key + "\t" + value + "\n")
+
+    return input_prefixes, duplicated_prefixes_list, duplicated_prefixes_dict
+
 # Get the prefixes contained within the RDF/XML file(s)
 # And get prefixes with the same Namespace but different URIs at the same time.
 def get_input_prefixes_rdf_xml(input_files, compression_mode):
     input_prefixes = []
     duplicated_namespaces = []
     duplicated_prefixes_dict = defaultdict(list) # Used for processing Namespace collision prevention when generating namespaces_dict to be passed to sheXer. ex. {'foaf:': ['http://xmlns.com/foaf/0.1/', 'http://xmlns.com/foaf/spec/#']}
     entity_namespaces_dict = {}
@@ -1603,44 +1726,56 @@
 # Determines if a file is to be processed based on the file passed as an argument and the target file type.
 def is_target_file(input_file_list, target_file_types):
 
     if input_file_list[1] is None:
         if input_file_list[2] == TURTLE:
             if FILE_TYPE_TTL in target_file_types:
                 return True
+        elif input_file_list[2] == JSON_LD:
+            if FILE_TYPE_JSON_LD in target_file_types:
+                return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT in target_file_types:
                 return True
         elif input_file_list[2] == RDF_XML:
             if FILE_TYPE_RDF_XML in target_file_types:
                 return True
     elif input_file_list[1] == GZ:
         if input_file_list[2] == TURTLE:
             if FILE_TYPE_TTL_GZ in target_file_types:
                 return True
+        elif input_file_list[2] == JSON_LD:
+            if FILE_TYPE_JSON_LD_GZ in target_file_types:
+                return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT_GZ in target_file_types:
                 return True
         elif input_file_list[2] == RDF_XML:
             if FILE_TYPE_RDF_XML_GZ in target_file_types:
                 return True
     elif input_file_list[1] == XZ:
         if input_file_list[2] == TURTLE:
             if FILE_TYPE_TTL_XZ in target_file_types:
                 return True
+        elif input_file_list[2] == JSON_LD:
+            if FILE_TYPE_JSON_LD_XZ in target_file_types:
+                return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT_XZ in target_file_types:
                 return True
         elif input_file_list[2] == RDF_XML:
             if FILE_TYPE_RDF_XML_XZ in target_file_types:
                 return True
     elif input_file_list[1] == ZIP:
         if input_file_list[2] == TURTLE:
             if FILE_TYPE_TTL_ZIP in target_file_types:
                 return True
+        elif input_file_list[2] == JSON_LD:
+            if FILE_TYPE_JSON_LD_ZIP in target_file_types:
+                return True
         elif input_file_list[2] == NT:
             if FILE_TYPE_NT_ZIP in target_file_types:
                 return True
         elif input_file_list[2] == RDF_XML:
             if FILE_TYPE_RDF_XML_ZIP in target_file_types:
                 return True
```

## Comparing `rdf_doctor-1.1.5.dist-info/LICENSE` & `rdf_doctor-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.5.dist-info/METADATA` & `rdf_doctor-1.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.5
+Version: 1.1.6
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask >=2.2.5
 Requires-Dist: Flask-Cors >=3.0.9
 Requires-Dist: rdflib >=6.3.1
 Requires-Dist: SPARQLWrapper >=2.0.0
 Requires-Dist: wlighter >=1.0.1
```

