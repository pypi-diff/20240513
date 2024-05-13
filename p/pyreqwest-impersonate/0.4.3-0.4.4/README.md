# Comparing `tmp/pyreqwest_impersonate-0.4.3.tar.gz` & `tmp/pyreqwest_impersonate-0.4.4.tar.gz`

## Comparing `pyreqwest_impersonate-0.4.3.tar` & `pyreqwest_impersonate-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.3/Cargo.toml
--rw-r--r--   0     1001      127     8345 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      766 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/.gitignore
--rw-r--r--   0     1001      127     8506 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/README.md
--rw-r--r--   0     1001      127      343 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/README.md
--rw-r--r--   0     1001      127     3484 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3719 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/generate_image.py
--rw-r--r--   0     1001      127      144 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/requirements.txt
--rw-r--r--   0     1001      127      990 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark/server.py
--rw-r--r--   0     1001      127   112338 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/benchmark.jpg
--rw-r--r--   0     1001      127    30089 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/src/response.rs
--rw-r--r--   0     1001      127     6274 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/tests/test_client.py
--rw-r--r--   0     1001      127     8329 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/tests/test_defs.py
--rw-r--r--   0     1001      127    41289 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-05-08 00:05:27.000000 pyreqwest_impersonate-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     9575 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.4/Cargo.toml
+-rw-r--r--   0     1001      127     8111 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/.gitignore
+-rw-r--r--   0     1001      127     8529 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/README.md
+-rw-r--r--   0     1001      127      343 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3719 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/generate_image.py
+-rw-r--r--   0     1001      127      144 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark/server.py
+-rw-r--r--   0     1001      127   112102 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/benchmark.jpg
+-rw-r--r--   0     1001      127    29788 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/src/response.rs
+-rw-r--r--   0     1001      127     6232 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/tests/test_client.py
+-rw-r--r--   0     1001      127     8287 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/tests/test_defs.py
+-rw-r--r--   0     1001      127    41270 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-13 00:13:53.000000 pyreqwest_impersonate-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9598 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.4/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.4.3/Cargo.toml` & `pyreqwest_impersonate-0.4.4/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.4.3"
+version = "0.4.4"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
@@ -21,15 +21,14 @@
     "multipart",  # to send a multipart/form-data body
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
 encoding_rs = { version = "0.8" }
-form_urlencoded = "1"  # to serialize `data` parameter
 pythonize = "0.21"
 serde_json = "1"
 tokio = { version = "1", features = ["fs", "rt"] }
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
```

### Comparing `pyreqwest_impersonate-0.4.3/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.4/.github/workflows/CI.yml`

 * *Files 3% similar despite different names*

```diff
@@ -253,15 +253,10 @@
         run: python benchmark/benchmark.py
       - name: Generate image and commit
         run: |
           python benchmark/generate_image.py
           git config --global user.name 'GitHub Actions'
           git config --global user.email 'actions@github.com'
           git add \*.jpg
-          git commit -m "Update generated image" || echo "No changes to commit"
-          # Reattach HEAD to the branch that initiated the workflow
-          if [[ "${{ github.event_name }}" == "pull_request" ]]; then
-            git checkout "${{ github.head_ref }}"
-          elif [[ "${{ github.event_name }}" == "create" && "${{ github.event.action }}" == "tag" ]]; then
-            git checkout "${{ github.ref }}"
-          fi
-          git push https://${{ secrets.PUSH_TOKEN }}@github.com/${{ github.repository }}
+          git diff --quiet && git diff --staged --quiet || git commit -m "Update generated image"
+          # Attempt to push changes only if there are changes to commit
+          git push https://${{ secrets.PUSH_TOKEN }}@github.com/${{ github.repository }} || echo "No changes to push"
```

### Comparing `pyreqwest_impersonate-0.4.3/.gitignore` & `pyreqwest_impersonate-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/README.md` & `pyreqwest_impersonate-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,17 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
-                "safari_17_2_1"
-            OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
+            Safari: "safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16","safari_16.5","safari_17.2.1", 
+                "safari_17.4.1"
+            OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
             Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
```

### Comparing `pyreqwest_impersonate-0.4.3/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.4/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/benchmark/generate_image.py` & `pyreqwest_impersonate-0.4.4/benchmark/generate_image.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/benchmark/server.py` & `pyreqwest_impersonate-0.4.4/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/benchmark.jpg` & `pyreqwest_impersonate-0.4.4/benchmark.jpg`

 * *Files 22% similar despite different names*

#### Image content

```diff
@@ -1,21 +1,21 @@
    ;:;;@88888X88888S8888X%X888@8@88@88@S88@88X888@@X8@@8;;::
- ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %:  8;t %
+ ::88;XS:%8tSSttS%X%X:@8X%SSt.8%SSXSt%@%SS%S%.  .  %;  8;t %
 S:;t      .           ..     .  .          .      S8 . X%8 t
-8.:%  . .    .    .t%   ::        .   . S .  tt . S8.  X8%.t
-S ;%  .:St8  :X ;t%88  :X: ..;;X  :%.S8S88 ;X X.;8@8 .8 8X.%
-  :% X@%88 8SStS %:88;.S. X;:8@ @8. t88.@%888 @X%X88SS@88@ t
-  ;;;;tS@X8S8Xt:tt%%@88X%888X88@8888SX;@@888XSt:.@X88XX%:;;;
-   ;:;;@88888888888%88@88XS@88X8@888888X@@8888888@@S8@@@;;::
- .:@8;X%:tXtXS%tS%%%X;88@%SSS:@SSSSStt@%X%X@X... . . ..8@S.t
-S;;%   .              .:  .  .    .     .     .       .%8% t
-8t%t .   .  .        .  ::     .    .  .  . .X%.  . .  S8X.%
-S %%   . :.  X@.   ;t :;%; .  .   :% ..tX8 ;%.@. .:%@ 8 8t t
-  :% tX8X8t8SXtX@tt8.SS@%%t8X8:XS8:8Xt:8888@@8%t8%@8SX88 X.t
-  ;;;;tS8@8X8Xt;:%X8S88@S888888888@8@XS@X@888%%;%8@@8S8%;;;:
-   ;:;X88888888@8@8t88S8888X@88S88@@@88X@@X8XS888X88888XS:;:
- ;%88;SX:;@;XX%t@;%%X:88XSXS%:8SSSSStt@%X%S@S...:     .8XS %
-S..t    .             .:     ..    . .   .    .  .    .S8S t
-8;t%   .    ..t        .;8:.     .     .   .  %    .   t8S.%
-S %t.   .:. %t8%  :;%8@8:X    .   :%..:%X .t8.@ . : 8 S%8t.t
-  :% tXXSS:@ 8%@; 888X88. S88XS8X8  t;;@8888@8@;8;88@.88 X %
-  ;;;;tSX88@8Xt:.tX8@@X%S888X8888888@XX8@X8888;;%88@8X@%;;;:
+8.:%  . .    .    .S8   ;;        .   . S .  t; . S8   @8S %
+S ;%  .:S;@  :X ;;S88  ;8. ..t.@  :%.%8S8X.tX.@.t8S8 .8 8X.t
+  :% X@ t8 8@ttS.%:@8t.S. @:.8@ @8  t8@ %8@88 @XSX88SS888@.t
+  ;;;;;XX@8X8Xt:t;S%@88X%888X88@8888XX@8X888SSt.:@X@8@S%:;;:
+   ;:;;888888888888%88@88XS@88X8@888888%8@@888888@@X8@@@t:;:
+ . 88;XS:S8%XX%tXtS%X;88@%SSS:8SSSSS;;8tS%S@X...  . .  88S %
+S;%t  .. .            .:  .       . .    .      .     .t;8 t
+8t%%     .  .        .  :.   .  .      .   . @%    .  .%X. %
+S t%  .  ..  S8.   ;% .;S: .      :S ..t88.;% 8. .:t8 @% X t
+  :% %@8X@%8SXtX@%t88  X8S;X8X:XS8:8St;888X@X:S:@:@8@S88:8 %
+ .;;;;tS8X8X8Xt;:%X8X888S888@@8888@8@XX888@8@S;;t88@8S8St;;:
+   :;:X88888888@8@8%88S8888X888S88@8@88X8@S88X88@8@8@88X%;::
+ ;%88tSX:;8:XSSt8;S%X:88@SXSS.8SS%XStt@%S%S@X.: . ..   8%S.t
+S.:t    .             .:   . .      .  .    .    . .  .%8S %
+8;;%   .     .%      . .:8:   . .  .    .  .  ..   .   %8S.t
+S %%    .:. %;8% .:;%8@8.8 .      :% .:St ;;8:8. .: 8 S;8t.t
+  :t.tXXS8 @.88X; @88X888X;8X8;8X8  t;t@88@8@.%;8.88@ 88 X %
+  ;;;;tS@88888;::tX8X@XXS88888888888@XX88@88X%t;t88X8X@%;;;:
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 100
 Y resolution: 100
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 18641
+Number of unique colors: 18576
 Comment: 
 EXIF data:
```

### Comparing `pyreqwest_impersonate-0.4.3/src/lib.rs` & `pyreqwest_impersonate-0.4.4/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 use std::collections::HashMap;
 use std::str::FromStr;
 use std::sync::{Arc, OnceLock};
 use std::time::Duration;
 
-use form_urlencoded::Serializer;
 use pyo3::exceptions;
 use pyo3::prelude::*;
-use pyo3::types::{PyBytes, PyDict, PyList, PyString};
+use pyo3::types::{PyBool, PyBytes, PyDict, PyString};
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
 use reqwest_impersonate::multipart;
 use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
 use tokio::runtime::{self, Runtime};
 
@@ -24,32 +23,34 @@
         runtime::Builder::new_current_thread()
             .enable_all()
             .build()
             .unwrap()
     })
 }
 
-/// Converts a Python dictionary to a Rust HashMap.
-fn py_dict_to_hashmap(_py: Python, py_dict: &PyDict) -> PyResult<HashMap<String, Vec<String>>> {
-    let mut map = HashMap::new();
-    for (key, value) in py_dict.iter() {
-        let key: String = key.extract()?;
-        let values: Vec<String> = if let Ok(py_list) = value.downcast::<PyList>() {
-            // If the value is a list, extract each item as a String
-            py_list
-                .iter()
-                .map(|item| item.extract::<String>())
-                .collect::<PyResult<_>>()?
-        } else {
-            // If the value is not a list, treat it as a single-item list
-            vec![value.extract::<String>()?]
-        };
-        map.insert(key, values);
+/// python json.dumps
+fn json_dumps(py: Python, pydict: Option<&Bound<'_, PyDict>>) -> PyResult<String> {
+    let json_module = PyModule::import_bound(py, "json")?;
+    let dumps = json_module.getattr("dumps")?;
+    match pydict {
+        Some(dict) => dumps.call1((dict,))?.extract::<String>(),
+        None => Ok("".to_string()),
+    }
+}
+
+/// python urllib.parse.urlencode
+fn url_encode(py: Python, pydict: Option<&Bound<'_, PyDict>>) -> PyResult<String> {
+    let urllib_parse = PyModule::import_bound(py, "urllib.parse")?;
+    let urlencode = urllib_parse.getattr("urlencode")?;
+    match pydict {
+        Some(dict) => urlencode
+            .call1((dict, ("doseq", py.get_type_bound::<PyBool>().call1(())?)))?
+            .extract::<String>(),
+        None => Ok("".to_string()),
     }
-    Ok(map)
 }
 
 #[pyclass]
 /// HTTP client that can impersonate web browsers.
 pub struct Client {
     client: Arc<reqwest_impersonate::Client>,
     auth: Option<(String, Option<String>)>,
@@ -125,16 +126,16 @@
             return Err(PyErr::new::<exceptions::PyValueError, _>(
                 "Cannot provide both auth and auth_bearer",
             ));
         }
 
         // Client builder
         let mut client_builder = reqwest_impersonate::Client::builder()
-            .enable_ech_grease(true)
-            .permute_extensions(true);
+            .enable_ech_grease()
+            .permute_extensions();
 
         // Headers
         if let Some(headers) = headers {
             let mut headers_new = HeaderMap::new();
             for (key, value) in headers {
                 headers_new.insert(
                     HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
@@ -257,25 +258,21 @@
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         let client = Arc::clone(&self.client);
         let auth = auth.or(self.auth.clone());
         let auth_bearer = auth_bearer.or(self.auth_bearer.clone());
         let params = params.or(self.params.clone());
         // Converts 'data' (if any) into a URL-encoded string for sending the data as `application/x-www-form-urlencoded` content type.
-        let data_str: Option<String> = data.map(|data_pydict| {
-            let data_map = py_dict_to_hashmap(py, data_pydict.as_gil_ref()).unwrap();
-            let mut serializer = Serializer::new(String::new());
-            let flattened_pairs = data_map.into_iter().flat_map(|(key, values)| {
-                values.into_iter().map(move |value| (key.to_owned(), value))
-            });
-            serializer.extend_pairs(flattened_pairs);
-            serializer.finish()
-        });
-        // Converts 'json' (if any) into a string for sending the data as `application/json` content type.
-        let json_str: Option<String> = json.map(|json_data| json_data.to_string());
+        let data_str = data
+            .map(|data_pydict| url_encode(py, Some(data_pydict)).ok())
+            .unwrap_or_else(|| None);
+        // Converts 'json' (if any) into a JSON string for sending the data as `application/json` content type.
+        let json_str = json
+            .map(|json_pydict| json_dumps(py, Some(json_pydict)).ok())
+            .unwrap_or_else(|| None);
 
         let future = async move {
             // Check if method is POST || PUT || PATCH
             let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
 
             // Method
             let method = match method {
```

### Comparing `pyreqwest_impersonate-0.4.3/src/response.rs` & `pyreqwest_impersonate-0.4.4/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/tests/test_client.py` & `pyreqwest_impersonate-0.4.4/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    assert json_data["data"] == "{\'key1\': \'value1\', \'key2\': \'value2\'}"
+    assert json_data["json"] == data
 
 
 @retry()
 def test_client_impersonate_chrome124():
     client = Client(impersonate="chrome_124", verify=False)
     response = client.get("https://tls.peet.ws/api/all")
     assert response.status_code == 200
```

### Comparing `pyreqwest_impersonate-0.4.3/tests/test_defs.py` & `pyreqwest_impersonate-0.4.4/tests/test_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     )
     assert response.status_code == 200
     json_data = response.json()
     assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
-    assert json_data["data"] == "{\'key1\': \'value1\', \'key2\': \'value2\'}"
+    assert json_data["json"] == data
 
 
 @retry()
 def test_patch():
     auth_bearer = "bearerXXXXXXXXXXXXXXXXXXXX"
     headers = {"X-Test": "test"}
     params = {"x": "aaa", "y": "bbb"}
```

### Comparing `pyreqwest_impersonate-0.4.3/Cargo.lock` & `pyreqwest_impersonate-0.4.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 name = "antidote"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34fde25430d87a9388dadbe6e34d7f72a462c8b43ac8d309b42b0a8505d7e2a5"
 
 [[package]]
 name = "async-compression"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e9eabd7a98fe442131a17c316bd9349c43695e49e730c3c8e12cfb5f4da2693"
+checksum = "9c90a406b4495d129f00461241616194cb8a032c8d1c53c657f0961d5f8e0498"
 dependencies = [
- "brotli 5.0.0",
+ "brotli 6.0.0",
  "flate2",
  "futures-core",
  "memchr",
  "pin-project-lite",
  "tokio",
 ]
 
@@ -154,17 +154,17 @@
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor 2.5.1",
 ]
 
 [[package]]
 name = "brotli"
-version = "5.0.0"
+version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
+checksum = "74f7971dbd9326d58187408ab83117d8ac1bb9c17b085fdacd1cf2f598719b6b"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor 4.0.0",
 ]
 
 [[package]]
@@ -884,18 +884,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.4.3"
+version = "0.4.4"
 dependencies = [
  "encoding_rs",
- "form_urlencoded",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
  "tokio",
 ]
 
@@ -954,17 +953,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest-impersonate"
-version = "0.11.77"
+version = "0.11.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7be6af65af12d9582d7fe87c3c0ba91e1312097d0b381223b5a1c186370dac27"
+checksum = "1b3ef1d8a08ef2150db45aae7e85dce08b96747357857fe4537cddd59624dc74"
 dependencies = [
  "async-compression",
  "base64",
  "boring-imp",
  "boring-sys-imp",
  "bytes",
  "cookie",
@@ -1024,37 +1023,37 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1098,17 +1097,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
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

### Comparing `pyreqwest_impersonate-0.4.3/pyproject.toml` & `pyreqwest_impersonate-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.3/PKG-INFO` & `pyreqwest_impersonate-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.4.3
+Version: 0.4.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -83,17 +83,17 @@
             in additional requests. Default is True.
         referer (bool, optional): Enable or disable automatic setting of the `Referer` header. Default is True.
         proxy (str, optional): Proxy URL for HTTP requests. Example: "socks5://127.0.0.1:9150". Default is None.
         impersonate (str, optional): Entity to impersonate. Example: "chrome_124". Default is None.
             Chrome: "chrome_99","chrome_100","chrome_101","chrome_104","chrome_105","chrome_106","chrome_108", 
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123","chrome_124"
-            Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5",
-                "safari_17_2_1"
-            OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
+            Safari: "safari_ios_17.2","safari_15.3","safari_15.5","safari_15.6.1","safari_16","safari_16.5","safari_17.2.1", 
+                "safari_17.4.1"
+            OkHttp: "okhttp_3.9","okhttp_3.11","okhttp_3.13","okhttp_3.14","okhttp_4.9","okhttp_4.10","okhttp_5"
             Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
```

