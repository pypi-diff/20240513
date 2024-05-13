# Comparing `tmp/pymtpng-1.0.2.tar.gz` & `tmp/pymtpng-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymtpng-1.0.2.tar", last modified: Wed Feb  7 17:35:46 2024, max compression
+gzip compressed data, was "pymtpng-1.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pymtpng-1.0.2.tar` & `pymtpng-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:35:46.588703 pymtpng-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:35:46.584703 pymtpng-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:35:46.588703 pymtpng-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-07 17:35:36.000000 pymtpng-1.0.2/.github/workflows/pypi-packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 17:35:36.000000 pymtpng-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-02-07 17:35:36.000000 pymtpng-1.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 17:35:36.000000 pymtpng-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-07 17:35:46.588703 pymtpng-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-07 17:35:36.000000 pymtpng-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-07 17:35:36.000000 pymtpng-1.0.2/mtpng.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-02-07 17:35:36.000000 pymtpng-1.0.2/pymtpng.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:35:46.588703 pymtpng-1.0.2/pymtpng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-07 17:35:46.000000 pymtpng-1.0.2/pymtpng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-07 17:35:46.000000 pymtpng-1.0.2/pymtpng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 17:35:46.000000 pymtpng-1.0.2/pymtpng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 17:35:46.000000 pymtpng-1.0.2/pymtpng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-07 17:35:36.000000 pymtpng-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 17:35:46.588703 pymtpng-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-07 17:35:36.000000 pymtpng-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 17:35:46.588703 pymtpng-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-07 17:35:36.000000 pymtpng-1.0.2/tests/test_mtpng.py
+-rw-r--r--   0        0        0     2670 2022-11-09 12:37:21.000000 pymtpng-1.0.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pymtpng-1.0.3/LICENSE
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pymtpng-1.0.3/README.md
+-rw-r--r--   0        0        0     1773 2022-11-09 12:37:21.000000 pymtpng-1.0.3/mtpng.hpp
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 pymtpng-1.0.3/pymtpng/__init__.py
+-rw-r--r--   0        0        0     9057 2022-11-09 12:37:21.000000 pymtpng-1.0.3/pymtpng.cpp
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pymtpng-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pymtpng-1.0.3/tests/test_mtpng.py
+-rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 pymtpng-1.0.3/PKG-INFO
```

### Comparing `pymtpng-1.0.2/CMakeLists.txt` & `pymtpng-1.0.3/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 cmake_minimum_required(VERSION 3.16)
 project(pymtpng CXX)
 
-include(FetchContent)
+find_package(
+  Python 3.9 REQUIRED
+  COMPONENTS Interpreter Development.Module
+  OPTIONAL_COMPONENTS Development.SABIModule
+)
 
-if(WIN32)
-  # Prevent pybind11 from sharing resources with other, potentially ABI incompatible modules
-  # https://github.com/pybind/pybind11/issues/2898
-  add_definitions(-DPYBIND11_COMPILER_TYPE="_${PROJECT_NAME}_abi")
-endif()
+# Use LTO for building this module
+set(CMAKE_INTERPROCEDURAL_OPTIMIZATION TRUE)
 
-# Fetch pybind11 library
+# Fetch nanobind library
+include(FetchContent)
 FetchContent_Declare(
-  pybind11
-  GIT_REPOSITORY https://github.com/pybind/pybind11
-  GIT_TAG        v2.11.1
-  GIT_SHALLOW    True
+  nanobind
+  GIT_REPOSITORY https://github.com/wjakob/nanobind
+  GIT_TAG        c5454462e35f29310df05b412b5c48997d634bdd
 )
-FetchContent_MakeAvailable(pybind11)
+FetchContent_MakeAvailable(nanobind)
 
 # Fetch mtpng source
 FetchContent_Declare(
   mtpng
-  GIT_REPOSITORY https://github.com/brion/mtpng
-  GIT_TAG        016c3fb07b6300bb8a08ee8790e80bc1c93b0c84
+  GIT_REPOSITORY https://github.com/bvibber/mtpng
+  GIT_TAG        40f389daf89603d493e22597fdbe3d5b592a49a6
 )
 FetchContent_MakeAvailable(mtpng)
 
 # Create target for mtpng library (built with cargo)
 if(WIN32)
   set(MTPNG_STATIC_LIB "${mtpng_SOURCE_DIR}/target/release/mtpng.lib")
 else()
@@ -48,21 +49,44 @@
 if(WIN32)
   target_link_libraries(mtpng_static INTERFACE userenv ntdll ws2_32 Bcrypt)
 else()
   target_link_libraries(mtpng_static INTERFACE z)
 endif()
 
 # Create target for python library
-pybind11_add_module(${PROJECT_NAME} "pymtpng.cpp" "mtpng.hpp")
+nanobind_add_module(${PROJECT_NAME}
+  STABLE_ABI
+  "pymtpng.cpp"
+  "mtpng.hpp"
+)
+nanobind_add_stub(
+  ${PROJECT_NAME}_stub
+  MODULE ${PROJECT_NAME}
+  OUTPUT ${PROJECT_NAME}.pyi
+  PYTHON_PATH $<TARGET_FILE_DIR:${PROJECT_NAME}>
+  DEPENDS ${PROJECT_NAME}
+  MARKER_FILE py.typed
+)
 target_link_libraries(${PROJECT_NAME} PRIVATE mtpng_static)
 set_target_properties(${PROJECT_NAME} PROPERTIES
   CXX_STANDARD 20
   CXX_STANDARD_REQUIRED ON
 )
+if(DEFINED SKBUILD_PROJECT_VERSION)
+  target_compile_definitions(${PROJECT_NAME} PRIVATE VERSION_INFO=${SKBUILD_PROJECT_VERSION})
+endif()
 
 if(CMAKE_CXX_COMPILER_ID MATCHES "GNU")
   target_compile_options(${PROJECT_NAME} PRIVATE -Wall -Wextra)
 elseif(CMAKE_CXX_COMPILER_ID MATCHES "MSVC")
   target_compile_options(${PROJECT_NAME} PUBLIC "/Zc:__cplusplus")
 endif()
 
-install(TARGETS ${PROJECT_NAME} DESTINATION ".")
+install(TARGETS ${PROJECT_NAME}
+  DESTINATION "${PROJECT_NAME}"
+)
+install(FILES
+  ${CMAKE_CURRENT_SOURCE_DIR}/${PROJECT_NAME}/__init__.py
+  ${${PROJECT_NAME}_BINARY_DIR}/py.typed
+  ${${PROJECT_NAME}_BINARY_DIR}/${PROJECT_NAME}.pyi
+  DESTINATION "${PROJECT_NAME}"
+)
```

### Comparing `pymtpng-1.0.2/LICENSE` & `pymtpng-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0.2/PKG-INFO` & `pymtpng-1.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pymtpng
-Version: 1.0.2
-Summary: Python bindings for MTPNG library
-Home-page: https://github.com/pwuertz/pymtpng
-Author: Peter Würtz
-Author-email: pwuertz@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python mtpng
 Python bindings for the [MTPNG library](https://github.com/brion/mtpng), a parallelized PNG encoder in Rust by Brion Vibber.
 
 # Usage
 ```python
 import pymtpng
 ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymtpng-1.0.2/mtpng.hpp` & `pymtpng-1.0.3/mtpng.hpp`

 * *Files identical despite different names*

### Comparing `pymtpng-1.0.2/pymtpng.cpp` & `pymtpng-1.0.3/pymtpng.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,69 @@
-#include <memory>
-#include <vector>
+#include <functional>
 #include <map>
+#include <memory>
 #include <string_view>
+#include <vector>
 
 #include <Python.h>
-#include "pybind11/pybind11.h"
-#include "pybind11/numpy.h"
-#include "pybind11/stl.h"
+#include <nanobind/nanobind.h>
+#include <nanobind/ndarray.h>
+#include <nanobind/stl/map.h>
+#include <nanobind/stl/string_view.h>
 
 #include "mtpng.hpp"
 
 
 using namespace std::string_view_literals;
-namespace py = pybind11;
-
-constexpr auto VERSION = "1.0.2"sv;
+namespace nb = nanobind;
+using namespace nb::literals;
 
 using stringv_map = std::map<std::string_view, std::string_view>;
 
-using np_uint8_array_t = py::array_t<uint8_t, py::array::c_style>;
-using np_uint16_array_t = py::array_t<uint16_t, py::array::c_style>;
+using np_uint8_array_t = nb::ndarray<uint8_t, nb::c_contig, nb::device::cpu>;
+using np_uint16_array_t = nb::ndarray<uint16_t, nb::c_contig, nb::device::cpu>;
+
+struct memoryview : public nb::object
+{
+    memoryview(const uint8_t* mem, const Py_ssize_t size)
+        : nb::object(makeMemoryView(mem, size), nb::detail::steal_t{})
+    { }
+
+private:
+    static PyObject* makeMemoryView(const uint8_t* mem, Py_ssize_t size)
+    {
+        auto* h = PyMemoryView_FromMemory(const_cast<char*>(reinterpret_cast<const char*>(mem)), size, PyBUF_READ);
+        if (!h) {
+            throw std::runtime_error("Failed creating memoryview");
+        }
+        return h;
+    }
+};
+
+struct Writer
+{
+    nb::callable py_write;
+    std::exception_ptr& eptr;
 
-using write_fn_t = std::function<size_t(const uint8_t* bytes, const size_t len)>;
+    size_t write(const uint8_t* bytes, const size_t len) {
+        try {
+            if (!eptr) {
+                return nb::cast<size_t>(py_write(memoryview(bytes, Py_ssize_t(len))));
+            }
+        } catch(...) {
+            eptr = std::current_exception();
+        }
+        return size_t{0};
+    };
+};
 
 extern "C" size_t write_func(void* user_data, const uint8_t* bytes, const size_t len)
 {
-    const write_fn_t& py_write_fn = *reinterpret_cast<const write_fn_t*>(user_data);
-    return py_write_fn(bytes, len);
+    Writer& writer = *reinterpret_cast<Writer*>(user_data);
+    return writer.write(bytes, len);
 }
 
 extern "C" bool flush_func([[maybe_unused]] void* user_data)
 {
     return true;
 }
 
@@ -69,18 +102,19 @@
     return MTPNG_RESULT_OK;
 }
 
 enum class Dtype {
     U8, U16
 };
 
+template <typename T>
 void encode_png_impl(
-    const py::array& image,
+    const nb::ndarray<T, nb::c_contig, nb::device::cpu>& image,
     const Dtype dtype,
-    const py::object& writable,
+    const nb::object& writable,
     const mtpng_filter_t filter,
     const mtpng_strategy_t strategy,
     const mtpng_compression_level_t compression_level,
     const stringv_map& info)
 {
     // Get array shape and data
     const auto ndim = image.ndim();
@@ -102,22 +136,18 @@
     // Verifier for mtpng return values (prioritizes exceptions caught in write callback)
     std::exception_ptr eptr;
     const auto TRY = [&](const mtpng_result r) {
         if (eptr) { std::rethrow_exception(eptr); }
         if (r != MTPNG_RESULT_OK) { throw std::runtime_error("mtpng error"); }
     };
 
-    // Create write callback, store python exceptions
-    write_fn_t py_write_fn = [&, writer = writable.attr("write")](const uint8_t* bytes, const size_t len) {
-        try {
-            if (!eptr) { return writer(py::memoryview::from_memory(bytes, Py_ssize_t(len))).cast<int>(); }
-        } catch(...) {
-            eptr = std::current_exception();
-        }
-        return 0;
+    // Create write adapter
+    Writer writer {
+        .py_write=writable.attr("write"),
+        .eptr=eptr,
     };
 
     // Create threadpool and encoder options
     const auto pool = create_threadpool();
     const auto options = create_encoder_options();
     TRY(mtpng_encoder_options_set_chunk_size(options.get(), 1024*1024));
     TRY(mtpng_encoder_options_set_filter(options.get(), filter));
@@ -128,101 +158,112 @@
     // Create PNG header
     const auto header = create_header();
     TRY(mtpng_header_set_size(header.get(), uint32_t(width), uint32_t(height)));
     TRY(mtpng_header_set_color(header.get(), color, (dtype == Dtype::U8) ? 8 : 16));
 
     // Encode and write PNG
     {
-        void* user_data = const_cast<write_fn_t*>(&py_write_fn);
+        void* user_data = &writer;
         const auto encoder = create_encoder(write_func, flush_func, user_data, options.get());
         TRY(mtpng_encoder_write_header(encoder.get(), header.get()));
         TRY(write_itxt_chunks(encoder.get(), info));
 
         const auto nitems_row = width * nchannels;
         if (dtype == Dtype::U8) {
             // Write U8 data rows directly
             const auto* row_data = reinterpret_cast<const uint8_t*>(image.data());
-            for (int y = 0; y < height; ++y) {
+            for (size_t y = 0; y < height; ++y) {
                 TRY(mtpng_encoder_write_image_rows(encoder.get(), row_data, 1 * nitems_row));
                 row_data += nitems_row;
             }
         } else {
             // Byteswap U16 data before writing rows (TODO: Check native byte order)
             const auto* row_data = reinterpret_cast<const uint16_t*>(image.data());
             std::vector<uint16_t> row_data_be(width * nchannels);
-            for (int y = 0; y < height; ++y) {
-                for (int x = 0; x < width; ++x) {
+            for (size_t y = 0; y < height; ++y) {
+                for (size_t x = 0; x < width; ++x) {
                     const uint16_t v = row_data[x];
                     row_data_be[x] = ((v & 0x00FF) << 8) | ((v & 0xFF00) >> 8);
                 }
                 TRY(mtpng_encoder_write_image_rows(
                     encoder.get(), reinterpret_cast<uint8_t*>(row_data_be.data()), 2 * nitems_row));
                 row_data += nitems_row;
             }
         }
     }
     // Done
 }
 
 void encode_u16_png(
     const np_uint16_array_t& image,
-    const py::object& writable,
+    const nb::object& writable,
     const mtpng_filter_t filter,
     const mtpng_strategy_t strategy,
     const mtpng_compression_level_t compression_level,
     const stringv_map& info)
 {
     encode_png_impl(image, Dtype::U16, writable, filter, strategy, compression_level, info);
 }
 
 void encode_png(
     const np_uint8_array_t& image,
-    const py::object& writable,
+    const nb::object& writable,
     const mtpng_filter_t filter,
     const mtpng_strategy_t strategy,
     const mtpng_compression_level_t compression_level,
     const stringv_map& info)
 {
     encode_png_impl(image, Dtype::U8, writable, filter, strategy, compression_level, info);
 }
 
-PYBIND11_MODULE(pymtpng, m) {
-
-    m.attr("__version__") = py::str(VERSION.data(), VERSION.size());
+NB_MODULE(pymtpng, m) {
 
-    py::enum_<mtpng_compression_level_t>(m, "CompressionLevel")
+    nb::enum_<mtpng_compression_level_t>(m, "CompressionLevel")
         .value("Fast", MTPNG_COMPRESSION_LEVEL_FAST)
         .value("Default", MTPNG_COMPRESSION_LEVEL_DEFAULT)
         .value("High", MTPNG_COMPRESSION_LEVEL_HIGH);
 
-    py::enum_<mtpng_filter_t>(m, "Filter")
+    nb::enum_<mtpng_filter_t>(m, "Filter")
         .value("Adaptive", MTPNG_FILTER_ADAPTIVE)
         .value("None", MTPNG_FILTER_NONE)
         .value("Sub", MTPNG_FILTER_SUB)
         .value("Up", MTPNG_FILTER_UP)
         .value("Average", MTPNG_FILTER_AVERAGE)
         .value("Paeth", MTPNG_FILTER_PAETH);
 
-    py::enum_<mtpng_strategy_t>(m, "Strategy")
+    nb::enum_<mtpng_strategy_t>(m, "Strategy")
         .value("Adaptive", MTPNG_STRATEGY_ADAPTIVE)
         .value("Default", MTPNG_STRATEGY_DEFAULT)
         .value("Filtered", MTPNG_STRATEGY_FILTERED)
         .value("Huffman", MTPNG_STRATEGY_HUFFMAN)
         .value("Rle", MTPNG_STRATEGY_RLE)
         .value("Fixed", MTPNG_STRATEGY_FIXED);
 
     m.def(
-        "encode_png", &encode_png, "Encode PNG to writable object.",
-        py::arg("image"), py::arg("writable"),
-        py::arg("filter") = MTPNG_FILTER_ADAPTIVE,
-        py::arg("strategy") = MTPNG_STRATEGY_RLE,
-        py::arg("compression_level") = MTPNG_COMPRESSION_LEVEL_DEFAULT,
-        py::arg("info") = stringv_map {});
+        "encode_png", &encode_png,
+        "image"_a,
+        "writable"_a,
+        "filter"_a = MTPNG_FILTER_ADAPTIVE,
+        "strategy"_a = MTPNG_STRATEGY_RLE,
+        "compression_level"_a = MTPNG_COMPRESSION_LEVEL_DEFAULT,
+        "info"_a = stringv_map {},
+        "Encode PNG to writable object.");
 
     m.def(
-        "encode_u16_png", &encode_u16_png, "Encode 16bit PNG to writable object.",
-        py::arg("image"), py::arg("writable"),
-        py::arg("filter") = MTPNG_FILTER_ADAPTIVE,
-        py::arg("strategy") = MTPNG_STRATEGY_RLE,
-        py::arg("compression_level") = MTPNG_COMPRESSION_LEVEL_DEFAULT,
-        py::arg("info") = stringv_map {});
+        "encode_u16_png", &encode_u16_png,
+        "image"_a,
+        "writable"_a,
+        "filter"_a = MTPNG_FILTER_ADAPTIVE,
+        "strategy"_a = MTPNG_STRATEGY_RLE,
+        "compression_level"_a = MTPNG_COMPRESSION_LEVEL_DEFAULT,
+        "info"_a = stringv_map {},
+        "Encode 16bit PNG to writable object.");
+
+
+#define STRINGIFY(x) #x
+#define MACRO_STRINGIFY(x) STRINGIFY(x)
+#ifdef VERSION_INFO    
+    m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
+#else
+    m.attr("__version__") = "dev";
+#endif
 }
```

### Comparing `pymtpng-1.0.2/tests/test_mtpng.py` & `pymtpng-1.0.3/tests/test_mtpng.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 
 def encode_png(
     image: np.ndarray,
     compression_level: pymtpng.CompressionLevel,
     strategy: pymtpng.Strategy,
 ) -> io.BytesIO:
-    encode_fns = {np.uint8: pymtpng.encode_png, np.uint16: pymtpng.encode_u16_png}
-    encode_fn = encode_fns[image.dtype]
+    encode_fn = pymtpng.encode_png if image.dtype == np.uint8 else pymtpng.encode_u16_png
     buffer = io.BytesIO()
     encode_fn(image, buffer, compression_level=compression_level, strategy=strategy)
     buffer.seek(0)
     return buffer
 
 
 def decode_png(buffer: io.BytesIO) -> np.ndarray:
```

