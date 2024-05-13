# Comparing `tmp/pyarc2-0.4.0.tar.gz` & `tmp/pyarc2-0.5.0.tar.gz`

## Comparing `pyarc2-0.4.0.tar` & `pyarc2-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 pyarc2-0.4.0/Cargo.toml
--rw-r--r--   0        0        0    16725 2024-03-22 17:43:29.000000 pyarc2-0.4.0/LICENSE
--rw-r--r--   0        0        0      131 2024-03-22 17:43:29.000000 pyarc2-0.4.0/MANIFEST.in
--rw-r--r--   0        0        0     1628 2024-03-22 17:43:29.000000 pyarc2-0.4.0/README.md
--rw-r--r--   0        0        0      634 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      138 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/api.rst
--rw-r--r--   0        0        0     2024 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/conf.py
--rw-r--r--   0        0        0     3437 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/index.rst
--rw-r--r--   0        0        0      800 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/make.bat
--rw-r--r--   0        0        0     9430 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/overview.rst
--rw-r--r--   0        0        0     4498 2024-03-22 17:43:29.000000 pyarc2-0.4.0/docs/upload.py
--rw-r--r--   0        0        0     9610 2024-03-22 17:43:29.000000 pyarc2-0.4.0/pyarc2/__init__.py
--rw-r--r--   0        0        0      215 2024-03-22 17:43:29.000000 pyarc2-0.4.0/pyarc2/_types.py
--rw-r--r--   0        0        0        0 2024-03-22 17:43:29.000000 pyarc2-0.4.0/pyarc2/py.typed
--rw-r--r--   0        0        0     5685 2024-03-22 17:43:29.000000 pyarc2-0.4.0/pyarc2/pyarc2.pyi
--rw-r--r--   0        0        0       12 2024-03-22 17:43:29.000000 pyarc2-0.4.0/requirements.txt
--rw-r--r--   0        0        0    53441 2024-03-22 17:43:29.000000 pyarc2-0.4.0/src/lib.rs
--rw-r--r--   0        0        0    15710 2024-03-22 17:44:18.000000 pyarc2-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     1714 2024-03-22 17:43:29.000000 pyarc2-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 pyarc2-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 pyarc2-0.5.0/Cargo.toml
+-rw-r--r--   0        0        0    16725 2024-05-13 12:37:05.000000 pyarc2-0.5.0/LICENSE
+-rw-r--r--   0        0        0      131 2024-05-13 12:37:05.000000 pyarc2-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     1627 2024-05-13 12:37:05.000000 pyarc2-0.5.0/README.md
+-rw-r--r--   0        0        0      634 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0      138 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/api.rst
+-rw-r--r--   0        0        0     2205 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0     3437 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0     9430 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/overview.rst
+-rw-r--r--   0        0        0     4498 2024-05-13 12:37:05.000000 pyarc2-0.5.0/docs/upload.py
+-rw-r--r--   0        0        0    10572 2024-05-13 12:37:05.000000 pyarc2-0.5.0/pyarc2/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-13 12:37:05.000000 pyarc2-0.5.0/pyarc2/_types.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:37:05.000000 pyarc2-0.5.0/pyarc2/py.typed
+-rw-r--r--   0        0        0     6019 2024-05-13 12:37:05.000000 pyarc2-0.5.0/pyarc2/pyarc2.pyi
+-rw-r--r--   0        0        0       12 2024-05-13 12:37:05.000000 pyarc2-0.5.0/requirements.txt
+-rw-r--r--   0        0        0    57610 2024-05-13 12:37:05.000000 pyarc2-0.5.0/src/lib.rs
+-rw-r--r--   0        0        0    14214 2024-05-13 12:37:57.000000 pyarc2-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     1714 2024-05-13 12:37:05.000000 pyarc2-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 pyarc2-0.5.0/PKG-INFO
```

### Comparing `pyarc2-0.4.0/Cargo.toml` & `pyarc2-0.5.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyarc2"
-version = "0.4.0"
+version = "0.5.0"
 authors = ["Spyros Stathopoulos <spyros@arc-instruments.co.uk>"]
 description = "High level Python bindings for the libarc2 library"
 edition = "2018"
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "http://arc-instruments.co.uk"
 repository = "https://github.com/arc-instruments/pyarc2"
@@ -37,15 +37,15 @@
 [lib]
 name = "pyarc2"
 crate-type = ["cdylib", "lib"]
 
 [dependencies]
 numpy = "0.17"
 ndarray = "0.15"
-libarc2 = { git = "https://github.com/arc-instruments/libarc2", tag = "0.4.0" }
+libarc2 = { git = "https://github.com/arc-instruments/libarc2", tag = "0.5.0" }
 
 [dependencies.pyo3]
 version = "0.17"
 features = ["extension-module"]
 
 [features]
 default = ["flag_addresses"]
```

### Comparing `pyarc2-0.4.0/LICENSE` & `pyarc2-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/README.md` & `pyarc2-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Python bindings for libarc2
 
-[![](https://img.shields.io/badge/-docs-default?logo=gitbook&logoColor=white)](https://files.arc-instruments.co.uk/documents/pyarc2/latest/)
+[![](https://img.shields.io/badge/-docs-default?logo=gitbook&logoColor=white)](https://files.arc-instruments.co.uk/documents/pyarc2/0.5.0/)
 
 ## Introduction
 
 This library presents a python interface to the low-level `libarc2` library
 used to interface with ArC TWO™. Most of the user-facing facilities of
 `libarc2` are present in this library. That being said, `pyarc2` itself is
 still relatively low-level and a general understanding of the internals of
```

### Comparing `pyarc2-0.4.0/docs/Makefile` & `pyarc2-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/docs/conf.py` & `pyarc2-0.5.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,23 +10,31 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
+import os
+import os.path
+import sys
+
+if sys.platform == 'win32':
+    thisdir = os.path.dirname(__file__)
+    os.add_dll_directory(os.path.abspath(os.path.dirname(thisdir)))
+
 
 # -- Project information -----------------------------------------------------
 
 project = 'pyarc2'
-copyright = '2022, ArC Instruments Ltd'
+copyright = '2022–2024, ArC Instruments Ltd'
 author = 'Spyros Stathopoulos'
 
 # The full version, including alpha/beta/rc tags
-release = '0.4.0'
+release = '0.5.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyarc2-0.4.0/docs/index.rst` & `pyarc2-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/docs/make.bat` & `pyarc2-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/docs/overview.rst` & `pyarc2-0.5.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/docs/upload.py` & `pyarc2-0.5.0/docs/upload.py`

 * *Files identical despite different names*

### Comparing `pyarc2-0.4.0/pyarc2/__init__.py` & `pyarc2-0.5.0/pyarc2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .pyarc2 import InstrumentLL as _InstrumentLL
 from .pyarc2 import BiasOrder, ControlMode, DataMode, ReadType, WaitFor, AuxDACFn
-from .pyarc2 import ReadAt, ReadAfter, ArC2Error
+from .pyarc2 import ReadAt, ReadAfter, ArC2Error, IODir
 from .pyarc2 import find_ids
 try:
     from .pyarc2 import LIBARC2_VERSION
 except (AttributeError, ImportError):
     LIBARC2_VERSION = None
 
 from collections.abc import Iterable
@@ -84,20 +84,23 @@
     >>> if len(ids) == 0:  # no instruments ound
     >>>     return
     >>> # Connect to the first available ArC TWO loading firmware "fw.bin"
     >>> arc = Instrument(ids[0], 'fw.bin')
 
     :param int port: The EFM id of the ArC TWO to connect to
     :param str firwmare: Path of the firmware to load
+    :param bool init: Run initialisation steps after loading firmware to
+                      bring ArC TWO to a known state (3.3 V logic and all
+                      DACs set at 0.0 V)
 
     :return: A new instance of ``pyarc2.Instrument``
     """
 
-    def __init__(self, port: int, firmware: str):
-        _InstrumentLL.__init__(port, firmware)
+    def __init__(self, port: int, firmware: str, init=True):
+        _InstrumentLL.__init__(port, firmware, init)
 
     def _array_iter_inner(self, mode: DataMode, rtype: ReadType):
         data = self.pick_one(mode, rtype)
         if data is None:
             return None
         return [data]
 
@@ -208,14 +211,18 @@
     def read_slice_masked(self, chan: int, mask: IntIterable, vread: float) -> np.ndarray:
         return super().read_slice_masked(chan, _ndarray_check(mask), vread)
 
     @_inheritdocs(_InstrumentLL.read_slice_open)
     def read_slice_open(self, highs: IntIterable, ground_after: bool) -> np.ndarray:
         return super().read_slice_open(_ndarray_check(highs), ground_after)
 
+    @_inheritdocs(_InstrumentLL.read_slice_open_deferred)
+    def read_slice_open_deferred(self, highs: IntIterable, ground_after: bool) -> 'Instrument':
+        return super().read_slice_open_deferred(_ndarray_check(highs), ground_after)
+
     @_inheritdocs(_InstrumentLL.pulse_slice_masked)
     def pulse_slice_masked(self, chan: int, voltage: float, nanos: int,
         mask: IntIterable) -> 'Instrument':
         i = super().pulse_slice_masked(chan, voltage, nanos, _ndarray_check(mask))
         return cast(Instrument, i)
 
     @_inheritdocs(_InstrumentLL.pulseread_slice_masked)
@@ -228,18 +235,27 @@
     def currents_from_address(self, addr: int, chans: IntIterable) -> np.ndarray:
         return super().currents_from_address(addr, _ndarray_check(chans))
 
     @_inheritdocs(_InstrumentLL.vread_channels)
     def vread_channels(self, chans: IntIterable, averaging: bool) -> List[float]:
         return super().vread_channels(_ndarray_check(chans), averaging)
 
+    @_inheritdocs(_InstrumentLL.vread_channels_deferred)
+    def vread_channels_deferred(self, chans: IntIterable, averaging: bool) -> 'Instrument':
+        return super().vread_channels_deferred(_ndarray_check(chans), averaging)
+
     @_inheritdocs(_InstrumentLL.generate_read_train)
     def generate_read_train(self, lows: Optional[IntIterable], highs: IntIterable,
         vread: float, nreads: int, inter_nanos: int, ground: bool) -> 'Instrument':
         return super().generate_read_train(_ndarray_check(lows),
             _ndarray_check(highs), vread, nreads, inter_nanos, ground)
 
     @_inheritdocs(_InstrumentLL.generate_vread_train)
     def generate_vread_train(self, chans: IntIterable, averaging: bool, npulses: int,
         inter_nanos: int) -> 'Instrument':
         return super().generate_vread_train(_ndarray_check(chans), averaging, npulses,
             inter_nanos)
+
+    @_inheritdocs(_InstrumentLL.set_logic)
+    def set_logic(self, mask: int, cl0: Optional[IODir] = None, cl1: Optional[IODir] = None,
+        cl2: Optional[IODir] = None, cl3: Optional[IODir] = None) -> 'Instrument':
+        return super().set_logic(mask, cl0, cl1, cl2, cl3)
```

### Comparing `pyarc2-0.4.0/pyarc2/pyarc2.pyi` & `pyarc2-0.5.0/pyarc2/pyarc2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     CREF: ClassVar[pyarc2.AuxDACFn] = ...
     CSET: ClassVar[pyarc2.AuxDACFn] = ...
     @classmethod
     def __init__(cls) -> None: ...
 
 class InstrumentLL:
     @classmethod
-    def __init__(cls, port: int, fw: str) -> None: ...
+    def __init__(cls, port: int, fw: str, init: Optional[bool]) -> None: ...
     def bit_currents_from_address(self, addr: int) -> np.ndarray: ...
     def busy(self) -> bool: ...
     def config_channels(self, input: Iterable[tuple[int, float]], base: Optional[float]) -> InstrumentLL: ...
     def config_aux_channels(self, input: Iterable[tuple[AuxDACFn, float]]) -> InstrumentLL: ...
     def config_selectors(self, input: Iterable[int]) -> InstrumentLL: ...
     def connect_to_gnd(self, chans: IntIterable) -> InstrumentLL: ...
     def gnd_add(self, chans: IntIterable) -> InstrumentLL: ...
@@ -83,19 +83,21 @@
     def pulseread_slice_masked(self, chan: int, mask: IntIterable, vpulse: float,
         nanos: int, vread: float) -> np.ndarray: ...
     def read_all(self, vread: float, order: BiasOrder) -> np.ndarray: ...
     def read_one(self, low: int, high: int, vread: float) -> float: ...
     def read_slice(self, chan: int, vread: float) -> np.ndarray: ...
     def read_slice_masked(self, chan: int, mask: IntIterable, vread: float) -> np.ndarray: ...
     def read_slice_open(self, highs: IntIterable, ground_after: bool) -> np.ndarray: ...
+    def read_slice_open_deferred(self, highs: IntIterable, ground_after: bool) -> InstrumentLL: ...
     def vread_channels(self, chans: IntIterable, averaging: bool) -> List[float]: ...
+    def vread_channels_deferred(self, chans: IntIterable, averaging: bool) -> InstrumentLL: ...
     def read_train(self, low: int, high: int, vread: float, interpulse: int,
         preload: Optional[float], condition: WaitFor) -> None: ...
     def set_control_mode(self, mode: ControlMode) -> InstrumentLL: ...
-    def set_logic(self, mask: int) -> InstrumentLL: ...
+    def set_logic(self, mask: int, cl0: Optional[pyarc2.IODir], cl1: Optional[pyarc2.IODir], cl2: Optional[pyarc2.IODir], cl3: Optional[pyarc2.IODir]) -> InstrumentLL: ...
     def wait(self) -> None: ...
     def word_currents_from_address(self, addr: int) -> np.ndarray: ...
 
 class ReadAfter:
     Block: ClassVar[pyarc2.ReadAfter] = ...
     Never: ClassVar[pyarc2.ReadAfter] = ...
     Pulse: ClassVar[pyarc2.ReadAfter] = ...
```

### Comparing `pyarc2-0.4.0/src/lib.rs` & `pyarc2-0.5.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #[cfg(all(any(target_os = "windows", target_os = "linux"), target_arch = "x86_64"))]
 use libarc2::Instrument;
 
 use libarc2::{BiasOrder, ControlMode, DataMode, ReadAt, ReadAfter, ReadType, find_ids, WaitFor};
 use libarc2::ArC2Error as LLArC2Error;
-use libarc2::registers::{IOMask, AuxDACFn};
+use libarc2::registers::{IOMask, IODir, AuxDACFn};
 use ndarray::{Ix1, Ix2, Array};
 use numpy::{PyArray, PyReadonlyArray};
 use std::convert::{From, Into, TryInto};
 use numpy::convert::IntoPyArray;
 use pyo3::prelude::{pymodule, pyclass, pymethods};
 use pyo3::prelude::{PyModule, PyRefMut, PyResult, Python, PyErr};
 use pyo3::create_exception;
@@ -478,14 +478,69 @@
 
 impl From<&PyAuxDACFn> for AuxDACFn {
     fn from(func: &PyAuxDACFn) -> Self {
         func._inner
     }
 }
 
+/// Identifier for selecting the direction of GPIO pins. Typically used
+/// with :meth:`pyarc2.Instrument.set_logic`. The ArC TWO GPIOs are
+/// organised in 4 clusters of 8 contiguous GPIO channels. As such an IO
+/// direction is shared by all 8 channels that are on the same cluster.
+/// Cluster 0 is GPIO 0 to 7, Cluster 1 is GPIO 8 to 15, Cluster 2 is
+/// GPIO 16 to 23 and Cluster 4 is GPIO 24 to 32.
+#[pyclass(name="IODir", module="pyarc2")]
+#[derive(Clone)]
+struct PyIODir { _inner: IODir }
+
+#[allow(non_snake_case)]
+#[pymethods]
+impl PyIODir {
+
+    /// GPIO direction: Input
+    #[classattr]
+    fn IN() -> PyIODir {
+        PyIODir { _inner: IODir::IN }
+    }
+
+    /// GPIO direction: Output
+    #[classattr]
+    fn OUT() -> PyIODir {
+        PyIODir { _inner: IODir::OUT }
+    }
+
+    fn __str__(&self) -> String {
+        let inner = self._inner;
+        if inner == IODir::OUT {
+            "IODir.OUT".to_string()
+        } else {
+            "IODir.IN".to_string()
+        }
+    }
+
+}
+
+impl From<IODir> for PyIODir {
+    fn from(dir: IODir) -> Self {
+        PyIODir { _inner: dir }
+    }
+}
+
+impl From<PyIODir> for IODir {
+    fn from(dir: PyIODir) -> Self {
+        dir._inner
+    }
+}
+
+impl From<&PyIODir> for IODir {
+    fn from(dir: &PyIODir) -> Self {
+        dir._inner
+    }
+}
+
 /// Catch-all exception for low-level ArC2 errors
 /// --
 #[pyclass(name="ArC2Error", module="pyarc2")]
 struct PyArC2Error { _inner: LLArC2Error }
 
 #[pymethods]
 impl PyArC2Error {
@@ -543,16 +598,20 @@
 }
 
 #[cfg(all(any(target_os = "windows", target_os = "linux"), target_arch = "x86_64"))]
 #[pymethods]
 impl PyInstrument {
 
     #[new(name="InstrumentLL")]
-    fn new(id: i32, fw: &str) -> PyResult<Self> {
-        match Instrument::open_with_fw(id, fw, true) {
+    fn new(id: i32, fw: &str, init: Option<bool>) -> PyResult<Self> {
+        let actual_init = match init {
+            Some(x) => x,
+            None => true
+        };
+        match Instrument::open_with_fw(id, fw, true, actual_init) {
             Ok(instr) => Ok(PyInstrument { _instrument: instr }),
             Err(err) => Err(ArC2Error::new_exception(err))
         }
     }
 
     /// delay(self, nanos, /)
     /// --
@@ -875,14 +934,33 @@
 
         let data = self._instrument.read_all(vread, order.into()).unwrap();
         let array = Array::from_shape_vec((32, 32), data).unwrap();
 
         array.into_pyarray(py)
     }
 
+    /// read_slice_open_deferred(self, highs, ground_after, /)
+    /// --
+    ///
+    /// Perform an open current measurement along the specified channels without immediately
+    /// returning a value. This can be used in an calling sequence that involves multiple
+    /// steps without flushing the internal command buffer.
+    fn read_slice_open_deferred<'py>(mut slf: PyRefMut<'py, Self>, highs: PyReadonlyArray<usize, Ix1>,
+        ground_after: Option<bool>) -> PyResult<PyRefMut<'py, Self>> {
+
+        let slice = highs.as_slice().unwrap();
+        let ground = ground_after.unwrap_or(true);
+
+        match slf._instrument.read_slice_open_deferred(slice, ground) {
+            Ok(_) => Ok(slf),
+            Err(err) => Err(ArC2Error::new_exception(err))
+        }
+
+    }
+
     /// read_slice_open(self, highs, ground_after, /)
     /// --
     ///
     /// Perform an open current measurement along the specified channels. This method does not do
     /// any bias-related setup. It's up to the user to setup channels before performing the read.
     /// If ``ground_after`` is True or None a ground operation will additionally be issued
     /// post-read.
@@ -1121,27 +1199,50 @@
         Array::from_shape_vec((32, 32), data).unwrap().into_pyarray(py)
 
     }
 
     /// vread_channels(self, chans, averaging, /)
     /// --
     ///
-    /// Do a voltage read across selected channels.
+    /// Do a voltage read across selected channels flushing the internal
+    /// command buffer and immediately returning a value.
     ///
     /// :param chans: A uint64 numpy array or Iterable of the channels to
     ///               read voltage from
     /// :param bool averaging: Whether averaging should be used
     ///
     /// :rtype: An array with the voltage readings of the selected channels
     ///         in ascending order
     fn vread_channels(&mut self, chans: PyReadonlyArray<usize, Ix1>, averaging: bool) -> Vec<f32> {
         let slice = chans.as_slice().unwrap();
         self._instrument.vread_channels(slice, averaging).unwrap()
     }
 
+    /// vread_channels_deferred(self, channels, averaging, /)
+    /// --
+    ///
+    /// Do a voltage read across selected channels without immediately returning
+    /// a value. This can be used in a calling sequence that involves multiple
+    /// steps without immediately flushing the internal command buffer.
+    ///
+    /// :param chans: A uint64 numpy array or Iterable of the channels to
+    ///               read voltage from
+    /// :param bool averaging: Whether averaging should be used
+    fn vread_channels_deferred<'py>(mut slf: PyRefMut<'py, Self>, chans: PyReadonlyArray<usize, Ix1>, averaging: bool) ->
+        PyResult<PyRefMut<'py, Self>> {
+
+        let slice = chans.as_slice().unwrap();
+
+        match slf._instrument.vread_channels_deferred(slice, averaging) {
+            Ok(_) => Ok(slf),
+            Err(err) => Err(ArC2Error::new_exception(err))
+        }
+
+    }
+
     /// execute(self, /)
     /// --
     ///
     /// Write everything in the command buffer to the instrument. This will cause ArC2
     /// to start executing the instructions provided.
     fn execute<'py>(mut slf: PyRefMut<'py, Self>) -> PyResult<PyRefMut<'py, Self>> {
         match slf._instrument.execute() {
@@ -1183,18 +1284,45 @@
     /// --
     ///
     /// Set the digital I/Os specified by ``mask`` to either high (when ``enable`` is ``True``)
     /// or low (when ``enable`` is ``False``). An :meth:`~pyarc2.Instrument.execute` is
     /// required to actually load the configuration.
     ///
     /// :param int mask: A ``u32`` bitmask of the channels this function will be applied to
-    fn set_logic<'py>(mut slf: PyRefMut<'py, Self>, mask: u32) -> PyResult<PyRefMut<'py, Self>> {
+    /// :param cl0: Direction of GPIO cluster 0 (channels 0–7). Defaults to output.
+    /// :param cl1: Direction of GPIO cluster 1 (channels 8–15). Defaults to output.
+    /// :param cl2: Direction of GPIO cluster 2 (channels 16–23). Defaults to output.
+    /// :param cl3: Direction of GPIO cluster 3 (channels 24–32). Defaults to output.
+    fn set_logic<'py>(mut slf: PyRefMut<'py, Self>, mask: u32,
+        cl0: Option<PyIODir>, cl1: Option<PyIODir>, cl2: Option<PyIODir>, cl3: Option<PyIODir>)
+        -> PyResult<PyRefMut<'py, Self>> {
+
         let mask = IOMask::from_vals(&[mask]);
 
-        match slf._instrument.set_logic(&mask) {
+        let actual_cl0 = match cl0 {
+            Some(x) => x._inner,
+            None => IODir::OUT
+        };
+
+        let actual_cl1 = match cl1 {
+            Some(x) => x._inner,
+            None => IODir::OUT
+        };
+
+        let actual_cl2 = match cl2 {
+            Some(x) => x._inner,
+            None => IODir::OUT
+        };
+
+        let actual_cl3 = match cl3 {
+            Some(x) => x._inner,
+            None => IODir::OUT
+        };
+
+        match slf._instrument.set_logic(actual_cl0, actual_cl1, actual_cl2, actual_cl3, &mask) {
             Ok(_) => Ok(slf),
             Err(err) => Err(ArC2Error::new_exception(err))
         }
     }
 
     /// currents_from_address(self, addr, channels, /)
     /// --
@@ -1443,14 +1571,15 @@
     m.add_class::<PyControlMode>()?;
     m.add_class::<PyDataMode>()?;
     m.add_class::<PyReadType>()?;
     m.add_class::<PyReadAt>()?;
     m.add_class::<PyReadAfter>()?;
     m.add_class::<PyWaitFor>()?;
     m.add_class::<PyAuxDACFn>()?;
+    m.add_class::<PyIODir>()?;
     m.add("ArC2Error", py.get_type::<ArC2Error>())?;
 
     m.setattr(intern!(m.py(), "LIBARC2_VERSION"), libarc2::LIBARC2_VERSION)?;
 
     Ok(())
 }
```

### Comparing `pyarc2-0.4.0/Cargo.lock` & `pyarc2-0.5.0/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "beastlink"
 version = "1.0.0"
 source = "git+https://github.com/arc-instruments/beastlink-rs#90e9203acbae0272cd1a216d674950662330579e"
 dependencies = [
  "ctor",
@@ -33,14 +33,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
  "funty",
  "radium",
@@ -68,17 +74,17 @@
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -91,38 +97,38 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libarc2"
-version = "0.4.0"
-source = "git+https://github.com/arc-instruments/libarc2?tag=0.4.0#cd9158375434882d0f1b54f4ffbd2d0c64104fa7"
+version = "0.5.0"
+source = "git+https://github.com/arc-instruments/libarc2?tag=0.5.0#307223d491707c8f352bbc713ec410c50c093239"
 dependencies = [
  "beastlink",
- "bitflags",
+ "bitflags 1.3.2",
  "bitvec",
  "lazy_static",
  "num-derive 0.4.2",
  "num-traits",
  "spin_sleep",
  "thiserror",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
@@ -154,17 +160,17 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-derive"
 version = "0.3.3"
@@ -180,31 +186,31 @@
 name = "num-derive"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.17.2"
@@ -224,47 +230,47 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyarc2"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "libarc2",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
@@ -326,17 +332,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -347,19 +353,19 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -388,17 +394,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -411,30 +417,30 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -459,130 +465,80 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
-name = "windows_i686_gnu"
-version = "0.52.4"
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
```

### Comparing `pyarc2-0.4.0/pyproject.toml` & `pyarc2-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pyarc2"
-version = "0.4.0"
+version = "0.5.0"
 description = "High level Python bindings for the libarc2 library"
 authors = ["Spyros Stathopoulos <spyros@arc-instruments.co.uk>"]
 
 #include = ["src/*", "Cargo.toml", "tests/*"]
 #exclude = ["pyarc2/*so", "pyarc2/*dll", "pyarc2/*pyd"]
 
 [project]
 name = "pyarc2"
-version = "0.4.0"
+version = "0.5.0"
 description = "High level Python bindings for the libarc2 library"
 readme = "README.md"
 authors = [
   { name = "Spyros Stathopoulos <spyros@arc-instruments.co.uk>"},
   { email = "spyros@arc-instruments.co.uk" }
 ]
 homepage = "http://arc-instruments.co.uk/"
```

### Comparing `pyarc2-0.4.0/PKG-INFO` & `pyarc2-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyarc2
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
@@ -24,15 +24,15 @@
 License: MPL-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/arc-instruments/pyarc2
 
 # Python bindings for libarc2
 
-[![](https://img.shields.io/badge/-docs-default?logo=gitbook&logoColor=white)](https://files.arc-instruments.co.uk/documents/pyarc2/latest/)
+[![](https://img.shields.io/badge/-docs-default?logo=gitbook&logoColor=white)](https://files.arc-instruments.co.uk/documents/pyarc2/0.5.0/)
 
 ## Introduction
 
 This library presents a python interface to the low-level `libarc2` library
 used to interface with ArC TWO™. Most of the user-facing facilities of
 `libarc2` are present in this library. That being said, `pyarc2` itself is
 still relatively low-level and a general understanding of the internals of
```

