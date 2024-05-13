# Comparing `tmp/avrotize-1.4.1.tar.gz` & `tmp/avrotize-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.4.1.tar` & `avrotize-1.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    26753 2024-05-10 15:20:18.212851 avrotize-1.4.1/README.md
--rw-r--r--   0        0        0     1673 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-10 15:20:22.324847 avrotize-1.4.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15557 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    43154 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58115 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13663 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1138 2024-05-10 15:20:18.216851 avrotize-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    27129 2024-05-13 09:05:17.610896 avrotize-1.5.0/README.md
+-rw-r--r--   0        0        0     1673 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-13 09:05:21.734894 avrotize-1.5.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15713 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    48267 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58076 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13663 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-13 09:05:17.610896 avrotize-1.5.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-13 09:05:17.614896 avrotize-1.5.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1138 2024-05-13 09:05:17.614896 avrotize-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    27796 1970-01-01 00:00:00.000000 avrotize-1.5.0/PKG-INFO
```

### Comparing `avrotize-1.4.1/README.md` & `avrotize-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -427,26 +427,30 @@
 Parameters:
 - `--avsc`: The path to the Avro schema file to be converted.
 - `--csharp`: The path to the C# directory to write the conversion result to.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
 - `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
 - `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
+- `--namespace`: (optional) The namespace to use in the generated C# classes.
 
 Conversion notes:
 - The tool generates C# classes that represent the Avro schema as data classes.
 - Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
   will add annotations for the respective JSON serialization library to the generated
   C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
   preserves the JSON Schema structure in the Avro schema, the generated C# classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
+- Only the `--system-text-json-annotation` option generates classes that support type unions.
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `.csproj` project file into the given
   directory if none exists.
 
+Read more about the C# code generation in the [C# code generation documentation](csharpcodegen.md).
+
 
 ### Generate Java code from Avro schema
 
 ```bash
 avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
 ```
 
@@ -467,14 +471,16 @@
   preserves the JSON Schema structure in the Avro schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
+Read more about the Java code generation in the [Java code generation documentation](javacodegen.md).
+
 ### Generate Python code from Avro schema
 
 This command generates Python dataclasses from an Avro schema.
 
 ```bash
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
```

### Comparing `avrotize-1.4.1/avrotize/__init__.py` & `avrotize-1.5.0/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/asn1toavro.py` & `avrotize-1.5.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotize.py` & `avrotize-1.5.0/avrotize/avrotize.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     a2csharp_parser = subparsers.add_parser('a2csharp', help='Convert Avro schema to C# classes')
     a2csharp_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2csharp_parser.add_argument('--csharp', type=str, help='Output path for the C# classes', required=True)
     a2csharp_parser.add_argument('--avro-annotation', action='store_true', help='Use Avro annotations', default=False)
     a2csharp_parser.add_argument('--system-text-json-annotation', action='store_true', help='Use System.Text.Json annotations', default=False)
     a2csharp_parser.add_argument('--newtonsoft-json-annotation', action='store_true', help='Use Newtonsoft.Json annotations', default=False)
     a2csharp_parser.add_argument('--pascal-properties', action='store_true', help='Use PascalCase properties', default=False)
+    a2csharp_parser.add_argument('--namespace', type=str, help='C# namespace', required=False)
     
     a2java_parser = subparsers.add_parser('a2java', help='Convert Avro schema to Java classes')
     a2java_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2java_parser.add_argument('--java', type=str, help='Output path for the Java classes', required=True)
     a2java_parser.add_argument('--package', type=str, help='Java package name', required=True)
     a2java_parser.add_argument('--avro-annotation', action='store_true', help='Use Avro annotations', default=False)
     a2java_parser.add_argument('--jackson-annotation', action='store_true', help='Use Jackson annotations', default=False)
@@ -184,16 +185,17 @@
     elif args.command == 'a2csharp':
         avro_schema_path = args.avsc
         csharp_path = args.csharp
         avro_annotation = args.avro_annotation
         system_text_json_annotation = args.system_text_json_annotation
         newtonsoft_json_annotation = args.newtonsoft_json_annotation
         pascal_properties = args.pascal_properties
+        namespace = args.namespace
         print(f'Converting Avro {avro_schema_path} to C# {csharp_path}')
-        convert_avro_to_csharp(avro_schema_path, csharp_path, avro_annotation=avro_annotation, system_text_json_annotation=system_text_json_annotation, newtonsoft_json_annotation=newtonsoft_json_annotation, pascal_properties=pascal_properties)
+        convert_avro_to_csharp(avro_schema_path, csharp_path, base_namespace=namespace, avro_annotation=avro_annotation, system_text_json_annotation=system_text_json_annotation, newtonsoft_json_annotation=newtonsoft_json_annotation, pascal_properties=pascal_properties)
     elif args.command == 'a2java':
         avro_schema_path = args.avsc
         java_path = args.java
         package = args.package
         avro_annotation = args.avro_annotation
         jackson_annotation = args.jackson_annotation
         pascal_properties = args.pascal_properties
```

### Comparing `avrotize-1.4.1/avrotize/avrotocsharp.py` & `avrotize-1.5.0/avrotize/avrotocsharp.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,23 +56,27 @@
 """
 
 AVRO_TOBYTEARRAY = \
 """
 if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
 {
     var stream = new System.IO.MemoryStream();
-    var writer = new Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
-    writer.Write(this, new Avro.IO.BinaryEncoder(stream));
+    var writer = new global::Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
+    var encoder = new global::Avro.IO.BinaryEncoder(stream);
+    writer.Write(this, encoder);
+    encoder.Flush();
     result = stream.ToArray();
 }
 else if (contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
 {
     var stream = new System.IO.MemoryStream();
-    var writer = new Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
-    writer.Write(this, new Avro.IO.JsonEncoder({type_name}.AvroSchema, stream));
+    var writer = new global::Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
+    var encoder = new global::Avro.IO.JsonEncoder({type_name}.AvroSchema, stream);
+    writer.Write(this, encoder);
+    encoder.Flush();
     result = stream.ToArray();
 }
 """
 
 SYSTEM_TEXT_JSON_TOBYTEARRAY = \
 """
 if (contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
@@ -100,16 +104,18 @@
     var stream = data switch
     {
         System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
         _ => throw new NotSupportedException("Data is not of a supported type for gzip decompression")
     };
     using (var gzip = new System.IO.Compression.GZipStream(stream, System.IO.Compression.CompressionMode.Decompress))
     {
-        data = new System.IO.MemoryStream();
-        gzip.CopyTo((System.IO.MemoryStream)data);
+        System.IO.MemoryStream memoryStream = new System.IO.MemoryStream();
+        gzip.CopyTo(memoryStream);
+        memoryStream.Position = 0;
+        data = memoryStream.ToArray();
     }
 }
 """
 
 EPILOGUE_FROMDATA = \
 """
 throw new System.NotSupportedException($"Unsupported media type {contentType.MediaType}");
@@ -127,14 +133,22 @@
     {
         return System.Text.Json.JsonSerializer.Deserialize<{type_name}>((string)data);
     }
     else if (data is System.BinaryData)
     {
         return ((System.BinaryData)data).ToObjectFromJson<{type_name}>();
     }
+    else if (data is byte[])
+    {
+        return System.Text.Json.JsonSerializer.Deserialize<{type_name}>(new ReadOnlySpan<byte>((byte[])data));
+    }
+    else if (data is System.IO.Stream)
+    {
+        return System.Text.Json.JsonSerializer.DeserializeAsync<{type_name}>((System.IO.Stream)data).Result;
+    }
 }
 """
 
 NEWTONSOFT_JSON_FROMDATA = \
 """
 if ( contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
 {
@@ -154,27 +168,40 @@
 if ( contentType.MediaType.StartsWith("avro/") || contentType.MediaType.StartsWith("application/vnd.apache.avro") )
 {
     var stream = data switch
     {
         System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
         _ => throw new NotSupportedException("Data is not of a supported type for conversion to Stream")
     };
+    #pragma warning disable CS8625 // Cannot convert null literal to non-nullable reference type.
     if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
     {
-        var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return reader.Read(new {type_name}(), new Avro.IO.BinaryDecoder(stream));
+        var reader = new global::Avro.Generic.GenericDatumReader<global::Avro.Generic.GenericRecord>({type_name}.AvroSchema, {type_name}.AvroSchema);
+        return new {type_name}(reader.Read(null, new global::Avro.IO.BinaryDecoder(stream)));
     }
     if ( contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
     {
-        var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return reader.Read(new {type_name}(), new Avro.IO.JsonDecoder({type_name}.AvroSchema, stream));
+        var reader = new global::Avro.Generic.GenericDatumReader<global::Avro.Generic.GenericRecord>({type_name}.AvroSchema, {type_name}.AvroSchema);
+        return new {type_name}(reader.Read(null, new global::Avro.IO.JsonDecoder({type_name}.AvroSchema, stream)));
     }
+    #pragma warning restore CS8625
 }    
 """
 
+AVRO_CLASS_PREAMBLE = \
+"""
+public {type_name}(global::Avro.Generic.GenericRecord obj)
+{
+    global::Avro.Specific.ISpecificRecord self = this;
+    for (int i = 0; obj.Schema.Fields.Count > i; ++i)
+    {
+        self.Put(i, obj.GetValue(i));
+    }
+}
+"""
 
 class AvroToCSharp:
     """ Converts Avro schema to C# classes """
 
     def __init__(self, base_namespace: str = '') -> None:
         self.base_namespace = base_namespace
         self.schema_doc: JsonNode = None
@@ -246,22 +273,15 @@
                 return 'Dictionary<string, object>'
             else:
                 non_null_types = [t for t in avro_type if t != 'null']
                 if len(non_null_types) == 1:
                     # Nullable type
                     return f"{self.convert_avro_type_to_csharp(class_name, field_name, non_null_types[0], parent_namespace)}?"
                 else:
-                    if self.system_text_json_annotation:
-                        return self.generate_embedded_union_class_system_json_text(class_name, field_name, non_null_types, parent_namespace, write_file=True)
-                    else:
-                        # Handle union by generating classes for complex types within
-                        for t in non_null_types:
-                            if isinstance(t, dict) and (t.get('type') == 'record' or t.get('type') == 'enum'):
-                                self.generate_class_or_enum(t, parent_namespace)
-                        return 'object'  # Placeholder for complex unions
+                    return self.generate_embedded_union(class_name, field_name, non_null_types, parent_namespace, write_file=True)
         elif isinstance(avro_type, dict):
             # Handle complex types: records, enums, arrays, and maps
             if avro_type['type'] in ['record', 'enum']:
                 return self.generate_class_or_enum(avro_type, parent_namespace, write_file=True)
             elif avro_type['type'] == 'array':
                 return f"List<{self.convert_avro_type_to_csharp(class_name, field_name+'List', avro_type['items'], parent_namespace)}>"
             elif avro_type['type'] == 'map':
@@ -277,99 +297,115 @@
             return self.generate_enum(avro_schema, parent_namespace, write_file)
         return ''
 
     def generate_class(self, avro_schema: Dict, parent_namespace: str, write_file: bool) -> str:
         """ Generates a Class """
         class_definition = ''
         avro_namespace = avro_schema.get('namespace', parent_namespace)
+        if not 'namespace' in avro_schema:
+            avro_schema['namespace'] = parent_namespace
         namespace = pascal(self.concat_namespace(self.base_namespace, avro_namespace))
         class_name = pascal(avro_schema['name'])
+        
         class_definition += f"/// <summary>\n/// { avro_schema.get('doc', class_name ) }\n/// </summary>\n"
         fields_str = [self.generate_property(field, class_name, avro_namespace) for field in avro_schema.get('fields', [])]
         class_body = "\n".join(fields_str)
         class_definition += f"public partial class {class_name}"
         if self.avro_annotation:
             class_definition += " : global::Avro.Specific.ISpecificRecord"
         class_definition += "\n{\n"+class_body
+        class_definition += f"\n{INDENT}/// <summary>\n{INDENT}/// Default constructor\n{INDENT}///</summary>\n"
+        class_definition += f"{INDENT}public {class_name}()\n{INDENT}{{\n{INDENT}}}"
+        if self.avro_annotation:
+            class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Constructor from Avro GenericRecord\n{INDENT}///</summary>\n"
+            class_definition += f"{INDENT}public {class_name}(global::Avro.Generic.GenericRecord obj)\n{INDENT}{{\n"
+            class_definition += f"{INDENT*2}global::Avro.Specific.ISpecificRecord self = this;\n"
+            class_definition += f"{INDENT*2}for (int i = 0; obj.Schema.Fields.Count > i; ++i)\n{INDENT*2}{{\n"
+            class_definition += f"{INDENT*3}self.Put(i, obj.GetValue(i));\n{INDENT*2}}}\n{INDENT}}}\n"
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             # wrap schema at 80 characters
             avro_schema_json = avro_schema_json.replace('"', '§')
             avro_schema_json = f"\"+\n{INDENT}\"".join(
                 [avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
             class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Avro schema for this class\n{INDENT}/// </summary>"
             class_definition += f"\n{INDENT}public static global::Avro.Schema AvroSchema = global::Avro.Schema.Parse(\n{INDENT}\"{avro_schema_json}\");\n"
-            class_definition += f"\n{INDENT}Schema global::Avro.Specific.ISpecificRecord.Schema => AvroSchema;\n"
+            class_definition += f"\n{INDENT}global::Avro.Schema global::Avro.Specific.ISpecificRecord.Schema => AvroSchema;\n"
             get_method = f"{INDENT}object global::Avro.Specific.ISpecificRecord.Get(int fieldPos)\n" + \
                 INDENT+"{"+f"\n{INDENT*2}switch (fieldPos)\n{INDENT*2}" + "{"
             put_method = f"{INDENT}void global::Avro.Specific.ISpecificRecord.Put(int fieldPos, object fieldValue)\n" + \
                 INDENT+"{"+f"\n{INDENT*2}switch (fieldPos)\n{INDENT*2}"+"{"
             for pos, field in enumerate(avro_schema.get('fields', [])):
                 field_name = field['name']
                 if self.is_csharp_reserved_word(field_name):
                     field_name = f"@{field_name}"
                 field_type = self.convert_avro_type_to_csharp(class_name, field_name, field['type'], avro_namespace)
                 if self.pascal_properties:
                     field_name = pascal(field_name)
                 if field_name == class_name:
                     field_name += "_"
-                get_method += f"\n{INDENT*3}case {pos}: return this.{field_name};"
-                put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = ({field_type})fieldValue; break;"
+                if class_name + '.' + field_type in self.generated_types and self.generated_types[class_name + '.' + field_type] == "union":
+                    get_method += f"\n{INDENT*3}case {pos}: return this.{field_name}?.ToObject();"
+                    put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = {field_type}.FromObject(fieldValue); break;"
+                else:    
+                    get_method += f"\n{INDENT*3}case {pos}: return this.{field_name};"
+                    put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = ({field_type})fieldValue; break;"
             get_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Get()\");"
             put_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Put()\");"
             get_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             put_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             class_definition += f"\n{get_method}\n{put_method}\n"
 
         # emit ToByteArray method
-        class_definition += f"\n{INDENT}/// <summary>\n{INDENT}/// Converts the object to a byte array\n{INDENT}/// </summary>"
-        class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the desired encoding</param>"
-        class_definition += f"\n{INDENT}/// <returns>The encoded data</returns>"
-        class_definition += f"\n{INDENT}public byte[] ToByteArray(string contentTypeString)\n{INDENT}{{"
-        class_definition += f'\n{INDENT*2}'.join((PREAMBLE_TOBYTEARRAY).split("\n"))
-        if self.avro_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                AVRO_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-        if self.system_text_json_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                SYSTEM_TEXT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-        if self.newtonsoft_json_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                NEWTONSOFT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-        if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
-            class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY_COMPRESSION).split("\n"))
-        class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY).split("\n"))+f"\n{INDENT}}}"
-
-        # emit FromData factory method
-        class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Creates an object from the data\n{INDENT}/// </summary>"
-        class_definition += f"\n{INDENT}/// <param name=\"data\">The input data to convert</param>"
-        class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the derired encoding</param>"
-        class_definition += f"\n{INDENT}/// <returns>The converted object</returns>"
-        class_definition += f"\n{INDENT}public static {class_name}? FromData(object? data, string? contentTypeString )\n{INDENT}{{"
-        class_definition += f'\n{INDENT*2}if ( data == null ) return null;'
-        class_definition += f'\n{INDENT*2}if ( data is {class_name}) return ({class_name})data;'
-        class_definition += f'\n{INDENT*2}if ( contentTypeString == null ) contentTypeString = System.Net.Mime.MediaTypeNames.Application.Octet;'
-        class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA)).split("\n"))
         if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
-            class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA_COMPRESSION)).split("\n"))
-        if self.avro_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                AVRO_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-        if self.system_text_json_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                SYSTEM_TEXT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-        if self.newtonsoft_json_annotation:
-            class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                NEWTONSOFT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-        class_definition += f"\n{INDENT*2}".join((EPILOGUE_FROMDATA).split('\n'))+f"\n{INDENT}}}"
+            class_definition += f"\n{INDENT}/// <summary>\n{INDENT}/// Converts the object to a byte array\n{INDENT}/// </summary>"
+            class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the desired encoding</param>"
+            class_definition += f"\n{INDENT}/// <returns>The encoded data</returns>"
+            class_definition += f"\n{INDENT}public byte[] ToByteArray(string contentTypeString)\n{INDENT}{{"
+            class_definition += f'\n{INDENT*2}'.join((PREAMBLE_TOBYTEARRAY).split("\n"))
+            if self.avro_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    AVRO_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
+            if self.system_text_json_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    SYSTEM_TEXT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
+            if self.newtonsoft_json_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    NEWTONSOFT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
+            if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
+                class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY_COMPRESSION).split("\n"))
+            class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY).split("\n"))+f"\n{INDENT}}}"
+
+            # emit FromData factory method
+            class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Creates an object from the data\n{INDENT}/// </summary>"
+            class_definition += f"\n{INDENT}/// <param name=\"data\">The input data to convert</param>"
+            class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the derired encoding</param>"
+            class_definition += f"\n{INDENT}/// <returns>The converted object</returns>"
+            class_definition += f"\n{INDENT}public static {class_name}? FromData(object? data, string? contentTypeString )\n{INDENT}{{"
+            class_definition += f'\n{INDENT*2}if ( data == null ) return null;'
+            class_definition += f'\n{INDENT*2}if ( data is {class_name}) return ({class_name})data;'
+            class_definition += f'\n{INDENT*2}if ( contentTypeString == null ) contentTypeString = System.Net.Mime.MediaTypeNames.Application.Octet;'
+            class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA)).split("\n"))
+            if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
+                class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA_COMPRESSION)).split("\n"))
+            if self.avro_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    AVRO_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
+            if self.system_text_json_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    SYSTEM_TEXT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
+            if self.newtonsoft_json_annotation:
+                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
+                    NEWTONSOFT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
+            class_definition += f"\n{INDENT*2}".join((EPILOGUE_FROMDATA).split('\n'))+f"\n{INDENT}}}"
 
-        # emit IsJsonMatch method for System.Text.Json
-        if self.system_text_json_annotation:
-            class_definition += self.create_is_json_match_method(avro_schema, avro_namespace, class_name)
+            # emit IsJsonMatch method for System.Text.Json
+            if self.system_text_json_annotation:
+                class_definition += self.create_is_json_match_method(avro_schema, avro_namespace, class_name)
         class_definition += "\n"+"}"
 
         if write_file:
             self.write_to_file(namespace, class_name, class_definition)
         ref = 'global::'+self.concat_namespace(namespace, class_name)
         self.generated_types[ref] = "class"
         return ref
@@ -478,17 +514,19 @@
         
         if write_file:
             self.write_to_file(namespace, enum_name, enum_definition)
         ref = 'global::'+self.concat_namespace(namespace, enum_name)
         self.generated_types[ref] = "enum"
         return ref
 
-    def generate_embedded_union_class_system_json_text(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
+    def generate_embedded_union(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
         """ Generates an embedded Union Class """
-        class_definition_ctors = class_definition_decls = class_definition_read = class_definition_write = class_definition = ''
+        class_definition_ctors = class_definition_decls = class_definition_read = ''
+        class_definition_write = class_definition = class_definition_toobject = ''
+        class_definition_objctr = class_definition_genericrecordctor = ''
         list_is_json_match: List [str] = []
         union_class_name = pascal(field_name)+'Union'
         union_types = [self.convert_avro_type_to_csharp(class_name, field_name+"Option"+str(i), t, parent_namespace) for i,t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             is_dict = is_list = False
             if union_type.startswith("Dictionary<"):
                 # get the type information from the dictionary
@@ -502,20 +540,25 @@
                 union_type_name = "Array" + pascal(match[0].rsplit('.', 1)[-1])
             elif union_type == "byte[]":
                 union_type_name = "bytes"
             else:
                 union_type_name = union_type.rsplit('.', 1)[-1]
             if self.is_csharp_reserved_word(union_type_name):
                 union_type_name = f"@{union_type_name}"
+            class_definition_objctr += f"{INDENT*3}if (obj is {union_type})\n{INDENT*3}{{\n{INDENT*4}self.{union_type_name} = ({union_type})obj;\n{INDENT*4}return self;\n{INDENT*3}}}\n"
+            if union_type in self.generated_types and self.generated_types[union_type] == "class":
+                class_definition_genericrecordctor += f"{INDENT*3}if (obj.Schema.Fullname == {union_type}.AvroSchema.Fullname)\n{INDENT*3}{{\n{INDENT*4}this.{union_type_name} = new {union_type}(obj);\n{INDENT*4}return;\n{INDENT*3}}}\n"     
             class_definition_ctors += \
                 f"{INDENT*2}/// <summary>\n{INDENT*2}/// Constructor for {union_type_name} values\n{INDENT*2}/// </summary>\n" + \
                 f"{INDENT*2}public {union_class_name}({union_type}? {union_type_name})\n{INDENT*2}{{\n{INDENT*3}this.{union_type_name} = {union_type_name};\n{INDENT*2}}}\n"
             class_definition_decls += \
                 f"{INDENT*2}/// <summary>\n{INDENT*2}/// Gets the {union_type_name} value\n{INDENT*2}/// </summary>\n" + \
-                f"{INDENT*2}public {union_type}? {union_type_name} {{ get; private set; }} = null;\n"            
+                f"{INDENT*2}public {union_type}? {union_type_name} {{ get; private set; }} = null;\n"     
+            class_definition_toobject += f"{INDENT*3}if ({union_type_name} != null) {{\n{INDENT*4}return {union_type_name};\n{INDENT*3}}}\n"
+              
             if is_dict:
                 class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.Object)\n{INDENT*3}{{\n" + \
                         f"{INDENT*4}var map = System.Text.Json.JsonSerializer.Deserialize<{union_type}>(element, options);\n" + \
                         f"{INDENT*4}if (map != null) {{ return new {union_class_name}(map); }} else {{ throw new NotSupportedException(); }};\n" + \
                         f"{INDENT*3}}}\n"
             elif is_list:
                 class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.Array)\n{INDENT*3}{{\n" + \
@@ -540,31 +583,68 @@
             class_definition_write += f"{INDENT*3}{'else ' if i>0 else ''}if (value.{union_type_name} != null)\n{INDENT*3}{{\n{INDENT*4}System.Text.Json.JsonSerializer.Serialize(writer, value.{union_type_name}, options);\n{INDENT*3}}}\n"
             gij = self.get_is_json_match_clause_type("element", class_name, union_type)
             if gij:
                 list_is_json_match.append(gij)
 
         class_definition = \
             f"/// <summary>\n/// {class_name}. Type union resolver. \n/// </summary>\n" + \
-            f"public partial class {class_name}\n{{\n{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof({union_class_name}))]\n{INDENT}public sealed class {union_class_name} : System.Text.Json.Serialization.JsonConverter<{union_class_name}>\n{INDENT}{{\n" + \
+            f"public partial class {class_name}\n{{\n" + \
+            f"{INDENT}/// <summary>\n{INDENT}/// Union class for {field_name}\n{INDENT}/// </summary>\n"
+        if self.system_text_json_annotation:
+            class_definition += \
+                f"{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof({union_class_name}))]\n"
+        class_definition += \
+            f"{INDENT}public sealed class {union_class_name}"
+        if self.system_text_json_annotation:
+            class_definition += f": System.Text.Json.Serialization.JsonConverter<{union_class_name}>"
+        class_definition += f"\n{INDENT}{{\n" + \
             f"{INDENT*2}/// <summary>\n{INDENT*2}/// Default constructor\n{INDENT*2}/// </summary>\n" + \
-            f"{INDENT*2}public {union_class_name}() {{ }}\n" + \
-            class_definition_ctors + \
+            f"{INDENT*2}public {union_class_name}() {{ }}\n"
+        class_definition += class_definition_ctors
+        if self.avro_annotation:
+            class_definition += \
+                f"{INDENT*2}/// <summary>\n{INDENT*2}/// Constructor for Avro decoder\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}internal static {union_class_name} FromObject(object obj)\n{INDENT*2}{{\n"
+            if class_definition_genericrecordctor:
+                class_definition += \
+                    f"{INDENT*3}if (obj is global::Avro.Generic.GenericRecord)\n{INDENT*3}{{\n" + \
+                    f"{INDENT*4}return new {union_class_name}((global::Avro.Generic.GenericRecord)obj);\n" + \
+                    f"{INDENT*3}}}\n"                    
+            class_definition += \
+                f"{INDENT*3}var self = new {union_class_name}();\n" + \
+                class_definition_objctr + \
+                f"{INDENT*3}throw new NotSupportedException(\"No record type matched the type\");\n" + \
+                f"{INDENT*2}}}\n"
+            if class_definition_genericrecordctor:
+                class_definition += f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Constructor from Avro GenericRecord\n{INDENT*2}/// </summary>\n" + \
+                    f"{INDENT*2}public {union_class_name}(global::Avro.Generic.GenericRecord obj)\n{INDENT*2}{{\n" + \
+                    class_definition_genericrecordctor + \
+                    f"{INDENT*3}throw new NotSupportedException(\"No record type matched the type\");\n" + \
+                    f"{INDENT*2}}}\n"
+        class_definition += \
             class_definition_decls + \
-            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Reads the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
-            f"{INDENT*2}public override {union_class_name}? Read(ref Utf8JsonReader reader, Type typeToConvert, JsonSerializerOptions options)\n{INDENT*2}{{\n{INDENT*3}var element = JsonElement.ParseValue(ref reader);\n" + \
-            class_definition_read + \
-            f"{INDENT*3}throw new NotSupportedException(\"No record type matched the JSON data\");\n{INDENT*2}}}\n" + \
-            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Writes the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
-            f"{INDENT*2}public override void Write(Utf8JsonWriter writer, {union_class_name} value, JsonSerializerOptions options)\n{INDENT*2}{{\n" + \
-            class_definition_write + \
-            f"{INDENT*3}else\n{INDENT*3}{{\n{INDENT*4}throw new NotSupportedException(\"No record type is set in the union\");\n{INDENT*3}}}\n{INDENT*2}}}\n" + \
-            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Checks if the JSON element matches the schema\n{INDENT*2}/// </summary>\n" + \
-            f"{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
-            f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n" + \
-            f"{INDENT*1}}}\n}}\n"
+            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Yields the current value of the union\n{INDENT*2}/// </summary>\n" + \
+            f"\n{INDENT*2}public Object ToObject()\n{INDENT*2}{{\n" + \
+            class_definition_toobject+ \
+            f"{INDENT*3}throw new NotSupportedException(\"No record type is set in the union\");\n" + \
+            f"{INDENT*2}}}\n"
+        if self.system_text_json_annotation:
+            class_definition += \
+                f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Reads the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}public override {union_class_name}? Read(ref Utf8JsonReader reader, Type typeToConvert, JsonSerializerOptions options)\n{INDENT*2}{{\n{INDENT*3}var element = JsonElement.ParseValue(ref reader);\n" + \
+                class_definition_read + \
+                f"{INDENT*3}throw new NotSupportedException(\"No record type matched the JSON data\");\n{INDENT*2}}}\n" + \
+                f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Writes the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}public override void Write(Utf8JsonWriter writer, {union_class_name} value, JsonSerializerOptions options)\n{INDENT*2}{{\n" + \
+                class_definition_write + \
+                f"{INDENT*3}else\n{INDENT*3}{{\n{INDENT*4}throw new NotSupportedException(\"No record type is set in the union\");\n{INDENT*3}}}\n{INDENT*2}}}\n" + \
+                f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Checks if the JSON element matches the schema\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
+                f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n"
+        class_definition += f"{INDENT}}}\n}}"
 
         if write_file:
             self.write_to_file(pascal(parent_namespace), class_name +"."+union_class_name, class_definition)
         self.generated_types[class_name+'.'+union_class_name] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
         return union_class_name
 
     def find_type(self, kind: str, avro_schema: JsonNode, type_name: str, type_namespace: str, parent_namespace = '') -> JsonNode:
@@ -634,16 +714,15 @@
             # Common using statements (add more as needed)
             file_content = "#pragma warning disable CS8618\n#pragma warning disable CS8603\n\nusing System;\nusing System.Collections.Generic;\n"
             if self.system_text_json_annotation:
                 file_content += "using System.Text.Json;\n"
                 file_content += "using System.Text.Json.Serialization;\n"
             if self.newtonsoft_json_annotation:
                 file_content += "using Newtonsoft.Json;\n"
-            if self.avro_annotation:
-                file_content += "using Avro;\nusing Avro.Specific;\n"
+            
             # Namespace declaration with correct indentation for the definition
             file_content += f"\nnamespace {namespace}\n{{\n"
             indented_definition = '\n'.join(
                 [f"{INDENT}{line}" for line in definition.split('\n')])
             file_content += f"{indented_definition}\n}}"
             file.write(file_content)
```

### Comparing `avrotize-1.4.1/avrotize/avrotojava.py` & `avrotize-1.5.0/avrotize/avrotojava.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,51 +119,47 @@
 }
 """
 
 AVRO_FROMDATA_THROWS = ",IOException"
 AVRO_FROMDATA = \
     """
 if ( mediaType == "avro/binary" || mediaType == "application/vnd.apache.avro+avro") {
-    DatumReader<{typeName}> reader = new SpecificDatumReader<{typeName}>({typeName}.AvroSchema);
     if (data instanceof byte[]) {
-        return reader.read(new {typeName}(), DecoderFactory.get().binaryDecoder((byte[])data, null));
+        return AVROREADER.read(new {typeName}(), DecoderFactory.get().binaryDecoder((byte[])data, null));
     } else if (data instanceof InputStream) {
-        return reader.read(new {typeName}(), DecoderFactory.get().binaryDecoder((InputStream)data, null));
+        return AVROREADER.read(new {typeName}(), DecoderFactory.get().binaryDecoder((InputStream)data, null));
     }
     throw new UnsupportedOperationException("Data is not of a supported type for Avro conversion to {typeName}");
 } else if ( mediaType == "avro/json" || mediaType == "application/vnd.apache.avro+json") {
-    DatumReader<{typeName}> reader = new SpecificDatumReader<{typeName}>({typeName}.AvroSchema);
     if (data instanceof byte[]) {
-        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, new ByteArrayInputStream((byte[])data)));
+        return AVROREADER.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AVROSCHEMA, new ByteArrayInputStream((byte[])data)));
     } else if (data instanceof InputStream) {
-        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, (InputStream)data));
+        return AVROREADER.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AVROSCHEMA, (InputStream)data));
     } else if (data instanceof String) {
-        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, (String)data));
+        return AVROREADER.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AVROSCHEMA, (String)data));
     }
     throw new UnsupportedOperationException("Data is not of a supported type for Avro conversion to {typeName}");
 }
 """
 
 
 AVRO_TOBYTEARRAY_THROWS = ",IOException"
 AVRO_TOBYTEARRAY = \
     """
 if ( mediaType == "avro/binary" || mediaType == "application/vnd.apache.avro+avro") {
-    DatumWriter<{typeName}> writer = new SpecificDatumWriter<{typeName}>({typeName}.AvroSchema);
     ByteArrayOutputStream out = new ByteArrayOutputStream();
     Encoder encoder = EncoderFactory.get().binaryEncoder(out, null);
-    writer.write(this, encoder);
+    AVROWRITER.write(this, encoder);
     encoder.flush();
     result = out.toByteArray();
 }
 else if ( mediaType == "avro/json" || mediaType == "application/vnd.apache.avro+json") {
-    DatumWriter<{typeName}> writer = new SpecificDatumWriter<{typeName}>({typeName}.AvroSchema);
     ByteArrayOutputStream out = new ByteArrayOutputStream();
-    Encoder encoder = EncoderFactory.get().jsonEncoder({typeName}.AvroSchema, out);
-    writer.write(this, encoder);
+    Encoder encoder = EncoderFactory.get().jsonEncoder({typeName}.AVROSCHEMA, out);
+    AVROWRITER.write(this, encoder);
     encoder.flush();
     result = out.toByteArray();
 }
 """
 
 
 JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | None
@@ -364,24 +360,27 @@
         
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')
             avro_schema_json = f"\"+\n{INDENT}\"".join(
                 [avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
-            class_definition += f"\n\n{INDENT}public static Schema AvroSchema = new Schema.Parser().parse(\n{INDENT}\"{avro_schema_json}\");\n"
+            class_definition += f"\n\n{INDENT}public static final Schema AVROSCHEMA = new Schema.Parser().parse(\n{INDENT}\"{avro_schema_json}\");"
+            class_definition += f"\n{INDENT}public static final DatumWriter<{class_name}> AVROWRITER = new SpecificDatumWriter<{class_name}>(AVROSCHEMA);"
+            class_definition += f"\n{INDENT}public static final DatumReader<{class_name}> AVROREADER = new SpecificDatumReader<{class_name}>(AVROSCHEMA);\n"
+            
             if self.jackson_annotations:
                 class_definition += f"\n{INDENT}@JsonIgnore"
-            class_definition += f"\n{INDENT}@Override\n{INDENT}public Schema getSchema(){{ return AvroSchema; }}\n"
+            class_definition += f"\n{INDENT}@Override\n{INDENT}public Schema getSchema(){{ return AVROSCHEMA; }}\n"
             class_definition += self.generate_avro_get_method(class_name, avro_schema.get('fields', []), namespace)
             class_definition += self.generate_avro_put_method(class_name, avro_schema.get('fields', []), namespace)
 
         # emit toByteArray method
         class_definition += f"\n\n{INDENT}/**\n{INDENT} * Converts the object to a byte array\n{INDENT} * @param contentType the content type of the byte array\n{INDENT} * @return the byte array\n{INDENT} */\n"
-        class_definition += f"\n\n{INDENT}public byte[] toByteArray(String contentType) throws UnsupportedOperationException" + \
+        class_definition += f"{INDENT}public byte[] toByteArray(String contentType) throws UnsupportedOperationException" + \
             f"{ JSON_TOBYTEARRAY_THROWS if self.jackson_annotations else '' }" + \
             f"{ AVRO_TOBYTEARRAY_THROWS if self.avro_annotation else '' }  {{"
         if self.jackson_annotations or self.avro_annotation:
             class_definition += f'\n{INDENT*2}'.join((PREAMBLE_TOBYTEARRAY).split("\n"))
         if self.avro_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 AVRO_TOBYTEARRAY.strip().replace("{typeName}", class_name).split("\n"))
@@ -391,15 +390,15 @@
         if self.avro_annotation or self.jackson_annotations:
             class_definition += f'\n{INDENT*2}'.join(EPILOGUE_TOBYTEARRAY_COMPRESSION.split("\n"))
             class_definition += f'\n{INDENT*2}if ( result != null ) {{ return result; }}'        
         class_definition += (f'\n{INDENT*2}'.join((EPILOGUE_TOBYTEARRAY.strip()).split("\n")))+f"\n{INDENT}}}"
 
         # emit fromData factory method
         class_definition += f"\n\n{INDENT}/**\n{INDENT} * Converts the data to an object\n{INDENT} * @param data the data to convert\n{INDENT} * @param contentType the content type of the data\n{INDENT} * @return the object\n{INDENT} */\n"
-        class_definition += f"\n\n{INDENT}public static {class_name} fromData(Object data, String contentType) throws UnsupportedOperationException" + \
+        class_definition += f"{INDENT}public static {class_name} fromData(Object data, String contentType) throws UnsupportedOperationException" + \
             f"{ JSON_FROMDATA_THROWS if self.jackson_annotations else '' }" + \
             f"{ AVRO_FROMDATA_THROWS if self.avro_annotation else '' }  {{"
         class_definition += f'\n{INDENT*2}if ( data instanceof {class_name}) return ({class_name})data;'
         
         if self.avro_annotation or self.jackson_annotations:
             class_definition += f'\n{INDENT*2}String mediaType = contentType.split(";")[0].trim().toLowerCase();'
             class_definition += f'\n{INDENT*2}'.join((PREAMBLE_FROMDATA_COMPRESSION).split("\n"))
@@ -712,15 +711,15 @@
             class_definition_decls += \
                 f"{INDENT*1}private {union_type.type_name} _{camel(union_variable_name)};\n" + \
                 f"{INDENT*1}public {union_type.type_name} get{union_variable_name}() {{ return _{camel(union_variable_name)}; }}\n";
                 
             class_definition_toobject += f"{INDENT*2}if (_{camel(union_variable_name)} != null) {{\n{INDENT*3}return _{camel(union_variable_name)};\n{INDENT*2}}}\n"
             
             if self.avro_annotation and union_type.is_class:            
-                class_definition_genericrecordctor += f"{INDENT*2}if ( {union_type.type_name}.AvroSchema.getName().equals(record.getSchema().getName()) && {union_type.type_name}.AvroSchema.getNamespace().equals(record.getSchema().getNamespace()) ) {{"
+                class_definition_genericrecordctor += f"{INDENT*2}if ( {union_type.type_name}.AVROSCHEMA.getName().equals(record.getSchema().getName()) && {union_type.type_name}.AVROSCHEMA.getNamespace().equals(record.getSchema().getNamespace()) ) {{"
                 class_definition_genericrecordctor += f"\n{INDENT*3}this._{camel(union_variable_name)} = new {union_type.type_name}(record);\n{INDENT*3}return;\n{INDENT*2}}}\n"
             
             # there can only be one list and one map in the union, so we don't need to differentiate this any further
             if is_list:
                 class_definition_fromobjectctor += f"{INDENT*2}if (obj instanceof List<?>) {{\n{INDENT*3}this._{camel(union_variable_name)} = ({union_type.type_name})obj;\n{INDENT*3}return;\n{INDENT*2}}}\n"
             elif is_dict:
                 class_definition_fromobjectctor += f"{INDENT*2}if (obj instanceof Map<?,?>) {{\n{INDENT*3}this._{camel(union_variable_name)} = ({union_type.type_name})obj;\n{INDENT*3}return;\n{INDENT*2}}}\n"
```

### Comparing `avrotize-1.4.1/avrotize/avrotojs.py` & `avrotize-1.5.0/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotojsons.py` & `avrotize-1.5.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotokusto.py` & `avrotize-1.5.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotoparquet.py` & `avrotize-1.5.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotoproto.py` & `avrotize-1.5.0/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotopython.py` & `avrotize-1.5.0/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotots.py` & `avrotize-1.5.0/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrototsql.py` & `avrotize-1.5.0/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/avrotoxsd.py` & `avrotize-1.5.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/common.py` & `avrotize-1.5.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/dependency_resolver.py` & `avrotize-1.5.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/generic/generic.avsc` & `avrotize-1.5.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/jsonstoavro.py` & `avrotize-1.5.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/kconnect.json` & `avrotize-1.5.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/kstructtoavro.py` & `avrotize-1.5.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/proto2parser.py` & `avrotize-1.5.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/proto3parser.py` & `avrotize-1.5.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototoavro.py` & `avrotize-1.5.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/any.avsc` & `avrotize-1.5.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/api.avsc` & `avrotize-1.5.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/duration.avsc` & `avrotize-1.5.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/field_mask.avsc` & `avrotize-1.5.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/struct.avsc` & `avrotize-1.5.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/timestamp.avsc` & `avrotize-1.5.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/type.avsc` & `avrotize-1.5.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/prototypes/wrappers.avsc` & `avrotize-1.5.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/avrotize/xsdtoavro.py` & `avrotize-1.5.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/pyproject.toml` & `avrotize-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.1/PKG-INFO` & `avrotize-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.4.1
+Version: 1.5.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -446,26 +446,30 @@
 Parameters:
 - `--avsc`: The path to the Avro schema file to be converted.
 - `--csharp`: The path to the C# directory to write the conversion result to.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
 - `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
 - `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
+- `--namespace`: (optional) The namespace to use in the generated C# classes.
 
 Conversion notes:
 - The tool generates C# classes that represent the Avro schema as data classes.
 - Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
   will add annotations for the respective JSON serialization library to the generated
   C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
   preserves the JSON Schema structure in the Avro schema, the generated C# classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
+- Only the `--system-text-json-annotation` option generates classes that support type unions.
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `.csproj` project file into the given
   directory if none exists.
 
+Read more about the C# code generation in the [C# code generation documentation](csharpcodegen.md).
+
 
 ### Generate Java code from Avro schema
 
 ```bash
 avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
 ```
 
@@ -486,14 +490,16 @@
   preserves the JSON Schema structure in the Avro schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
+Read more about the Java code generation in the [Java code generation documentation](javacodegen.md).
+
 ### Generate Python code from Avro schema
 
 This command generates Python dataclasses from an Avro schema.
 
 ```bash
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
```

