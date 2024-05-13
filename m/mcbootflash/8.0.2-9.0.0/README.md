# Comparing `tmp/mcbootflash-8.0.2.tar.gz` & `tmp/mcbootflash-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbootflash-8.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mcbootflash-9.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mcbootflash-8.0.2.tar` & `mcbootflash-9.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/.github/workflows/main.yml
--rw-r--r--   0        0        0     3090 2022-06-08 18:37:37.758584 mcbootflash-8.0.2/.gitignore
--rw-r--r--   0        0        0    10422 2024-05-11 15:49:58.395449 mcbootflash-8.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1058 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/LICENSE
--rw-r--r--   0        0        0     3583 2023-11-10 18:57:54.826438 mcbootflash-8.0.2/README.md
--rw-r--r--   0        0        0      465 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/docs/api.md
--rw-r--r--   0        0        0       44 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/changelog.md
--rw-r--r--   0        0        0     3473 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/develop.md
--rw-r--r--   0        0        0       41 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/docs/index.md
--rw-r--r--   0        0        0      836 2024-02-10 19:54:03.187436 mcbootflash-8.0.2/mkdocs.yml
--rw-r--r--   0        0        0     1732 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/pyproject.toml
--rw-r--r--   0        0        0      685 2024-05-11 15:43:36.176115 mcbootflash-8.0.2/src/mcbootflash/__init__.py
--rw-r--r--   0        0        0     7590 2024-05-11 15:43:36.176115 mcbootflash-8.0.2/src/mcbootflash/__main__.py
--rw-r--r--   0        0        0      989 2023-11-09 22:11:17.471011 mcbootflash-8.0.2/src/mcbootflash/error.py
--rw-r--r--   0        0        0    12015 2024-05-11 15:43:36.180115 mcbootflash-8.0.2/src/mcbootflash/flash.py
--rw-r--r--   0        0        0     8775 2024-02-10 19:54:46.070837 mcbootflash-8.0.2/src/mcbootflash/types.py
--rw-r--r--   0        0        0     1545 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/src/mcbootflash/util.py
--rw-r--r--   0        0        0   107316 2024-05-11 15:43:36.180115 mcbootflash-8.0.2/tests/test_mcbootflash.json
--rw-r--r--   0        0        0     6248 2024-05-11 15:49:58.395449 mcbootflash-8.0.2/tests/test_mcbootflash.py
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/checksum_error/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/flash/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/flash_empty/test.hex
--rw-r--r--   0        0        0     2932 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/no_data/test.hex
--rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-8.0.2/tests/testcases/no_response/test.hex
--rw-r--r--   0        0        0      565 2024-02-10 19:54:03.191436 mcbootflash-8.0.2/tox.ini
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 mcbootflash-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3090 2022-06-08 18:37:37.758584 mcbootflash-9.0.0/.gitignore
+-rw-r--r--   0        0        0    11498 2024-05-13 19:58:10.674425 mcbootflash-9.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1058 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/LICENSE
+-rw-r--r--   0        0        0     3583 2023-11-10 18:57:54.826438 mcbootflash-9.0.0/README.md
+-rw-r--r--   0        0        0      465 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/docs/api.md
+-rw-r--r--   0        0        0       44 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/changelog.md
+-rw-r--r--   0        0        0     3473 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/develop.md
+-rw-r--r--   0        0        0       41 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/docs/index.md
+-rw-r--r--   0        0        0      836 2024-02-10 19:54:03.187436 mcbootflash-9.0.0/mkdocs.yml
+-rw-r--r--   0        0        0     1732 2024-02-10 19:54:03.191436 mcbootflash-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0      685 2024-05-13 20:06:51.233865 mcbootflash-9.0.0/src/mcbootflash/__init__.py
+-rw-r--r--   0        0        0     7250 2024-05-13 19:54:58.266181 mcbootflash-9.0.0/src/mcbootflash/__main__.py
+-rw-r--r--   0        0        0      989 2023-11-09 22:11:17.471011 mcbootflash-9.0.0/src/mcbootflash/error.py
+-rw-r--r--   0        0        0    11757 2024-05-13 19:54:06.757043 mcbootflash-9.0.0/src/mcbootflash/flash.py
+-rw-r--r--   0        0        0     8642 2024-05-13 19:54:06.757043 mcbootflash-9.0.0/src/mcbootflash/types.py
+-rw-r--r--   0        0        0     1545 2024-05-13 19:51:55.886146 mcbootflash-9.0.0/src/mcbootflash/util.py
+-rw-r--r--   0        0        0   101873 2024-05-13 19:56:09.803760 mcbootflash-9.0.0/tests/test_mcbootflash.json
+-rw-r--r--   0        0        0     5427 2024-05-13 19:56:09.803760 mcbootflash-9.0.0/tests/test_mcbootflash.py
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/checksum_error/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/flash/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/flash_empty/test.hex
+-rw-r--r--   0        0        0     2932 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/no_data/test.hex
+-rw-r--r--   0        0        0     5628 2022-12-03 16:05:22.909458 mcbootflash-9.0.0/tests/testcases/no_response/test.hex
+-rw-r--r--   0        0        0      565 2024-02-10 19:54:03.191436 mcbootflash-9.0.0/tox.ini
+-rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 mcbootflash-9.0.0/PKG-INFO
```

### Comparing `mcbootflash-8.0.2/.github/workflows/main.yml` & `mcbootflash-9.0.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/.gitignore` & `mcbootflash-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/CHANGELOG.md` & `mcbootflash-9.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 # Changelog
 
-## [8.0.3] - Development
+## [9.0.1] - Development
+
+## [9.0.0] - 2024-05-13
+
+### Changed
+
+- Disable checksumming by default in CLI, enable with `--checksum` flag ([`b685bb5`](https://github.com/bessman/mcbootflash/commit/b685bb56165805706fdc87adcba76c1285cc3416))
+- Unconditionally erase before flashing with CLI ([`9a4ddc6`](https://github.com/bessman/mcbootflash/commit/9a4ddc629b1df47fe06149ceafdc3f4131a5e6e6))
+
+### Added
+
+- Add CLI flag `--reset` to reset device after flashing ([`e38cefb`](https://github.com/bessman/mcbootflash/commit/e38cefbfee740b46c994d678f1fd884d8caeec9c))
+
+### Removed
+
+- __Breaking__: Remove `.has_checksum` attribute of `BootAttrs` ([`b685bb5`](https://github.com/bessman/mcbootflash/commit/b685bb56165805706fdc87adcba76c1285cc3416))
+
+### Fixed
+
+- Fix error messages not being shown in CLI ([`c499eb9`](https://github.com/bessman/mcbootflash/commit/c499eb94f193b2910aed6c6fb62f108854ce8026))
+- Fix wrong pad value in `chunked` ([`58ad227`](https://github.com/bessman/mcbootflash/commit/58ad227b9304ddea3f9c0e4acad1494901a47031))
 
 ## [8.0.2] - 2024-05-11
 
 ### Fixed
 
 - Continue with warning on `BadAddress` during checksum ([`b8734ea`](https://github.com/bessman/mcbootflash/commit/b8734ea2d4b63a3ae005031629a1b6c73c83dd49))
 
@@ -240,14 +260,15 @@
 
 - Fix off-by-one error when firmware uses all available space
 
 ## [1.0.0] - 2022-05-27
 
 _Initial release._
 
+[9.0.0]: https://github.com/bessman/mcbootflash/releases/tag/9.0.0
 [8.0.2]: https://github.com/bessman/mcbootflash/releases/tag/8.0.2
 [8.0.1]: https://github.com/bessman/mcbootflash/releases/tag/8.0.1
 [8.0.0]: https://github.com/bessman/mcbootflash/releases/tag/v8.0.0
 [7.0.6]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.6
 [7.0.5]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.5
 [7.0.4]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.4
 [7.0.3]: https://github.com/bessman/mcbootflash/releases/tag/v7.0.3
```

### Comparing `mcbootflash-8.0.2/LICENSE` & `mcbootflash-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/README.md` & `mcbootflash-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/docs/develop.md` & `mcbootflash-9.0.0/docs/develop.md`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/mkdocs.yml` & `mcbootflash-9.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/pyproject.toml` & `mcbootflash-9.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/src/mcbootflash/__init__.py` & `mcbootflash-9.0.0/src/mcbootflash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "erase_flash",
     "get_boot_attrs",
     "reset",
     "self_verify",
     "write_flash",
 ]
 
-__version__ = "8.0.2"
+__version__ = "9.0.0"
```

### Comparing `mcbootflash-8.0.2/src/mcbootflash/__main__.py` & `mcbootflash-9.0.0/src/mcbootflash/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,30 @@
         required=True,
         help="symbol rate of device's serial bus",
     )
     parser.add_argument(
         "-t",
         "--timeout",
         type=float,
-        default=5,
+        default=10,
         help="try to read data from the bus for this many seconds before giving up",
     )
     parser.add_argument(
+        "-c",
+        "--checksum",
+        action="store_true",
+        help="verify flashed data by checksumming after write",
+    )
+    parser.add_argument(
+        "-r",
+        "--reset",
+        action="store_true",
+        help="reset device after flashing is complete",
+    )
+    parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="print debug messages",
     )
     parser.add_argument(
         "-q",
@@ -104,54 +116,38 @@
             port=args.port,
             baudrate=args.baudrate,
             timeout=args.timeout,
         )
         bootattrs = mcbf.get_boot_attrs(connection)
         _logger.info("Connected")
         total_bytes, chunks = mcbf.chunked(args.hexfile, bootattrs)
-        connection.timeout *= 10
-        erase(connection, bootattrs.memory_range, bootattrs.erase_size)
-        connection.timeout /= 10
+        _logger.debug("Erasing program area...")
+        mcbf.erase_flash(connection, bootattrs.memory_range, bootattrs.erase_size)
         _logger.info(f"Flashing {args.hexfile}")
         flash(
             connection=connection,
             chunks=chunks,
             total_bytes=total_bytes,
-            bootattrs=bootattrs,
+            checksum=args.checksum,
         )
         mcbf.self_verify(connection)
         _logger.info("Self verify OK")
-    except Exception as exc:  # noqa: BLE001
-        _logger.error(exc)  # noqa: TRY400
-        _logger.debug("", exc_info=True)
 
-
-def erase(connection: Serial, erase_range: tuple[int, int], erase_size: int) -> None:
-    """Erase flash if an application is detected, and verify erasure."""
-    try:
-        mcbf.self_verify(connection)
-        _logger.info("Existing application detected, erasing...")
-        mcbf.erase_flash(connection, erase_range, erase_size)
-    except mcbf.VerifyFail:
-        _logger.info("No application detected, skipping erase")
-        return
-
-    try:
-        mcbf.self_verify(connection)
-        msg = "Erase failed"
-        raise mcbf.BootloaderError(msg)
-    except mcbf.VerifyFail:
-        _logger.info("Application erased")
+        if args.reset:
+            mcbf.reset(connection)
+    except Exception:
+        _logger.exception("An error occurred:")
 
 
 def flash(
     connection: Serial,
     chunks: Iterator[mcbf.Chunk],
+    *,
     total_bytes: int,
-    bootattrs: mcbf.BootAttrs,
+    checksum: bool,
 ) -> None:
     """Flash application firmware.
 
     Parameters
     ----------
     connection : serial.Serial
         Open serial connection to device in bootloader mode.
@@ -164,15 +160,15 @@
     """
     written_bytes = 0
     start = time.time()
 
     for chunk in chunks:
         mcbf.write_flash(connection, chunk)
 
-        if bootattrs.has_checksum:
+        if checksum:
             mcbf.checksum(connection, chunk)
 
         written_bytes += len(chunk.data)
         _logger.debug(
             f"{written_bytes} bytes written of {total_bytes} "
             f"({written_bytes / total_bytes * 100:.2f}%)",
         )
```

### Comparing `mcbootflash-8.0.2/src/mcbootflash/error.py` & `mcbootflash-9.0.0/src/mcbootflash/error.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/src/mcbootflash/flash.py` & `mcbootflash-9.0.0/src/mcbootflash/flash.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,29 +66,21 @@
         max_packet_length,
         device_id,
         erase_size,
         write_size,
     ) = _read_version(connection)
     memory_range = _get_memory_address_range(connection)
 
-    try:
-        _get_remote_checksum(connection, memory_range[0], write_size)
-        has_checksum = True
-    except UnsupportedCommand:
-        _logger.warning("Bootloader does not support checksumming")
-        has_checksum = False
-
     return BootAttrs(
         version,
         max_packet_length,
         device_id,
         erase_size,
         write_size,
         memory_range,
-        has_checksum,
     )
 
 
 def _read_version(connection: Connection) -> tuple[int, int, int, int, int]:
     """Read bootloader version and some other useful information.
 
     Parameters
```

### Comparing `mcbootflash-8.0.2/src/mcbootflash/types.py` & `mcbootflash-9.0.0/src/mcbootflash/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,25 +227,22 @@
         area which should be erased is given in number of erase pages.
     write_size : int
         Size of a write block in bytes. When writing to flash, the data must align with
         a write block.
     memory_range : tuple[int, int]
         Tuple of addresses specifying the program memory range. The range is half-open,
         i.e. the upper address is not part of the program memory range.
-    has_checksum : bool
-        Indicates whether or not the bootloader supports the `CALC_CHECKSUM` command.
     """
 
     version: int
     max_packet_length: int
     device_id: int
     erase_size: int
     write_size: int
     memory_range: tuple[int, int]
-    has_checksum: bool
 
 
 class Chunk(Protocol):
     """A piece of a firmware image.
 
     `mcbootflash.chunked` can be used to generate correctly aligned and sized chunks
     from a HEX file.
```

### Comparing `mcbootflash-8.0.2/src/mcbootflash/util.py` & `mcbootflash-9.0.0/src/mcbootflash/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 
     if total_bytes == 0:
         msg = "HEX file contains no data within program memory range"
         raise ValueError(msg)
 
     total_bytes += (bootattrs.write_size - total_bytes) % bootattrs.write_size
     align = bootattrs.write_size // hexdata.word_size_bytes
-    return total_bytes, hexdata.segments.chunks(chunk_size, align, b"\x00\x00")
+    return total_bytes, hexdata.segments.chunks(chunk_size, align, b"\xff\xff")
```

### Comparing `mcbootflash-8.0.2/tests/test_mcbootflash.json` & `mcbootflash-9.0.0/tests/test_mcbootflash.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753646179497389%*

 * *Differences: {"'test_checksum_bad_address_warning'": "{'rx': {delete: [70, 69, 68, 66, 65, 64, 63, 62, 61, 60, "*

 * *                                        "59, 58, 57, 56]}, 'tx': {delete: [30, 23, 22, 19, 18, 17, "*

 * *                                        '16, 15, 14, 13, 12]}}',*

 * * "'test_checksum_error'": "{'rx': {delete: [70, 69, 68, 66, 65, 64, 63, 62, 61, 60, 59, 58, 57, "*

 * *                          "56]}, 'tx': {delete: [30, 23, 22, 19, 18, 17, 16, 15, 14, 13, 12]}}",*

 * * "'test_cli[False-False]'": "{'rx': {delete: [106,  […]*

```diff
@@ -55,28 +55,14 @@
             0,
             0,
             254,
             167,
             2,
             0,
             8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26,
-            8,
             0,
             0,
             0,
             0,
             0,
             0,
             136,
@@ -105,25 +91,14 @@
             0,
             0,
             0,
             0,
             0,
             0,
             8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            8,
             240,
             0,
             0,
             0,
             0,
             0,
             136,
@@ -200,28 +175,14 @@
             0,
             0,
             24,
             0,
             0,
             1,
             252,
-            1,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            252,
             1
         ],
         "tx": [
             0,
             0,
             0,
             0,
@@ -249,25 +210,14 @@
             0,
             0,
             0,
             0,
             0,
             24,
             0,
-            0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
             0
         ]
     },
     "test_checksum_not_supported": {
         "rx": [
             0,
             0,
@@ -1888,64 +1838,26 @@
             24,
             0,
             0,
             254,
             167,
             2,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            1,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
             1,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            252,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -2104,58 +2016,25 @@
             0,
             0,
             0,
             0,
             0,
             0,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -3346,64 +3225,26 @@
             24,
             0,
             0,
             254,
             167,
             2,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            1,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
             1,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            252,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -3562,58 +3403,25 @@
             0,
             0,
             0,
             0,
             0,
             0,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -4804,64 +4612,26 @@
             24,
             0,
             0,
             254,
             167,
             2,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            1,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
             1,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            252,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -5020,58 +4790,25 @@
             0,
             0,
             0,
             0,
             0,
             0,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             2,
             240,
             0,
             85,
             0,
             170,
             0,
@@ -6262,64 +5999,26 @@
             24,
             0,
             0,
             254,
             167,
             2,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            1,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
             0,
-            1,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            252
+            1
         ],
         "tx": [
             0,
             0,
             0,
             0,
             0,
@@ -6336,57 +6035,24 @@
             0,
             0,
             0,
             0,
             0,
             0,
             0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             3,
             82,
             0,
             85,
             0,
             170,
             0,
             0,
             24,
             0,
-            0,
-            10,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
             0
         ]
     },
     "test_erase_empty": {
         "rx": [
             0,
             0,
@@ -6752,29 +6418,15 @@
             0,
             24,
             0,
             0,
             254,
             167,
             2,
-            0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
-            0,
-            1,
-            228,
-            26
+            0
         ],
         "tx": [
             0,
             0,
             0,
             0,
             0,
@@ -6790,25 +6442,14 @@
             0,
             0,
             0,
             0,
             0,
             0,
             0,
-            0,
-            8,
-            8,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            24,
-            0,
             0
         ]
     },
     "test_reset": {
         "rx": [
             9,
             0,
```

### Comparing `mcbootflash-8.0.2/tests/test_mcbootflash.py` & `mcbootflash-9.0.0/tests/test_mcbootflash.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 def test_cli(reserial, caplog, verbose, quiet):
     caplog.set_level(logging.INFO)
     main.main(
         argparse.Namespace(
             hexfile="tests/testcases/flash/test.hex",
             port=PORTNAME,
             baudrate=BAUDRATE,
-            timeout=1,
+            timeout=10,
+            checksum=True,
+            reset=False,
             verbose=verbose,
             quiet=quiet,
         ),
     )
     assert "Self verify OK" in caplog.messages[-1]
 
 
@@ -54,15 +56,17 @@
 
     caplog.set_level(logging.INFO)
     main.main(
         argparse.Namespace(
             hexfile="tests/testcases/flash/test.hex",
             port=PORTNAME,
             baudrate=BAUDRATE,
-            timeout=1,
+            timeout=10,
+            checksum=True,
+            reset=False,
             verbose=True,
             quiet=False,
         ),
     )
     assert caplog.records[-1].levelno == logging.ERROR
 
 
@@ -91,104 +95,74 @@
     assert bf.get_boot_attrs(connection) == bf.BootAttrs(
         version=258,
         max_packet_length=256,
         device_id=13398,
         erase_size=2048,
         write_size=8,
         memory_range=(6144, 174080),
-        has_checksum=True,
     )
 
 
 def test_erase(reserial, caplog, connection):
-    # To record data for this test, connect a device with a program installed.
-    caplog.set_level(logging.INFO)
+    caplog.set_level(logging.DEBUG)
     bootattrs = bf.get_boot_attrs(connection)
     connection.timeout = 10
-    main.erase(connection, bootattrs.memory_range, bootattrs.erase_size)
-    assert "Application erased" in caplog.messages[-1]
-
-
-def test_erase_empty(reserial, caplog, connection):
-    # To record data for this test, connect a device with no program installed.
-    caplog.set_level(logging.INFO)
-    bootattrs = bf.get_boot_attrs(connection)
-    main.erase(connection, bootattrs.memory_range, bootattrs.erase_size)
-    assert "No application detected, skipping erase" in caplog.messages[-1]
-
-
-def test_erase_fail(reserial, connection):
-    # To record data for this test, connect a device with a program installed.
-    bootattrs = bf.get_boot_attrs(connection)
-    mcbootflash.flash._FLASH_UNLOCK_KEY = 0
-    with pytest.raises(bf.BootloaderError) as excinfo:
-        main.erase(
-            connection,
-            bootattrs.memory_range,
-            bootattrs.erase_size,
-        )
-    assert "Erase failed" in str(excinfo.value)
+    bf.erase_flash(connection, bootattrs.memory_range, bootattrs.erase_size)
+    assert "Erasing addresses" in caplog.messages[-4]
 
 
 def test_erase_misaligned():
     with pytest.raises(ValueError) as excinfo:
         bf.erase_flash(Serial(), (0, 1), 2)
     assert "not a multiple" in str(excinfo.value)
 
 
+def test_verify_fail(reserial, connection):
+    with pytest.raises(bf.VerifyFail):
+        bf.self_verify(connection)
+
+
 def test_checksum_error(reserial, connection):
     bootattrs = bf.get_boot_attrs(connection)
     chunk = bincopy.Segment(
         minimum_address=bootattrs.memory_range[0],
         maximum_address=bootattrs.memory_range[0] + bootattrs.write_size,
         data=bytes(bootattrs.write_size),
         word_size_bytes=1,
     )
     with pytest.raises(bf.BootloaderError) as excinfo:
         bf.checksum(connection, chunk)
     assert "Checksum mismatch" in str(excinfo.value)
 
 
-def test_checksum_not_supported(reserial, caplog, connection):
-    bf.get_boot_attrs(connection)
-    assert "Bootloader does not support checksumming" in caplog.messages
-
-
 def test_no_data():
     bootattrs = bf.BootAttrs(
         version=258,
         max_packet_length=256,
         device_id=13398,
         erase_size=2048,
         write_size=8,
         memory_range=(6144, 174080),
-        has_checksum=True,
     )
     with pytest.raises(ValueError) as excinfo:
         bf.chunked("tests/testcases/no_data/test.hex", bootattrs)
     assert "no data" in str(excinfo.value)
 
 
-def test_reset(reserial, caplog, connection):
-    caplog.set_level(logging.DEBUG)
-    bf.reset(connection)
-    assert "Device reset" in caplog.messages[-1]
-
-
 def test_unexpected_response(reserial, connection):
+    if Path(PORTNAME).exists():
+        # Unexpected response uses synthetic data.
+        msg = f"{PORTNAME} exists: skipping unexpected response test"
+        pytest.skip(msg)
+
     with pytest.raises(bf.BootloaderError) as excinfo:
         bf.reset(connection)
     assert "Command code mismatch" in str(excinfo.value)
 
 
-def test_verify_fail(reserial, connection):
-    with pytest.raises(bf.VerifyFail):
-        bf.self_verify(connection)
-
-
 def test_read_flash():
     with pytest.raises(NotImplementedError):
         mcbootflash.flash._read_flash()
 
 
 def test_format_debug_bytes():
     testbytes_tx = b"0123"
@@ -206,7 +180,13 @@
         minimum_address=boot_attrs.memory_range[1] - payload_size // 2,
         maximum_address=boot_attrs.memory_range[1],
         data=b"\xff" * payload_size,
         word_size_bytes=1,
     )
     bf.checksum(connection, chunk)
     assert "BadAddress" in caplog.messages[-1]
+
+
+def test_reset(reserial, caplog, connection):
+    caplog.set_level(logging.DEBUG)
+    bf.reset(connection)
+    assert "Device reset" in caplog.messages[-1]
```

### Comparing `mcbootflash-8.0.2/tests/testcases/checksum_error/test.hex` & `mcbootflash-9.0.0/tests/testcases/checksum_error/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/tests/testcases/flash/test.hex` & `mcbootflash-9.0.0/tests/testcases/flash/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/tests/testcases/flash_empty/test.hex` & `mcbootflash-9.0.0/tests/testcases/flash_empty/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/tests/testcases/no_data/test.hex` & `mcbootflash-9.0.0/tests/testcases/no_data/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/tests/testcases/no_response/test.hex` & `mcbootflash-9.0.0/tests/testcases/no_response/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/tox.ini` & `mcbootflash-9.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `mcbootflash-8.0.2/PKG-INFO` & `mcbootflash-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcbootflash
-Version: 8.0.2
+Version: 9.0.0
 Summary: Flash firmware to devices running Microchip's 16-bit bootloader.
 Keywords: firmware,flashing,bootloader,serial,uart,microchip,pic24,dspic33,16-bit
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

