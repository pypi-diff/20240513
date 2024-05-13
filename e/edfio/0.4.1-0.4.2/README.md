# Comparing `tmp/edfio-0.4.1.tar.gz` & `tmp/edfio-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edfio-0.4.1.tar", max compression
+gzip compressed data, was "edfio-0.4.2.tar", max compression
```

## Comparing `edfio-0.4.1.tar` & `edfio-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-30 09:51:37.185584 edfio-0.4.1/LICENSE
--rw-r--r--   0        0        0     3200 2024-04-30 09:51:37.189584 edfio-0.4.1/README.md
--rw-r--r--   0        0        0      481 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/__init__.py
--rw-r--r--   0        0        0     2349 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/_header_field.py
--rw-r--r--   0        0        0    40733 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf.py
--rw-r--r--   0        0        0     4733 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_annotations.py
--rw-r--r--   0        0        0     9612 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_header.py
--rw-r--r--   0        0        0    14927 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_signal.py
--rw-r--r--   0        0        0        0 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/py.typed
--rw-r--r--   0        0        0     1577 2024-04-30 09:51:48.585663 edfio-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 edfio-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 13:14:17.167001 edfio-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3200 2024-05-13 13:14:17.167001 edfio-0.4.2/README.md
+-rw-r--r--   0        0        0      481 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/__init__.py
+-rw-r--r--   0        0        0     2349 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/_header_field.py
+-rw-r--r--   0        0        0    41835 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/edf.py
+-rw-r--r--   0        0        0     4733 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/edf_annotations.py
+-rw-r--r--   0        0        0     9612 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/edf_header.py
+-rw-r--r--   0        0        0    15537 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/edf_signal.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:14:17.171001 edfio-0.4.2/edfio/py.typed
+-rw-r--r--   0        0        0     1577 2024-05-13 13:14:31.783192 edfio-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 edfio-0.4.2/PKG-INFO
```

### Comparing `edfio-0.4.1/LICENSE` & `edfio-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edfio-0.4.1/README.md` & `edfio-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `edfio-0.4.1/edfio/_header_field.py` & `edfio-0.4.2/edfio/_header_field.py`

 * *Files identical despite different names*

### Comparing `edfio-0.4.1/edfio/edf.py` & `edfio-0.4.2/edfio/edf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from fractions import Fraction
 from functools import singledispatch
 from math import ceil, floor
 from pathlib import Path
 from typing import Any, Literal
 
 import numpy as np
+import numpy.typing as npt
 
 from edfio._header_field import (
     decode_date,
     decode_float,
     decode_str,
     decode_time,
     encode_date,
@@ -200,15 +201,19 @@
         """
         return decode_str(self._local_recording_identification)
 
     @local_recording_identification.setter
     def local_recording_identification(self, value: str) -> None:
         self._local_recording_identification = encode_str(value, 80)
 
-    def _load_data(self, file: Path | io.BufferedReader | io.BytesIO) -> None:
+    def _load_data(
+        self, file: Path | io.BufferedReader | io.BytesIO, *, lazy_load_data: bool
+    ) -> None:
+        if lazy_load_data and not isinstance(file, Path):
+            raise ValueError("Lazy loading is only supported for local file paths")
         lens = [signal.samples_per_data_record for signal in self._signals]
         datarecord_len = sum(lens)
         truncated = False
         if not isinstance(file, Path):
             data_bytes = file.read()
             actual_records = len(data_bytes) // (datarecord_len * 2)
             if actual_records * datarecord_len * 2 < len(data_bytes):
@@ -238,15 +243,22 @@
                 f"EDF header indicates {self.num_data_records} data records, but file contains {actual_records} records. Updating header."
             )
             self._set_num_data_records(actual_records)
         ends = np.cumsum(lens)
         starts = ends - lens
 
         for signal, start, end in zip(self._signals, starts, ends):
-            signal._digital = datarecords[:, start:end].flatten()
+            if lazy_load_data:
+
+                def lazy_load(s: int = start, e: int = end) -> npt.NDArray[np.int16]:
+                    return datarecords[:, s:e].flatten()
+
+                signal._lazy_loader = lazy_load
+            else:
+                signal._digital = datarecords[:, start:end].flatten()
 
     def _read_header(self, buffer: io.BufferedReader | io.BytesIO) -> None:
         for header_name, length in Edf._header_fields:
             setattr(self, "_" + header_name, buffer.read(length))
         self._signals = self._parse_signal_headers(
             buffer.read(256 * self._total_num_signals)
         )
@@ -275,25 +287,25 @@
         self,
         signals: Sequence[EdfSignal],
     ) -> None:
         if not signals:
             num_data_records = 1
         else:
             signal_durations = [
-                round(len(s._digital) / s.sampling_frequency, 12) for s in signals
+                round(len(s.digital) / s.sampling_frequency, 12) for s in signals
             ]
             if any(v != signal_durations[0] for v in signal_durations[1:]):
                 raise ValueError(
                     f"Inconsistent signal durations (in seconds): {signal_durations}"
                 )
             num_data_records = _calculate_num_data_records(
                 signal_durations[0],
                 self.data_record_duration,
             )
-            signal_lengths = [len(s._digital) for s in signals]
+            signal_lengths = [len(s.digital) for s in signals]
             if any(l % num_data_records for l in signal_lengths):
                 raise ValueError(
                     f"Not all signal lengths can be split into {num_data_records} data records: {signal_lengths}"
                 )
         self._set_num_data_records(num_data_records)
 
     def _parse_signal_headers(self, raw_signal_headers: bytes) -> tuple[EdfSignal, ...]:
@@ -332,37 +344,35 @@
         ----------
         target : Path | str | io.BufferedWriter | io.BytesIO
             The file location (path object or string) or file-like object to write to.
         """
         if self.num_data_records == -1:
             warnings.warn("num_data_records=-1, determining correct value from data")
             num_data_records = _calculate_num_data_records(
-                len(self._signals[0]._digital) * self._signals[0].sampling_frequency,
+                len(self._signals[0].digital) * self._signals[0].sampling_frequency,
                 self.data_record_duration,
             )
         else:
             num_data_records = self.num_data_records
         for signal in self._signals:
-            signal._set_samples_per_data_record(
-                len(signal._digital) // num_data_records
-            )
+            signal._set_samples_per_data_record(len(signal.digital) // num_data_records)
         header_records = []
         for header_name, _ in Edf._header_fields:
             header_records.append(getattr(self, "_" + header_name))
         for header_name, _ in EdfSignal._header_fields:
             for signal in self._signals:
                 header_records.append(getattr(signal, "_" + header_name))
         header_record = b"".join(header_records)
 
         lens = [signal.samples_per_data_record for signal in self._signals]
         ends = np.cumsum(lens)
         starts = ends - lens
         data_record = np.empty((num_data_records, sum(lens)), dtype=np.int16)
         for signal, start, end in zip(self._signals, starts, ends):
-            data_record[:, start:end] = signal._digital.reshape((-1, end - start))
+            data_record[:, start:end] = signal.digital.reshape((-1, end - start))
 
         if isinstance(target, str):
             target = Path(target)
         if isinstance(target, io.BufferedWriter):
             target.write(header_record)
             data_record.tofile(target)
         elif isinstance(target, io.BytesIO):
@@ -475,15 +485,15 @@
         recording_subfields = self.local_recording_identification.split()
         recording_subfields[1] = _encode_edfplus_date(startdate)
         self.local_recording_identification = " ".join(recording_subfields)
 
     @property
     def _subsecond_offset(self) -> float:
         try:
-            timekeeping_raw = self._timekeeping_signal._digital.tobytes()
+            timekeeping_raw = self._timekeeping_signal.digital.tobytes()
             first_data_record = timekeeping_raw[: timekeeping_raw.find(b"\x00") + 1]
             return _EdfAnnotationsDataRecord.from_bytes(first_data_record).tals[0].onset
         except StopIteration:
             return 0
 
     @property
     def starttime(self) -> datetime.time:
@@ -505,15 +515,15 @@
     @starttime.setter
     def starttime(self, starttime: datetime.time) -> None:
         onset_change = starttime.microsecond / 1000000 - self._subsecond_offset
         self._starttime = encode_time(starttime.replace(microsecond=0))
         if starttime.microsecond != self.starttime.microsecond:
             timekeeping_signal = self._timekeeping_signal
             data_records = []
-            for data_record in timekeeping_signal._digital.reshape(
+            for data_record in timekeeping_signal.digital.reshape(
                 (-1, timekeeping_signal.samples_per_data_record)
             ):
                 annot_dr = _EdfAnnotationsDataRecord.from_bytes(data_record.tobytes())
                 for tal in annot_dr.tals:
                     tal.onset = round(tal.onset + onset_change, 12)
                 data_records.append(annot_dr.to_bytes())
             maxlen = max(len(data_record) for data_record in data_records)
@@ -632,15 +642,15 @@
         self, data_record_duration: float, num_data_records: int
     ) -> None:
         signals = list(self._signals)
         for idx, signal in enumerate(self._signals):
             if signal not in self._annotation_signals:
                 continue
             annotations = []
-            for data_record in signal._digital.reshape(
+            for data_record in signal.digital.reshape(
                 (-1, signal.samples_per_data_record)
             ):
                 annot_dr = _EdfAnnotationsDataRecord.from_bytes(data_record.tobytes())
                 if signal is self._timekeeping_signal:
                     annotations.extend(annot_dr.annotations[1:])
                 else:
                     annotations.extend(annot_dr.annotations)
@@ -655,15 +665,15 @@
                 subsecond_offset=self._subsecond_offset,
             )
         self._signals = tuple(signals)
 
     def _pad_or_truncate_data(self, new_duration: float) -> None:
         for signal in self.signals:
             n_samples = round(new_duration * signal.sampling_frequency)
-            diff = n_samples - len(signal._digital)
+            diff = n_samples - len(signal.digital)
             if diff > 0:
                 physical_pad_value = 0.0
                 if signal.physical_min > 0 or signal.physical_max < 0:
                     physical_pad_value = signal.physical_min
                 signal._set_data(
                     np.pad(signal.data, (0, diff), constant_values=physical_pad_value)
                 )
@@ -767,15 +777,15 @@
         """
         All annotations contained in the Edf, sorted chronologically.
 
         Does not include timekeeping annotations.
         """
         annotations: list[EdfAnnotation] = []
         for i, signal in enumerate(self._annotation_signals):
-            for data_record in signal._digital.reshape(
+            for data_record in signal.digital.reshape(
                 (-1, signal.samples_per_data_record)
             ):
                 annot_dr = _EdfAnnotationsDataRecord.from_bytes(data_record.tobytes())
                 if i == 0:
                     # from https://www.edfplus.info/specs/edfplus.html#timekeeping:
                     # The first annotation of the first 'EDF Annotations' signal in each
                     # data record is empty, but its timestamp specifies how many seconds
@@ -798,15 +808,15 @@
 
         Parameters
         ----------
         text : str
             All annotations whose text exactly matches this parameter are removed.
         """
         for signal in self._annotation_signals:
-            for data_record in signal._digital.reshape(
+            for data_record in signal.digital.reshape(
                 (-1, signal.samples_per_data_record)
             ):
                 annotations = _EdfAnnotationsDataRecord.from_bytes(
                     data_record.tobytes()
                 )
                 annotations.drop_annotations_with_text(text)
                 data_record[:] = np.frombuffer(
@@ -867,15 +877,15 @@
                         stop=stop,
                         keep_all_annotations=keep_all_annotations,
                     )
                 )
             else:
                 start_index = start * signal.sampling_frequency
                 stop_index = stop * signal.sampling_frequency
-                signal._digital = signal._digital[int(start_index) : int(stop_index)]
+                signal._digital = signal.digital[int(start_index) : int(stop_index)]
                 signals.append(signal)
         self._set_signals(signals)
         self._shift_startdatetime(int(start))
 
     def slice_between_annotations(
         self,
         start_text: str,
@@ -964,17 +974,15 @@
         *,
         start: float,
         stop: float,
         keep_all_annotations: bool,
     ) -> EdfSignal:
         is_timekeeping_signal = signal == self._timekeeping_signal
         annotations: list[EdfAnnotation] = []
-        for data_record in signal._digital.reshape(
-            (-1, signal.samples_per_data_record)
-        ):
+        for data_record in signal.digital.reshape((-1, signal.samples_per_data_record)):
             annot_dr = _EdfAnnotationsDataRecord.from_bytes(data_record.tobytes())
             if is_timekeeping_signal:
                 annotations.extend(annot_dr.annotations[1:])
             else:
                 annotations.extend(annot_dr.annotations)
         annotations = [
             EdfAnnotation(round(a.onset - start, 12), a.duration, a.text)
@@ -1009,60 +1017,67 @@
 
 def _calculate_data_record_duration(signals: Sequence[EdfSignal]) -> float:
     fs = (Fraction(s.sampling_frequency).limit_denominator(99999999) for s in signals)
     return math.lcm(*(fs_.denominator for fs_ in fs))
 
 
 @singledispatch
-def _read_edf(edf_file: Any) -> Edf:
+def _read_edf(edf_file: Any, *, lazy_load_data: bool) -> Edf:
     edf = object.__new__(Edf)
     edf._read_header(edf_file)
-    edf._load_data(edf_file)
+    edf._load_data(edf_file, lazy_load_data=lazy_load_data)
     return edf
 
 
 @_read_edf.register
-def _(edf_file: Path) -> Edf:
+def _(edf_file: Path, *, lazy_load_data: bool) -> Edf:
     edf = object.__new__(Edf)
     edf_file = edf_file.expanduser()
     with edf_file.open("rb") as file:
         edf._read_header(file)
-    edf._load_data(edf_file)
+    edf._load_data(edf_file, lazy_load_data=lazy_load_data)
     return edf
 
 
 @_read_edf.register
-def _(edf_file: str) -> Edf:
-    return _read_edf(Path(edf_file))
+def _(edf_file: str, *, lazy_load_data: bool) -> Edf:
+    return _read_edf(Path(edf_file), lazy_load_data=lazy_load_data)
 
 
 @_read_edf.register
-def _(edf_file: bytes) -> Edf:
-    return _read_edf(io.BytesIO(edf_file))
+def _(edf_file: bytes, *, lazy_load_data: bool) -> Edf:
+    return _read_edf(io.BytesIO(edf_file), lazy_load_data=lazy_load_data)
 
 
 # Pyright loses information about parameters for singledispatch functions. Hiding it
 # behind this normal function makes things work again.
 def read_edf(
     edf_file: Path
     | str
     | io.BufferedReader
     | io.BytesIO
     | bytes
     | tempfile.SpooledTemporaryFile[bytes],
+    lazy_load_data: bool | Literal["auto"] = "auto",
 ) -> Edf:
     """
     Read an EDF file into an :class:`Edf` object.
 
     If a file-like object is passed, its stream position is moved to EOF.
 
     Parameters
     ----------
     edf_file : Path | str | io.BufferedReader | io.BytesIO
         The file location (path object or string) or file-like object to read from.
+    lazy_load_data : bool | {"auto"}, default: "auto"
+        If `True`, the raw signal data is not loaded into memory until it is accessed. If `False`,
+        the data is loaded immediately. If `"auto"`, the data is loaded lazily if
+        the specified edf_file represents a local path and eagerly otherwise.
 
     Returns
     -------
     Edf
         The resulting :class:`Edf` object.
     """
-    return _read_edf(edf_file)
+    if lazy_load_data == "auto":
+        lazy_load_data = isinstance(edf_file, (Path, str))
+    return _read_edf(edf_file, lazy_load_data=lazy_load_data)
```

### Comparing `edfio-0.4.1/edfio/edf_annotations.py` & `edfio-0.4.2/edfio/edf_annotations.py`

 * *Files identical despite different names*

### Comparing `edfio-0.4.1/edfio/edf_header.py` & `edfio-0.4.2/edfio/edf_header.py`

 * *Files identical despite different names*

### Comparing `edfio-0.4.1/edfio/edf_signal.py` & `edfio-0.4.2/edfio/edf_signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,17 @@
         ("digital_min", 8),
         ("digital_max", 8),
         ("prefiltering", 80),
         ("samples_per_data_record", 8),
         ("reserved", 32),
     )
 
+    _digital: npt.NDArray[np.int16] | None = None
+    _lazy_loader: Callable[[], npt.NDArray[np.int16]] | None = None
+
     def __init__(
         self,
         data: npt.NDArray[np.float64],
         sampling_frequency: float,
         *,
         label: str = "",
         transducer_type: str = "",
@@ -293,14 +296,28 @@
 
     @property
     def sampling_frequency(self) -> float:
         """The sampling frequency in Hz."""
         return self._sampling_frequency
 
     @property
+    def digital(self) -> npt.NDArray[np.int16]:
+        """
+        Numpy array containing the digital (uncalibrated) signal values as 16-bit integers.
+
+        The values of the array may be accessed and modified directly.
+        """
+        if self._digital is None:
+            if self._lazy_loader is None:
+                raise ValueError("Signal data not set")
+            self._digital = self._lazy_loader()
+            self._lazy_loader = None
+        return self._digital
+
+    @property
     def data(self) -> npt.NDArray[np.float64]:
         """
         Numpy array containing the physical signal values as floats.
 
         To simplify avoiding inconsistencies between signal data and header fields,
         individual values in the returned array can not be modified. Use
         :meth:`EdfSignal.update_data` to overwrite with new physical data.
@@ -309,22 +326,22 @@
             gain, offset = _calculate_gain_and_offset(
                 self.digital_min,
                 self.digital_max,
                 self.physical_min,
                 self.physical_max,
             )
         except ZeroDivisionError:
-            data = self._digital.astype(np.float64)
+            data = self.digital.astype(np.float64)
             warnings.warn(
                 f"Digital minimum equals digital maximum ({self.digital_min}) for {self.label}, returning uncalibrated signal."
             )
         except ValueError:
-            data = self._digital.astype(np.float64)
+            data = self.digital.astype(np.float64)
         else:
-            data = (self._digital + offset) * gain
+            data = (self.digital + offset) * gain
         data.setflags(write=False)
         return data
 
     def update_data(
         self,
         data: npt.NDArray[np.float64],
         *,
@@ -340,36 +357,36 @@
             The new physical data.
         keep_physical_range : bool, default: False
             If `True`, the `physical_range` is not modified to accomodate the new data.
         sampling_frequency : float | None, default: None
             If not `None`, the `sampling_frequency` is updated to the new value. The new
             data must match the expected length for the new sampling frequency.
         """
-        expected_length = len(self._digital)
+        expected_length = len(self.digital)
         if (
             sampling_frequency is not None
             and sampling_frequency != self._sampling_frequency
         ):
             expected_length = self._get_expected_new_length(sampling_frequency)
         if len(data) != expected_length:
             raise ValueError(
-                f"Signal lengths must match: got {len(data)}, expected {len(self._digital)}."
+                f"Signal lengths must match: got {len(data)}, expected {len(self.digital)}."
             )
         physical_range = self.physical_range if keep_physical_range else None
         self._set_physical_range(physical_range, data)
         if sampling_frequency is not None:
             self._sampling_frequency = sampling_frequency
         self._set_data(data)
 
     def _get_expected_new_length(self, sampling_frequency: float) -> int:
         if sampling_frequency <= 0:
             raise ValueError(
                 f"Sampling frequency must be positive, got {sampling_frequency}"
             )
-        current_length = len(self._digital)
+        current_length = len(self.digital)
         expected_length_f = (
             sampling_frequency / self._sampling_frequency * current_length
         )
         if not math.isclose(expected_length_f, round(expected_length_f), rel_tol=1e-10):
             raise ValueError(
                 f"Sampling frequency of {sampling_frequency} results in non-integer number of samples ({expected_length_f})"
             )
```

### Comparing `edfio-0.4.1/pyproject.toml` & `edfio-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edfio"
-version = "0.4.1"
+version = "0.4.2"
 description = "Read and write EDF/EDF+ files."
 license = "Apache-2.0"
 authors = ["The Siesta Group <opensource@thesiestagroup.com>"]
 readme = "README.md"
 repository = "https://github.com/the-siesta-group/edfio"
 documentation = "https://edfio.readthedocs.io"
```

### Comparing `edfio-0.4.1/PKG-INFO` & `edfio-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edfio
-Version: 0.4.1
+Version: 0.4.2
 Summary: Read and write EDF/EDF+ files.
 Home-page: https://github.com/the-siesta-group/edfio
 License: Apache-2.0
 Author: The Siesta Group
 Author-email: opensource@thesiestagroup.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

