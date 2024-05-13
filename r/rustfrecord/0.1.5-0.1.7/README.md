# Comparing `tmp/rustfrecord-0.1.5.tar.gz` & `tmp/rustfrecord-0.1.7.tar.gz`

## Comparing `rustfrecord-0.1.5.tar` & `rustfrecord-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 rustfrecord-0.1.5/Cargo.toml
--rw-r--r--   0      502       20     1341 2024-04-11 08:51:17.000000 rustfrecord-0.1.5/.devcontainer/devcontainer.json
--rw-r--r--   0      502       20     5102 2024-04-16 11:33:55.000000 rustfrecord-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0      502       20       85 2024-04-15 12:50:52.000000 rustfrecord-0.1.5/.gitignore
--rw-r--r--   0      502       20      166 2024-04-15 10:44:23.000000 rustfrecord-0.1.5/.vscode/settings.json
--rw-r--r--   0      502       20     1518 2024-04-17 08:48:24.000000 rustfrecord-0.1.5/README.md
--rw-r--r--   0      502       20     2536 2024-04-15 13:20:59.000000 rustfrecord-0.1.5/requirements-linux.txt
--rw-r--r--   0      502       20      508 2024-04-15 13:20:18.000000 rustfrecord-0.1.5/requirements-macos.txt
--rw-r--r--   0      502       20     1258 2024-04-17 12:52:44.000000 rustfrecord-0.1.5/src/lib.rs
--rw-r--r--   0      502       20     1571 2024-04-11 10:57:05.000000 rustfrecord-0.1.5/src/pyo3_tch.rs
--rw-r--r--   0      502       20     2297 2024-04-17 11:38:13.000000 rustfrecord-0.1.5/src/tfrecord_reader.rs
--rw-r--r--   0      502       20     1758 2024-04-17 12:59:35.000000 rustfrecord-0.1.5/test_rustfrecord.py
--rw-r--r--   0      502       20    45986 2024-04-17 12:54:10.000000 rustfrecord-0.1.5/Cargo.lock
--rw-r--r--   0      502       20      571 2024-04-16 07:56:44.000000 rustfrecord-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 rustfrecord-0.1.5/PKG-INFO
+-rw-r--r--   0     1001      127      486 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/tfrecord_reader/Cargo.toml
+-rw-r--r--   0     1001      127     2530 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/tfrecord_reader/src/lib.rs
+-rw-r--r--   0     1001      127      434 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/tfrecord_reader/src/tests.rs
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 rustfrecord-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      127     1341 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/.devcontainer/devcontainer.json
+-rw-r--r--   0     1001      127     5165 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127       85 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/.gitignore
+-rw-r--r--   0     1001      127      248 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/.vscode/settings.json
+-rw-r--r--   0     1001      127     1518 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/README.md
+-rw-r--r--   0     1001      127     2536 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/requirements-linux.txt
+-rw-r--r--   0     1001      127      508 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/requirements-macos.txt
+-rw-r--r--   0     1001      127     2443 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      127     2591 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/test_rustfrecord.py
+-rw-r--r--   0     1001      127    31442 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      127      571 2024-05-13 12:39:54.000000 rustfrecord-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 rustfrecord-0.1.7/PKG-INFO
```

### Comparing `rustfrecord-0.1.5/.devcontainer/devcontainer.json` & `rustfrecord-0.1.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.5/.github/workflows/CI.yml` & `rustfrecord-0.1.7/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
     strategy:
       matrix:
         platform:
           - runner: ubuntu-latest
             target: x86_64
           # Disable aarch64 for now due to torch-sys build issues
-          # - runner: ubuntu-latest
-          #   target: aarch64
+          - runner: ubuntu-latest
+            target: aarch64
 
     steps:
       - uses: actions/checkout@v4
 
       # - uses: actions/setup-python@v5
       #   with:
       #     python-version: ${{ env.PYTHON_VERSION }}
@@ -78,14 +78,15 @@
           before-script-linux: |
             # Install the correct version of libtorch
             # export GLIBCXX_USE_CXX11_ABI=0
 
             # Dependencies for building the torch-sys crate:
             python${{ env.PYTHON_VERSION }} -m pip install \
               torch==2.2.0 \
+              setuptools==69.5.1 `# seems necessary for aarch64` \
             ;
             # numpy==1.24.1 \
             # --index-url https://download.pytorch.org/whl/cpu
 
             ln -sf python${{ env.PYTHON_VERSION }} /usr/local/bin/python3 # manylinux x86_64
             ln -sf python${{ env.PYTHON_VERSION }} /usr/bin/python3 # manylinux aarch64
```

### Comparing `rustfrecord-0.1.5/README.md` & `rustfrecord-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.5/requirements-linux.txt` & `rustfrecord-0.1.7/requirements-linux.txt`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.5/src/tfrecord_reader.rs` & `rustfrecord-0.1.7/tfrecord_reader/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -3,73 +3,92 @@
     fs,
     io::Read,
     path::Path,
 };
 
 use anyhow::{Context, Result};
 use flate2::read::GzDecoder;
-use tch::Tensor;
 use tfrecord::{Example, ExampleIter, FeatureKind, RecordReaderConfig};
+pub use tfrecord::Error;
+
+#[cfg(test)]
+mod tests;
+
+pub enum Compression {
+    None,
+    Gzip,
+}
+
+pub enum Array {
+    Bytes(Vec<Vec<u8>>),
+    F32(Vec<f32>),
+    I64(Vec<i64>),
+    None,
+}
 
 pub struct Reader {
     example_iter: ExampleIter<Box<dyn Read + Send>>,
     features: HashSet<String>,
 }
 
 impl Reader {
-    pub fn new(filename: &str, compressed: bool, features: &[impl AsRef<str>]) -> Result<Self> {
+    pub fn new(
+        filename: &str,
+        compression: Compression,
+        features: &[impl AsRef<str>],
+    ) -> Result<Self> {
         let path = Path::new(filename);
 
         let conf = RecordReaderConfig {
             check_integrity: false,
         };
 
         let file = fs::File::open(path).with_context(|| format!("failed to open {path:?}"))?;
 
-        let reader: Box<dyn Read + Send> = if compressed {
-            Box::new(GzDecoder::new(file))
-        } else {
-            Box::new(file)
+        let reader: Box<dyn Read + Send> = match compression {
+            Compression::Gzip => Box::new(GzDecoder::new(file)),
+            Compression::None => Box::new(file),
         };
 
         let example_iter = ExampleIter::from_reader(reader, conf);
+        let features = features.iter().map(|s| s.as_ref().to_string()).collect();
 
         Ok(Self {
             example_iter,
-            features: features.iter().map(|s| s.as_ref().to_string()).collect(),
+            features,
         })
     }
 }
 
 impl Iterator for Reader {
     // Iterate over Examples.
     //
     // Comment from example.proto:
     //
     // An Example is a mostly-normalized data format for storing data for training and inference.
     // It contains a key-value store (features); where each key (string) maps to a Feature message
     // (which is one of packed BytesList, FloatList, or Int64List).
 
-    type Item = tfrecord::Result<HashMap<String, Tensor>>;
+    type Item = tfrecord::Result<HashMap<String, Array>>;
 
     fn next(&mut self) -> Option<Self::Item> {
         self.example_iter
             .next()
             .map(|e| e.map(|e| example_to_hashmap(e, &self.features)))
     }
 }
 
-fn example_to_hashmap(example: Example, features: &HashSet<String>) -> HashMap<String, Tensor> {
+fn example_to_hashmap(example: Example, features: &HashSet<String>) -> HashMap<String, Array> {
     example
         .into_iter()
         .filter(|(name, _)| features.is_empty() || features.contains(name))
         .map(|(name, feature)| {
-            let tensor = match feature.into_kinds() {
-                Some(FeatureKind::F32(value)) => Tensor::from_slice(&value),
-                Some(FeatureKind::I64(value)) => Tensor::from_slice(&value),
-                Some(FeatureKind::Bytes(value)) => Tensor::from_slice2(&value),
-                None => Tensor::new(),
+            let array = match feature.into_kinds() {
+                Some(FeatureKind::F32(value)) => Array::F32(value),
+                Some(FeatureKind::I64(value)) => Array::I64(value),
+                Some(FeatureKind::Bytes(value)) => Array::Bytes(value),
+                None => Array::None,
             };
-            (name, tensor)
+            (name, array)
         })
         .collect()
 }
```

### Comparing `rustfrecord-0.1.5/test_rustfrecord.py` & `rustfrecord-0.1.7/test_rustfrecord.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import torch
 from rustfrecord import Reader
 from torch import Tensor
 
+# torch.set_num_threads(1)
+# torch.set_num_interop_threads(1)
+
 
 class TFRecordDataset(torch.utils.data.IterableDataset):
     def __init__(self, filename: str, compressed: bool = True, features: list = None):
         super().__init__()
         self.filename = filename
         self.compressed = compressed
         self.features = features
@@ -15,58 +18,83 @@
             self.filename,
             compressed=self.compressed,
             features=self.features,
         )
         return iter(reader)
 
 
-def test_dataset():
-    filename = "data/002scattered.training_examples.tfrecord.gz"
+def test_loader():
+    filename = "data/002scattered.training_examples.tfrecord"
     ds = TFRecordDataset(
         filename,
-        compressed=True,
+        compressed=filename.endswith(".gz"),
         features=[
             "label",
             "image/encoded",
             "image/shape",
         ],
     )
+
+    batch_size = 256
+    loader = torch.utils.data.DataLoader(ds, batch_size=batch_size)
+
     print()
 
-    loader = torch.utils.data.DataLoader(ds, batch_size=100)
+    for i, batch in enumerate(loader):
+        labels: Tensor = batch["label"]
+        shapes: Tensor = batch["image/shape"]
+        images: Tensor = batch["image/encoded"]
+
+        j = 0
+        label = labels[j]
+        shape = torch.Size(tuple(shapes[j]))
+        image = images[j].reshape(shape)
+        print(f"batch={i} ({len(labels)}), {j=}, {label=}, {image.shape}")
+
 
-    for batch in enumerate(loader):
-        print(batch)
+def test_dataset():
+    filename = "data/002scattered.training_examples.tfrecord"
+
+    for _ in range(10):
+        ds = TFRecordDataset(
+            filename,
+            compressed=filename.endswith(".gz"),
+            features=[
+                "label",
+                "image/encoded",
+                "image/shape",
+            ],
+        )
 
-        # if i % 1000 == 0:
-        #     print(i)
+        print()
 
-        # break # Exit after a single batch
+        for i, features in enumerate(ds):
+            label: Tensor = features["label"]
+            shape = torch.Size(tuple(features["image/shape"]))
+            image: Tensor = features["image/encoded"][0].reshape(shape)
+
+            if i % 1000 == 0:
+                print(i, label, image.shape)
 
 
 def test_reader():
-    filename = "data/002scattered.training_examples.tfrecord.gz"
-    r = Reader(filename, compressed=True)
+    filename = "data/002scattered.training_examples.tfrecord"
 
-    for i, features in enumerate(r):
-        """
-        >>> print(i, features.keys())
-        [
-            "variant_type",
+    r = Reader(
+        filename,
+        compressed=filename.endswith(".gz"),
+        features=[
+            "label",
             "image/encoded",
             "image/shape",
-            "variant/encoded",
-            "label",
-            "alt_allele_indices/encoded",
-            "locus",
-            "sequencing_type",
-        ]
-        """
+        ],
+    )
+
+    print()
 
+    for i, features in enumerate(r):
         label: Tensor = features["label"]
         shape = torch.Size(tuple(features["image/shape"]))
         image: Tensor = features["image/encoded"][0].reshape(shape)
 
-        print(i, label, image.shape)
-
-        if i >= 3:
-            break
+        if i % 1000 == 0:
+            print(i, label, image.shape)
```

### Comparing `rustfrecord-0.1.5/Cargo.lock` & `rustfrecord-0.1.7/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -14,25 +14,14 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "aes"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
-dependencies = [
- "cfg-if",
- "cipher",
- "cpufeatures",
-]
-
-[[package]]
 name = "aho-corasick"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
@@ -65,147 +54,64 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
-
-[[package]]
-name = "base64ct"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
-
-[[package]]
-name = "bit_field"
-version = "0.10.2"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
-name = "block-buffer"
-version = "0.10.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
-name = "byteorder"
-version = "1.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
-
-[[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
-name = "bzip2"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
-dependencies = [
- "bzip2-sys",
- "libc",
-]
-
-[[package]]
-name = "bzip2-sys"
-version = "0.1.11+1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "736a955f3fa7875102d57c82b8cac37ec45224a07fd32d58f9f7a186b6cd4cdc"
-dependencies = [
- "cc",
- "libc",
- "pkg-config",
-]
-
-[[package]]
 name = "cc"
 version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
-dependencies = [
- "jobserver",
- "libc",
-]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "cipher"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
-dependencies = [
- "crypto-common",
- "inout",
-]
-
-[[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
 
 [[package]]
-name = "color_quant"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
-
-[[package]]
-name = "constant_time_eq"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
-
-[[package]]
-name = "cpufeatures"
-version = "0.2.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "crc"
 version = "3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69e6e4d7b33a94f0991c26729976b10ebde1d34c3ee82408fb536164fa10d636"
 dependencies = [
  "crc-catalog",
 ]
@@ -222,79 +128,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "crossbeam-deque"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
-dependencies = [
- "crossbeam-epoch",
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-epoch"
-version = "0.9.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
-dependencies = [
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-utils"
-version = "0.8.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
-
-[[package]]
-name = "crunchy"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
-
-[[package]]
-name = "crypto-common"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
-dependencies = [
- "generic-array",
- "typenum",
-]
-
-[[package]]
-name = "deranged"
-version = "0.3.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
-dependencies = [
- "powerfmt",
-]
-
-[[package]]
-name = "digest"
-version = "0.10.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
-dependencies = [
- "block-buffer",
- "crypto-common",
- "subtle",
-]
-
-[[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -305,43 +150,18 @@
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys",
 ]
 
 [[package]]
-name = "exr"
-version = "1.72.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "887d93f60543e9a9362ef8a21beedd0a833c5d9610e18c67abe15a5963dcb1a4"
-dependencies = [
- "bit_field",
- "flume",
- "half",
- "lebe",
- "miniz_oxide",
- "rayon-core",
- "smallvec",
- "zune-inflate",
-]
-
-[[package]]
 name = "fastrand"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
-
-[[package]]
-name = "fdeflate"
-version = "0.3.4"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
-dependencies = [
- "simd-adler32",
-]
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
@@ -365,112 +185,64 @@
 dependencies = [
  "crc32fast",
  "libz-ng-sys",
  "miniz_oxide",
 ]
 
 [[package]]
-name = "flume"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55ac459de2512911e4b674ce33cf20befaba382d05b62b008afc1c8b57cbf181"
-dependencies = [
- "spin",
-]
-
-[[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
-name = "generic-array"
-version = "0.14.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
-dependencies = [
- "typenum",
- "version_check",
-]
-
-[[package]]
 name = "getrandom"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
-name = "gif"
-version = "0.13.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb2d69b19215e18bb912fa30f7ce15846e301408695e44e0ef719f1da9e19f2"
-dependencies = [
- "color_quant",
- "weezl",
-]
-
-[[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
-name = "half"
-version = "2.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
-dependencies = [
- "cfg-if",
- "crunchy",
-]
-
-[[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
-name = "hmac"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
-dependencies = [
- "digest",
-]
-
-[[package]]
 name = "hostname"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c731c3e10504cc8ed35cfe2f1db4c9274c3d35fa486e3b31df46f068ef3e867"
 dependencies = [
  "libc",
  "match_cfg",
@@ -484,32 +256,14 @@
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
-name = "image"
-version = "0.24.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5690139d2f55868e080017335e4b94cb7414274c74f1669c84fb5feba2c9f69d"
-dependencies = [
- "bytemuck",
- "byteorder",
- "color_quant",
- "exr",
- "gif",
- "jpeg-decoder",
- "num-traits",
- "png",
- "qoi",
- "tiff",
-]
-
-[[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
@@ -518,23 +272,14 @@
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
-name = "inout"
-version = "0.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
 name = "integer-encoding"
 version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "924df4f0e24e2e7f9cdd90babb0b96f93b20f3ecfa949ea9e6613756b8c8e1bf"
 
 [[package]]
 name = "itertools"
@@ -551,50 +296,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
-name = "itoa"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
-
-[[package]]
-name = "jobserver"
-version = "0.1.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "jpeg-decoder"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
-dependencies = [
- "rayon",
-]
-
-[[package]]
-name = "lazy_static"
-version = "1.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
-
-[[package]]
-name = "lebe"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
-
-[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libz-ng-sys"
@@ -662,15 +371,14 @@
 [[package]]
 name = "miniz_oxide"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
- "simd-adler32",
 ]
 
 [[package]]
 name = "multimap"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "defc4c55412d89136f966bbb339008b474350e5e6e78d2714439c386b3137a03"
@@ -695,17 +403,17 @@
 checksum = "978fe6e6ebc0bf53de533cd456ca2d9de13de13856eda1518a285d7705a213af"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -728,20 +436,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "num-conv"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
-
-[[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
@@ -775,14 +477,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "numpy"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
+dependencies = [
+ "libc",
+ "ndarray",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "pyo3",
+ "rustc-hash",
+]
+
+[[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
@@ -813,37 +530,14 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "password-hash"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7676374caaee8a325c9e7a2ae557f216c5563a171d6997b0ef8a65af35147700"
-dependencies = [
- "base64ct",
- "rand_core",
- "subtle",
-]
-
-[[package]]
-name = "pbkdf2"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
-dependencies = [
- "digest",
- "hmac",
- "password-hash",
- "sha2",
-]
-
-[[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "petgraph"
@@ -852,51 +546,20 @@
 checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
-name = "pkg-config"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
-
-[[package]]
-name = "png"
-version = "0.17.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
-dependencies = [
- "bitflags 1.3.2",
- "crc32fast",
- "fdeflate",
- "flate2",
- "miniz_oxide",
-]
-
-[[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
-name = "powerfmt"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
-
-[[package]]
-name = "ppv-lite86"
-version = "0.2.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
-
-[[package]]
 name = "prettyplease"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
 dependencies = [
  "proc-macro2",
  "syn",
@@ -1024,88 +687,29 @@
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
-name = "qoi"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
-dependencies = [
- "bytemuck",
-]
-
-[[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "rand"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
-dependencies = [
- "libc",
- "rand_chacha",
- "rand_core",
-]
-
-[[package]]
-name = "rand_chacha"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
-dependencies = [
- "ppv-lite86",
- "rand_core",
-]
-
-[[package]]
-name = "rand_core"
-version = "0.6.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
-name = "rayon"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
-dependencies = [
- "either",
- "rayon-core",
-]
-
-[[package]]
-name = "rayon-core"
-version = "1.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
-dependencies = [
- "crossbeam-deque",
- "crossbeam-utils",
-]
-
-[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -1157,164 +761,90 @@
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustfrecord"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "anyhow",
- "flate2",
+ "numpy",
  "pyo3",
- "tch",
- "tfrecord",
- "torch-sys",
+ "tfrecord_reader",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
-name = "ryu"
-version = "1.0.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
-
-[[package]]
-name = "safetensors"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d93279b86b3de76f820a8854dd06cbc33cfa57a417b19c47f6a25280112fb1df"
-dependencies = [
- "serde",
- "serde_json",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "serde"
-version = "1.0.197"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
-dependencies = [
- "serde_derive",
-]
-
-[[package]]
-name = "serde_derive"
-version = "1.0.197"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "serde_json"
-version = "1.0.115"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
-dependencies = [
- "itoa",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "sha1"
-version = "0.10.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
-dependencies = [
- "cfg-if",
- "cpufeatures",
- "digest",
-]
-
-[[package]]
-name = "sha2"
-version = "0.10.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
-dependencies = [
- "cfg-if",
- "cpufeatures",
- "digest",
-]
-
-[[package]]
-name = "simd-adler32"
-version = "0.3.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d66dc143e6b11c1eddc06d5c423cfc97062865baf299914ab64caa38182078fe"
-
-[[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
-dependencies = [
- "lock_api",
-]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
@@ -1343,31 +873,14 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
-name = "tch"
-version = "0.15.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7cb00bc2770454b515388d45be7097a3ded2eca172f3dcdb7ca4cc06c40bf1"
-dependencies = [
- "half",
- "lazy_static",
- "libc",
- "ndarray",
- "rand",
- "safetensors",
- "thiserror",
- "torch-sys",
- "zip",
-]
-
-[[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -1383,31 +896,37 @@
  "anyhow",
  "bytemuck",
  "crc",
  "flate2",
  "glob",
  "hex",
  "hostname",
- "image",
  "integer-encoding",
  "itertools 0.11.0",
  "noisy_float",
  "num",
  "num-traits",
  "once_cell",
  "prost",
  "prost-build",
- "serde",
  "tar",
- "tch",
  "thiserror",
  "ureq",
 ]
 
 [[package]]
+name = "tfrecord_reader"
+version = "0.1.7"
+dependencies = [
+ "anyhow",
+ "flate2",
+ "tfrecord",
+]
+
+[[package]]
 name = "thiserror"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
@@ -1420,44 +939,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
-name = "tiff"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
-dependencies = [
- "flate2",
- "jpeg-decoder",
- "weezl",
-]
-
-[[package]]
-name = "time"
-version = "0.3.36"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
-dependencies = [
- "deranged",
- "num-conv",
- "powerfmt",
- "serde",
- "time-core",
-]
-
-[[package]]
-name = "time-core"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
-
-[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
@@ -1465,32 +954,14 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
-name = "torch-sys"
-version = "0.15.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29e0244e5b148a31dd7fe961165037d1927754d024095c1013937532d7e73a22"
-dependencies = [
- "anyhow",
- "cc",
- "libc",
- "zip",
-]
-
-[[package]]
-name = "typenum"
-version = "1.17.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
-
-[[package]]
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
@@ -1517,17 +988,17 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
  "base64",
  "flate2",
  "log",
  "once_cell",
  "rustls",
  "rustls-pki-types",
@@ -1544,20 +1015,14 @@
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
-name = "version_check"
-version = "0.9.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
-
-[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "webpki-roots"
@@ -1565,20 +1030,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
 dependencies = [
  "rustls-pki-types",
 ]
 
 [[package]]
-name = "weezl"
-version = "0.1.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
-
-[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -1598,15 +1057,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1618,110 +1077,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
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
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
@@ -1731,65 +1197,7 @@
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
-
-[[package]]
-name = "zip"
-version = "0.6.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
-dependencies = [
- "aes",
- "byteorder",
- "bzip2",
- "constant_time_eq",
- "crc32fast",
- "crossbeam-utils",
- "flate2",
- "hmac",
- "pbkdf2",
- "sha1",
- "time",
- "zstd",
-]
-
-[[package]]
-name = "zstd"
-version = "0.11.2+zstd.1.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
-dependencies = [
- "zstd-safe",
-]
-
-[[package]]
-name = "zstd-safe"
-version = "5.0.2+zstd.1.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
-dependencies = [
- "libc",
- "zstd-sys",
-]
-
-[[package]]
-name = "zstd-sys"
-version = "2.0.10+zstd.1.5.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
-dependencies = [
- "cc",
- "pkg-config",
-]
-
-[[package]]
-name = "zune-inflate"
-version = "0.2.54"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
-dependencies = [
- "simd-adler32",
-]
```

### Comparing `rustfrecord-0.1.5/pyproject.toml` & `rustfrecord-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.5/PKG-INFO` & `rustfrecord-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rustfrecord
-Version: 0.1.5
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: setuptools ==69.5.1
 Requires-Dist: torch ==2.2.0
 Requires-Dist: maturin ==1.5.1
 Requires-Dist: pip ==24.0
 Requires-Dist: numpy ==1.24.4
```

