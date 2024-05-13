# Comparing `tmp/pepeline-0.3.1.tar.gz` & `tmp/pepeline-0.3.2.tar.gz`

## Comparing `pepeline-0.3.1.tar` & `pepeline-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pepeline-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     2162 2024-05-08 17:32:11.000000 pepeline-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     2844 2024-05-08 17:32:11.000000 pepeline-0.3.1/.github/workflows/pipl.yml
--rw-r--r--   0     1001      127      686 2024-05-08 17:32:11.000000 pepeline-0.3.1/.gitignore
--rw-r--r--   0     1001      127     1065 2024-05-08 17:32:11.000000 pepeline-0.3.1/LICENSE
--rw-r--r--   0     1001      127      781 2024-05-08 17:32:11.000000 pepeline-0.3.1/README.md
--rw-r--r--   0     1001      127     4036 2024-05-08 17:32:11.000000 pepeline-0.3.1/pepeline.pyi
--rw-r--r--   0     1001      127      892 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127      557 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/array/utils.rs
--rw-r--r--   0     1001      127     1035 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/color_levels.rs
--rw-r--r--   0     1001      127     2780 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/convert.rs
--rw-r--r--   0     1001      127     4883 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/cvt_color_float.rs
--rw-r--r--   0     1001      127     1033 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/cvt_constants.rs
--rw-r--r--   0     1001      127      712 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/enums.rs
--rw-r--r--   0     1001      127     1258 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/core/noise.rs
--rw-r--r--   0     1001      127     2256 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/functions/color_function.rs
--rw-r--r--   0     1001      127     3979 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/functions/core_funcion.rs
--rw-r--r--   0     1001      127     1076 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/functions/halftone_function.rs
--rw-r--r--   0     1001      127     2463 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/functions/img_function.rs
--rw-r--r--   0     1001      127     6986 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/halftone/dot.rs
--rw-r--r--   0     1001      127     2387 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/halftone/screentone_add.rs
--rw-r--r--   0     1001      127      557 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/halftone/utils_halftone.rs
--rw-r--r--   0     1001      127    11014 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/image/decode.rs
--rw-r--r--   0     1001      127     1254 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/image/save.rs
--rw-r--r--   0     1001      127      522 2024-05-08 17:32:11.000000 pepeline-0.3.1/src/utils/mod.rs
--rw-r--r--   0     1001      127    34628 2024-05-08 17:32:15.000000 pepeline-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127      428 2024-05-08 17:32:11.000000 pepeline-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 pepeline-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 pepeline-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     2162 2024-05-13 04:53:18.000000 pepeline-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     2844 2024-05-13 04:53:18.000000 pepeline-0.3.2/.github/workflows/pipl.yml
+-rw-r--r--   0     1001      127      686 2024-05-13 04:53:18.000000 pepeline-0.3.2/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-05-13 04:53:18.000000 pepeline-0.3.2/LICENSE
+-rw-r--r--   0     1001      127     1182 2024-05-13 04:53:18.000000 pepeline-0.3.2/README.md
+-rw-r--r--   0     1001      127     4334 2024-05-13 04:53:18.000000 pepeline-0.3.2/pepeline.pyi
+-rw-r--r--   0     1001      127      967 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127     1139 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/color_levels.rs
+-rw-r--r--   0     1001      127     2780 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/convert.rs
+-rw-r--r--   0     1001      127     4883 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/cvt_color_float.rs
+-rw-r--r--   0     1001      127     1033 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/cvt_constants.rs
+-rw-r--r--   0     1001      127      718 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/enums.rs
+-rw-r--r--   0     1001      127     1258 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/core/noise.rs
+-rw-r--r--   0     1001      127     2244 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/functions/color_function.rs
+-rw-r--r--   0     1001      127     3983 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/functions/core_funcion.rs
+-rw-r--r--   0     1001      127     1580 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/functions/halftone_function.rs
+-rw-r--r--   0     1001      127     2475 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/functions/img_function.rs
+-rw-r--r--   0     1001      127     6979 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/halftone/dot.rs
+-rw-r--r--   0     1001      127     2313 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/halftone/screentone_add.rs
+-rw-r--r--   0     1001      127      555 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/halftone/utils_halftone.rs
+-rw-r--r--   0     1001      127    11014 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/image/decode.rs
+-rw-r--r--   0     1001      127     1254 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/image/save.rs
+-rw-r--r--   0     1001      127      501 2024-05-13 04:53:18.000000 pepeline-0.3.2/src/utils/mod.rs
+-rw-r--r--   0     1001      127    34628 2024-05-13 04:53:24.000000 pepeline-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127      428 2024-05-13 04:53:18.000000 pepeline-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 pepeline-0.3.2/PKG-INFO
```

### Comparing `pepeline-0.3.1/Cargo.toml` & `pepeline-0.3.2/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "pepeline"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pepeline"
 crate-type = ["cdylib"]
 
 
 [dependencies]
-pyo3 = { version = "0.20.0", features = ["extension-module"] }
-numpy = "0.20.0"
+pyo3 = { version = "0.21", features = ["gil-refs"] }
+numpy = "0.21.0"
 ndarray = "0.15.6"
 image = "0.25.0"
 zune-jpeg = "0.4.11"
 zune-psd = "0.4.0"
 filebuffer = "0.4.0"
 noise = "0.9.0"
 rand = "0.8.5"
```

### Comparing `pepeline-0.3.1/.github/workflows/CI.yml` & `pepeline-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/.github/workflows/pipl.yml` & `pepeline-0.3.2/.github/workflows/pipl.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/.gitignore` & `pepeline-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/LICENSE` & `pepeline-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/pepeline.pyi` & `pepeline-0.3.2/pepeline.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
+from typing import Optional
 
 import numpy as np
 
 
 class TypeNoise(Enum):
     PERLIN = 0,
     SIMPLEX = 1,
@@ -38,28 +39,28 @@
     ELLIPSE = 2,
     LINE = 2,
     INVLINE = 3
 
 
 def read(
         path: str,
-        mode: None | int,
-        format: None | int
+        mode: Optional[int] = None,
+        format: Optional[int] = None
 ) -> np.ndarray:
     """ The function to read the image. input parameters:
     \n path -> str file path 
     \n mode -> uint 0 -> gray 1-> rgb 2-> psd dynamic format, and in other cases rgb, None = 2
     \n format -> uint 0 -> f32 0-1 img, 1+ -> u8 0-255, None = 1"""
 
 
 def screentone(
         array: np.ndarray,
         dot_size: int,
-        angle: None | int,
-        dot_type: None | TypeDot
+        angle: Optional[int] = None,
+        dot_type: Optional[TypeDot] = None
 ) -> np.ndarray:
     """
     Halftone overlay function.
 
     Parameters:
     - array (np.ndarray): Input array representing an image with dtype np.float32 (values ranging from 0 to 1).
     - dot_size (int): Size of the screentone dots in pixels (uint).
@@ -74,14 +75,22 @@
     - 'dot_size' determines the size of the halftone dots in pixels.
     - 'angle' specifies the rotation angle of the halftone pattern in degrees. If not provided, the pattern is not rotated.
     - 'dot_type' specifies the type of dot pattern to use. If not provided, a default dot pattern is used.
     The function returns the array with the halftone overlay applied.
     """
 
 
+# def halftone(
+#         array: np.ndarray,
+#         dot_size: int,
+#         angle: Optional[int] = None,
+#         dot_type: Optional[TypeDot] = None
+# ) -> np.ndarray: ...
+
+
 def cvt_color(array: np.ndarray, cvt_type: CvtType) -> np.ndarray:
     """
     Convert the color space of an array of type np.ndarray.
 
     Parameters:
     - array (np.ndarray): The input array, typically representing an image, with dtype np.float32. (YCbCr only 0-1)
     - cvt_type (CvtType): The type of color space conversion to perform.
@@ -98,32 +107,32 @@
 def crop_cord(array: np.ndarray) -> (
         int, int, int, int):
     """returns image coordinates not equal to 0, made for cropping using the Laplace operator"""
 
 
 def fast_color_level(
         array: np.ndarray,
-        in_low: None | int,
-        in_high: None | int,
-        out_low: None | int,
-        out_high: None | int,
-        gamma: None | float,
+        in_low: Optional[int] = 0,
+        in_high: Optional[int] = 255,
+        out_low: Optional[int] = 0,
+        out_high: Optional[int] = 255,
+        gamma: Optional[float] = 1.0,
 ) -> np.ndarray:
     """ array:np.float32
     \n in_low...out_high:uint8
     \n gamma:float32"""
 
 
 def noise_generate(
         size: tuple[int, int] | tuple[int, int, int],
         type_noise: TypeNoise,
         octaves: int,
         frequency: float,
         lacunarity: float,
-        seed: int | None,
+        seed: Optional[int] = None,
 ) -> np.ndarray:
     """ size: tuple 2d or 3d
     \n type_noise: TypeNoise
     \n octaves: uint
     \n frequency: float32
     \n lacunarity: float32
     \n seed: uint"""
```

### Comparing `pepeline-0.3.1/src/lib.rs` & `pepeline-0.3.2/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mod utils;
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn pepeline(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(img_function::read, m)?)?;
     m.add_function(wrap_pyfunction!(halftone_function::screentone, m)?)?;
+    // m.add_function(wrap_pyfunction!(halftone_function::halftone, m)?)?;
     m.add_function(wrap_pyfunction!(core_funcion::noise_generate, m)?)?;
     m.add_function(wrap_pyfunction!(img_function::save, m)?)?;
     m.add_function(wrap_pyfunction!(core_funcion::crop_cord, m)?)?;
     m.add_function(wrap_pyfunction!(color_function::fast_color_level, m)?)?;
     m.add_function(wrap_pyfunction!(color_function::cvt_color, m)?)?;
     m.add_class::<TypeNoise>()?;
     m.add_class::<TypeDot>()?;
```

### Comparing `pepeline-0.3.1/src/utils/core/convert.rs` & `pepeline-0.3.2/src/utils/core/convert.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/src/utils/core/cvt_color_float.rs` & `pepeline-0.3.2/src/utils/core/cvt_color_float.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/src/utils/core/cvt_constants.rs` & `pepeline-0.3.2/src/utils/core/cvt_constants.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/src/utils/core/enums.rs` & `pepeline-0.3.2/src/utils/core/enums.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 use pyo3::pyclass;
 
-#[pyclass]
 #[derive(Clone)]
+#[pyclass]
 pub enum TypeNoise {
     PERLIN = 0,
     SIMPLEX = 1,
     OPENSIMPLEX = 2,
     SUPERSIMPLEX = 3,
     PERLINSURFLET = 4,
 }
 
-#[pyclass]
 #[derive(Clone)]
+#[pyclass]
 pub enum CvtType {
     RGB2Gray = 0, //NTSC
     RGB2GrayAverage = 1,
     RGB2GrayBt709 = 2,
     RGB2GrayBt2020 = 3,
     RGB2CMYK = 4,
     CMYK2RGB = 5,
@@ -28,15 +28,15 @@
     RGB2BGR = 12,
     BGR2RGB = 13,
     GRAY2RGB = 14,
     RGB2Luma = 15,
 }
 
 #[pyclass]
-#[derive(Clone)]
+#[derive(Clone, Copy)]
 pub enum TypeDot {
     CIRCLE = 0,
     CROSS = 1,
     ELLIPSE = 2,
     LINE = 3,
     INVLINE = 4,
 }
```

### Comparing `pepeline-0.3.1/src/utils/core/noise.rs` & `pepeline-0.3.2/src/utils/core/noise.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/src/utils/functions/color_function.rs` & `pepeline-0.3.2/src/utils/functions/color_function.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use ndarray::{Array2, Array3};
 use numpy::{PyArrayDyn, PyReadonlyArrayDyn, ToPyArray};
-use pyo3::{pyfunction, Py, PyObject, PyResult, Python};
+use pyo3::{pyfunction, Py, PyResult, Python};
 
-use crate::utils::core::array::utils::py_obj_to_array;
 use crate::utils::core::color_levels::levels;
 use crate::utils::core::cvt_color_float::cvt_color_float;
 use crate::utils::core::enums::CvtType;
 
 #[pyfunction]
 pub fn fast_color_level<'py>(
     input: PyReadonlyArrayDyn<f32>,
@@ -18,26 +17,31 @@
     py: Python,
 ) -> PyResult<Py<PyArrayDyn<f32>>> {
     let in_low = in_low.unwrap_or(0u8);
     let in_high = in_high.unwrap_or(255u8);
     let out_low = out_low.unwrap_or(0u8);
     let out_high = out_high.unwrap_or(255u8);
     let gamma = gamma.unwrap_or(1.0f32);
-    let array = input.as_array().to_owned();
-    let array = levels(array, in_low, in_high, out_low, out_high, gamma);
+    let mut array = input.as_array().to_owned();
 
-    Ok(array.to_pyarray(py).to_owned())
+    levels(&mut array, in_low, in_high, out_low, out_high, gamma);
+    Ok(array.to_pyarray_bound(py).into())
 }
 
 #[pyfunction]
-pub fn cvt_color(input: PyObject, cvt_type: CvtType, py: Python) -> PyResult<Py<PyArrayDyn<f32>>> {
-    let array = py_obj_to_array(input, py)?;
-    let binding = array.clone();
-    let shape = binding.shape();
-    let vec = array.into_raw_vec();
+pub fn cvt_color<'py>(
+    img: PyReadonlyArrayDyn<f32>,
+    cvt_type: CvtType,
+    py: Python,
+) -> PyResult<Py<PyArrayDyn<f32>>> {
+    let array = img.as_array();
+    let array_shape = array.clone().to_owned();
+    let shape = array_shape.shape();
+
+    let vec = array.to_owned().into_raw_vec();
     let result_vec = cvt_color_float(&vec, cvt_type.clone());
     let array = match cvt_type {
         CvtType::RGB2Gray
         | CvtType::RGB2GrayAverage
         | CvtType::RGB2GrayBt709
         | CvtType::RGB2GrayBt2020
         | CvtType::RGB2Luma => {
@@ -57,9 +61,10 @@
                 .into_dyn()
         }
         CvtType::RGB2CMYK => {
             unsafe { Array3::from_shape_vec_unchecked([shape[0], shape[1], 4], result_vec) }
                 .into_dyn()
         }
     };
-    Ok(array.to_pyarray(py).to_owned())
+
+    Ok(array.to_pyarray_bound(py).into())
 }
```

### Comparing `pepeline-0.3.1/src/utils/functions/core_funcion.rs` & `pepeline-0.3.2/src/utils/functions/core_funcion.rs`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,23 @@
     match size.len() {
         2 => {
             let mut array: Array2<f32> = Array2::zeros((size[0], size[1]));
             let type_fn = generate_noise2d(type_noise, seed);
             for ((x, y), value) in array.indexed_iter_mut() {
                 *value = noise_2d(&type_fn, x, y, octaves, frequency, lacunarity);
             }
-            Ok(array.into_dyn().to_pyarray(py).to_owned())
+            Ok(array.into_dyn().to_pyarray_bound(py).into())
         }
         3 => {
             let mut array: Array3<f32> = Array3::zeros((size[0], size[1], size[2]));
             let type_fn = generate_noise3d(type_noise, seed);
             for ((x, y, z), value) in array.indexed_iter_mut() {
                 *value = noise_3d(&type_fn, x, y, z, octaves, frequency, lacunarity);
             }
-            Ok(array.into_dyn().to_pyarray(py).to_owned())
+            Ok(array.into_dyn().to_pyarray_bound(py).into())
         }
         _ => Err(pyo3::exceptions::PyValueError::new_err(
             "Unsupported dimensions",
         )),
     }
 }
```

### Comparing `pepeline-0.3.1/src/utils/functions/halftone_function.rs` & `pepeline-0.3.2/src/utils/functions/halftone_function.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 use numpy::{PyArray2, PyReadonlyArray2, ToPyArray};
-use pyo3::{pyfunction, Py, PyResult, Python};
+use pyo3::{Py, pyfunction, PyResult, Python};
 
 use crate::utils::core::enums::TypeDot;
+// use crate::utils::halftone::halftone_add::{halftone_add, RgbHalftone};
 use crate::utils::halftone::screentone_add::{screentone_add, screentone_rotate_add};
 
+// #[pyfunction]
+// pub fn halftone<'py>(
+//     input: PyReadonlyArray3<f32>,
+//     halftone: RgbHalftone,
+//     py: Python,
+// ) -> PyResult<Py<PyArray3<f32>>> {
+//     // halftone overlay function:
+//     //     input -> array only 2D f32 0-1
+//     //     dot_size -> uint screenton size in pixels
+//     //     angle -> i16 degree by which we rotate the pattern
+//     let mut array = input.as_array().to_owned();
+//     halftone_add(&mut array, halftone);
+//
+//     Ok(array.to_pyarray_bound(py).into())
+// }
+
 #[pyfunction]
 pub fn screentone<'py>(
     input: PyReadonlyArray2<f32>,
     dot_size: usize,
     angle: Option<i16>,
     dot_type: Option<TypeDot>,
     py: Python,
@@ -18,14 +35,12 @@
     //     angle -> i16 degree by which we rotate the pattern
     let angle = angle.unwrap_or(0);
     let mut array = input.as_array().to_owned();
     let dot_type = dot_type.unwrap_or(TypeDot::CIRCLE);
     if angle != 0 {
         screentone_rotate_add(&mut array, dot_size, (angle as f32).to_radians(), dot_type);
     } else {
-        let lx_plus = dot_size / 2;
-        let ly_plus = dot_size / 2;
-        screentone_add(&mut array, dot_size, ly_plus, lx_plus, dot_type);
+        screentone_add(&mut array, dot_size, dot_type);
     }
 
-    Ok(array.to_pyarray(py).to_owned())
+    Ok(array.to_pyarray_bound(py).into())
 }
```

### Comparing `pepeline-0.3.1/src/utils/functions/img_function.rs` & `pepeline-0.3.2/src/utils/functions/img_function.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
     let path = Path::new(&path);
     let mode = mode.unwrap_or(2u8);
     let format = format.unwrap_or(1u8);
 
     match format {
         0 => match all_read_f32(path, mode) {
-            Ok(array) => Ok(array.to_pyarray(py).into()),
+            Ok(array) => Ok(array.to_pyarray_bound(py).into()),
             Err(err) => Err(PyErr::new::<PyOSError, _>(format!(
                 "Error reading file: {}",
                 err
             ))),
         },
         _ => match all_read_u8(path, mode) {
-            Ok(array) => Ok(array.to_pyarray(py).into()),
+            Ok(array) => Ok(array.to_pyarray_bound(py).into()),
             Err(err) => Err(PyErr::new::<PyOSError, _>(format!(
                 "Error reading file: {}",
                 err
             ))),
         },
     }
 }
```

### Comparing `pepeline-0.3.1/src/utils/halftone/dot.rs` & `pepeline-0.3.2/src/utils/halftone/dot.rs`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         n += 1;
     }
 
     return dot;
 }
 
 fn dot(dot_inv: Array2<f32>) -> Array2<f32> {
-    let dot = dot_inv * -1.0 + 1.0;
+    let dot = 1.0 - dot_inv;
 
     return dot;
 }
 
 pub fn create_dot(dot_size: usize, dot_type: TypeDot) -> (Array2<f32>, Array2<f32>) {
     let dot_inv = match dot_type {
         TypeDot::CROSS => dot_cross_inv(dot_size),
```

### Comparing `pepeline-0.3.1/src/utils/halftone/screentone_add.rs` & `pepeline-0.3.2/src/utils/halftone/screentone_add.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,62 +10,53 @@
     angle: f32,
     dot_type: TypeDot,
 ) {
     let (dot, dot_inv) = create_dot(dot_size, dot_type);
     let mut src_values: f32;
     let mut colum: usize;
     let (w, h) = (array.shape()[0], array.shape()[1]);
-    let lx_plus = w / 2;
-    let ly_plus = h / 2;
+    let lx_bias = w / 2;
+    let ly_bias = h / 2;
     let cos_sin = compute_cos_sin(angle);
-    let ww = 0..w;
-    let hh = 0..h;
-    for ly in ww {
-        let ly2 = ly + ly_plus;
-
-        for lx in hh.clone() {
+    for ly in 0..w {
+        let ly2 = ly + ly_bias;
+        for lx in 0..h {
             let value = &mut array[[ly, lx]];
             if *value > 0.0 && *value < 1.0 {
-                let lx2 = lx + lx_plus;
+                let lx2 = lx + lx_bias;
                 let rot = rotate_pixel_coordinates(
-                    lx2 as f32, ly2 as f32, w as f32, h as f32, cos_sin.0, cos_sin.1,
+                    lx2 as f32, ly2 as f32, w as f32, h as f32, cos_sin[0], cos_sin[1],
                 );
                 colum = rot.1 / dot_size;
                 src_values = if (colum + rot.0 / dot_size) % 2 == 1 {
                     dot_inv[[rot.0 % dot_size, rot.1 % dot_size]]
                 } else {
                     dot[[rot.0 % dot_size, rot.1 % dot_size]]
                 };
                 let src_value = src_values;
                 *value = if *value < src_value { 0.0 } else { 1.0 };
             }
         }
     }
 }
 
-pub fn screentone_add(
-    array: &mut Array2<f32>,
-    dot_size: usize,
-    ly_plus: usize,
-    lx_plus: usize,
-    dot_type: TypeDot,
-) {
+pub fn screentone_add(array: &mut Array2<f32>, dot_size: usize, dot_type: TypeDot) {
     let (dot, dot_inv) = create_dot(dot_size, dot_type);
+    let lx_bias = dot_size / 2;
+    let ly_bias = dot_size / 2;
     let mut src_values: f32;
     let mut colum: usize;
     let (w, h) = (array.shape()[0], array.shape()[1]);
-    let ww = 0..w;
-    let hh = 0..h;
-    for ly in ww {
-        let ly2 = ly + ly_plus;
+    for ly in 0..w {
+        let ly2 = ly + ly_bias;
         colum = ly2 / dot_size;
-        for lx in hh.clone() {
+        for lx in 0..h {
             let value = &mut array[[ly, lx]];
             if *value > 0.0 && *value < 1.0 {
-                let lx2 = lx + lx_plus;
+                let lx2 = lx + lx_bias;
                 src_values = if (colum + lx2 / dot_size) % 2 == 1 {
                     dot_inv[[lx2 % dot_size, ly2 % dot_size]]
                 } else {
                     dot[[lx2 % dot_size, ly2 % dot_size]]
                 };
                 let src_value = src_values;
                 *value = if *value < src_value { 0.0 } else { 1.0 };
```

### Comparing `pepeline-0.3.1/src/utils/halftone/utils_halftone.rs` & `pepeline-0.3.2/src/utils/halftone/utils_halftone.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 
     let rotated_x = (cos_theta * x_rel - sin_theta * y_rel + center_x) as usize;
     let rotated_y = (sin_theta * x_rel + cos_theta * y_rel + center_y) as usize;
 
     (rotated_x, rotated_y)
 }
 
-pub fn compute_cos_sin(theta: f32) -> (f32, f32) {
+pub fn compute_cos_sin(theta: f32) -> [f32; 2] {
     let cos_theta = theta.cos();
     let sin_theta = theta.sin();
-    (cos_theta, sin_theta)
+    [cos_theta, sin_theta]
 }
```

### Comparing `pepeline-0.3.1/src/utils/image/decode.rs` & `pepeline-0.3.2/src/utils/image/decode.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/src/utils/image/save.rs` & `pepeline-0.3.2/src/utils/image/save.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.3.1/Cargo.lock` & `pepeline-0.3.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -606,17 +606,17 @@
 checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -656,15 +656,15 @@
 name = "paste"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pepeline"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "filebuffer",
  "image",
  "ndarray",
  "noise",
  "numpy",
  "pyo3",
@@ -730,17 +730,17 @@
 dependencies = [
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -748,49 +748,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -1021,17 +1021,17 @@
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.61"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `pepeline-0.3.1/PKG-INFO` & `pepeline-0.3.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-Metadata-Version: 2.3
-Name: pepeline
-Version: 0.3.1
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy >=1.16.0
-License-File: LICENSE
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 [pypl](https://pypi.org/project/pepeline/)
 
 [git](https://github.com/scanlate-wiki/pipeline-rs)
 
 
 # pepeline-rs
 Fast rust-python librarian for internal needs of an organization
 ```py
-from pepeline import screentone, fast_color_level, read, save
+from pepeline import screentone, fast_color_level, read, save, cvt_color, CvtType
 img = read(<"img path">, 0, 0)
 img = fast_color_level(
     img,     
     in_low = 10,
     in_high = 240,
     out_low = 0,
     out_high = 255,
     gamma = 1.0
 )
-img = screenton(img, dot_size=7)
+img = cvt_color(img, CvtType.RGB2CMYK)
+img[:, :, 0] = screenton(img[:, :, 0], dot_size=7, angle=-15)
+img[:, :, 1] = screenton(img[:, :, 1], dot_size=7, angle=0)
+img[:, :, 2] = screenton(img[:, :, 2], dot_size=7, angle=15)
+img[:, :, 3] = screenton(img[:, :, 3], dot_size=7, angle=30)
+img = cvt_color(img, CvtType.CMYK2RGB)
 save(img, "out.png")
 ```
 # TODO:
 - resize❓
 - documentation ♻️
 - refactoring ♻️
 - add tests ♻️
@@ -39,8 +33,8 @@
 - simd ❓
 # Function:
 - read - read img (supports psd)
 - screentone - add screenton patern.
 - fast_color_level - color levels correction
 - noise_generate - ganerate noise array
 - save - fast save image
-
+- cvt_color - converts color extensions, currently only supports f32 and in some places 0-1
```

