# Comparing `tmp/trame-rca-0.4.1.tar.gz` & `tmp/trame-rca-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-rca-0.4.1.tar", last modified: Wed Oct 18 16:06:10 2023, max compression
+gzip compressed data, was "trame-rca-0.4.2.tar", last modified: Mon May 13 21:40:11 2024, max compression
```

## Comparing `trame-rca-0.4.1.tar` & `trame-rca-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.237026 trame-rca-0.4.1/
--rw-r--r--   0 root         (0) root         (0)      583 2023-10-18 16:05:43.000000 trame-rca-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-10-18 16:05:43.000000 trame-rca-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1847 2023-10-18 16:06:10.237026 trame-rca-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1070 2023-10-18 16:05:43.000000 trame-rca-0.4.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      928 2023-10-18 16:06:10.237026 trame-rca-0.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-18 16:05:43.000000 trame-rca-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame/modules/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame/widgets/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame_rca/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame_rca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame_rca/module/
--rw-r--r--   0 root         (0) root         (0)      624 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame_rca/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame_rca/module/serve/
--rw-r--r--   0 root         (0) root         (0)    93424 2023-10-18 16:06:05.000000 trame-rca-0.4.1/trame_rca/module/serve/trame-rca.umd.js
--rw-r--r--   0 root         (0) root         (0)     2531 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame_rca/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.237026 trame-rca-0.4.1/trame_rca/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame_rca/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-10-18 16:05:43.000000 trame-rca-0.4.1/trame_rca/widgets/rca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 16:06:10.233026 trame-rca-0.4.1/trame_rca.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-10-18 16:06:10.000000 trame-rca-0.4.1/trame_rca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-10-18 16:06:10.000000 trame-rca-0.4.1/trame_rca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 16:06:10.000000 trame-rca-0.4.1/trame_rca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-10-18 16:06:10.000000 trame-rca-0.4.1/trame_rca.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-10-18 16:06:10.000000 trame-rca-0.4.1/trame_rca.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.143747 trame-rca-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-13 21:39:46.000000 trame-rca-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 21:39:46.000000 trame-rca-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1847 2024-05-13 21:40:11.143747 trame-rca-0.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-13 21:39:46.000000 trame-rca-0.4.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      928 2024-05-13 21:40:11.143747 trame-rca-0.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 21:39:46.000000 trame-rca-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.139747 trame-rca-0.4.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.139747 trame-rca-0.4.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame/modules/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.139747 trame-rca-0.4.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame/widgets/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.139747 trame-rca-0.4.2/trame_rca/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame_rca/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.143747 trame-rca-0.4.2/trame_rca/module/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame_rca/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.143747 trame-rca-0.4.2/trame_rca/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    93359 2024-05-13 21:40:07.000000 trame-rca-0.4.2/trame_rca/module/serve/trame-rca.umd.js
+-rw-r--r--   0 root         (0) root         (0)     2531 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame_rca/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.143747 trame-rca-0.4.2/trame_rca/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame_rca/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-05-13 21:39:46.000000 trame-rca-0.4.2/trame_rca/widgets/rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 21:40:11.143747 trame-rca-0.4.2/trame_rca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1847 2024-05-13 21:40:11.000000 trame-rca-0.4.2/trame_rca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2024-05-13 21:40:11.000000 trame-rca-0.4.2/trame_rca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 21:40:11.000000 trame-rca-0.4.2/trame_rca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-13 21:40:11.000000 trame-rca-0.4.2/trame_rca.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-13 21:40:11.000000 trame-rca-0.4.2/trame_rca.egg-info/top_level.txt
```

### Comparing `trame-rca-0.4.1/LICENSE` & `trame-rca-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-rca-0.4.1/PKG-INFO` & `trame-rca-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-rca
-Version: 0.4.1
+Version: 0.4.2
 Summary: Remote Controlled Area widget for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-rca-0.4.1/README.rst` & `trame-rca-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-rca-0.4.1/setup.cfg` & `trame-rca-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-rca
-version = 0.4.1
+version = 0.4.2
 description = Remote Controlled Area widget for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-rca-0.4.1/trame_rca/module/__init__.py` & `trame-rca-0.4.2/trame_rca/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-rca-0.4.1/trame_rca/module/serve/trame-rca.umd.js` & `trame-rca-0.4.2/trame_rca/module/serve/trame-rca.umd.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
         }
         update(t, r) {
             window.URL.revokeObjectURL(this.url), this.blob = new Blob([r], {
                 type: t
             }), this.url = URL.createObjectURL(this.blob), this.img.src = this.url
         }
     }
-    const tt = {
+    const Qe = {
         props: {
             name: {
                 type: String,
                 default: "default"
             },
             origin: {
                 type: String,
@@ -79,15 +79,15 @@
         queueChunk(t) {
             this.mediaSource.readyState === "open" && this.sourceBuffer && this.sourceBuffer.updating === !1 ? (this.sourceBuffer.appendBuffer(t), this.loaded += 1) : this.mediaSegments.push(t)
         }
         exit() {
             this.sourceBuffer.abort(), this.mediaSource.endOfStream(), this.videoElement.play(), URL.revokeObjectURL(this.videoElement.src)
         }
     }
-    const nt = {
+    const Ie = {
             props: {
                 name: {
                     type: String,
                     default: "default"
                 },
                 origin: {
                     type: String,
@@ -133,16 +133,16 @@
             template: `
     <video autoplay="autoplay" muted="muted" v-show="hasContent">
       Your browser does not support the video tag.
     </video>
   `
         },
         yn = 1,
-        dn = 2,
-        gn = 3,
+        gn = 2,
+        dn = 3,
         mn = 4,
         wn = 5,
         Sn = 6,
         En = `
 
 function reportError(e) {
   console.log(e.message);
@@ -230,29 +230,29 @@
             this.worker.postMessage({
                 action: r,
                 canvas: n
             }, [n])
         }
         setContentType(t, r, n) {
             if (this.codec !== t || this.width !== r || this.height !== n) {
-                const i = dn;
+                const a = gn;
                 this.codec = t, this.width = r, this.height = n, this.worker.postMessage({
-                    action: i,
+                    action: a,
                     config: {
                         codec: t,
                         codedWidth: r,
                         codedHeight: n
                     }
                 })
             }
         }
         pushChunk(t, r, n) {
-            const i = gn;
+            const a = dn;
             this.worker.postMessage({
-                action: i,
+                action: a,
                 timestamp: t,
                 type: r,
                 data: n
             }, [n])
         }
         flush() {
             this.worker.postMessage({
@@ -266,15 +266,15 @@
         }
         terminate() {
             this.worker.postMessage({
                 action: Sn
             }), this.worker.terminate(), this.worker = null
         }
     }
-    const rt = {
+    const et = {
             props: {
                 name: {
                     type: String,
                     default: "default"
                 },
                 origin: {
                     type: String,
@@ -293,16 +293,16 @@
                 if (this.isSupported) {
                     const e = this.$el.querySelector(".js-canvas");
                     this.worker.bindCanvas(e), this.onChunkAvailable = ([{
                         name: t,
                         meta: r,
                         content: n
                     }]) => {
-                        !r.type.includes("application/octet-stream") || !r.codec.length || r.codec.includes("unknown") || this.name === t && r.codec.length && (this.worker.setContentType(r.codec, r.w, r.h), n.arrayBuffer().then(i => {
-                            this.worker.pushChunk(r.st, r.key, i)
+                        !r.type.includes("application/octet-stream") || !r.codec.length || r.codec.includes("unknown") || this.name === t && r.codec.length && (this.worker.setContentType(r.codec, r.w, r.h), n.arrayBuffer().then(a => {
+                            this.worker.pushChunk(r.st, r.key, a)
                         }))
                     }, this.trame && (this.wslinkSubscription = this.trame.client.getConnection().getSession().subscribe("trame.rca.topic.stream", this.onChunkAvailable))
                 }
             },
             beforeUnmount() {
                 this.worker && (this.worker.terminate(), this.worker = null), this.wslinkSubscription && (this.trame && (this.trame.client.getConnection().getSession().unsubscribe(this.wslinkSubscription), this.wslinkSubscription = null), this.destroyDecoder())
             },
@@ -310,15 +310,15 @@
             template: `
     <div>
       <h1 v-if="!isSupported">WebCodecs API is not supported.</h1>
       <canvas class="js-canvas"></canvas>
     </div>
   `
         },
-        ot = {
+        tt = {
             props: {
                 name: {
                     type: String,
                     default: "default"
                 },
                 origin: {
                     type: String,
@@ -330,48 +330,49 @@
                     hasContent: !1
                 }
             },
             mounted() {
                 this.wslinkSubscription = null;
                 const e = this.$el,
                     t = e.getContext("2d");
-                this.onImage = ([{
+                this.onImage = async ([{
                     name: r,
                     meta: n,
-                    content: i
+                    content: a
                 }]) => {
-                    this.name === r && (n.type.includes("image/rgb24") ? i.arrayBuffer().then(h => {
-                        const v = new Uint8Array(h);
+                    if (this.name === r)
+                        if (n.type.includes("image/rgb24")) {
+                            const l = a.buffer ? a : new Uint8Array(await a.arrayBuffer());
+                            e.width = n.w, e.height = n.h;
+                            const v = t.createImageData(n.w, n.h),
+                                u = v.data;
+                            let i = 0,
+                                s = 0;
+                            for (; s < u.length;) u[s++] = l[i++], u[s++] = l[i++], u[s++] = l[i++], u[s++] = 255;
+                            t.putImageData(v, 0, 0), this.hasContent = !0
+                        } else if (n.type.includes("image/rgba32")) {
+                        const l = a.buffer ? a : new Uint8Array(await a.arrayBuffer());
                         e.width = n.w, e.height = n.h;
-                        const u = t.createImageData(n.w, n.h),
-                            a = u.data;
-                        let s = 0,
-                            c = 0;
-                        for (; c < a.length;) a[c++] = v[s++], a[c++] = v[s++], a[c++] = v[s++], a[c++] = 255;
-                        t.putImageData(u, 0, 0), this.hasContent = !0
-                    }) : n.type.includes("image/rgba32") ? i.arrayBuffer().then(h => {
-                        const v = new Uint8ClampedArray(h);
-                        e.width = n.w, e.height = n.h;
-                        const u = new ImageData(v, n.w, n.h);
-                        t.putImageData(u, 0, 0), this.hasContent = !0
-                    }) : this.hasContent = !1)
+                        const v = new ImageData(l, n.w, n.h);
+                        t.putImageData(v, 0, 0), this.hasContent = !0
+                    } else this.hasContent = !1
                 }, this.trame && (this.wslinkSubscription = this.trame.client.getConnection().getSession().subscribe("trame.rca.topic.stream", this.onImage))
             },
             beforeUnmount() {
                 this.wslinkSubscription && this.trame && (this.trame.client.getConnection().getSession().unsubscribe(this.wslinkSubscription), this.wslinkSubscription = null)
             },
             inject: ["trame"],
             template: '<canvas class="js-canvas" v-show="hasContent"></canvas>'
         },
-        Tn = {
+        kn = {
             components: {
-                ImageDisplayArea: tt,
-                MediaSourceDisplayArea: nt,
-                VideoDecoderDisplayArea: rt,
-                RawImageDisplayArea: ot
+                ImageDisplayArea: Qe,
+                MediaSourceDisplayArea: Ie,
+                VideoDecoderDisplayArea: et,
+                RawImageDisplayArea: tt
             },
             props: {
                 name: {
                     type: String,
                     default: "default"
                 },
                 origin: {
@@ -388,45 +389,45 @@
       <image-display-area v-if="display === 'image'" :name="name" :origin="origin" :poolSize="4" />
       <media-source-display-area v-if="display === 'media-source'" :name="name" :origin="origin" />
       <video-decoder-display-area v-if="display === 'video-decoder'" :name="name" :origin="origin" />
       <raw-image-display-area v-if="display === 'raw-image'" :name="name" :origin="origin" />
     </div>
   `
         },
-        kn = ["B/s", "KB/s", "MB/s"];
+        Tn = ["B/s", "KB/s", "MB/s"];
     class Rn {
         constructor(t = 255, r = 10, n = 1e3) {
             this.windowSize = t, this.windowStatSize = r, this.newInteractionThreshold = n, this.lastTS = 0, this.serverTime = [], this.clientTimes = [], this.packetSizes = [], this.statWindow = []
         }
         trim() {
             for (; this.serverTime.length > this.windowSize;) this.serverTime.shift(), this.clientTimes.shift(), this.packetSizes.shift();
             for (; this.statWindow.length > this.windowStatSize;) this.statWindow.shift()
         }
         compute() {
             if (this.statWindow.length < 2) return null;
             const t = this.statWindow[0],
                 n = (this.statWindow[this.statWindow.length - 1] - t) / (this.statWindow.length - 1),
-                i = 1e3 / n,
-                h = [],
+                a = 1e3 / n,
+                l = [],
                 v = [],
                 u = [0, 0];
-            let a = this.clientTimes[0],
+            let i = this.clientTimes[0],
                 s = this.serverTime[0],
                 c = 0;
-            for (let l = 0; l < this.clientTimes.length; l++) {
-                const p = this.clientTimes[l] - a,
-                    o = this.serverTime[l] - s;
-                c += this.packetSizes[l], h.push(p), v.push(o), a += n, s += n;
+            for (let h = 0; h < this.clientTimes.length; h++) {
+                const p = this.clientTimes[h] - i,
+                    o = this.serverTime[h] - s;
+                c += this.packetSizes[h], l.push(p), v.push(o), i += n, s += n;
                 const f = p < o ? p : o,
                     y = p > o ? p : o;
                 u[0] > f && (u[0] = f), u[1] < y && (u[1] = y)
             }
-            return c *= i / this.packetSizes.length, {
-                avgFps: i,
-                client: h,
+            return c *= a / this.packetSizes.length, {
+                avgFps: a,
+                client: l,
                 server: v,
                 minMax: u,
                 totalSize: c
             }
         }
         addEntry(t, r) {
             const n = Date.now();
@@ -492,43 +493,43 @@
                 this.monitor.newInteractionThreshold = e
             }
         },
         methods: {
             sizeUnit(e) {
                 let t = e;
                 for (let r = 0; r < 3; r++) {
-                    if (t < 1e3) return `${t.toFixed(1)} ${kn[r]}`;
+                    if (t < 1e3) return `${t.toFixed(1)} ${Tn[r]}`;
                     t /= 1e3
                 }
             },
             draw(e, t, r = "#1DE9B688", n = "#EF9A9A") {
                 if (!this.$el) return;
                 const {
-                    cw: i,
-                    ch: h
-                } = this, u = this.$el.querySelector(".js-canvas").getContext("2d"), a = Math.floor(h * .5 + .5), s = a / (1001 * this.fpsDelta), c = i / (e.length - 2);
-                u.clearRect(0, 0, i, h), u.strokeStyle = "black", u.beginPath(), u.moveTo(0, a), u.lineTo(i, a), u.stroke(), u.strokeStyle = "#eee";
-                for (let l = 0; l < this.fpsDelta; l++) u.beginPath(), u.moveTo(0, a + 1e3 * (l + 1) * s), u.lineTo(i, a + 1e3 * (l + 1) * s), u.stroke(), u.beginPath(), u.moveTo(0, a - 1e3 * (l + 1) * s), u.lineTo(i, a - 1e3 * (l + 1) * s), u.stroke();
-                u.strokeStyle = r, u.lineWidth = 8, u.beginPath(), u.moveTo(0, a - s * e[1]);
-                for (let l = 2; l < e.length; l++) u.lineTo((l - 1) * c, a - s * e[l]);
-                u.stroke(), u.strokeStyle = n, u.lineWidth = 2, u.beginPath(), u.moveTo(0, a - s * t[1]);
-                for (let l = 2; l < t.length; l++) u.lineTo((l - 1) * c, a - s * t[l]);
+                    cw: a,
+                    ch: l
+                } = this, u = this.$el.querySelector(".js-canvas").getContext("2d"), i = Math.floor(l * .5 + .5), s = i / (1001 * this.fpsDelta), c = a / (e.length - 2);
+                u.clearRect(0, 0, a, l), u.strokeStyle = "black", u.beginPath(), u.moveTo(0, i), u.lineTo(a, i), u.stroke(), u.strokeStyle = "#eee";
+                for (let h = 0; h < this.fpsDelta; h++) u.beginPath(), u.moveTo(0, i + 1e3 * (h + 1) * s), u.lineTo(a, i + 1e3 * (h + 1) * s), u.stroke(), u.beginPath(), u.moveTo(0, i - 1e3 * (h + 1) * s), u.lineTo(a, i - 1e3 * (h + 1) * s), u.stroke();
+                u.strokeStyle = r, u.lineWidth = 8, u.beginPath(), u.moveTo(0, i - s * e[1]);
+                for (let h = 2; h < e.length; h++) u.lineTo((h - 1) * c, i - s * e[h]);
+                u.stroke(), u.strokeStyle = n, u.lineWidth = 2, u.beginPath(), u.moveTo(0, i - s * t[1]);
+                for (let h = 2; h < t.length; h++) u.lineTo((h - 1) * c, i - s * t[h]);
                 u.stroke()
             }
         },
         created() {
             this.monitor = new Rn(this.historyWindowSize, this.statWindowSize), this.wslinkSubscription = null, this.onStreamPacket = ([e]) => {
                 const {
                     name: t,
                     serverTime: r,
                     contentSize: n
                 } = this.packetDecorator(e);
                 if (this.name === t) {
-                    const i = this.monitor.addEntry(r, n);
-                    i && (this.avg = i.avgFps, this.totalSize = i.totalSize, this.delta = 1e3 / (i.minMax[1] - i.minMax[0]), this.draw(i.client, i.server))
+                    const a = this.monitor.addEntry(r, n);
+                    a && (this.avg = a.avgFps, this.totalSize = a.totalSize, this.delta = 1e3 / (a.minMax[1] - a.minMax[0]), this.draw(a.client, a.server))
                 }
             }, this.trame && (this.wslinkSubscription = this.trame.client.getConnection().getSession().subscribe(this.wsLinkTopic, this.onStreamPacket)), this.observer = new ResizeObserver(() => {
                 if (!this.$el) return;
                 const {
                     width: e,
                     height: t
                 } = this.$el.getBoundingClientRect();
@@ -559,44 +560,44 @@
       </v-row>
       <canvas style="position: absolute; left: 0; top: 0;" class="js-canvas" :width="cw" :height="ch">
       </canvas>
     </v-col>
   `
     };
 
-    function Me(e, t) {
+    function De(e, t) {
         (t == null || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
 
     function Dn(e) {
-        if (Array.isArray(e)) return Me(e)
+        if (Array.isArray(e)) return De(e)
     }
 
     function jn(e) {
         if (typeof Symbol < "u" && e[Symbol.iterator] != null || e["@@iterator"] != null) return Array.from(e)
     }
 
-    function at(e, t) {
+    function nt(e, t) {
         if (e) {
-            if (typeof e == "string") return Me(e, t);
+            if (typeof e == "string") return De(e, t);
             var r = Object.prototype.toString.call(e).slice(8, -1);
             if (r === "Object" && e.constructor && (r = e.constructor.name), r === "Map" || r === "Set") return Array.from(e);
-            if (r === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return Me(e, t)
+            if (r === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return De(e, t)
         }
     }
 
     function Cn() {
         throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
     }
 
     function se(e) {
-        return Dn(e) || jn(e) || at(e) || Cn()
+        return Dn(e) || jn(e) || nt(e) || Cn()
     }
 
     function V(e, t, r) {
         return t in e ? Object.defineProperty(e, t, {
             value: r,
             enumerable: !0,
             configurable: !0,
@@ -608,78 +609,78 @@
         if (Array.isArray(e)) return e
     }
 
     function Ln(e, t) {
         var r = e == null ? null : typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
         if (r != null) {
             var n = [],
-                i = !0,
-                h = !1,
+                a = !0,
+                l = !1,
                 v, u;
             try {
-                for (r = r.call(e); !(i = (v = r.next()).done) && (n.push(v.value), !(t && n.length === t)); i = !0);
-            } catch (a) {
-                h = !0, u = a
+                for (r = r.call(e); !(a = (v = r.next()).done) && (n.push(v.value), !(t && n.length === t)); a = !0);
+            } catch (i) {
+                l = !0, u = i
             } finally {
                 try {
-                    !i && r.return != null && r.return()
+                    !a && r.return != null && r.return()
                 } finally {
-                    if (h) throw u
+                    if (l) throw u
                 }
             }
             return n
         }
     }
 
     function Fn() {
         throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
     }
 
-    function De(e, t) {
-        return _n(e) || Ln(e, t) || at(e, t) || Fn()
+    function je(e, t) {
+        return _n(e) || Ln(e, t) || nt(e, t) || Fn()
     }
 
     function K(e) {
         "@babel/helpers - typeof";
         return K = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
             return typeof t
         } : function(t) {
             return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         }, K(e)
     }
 
     function ue(e, t) {
-        return ue = Object.setPrototypeOf || function(n, i) {
-            return n.__proto__ = i, n
+        return ue = Object.setPrototypeOf || function(n, a) {
+            return n.__proto__ = a, n
         }, ue(e, t)
     }
 
     function Un() {
         if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
         if (typeof Proxy == "function") return !0;
         try {
             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
         } catch {
             return !1
         }
     }
 
     function ce(e, t, r) {
-        return Un() ? ce = Reflect.construct : ce = function(i, h, v) {
+        return Un() ? ce = Reflect.construct : ce = function(a, l, v) {
             var u = [null];
-            u.push.apply(u, h);
-            var a = Function.bind.apply(i, u),
-                s = new a;
+            u.push.apply(u, l);
+            var i = Function.bind.apply(a, u),
+                s = new i;
             return v && ue(s, v.prototype), s
         }, ce.apply(null, arguments)
     }
     var B = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-    function it(e) {
+    function rt(e) {
         return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e
     }
 
     function Bn(e) {
         if (e.__esModule) return e;
         var t = e.default;
         if (typeof t == "function") {
@@ -687,72 +688,72 @@
                 return this instanceof n ? Reflect.construct(t, arguments, this.constructor) : t.apply(this, arguments)
             };
             r.prototype = t.prototype
         } else r = {};
         return Object.defineProperty(r, "__esModule", {
             value: !0
         }), Object.keys(e).forEach(function(n) {
-            var i = Object.getOwnPropertyDescriptor(e, n);
-            Object.defineProperty(r, n, i.get ? i : {
+            var a = Object.getOwnPropertyDescriptor(e, n);
+            Object.defineProperty(r, n, a.get ? a : {
                 enumerable: !0,
                 get: function() {
                     return e[n]
                 }
             })
         }), r
     }
-    var Wn = function e(t, r) {
+    var $n = function e(t, r) {
         if (t === r) return !0;
         if (t && r && typeof t == "object" && typeof r == "object") {
             if (t.constructor !== r.constructor) return !1;
-            var n, i, h;
+            var n, a, l;
             if (Array.isArray(t)) {
                 if (n = t.length, n != r.length) return !1;
-                for (i = n; i-- !== 0;)
-                    if (!e(t[i], r[i])) return !1;
+                for (a = n; a-- !== 0;)
+                    if (!e(t[a], r[a])) return !1;
                 return !0
             }
             if (t.constructor === RegExp) return t.source === r.source && t.flags === r.flags;
             if (t.valueOf !== Object.prototype.valueOf) return t.valueOf() === r.valueOf();
             if (t.toString !== Object.prototype.toString) return t.toString() === r.toString();
-            if (h = Object.keys(t), n = h.length, n !== Object.keys(r).length) return !1;
-            for (i = n; i-- !== 0;)
-                if (!Object.prototype.hasOwnProperty.call(r, h[i])) return !1;
-            for (i = n; i-- !== 0;) {
-                var v = h[i];
+            if (l = Object.keys(t), n = l.length, n !== Object.keys(r).length) return !1;
+            for (a = n; a-- !== 0;)
+                if (!Object.prototype.hasOwnProperty.call(r, l[a])) return !1;
+            for (a = n; a-- !== 0;) {
+                var v = l[a];
                 if (!e(t[v], r[v])) return !1
             }
             return !0
         }
         return t !== t && r !== r
     };
-    const zn = it(Wn);
-    var st = Object.prototype.toString,
-        ut = function(t) {
-            var r = st.call(t),
+    const Wn = rt($n);
+    var ot = Object.prototype.toString,
+        at = function(t) {
+            var r = ot.call(t),
                 n = r === "[object Arguments]";
-            return n || (n = r !== "[object Array]" && t !== null && typeof t == "object" && typeof t.length == "number" && t.length >= 0 && st.call(t.callee) === "[object Function]"), n
+            return n || (n = r !== "[object Array]" && t !== null && typeof t == "object" && typeof t.length == "number" && t.length >= 0 && ot.call(t.callee) === "[object Function]"), n
         },
-        je, ct;
+        Ce, it;
 
-    function $n() {
-        if (ct) return je;
-        ct = 1;
+    function zn() {
+        if (it) return Ce;
+        it = 1;
         var e;
         if (!Object.keys) {
             var t = Object.prototype.hasOwnProperty,
                 r = Object.prototype.toString,
-                n = ut,
-                i = Object.prototype.propertyIsEnumerable,
-                h = !i.call({
+                n = at,
+                a = Object.prototype.propertyIsEnumerable,
+                l = !a.call({
                     toString: null
                 }, "toString"),
-                v = i.call(function() {}, "prototype"),
+                v = a.call(function() {}, "prototype"),
                 u = ["toString", "toLocaleString", "valueOf", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "constructor"],
-                a = function(p) {
+                i = function(p) {
                     var o = p.constructor;
                     return o && o.prototype === p
                 },
                 s = {
                     $applicationCache: !0,
                     $console: !0,
                     $external: !0,
@@ -777,184 +778,194 @@
                     $webkitStorageInfo: !0,
                     $window: !0
                 },
                 c = function() {
                     if (typeof window > "u") return !1;
                     for (var p in window) try {
                         if (!s["$" + p] && t.call(window, p) && window[p] !== null && typeof window[p] == "object") try {
-                            a(window[p])
+                            i(window[p])
                         } catch {
                             return !0
                         }
                     } catch {
                         return !0
                     }
                     return !1
                 }(),
-                l = function(p) {
-                    if (typeof window > "u" || !c) return a(p);
+                h = function(p) {
+                    if (typeof window > "u" || !c) return i(p);
                     try {
-                        return a(p)
+                        return i(p)
                     } catch {
                         return !1
                     }
                 };
             e = function(o) {
                 var f = o !== null && typeof o == "object",
                     y = r.call(o) === "[object Function]",
-                    g = n(o),
+                    d = n(o),
                     m = f && r.call(o) === "[object String]",
                     w = [];
-                if (!f && !y && !g) throw new TypeError("Object.keys called on a non-object");
-                var T = v && y;
+                if (!f && !y && !d) throw new TypeError("Object.keys called on a non-object");
+                var k = v && y;
                 if (m && o.length > 0 && !t.call(o, 0))
-                    for (var d = 0; d < o.length; ++d) w.push(String(d));
-                if (g && o.length > 0)
+                    for (var g = 0; g < o.length; ++g) w.push(String(g));
+                if (d && o.length > 0)
                     for (var S = 0; S < o.length; ++S) w.push(String(S));
                 else
-                    for (var E in o) !(T && E === "prototype") && t.call(o, E) && w.push(String(E));
-                if (h)
-                    for (var O = l(o), b = 0; b < u.length; ++b) !(O && u[b] === "constructor") && t.call(o, u[b]) && w.push(u[b]);
+                    for (var E in o) !(k && E === "prototype") && t.call(o, E) && w.push(String(E));
+                if (l)
+                    for (var O = h(o), b = 0; b < u.length; ++b) !(O && u[b] === "constructor") && t.call(o, u[b]) && w.push(u[b]);
                 return w
             }
         }
-        return je = e, je
+        return Ce = e, Ce
     }
     var Gn = Array.prototype.slice,
-        Nn = ut,
-        ft = Object.keys,
-        de = ft ? function(t) {
-            return ft(t)
-        } : $n(),
-        lt = Object.keys;
-    de.shim = function() {
+        Nn = at,
+        st = Object.keys,
+        ye = st ? function(t) {
+            return st(t)
+        } : zn(),
+        ut = Object.keys;
+    ye.shim = function() {
         if (Object.keys) {
             var t = function() {
                 var r = Object.keys(arguments);
                 return r && r.length === arguments.length
             }(1, 2);
             t || (Object.keys = function(n) {
-                return Nn(n) ? lt(Gn.call(n)) : lt(n)
+                return Nn(n) ? ut(Gn.call(n)) : ut(n)
             })
-        } else Object.keys = de;
-        return Object.keys || de
+        } else Object.keys = ye;
+        return Object.keys || ye
     };
-    var Vn = de,
-        Kn = function() {
+    var Vn = ye,
+        Kn = Error,
+        qn = EvalError,
+        Pn = RangeError,
+        Xn = ReferenceError,
+        ct = SyntaxError,
+        ft = TypeError,
+        Hn = URIError,
+        Yn = function() {
             if (typeof Symbol != "function" || typeof Object.getOwnPropertySymbols != "function") return !1;
             if (typeof Symbol.iterator == "symbol") return !0;
             var t = {},
                 r = Symbol("test"),
                 n = Object(r);
             if (typeof r == "string" || Object.prototype.toString.call(r) !== "[object Symbol]" || Object.prototype.toString.call(n) !== "[object Symbol]") return !1;
-            var i = 42;
-            t[r] = i;
+            var a = 42;
+            t[r] = a;
             for (r in t) return !1;
             if (typeof Object.keys == "function" && Object.keys(t).length !== 0 || typeof Object.getOwnPropertyNames == "function" && Object.getOwnPropertyNames(t).length !== 0) return !1;
-            var h = Object.getOwnPropertySymbols(t);
-            if (h.length !== 1 || h[0] !== r || !Object.prototype.propertyIsEnumerable.call(t, r)) return !1;
+            var l = Object.getOwnPropertySymbols(t);
+            if (l.length !== 1 || l[0] !== r || !Object.prototype.propertyIsEnumerable.call(t, r)) return !1;
             if (typeof Object.getOwnPropertyDescriptor == "function") {
                 var v = Object.getOwnPropertyDescriptor(t, r);
-                if (v.value !== i || v.enumerable !== !0) return !1
+                if (v.value !== a || v.enumerable !== !0) return !1
             }
             return !0
         },
-        ht = typeof Symbol < "u" && Symbol,
-        qn = Kn,
-        Pn = function() {
-            return typeof ht != "function" || typeof Symbol != "function" || typeof ht("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : qn()
+        lt = typeof Symbol < "u" && Symbol,
+        An = Yn,
+        Jn = function() {
+            return typeof lt != "function" || typeof Symbol != "function" || typeof lt("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : An()
         },
-        pt = {
+        _e = {
+            __proto__: null,
             foo: {}
         },
-        Xn = Object,
-        Hn = function() {
+        Zn = Object,
+        Qn = function() {
             return {
-                __proto__: pt
-            }.foo === pt.foo && !({
-                    __proto__: null
-                }
-                instanceof Xn)
-        },
-        Yn = "Function.prototype.bind called on incompatible ",
-        An = Object.prototype.toString,
-        Jn = Math.max,
-        Zn = "[object Function]",
-        vt = function(t, r) {
-            for (var n = [], i = 0; i < t.length; i += 1) n[i] = t[i];
-            for (var h = 0; h < r.length; h += 1) n[h + t.length] = r[h];
+                __proto__: _e
+            }.foo === _e.foo && !(_e instanceof Zn)
+        },
+        In = "Function.prototype.bind called on incompatible ",
+        er = Object.prototype.toString,
+        tr = Math.max,
+        nr = "[object Function]",
+        ht = function(t, r) {
+            for (var n = [], a = 0; a < t.length; a += 1) n[a] = t[a];
+            for (var l = 0; l < r.length; l += 1) n[l + t.length] = r[l];
             return n
         },
-        Qn = function(t, r) {
-            for (var n = [], i = r || 0, h = 0; i < t.length; i += 1, h += 1) n[h] = t[i];
+        rr = function(t, r) {
+            for (var n = [], a = r || 0, l = 0; a < t.length; a += 1, l += 1) n[l] = t[a];
             return n
         },
-        In = function(e, t) {
+        or = function(e, t) {
             for (var r = "", n = 0; n < e.length; n += 1) r += e[n], n + 1 < e.length && (r += t);
             return r
         },
-        er = function(t) {
+        ar = function(t) {
             var r = this;
-            if (typeof r != "function" || An.apply(r) !== Zn) throw new TypeError(Yn + r);
-            for (var n = Qn(arguments, 1), i, h = function() {
-                    if (this instanceof i) {
-                        var c = r.apply(this, vt(n, arguments));
+            if (typeof r != "function" || er.apply(r) !== nr) throw new TypeError(In + r);
+            for (var n = rr(arguments, 1), a, l = function() {
+                    if (this instanceof a) {
+                        var c = r.apply(this, ht(n, arguments));
                         return Object(c) === c ? c : this
                     }
-                    return r.apply(t, vt(n, arguments))
-                }, v = Jn(0, r.length - n.length), u = [], a = 0; a < v; a++) u[a] = "$" + a;
-            if (i = Function("binder", "return function (" + In(u, ",") + "){ return binder.apply(this,arguments); }")(h), r.prototype) {
+                    return r.apply(t, ht(n, arguments))
+                }, v = tr(0, r.length - n.length), u = [], i = 0; i < v; i++) u[i] = "$" + i;
+            if (a = Function("binder", "return function (" + or(u, ",") + "){ return binder.apply(this,arguments); }")(l), r.prototype) {
                 var s = function() {};
-                s.prototype = r.prototype, i.prototype = new s, s.prototype = null
+                s.prototype = r.prototype, a.prototype = new s, s.prototype = null
             }
-            return i
+            return a
         },
-        tr = er,
-        nr = Function.prototype.bind || tr,
-        yt = {}.hasOwnProperty,
-        Ce = Function.prototype.call,
-        rr = Ce.bind ? Ce.bind(yt) : function(e, t) {
-            return Ce.call(yt, e, t)
-        },
-        x, Q = SyntaxError,
-        dt = Function,
-        I = TypeError,
-        _e = function(e) {
+        ir = ar,
+        pt = Function.prototype.bind || ir,
+        sr = Function.prototype.call,
+        ur = Object.prototype.hasOwnProperty,
+        cr = pt,
+        fr = cr.call(sr, ur),
+        x, lr = Kn,
+        hr = qn,
+        pr = Pn,
+        vr = Xn,
+        Q = ct,
+        I = ft,
+        yr = Hn,
+        vt = Function,
+        Le = function(e) {
             try {
-                return dt('"use strict"; return (' + e + ").constructor;")()
+                return vt('"use strict"; return (' + e + ").constructor;")()
             } catch {}
         },
         q = Object.getOwnPropertyDescriptor;
     if (q) try {
         q({}, "")
     } catch {
         q = null
     }
-    var Le = function() {
+    var Fe = function() {
             throw new I
         },
-        or = q ? function() {
+        gr = q ? function() {
             try {
-                return arguments.callee, Le
+                return arguments.callee, Fe
             } catch {
                 try {
                     return q(arguments, "callee").get
                 } catch {
-                    return Le
+                    return Fe
                 }
             }
-        }() : Le,
-        ee = Pn(),
-        ar = Hn(),
-        j = Object.getPrototypeOf || (ar ? function(e) {
+        }() : Fe,
+        ee = Jn(),
+        dr = Qn(),
+        j = Object.getPrototypeOf || (dr ? function(e) {
             return e.__proto__
         } : null),
         te = {},
-        ir = typeof Uint8Array > "u" || !j ? x : j(Uint8Array),
+        mr = typeof Uint8Array > "u" || !j ? x : j(Uint8Array),
         P = {
+            __proto__: null,
             "%AggregateError%": typeof AggregateError > "u" ? x : AggregateError,
             "%Array%": Array,
             "%ArrayBuffer%": typeof ArrayBuffer > "u" ? x : ArrayBuffer,
             "%ArrayIteratorPrototype%": ee && j ? j([][Symbol.iterator]()) : x,
             "%AsyncFromSyncIteratorPrototype%": x,
             "%AsyncFunction%": te,
             "%AsyncGenerator%": te,
@@ -967,21 +978,21 @@
             "%Boolean%": Boolean,
             "%DataView%": typeof DataView > "u" ? x : DataView,
             "%Date%": Date,
             "%decodeURI%": decodeURI,
             "%decodeURIComponent%": decodeURIComponent,
             "%encodeURI%": encodeURI,
             "%encodeURIComponent%": encodeURIComponent,
-            "%Error%": Error,
+            "%Error%": lr,
             "%eval%": eval,
-            "%EvalError%": EvalError,
+            "%EvalError%": hr,
             "%Float32Array%": typeof Float32Array > "u" ? x : Float32Array,
             "%Float64Array%": typeof Float64Array > "u" ? x : Float64Array,
             "%FinalizationRegistry%": typeof FinalizationRegistry > "u" ? x : FinalizationRegistry,
-            "%Function%": dt,
+            "%Function%": vt,
             "%GeneratorFunction%": te,
             "%Int8Array%": typeof Int8Array > "u" ? x : Int8Array,
             "%Int16Array%": typeof Int16Array > "u" ? x : Int16Array,
             "%Int32Array%": typeof Int32Array > "u" ? x : Int32Array,
             "%isFinite%": isFinite,
             "%isNaN%": isNaN,
             "%IteratorPrototype%": ee && j ? j(j([][Symbol.iterator]())) : x,
@@ -991,58 +1002,59 @@
             "%Math%": Math,
             "%Number%": Number,
             "%Object%": Object,
             "%parseFloat%": parseFloat,
             "%parseInt%": parseInt,
             "%Promise%": typeof Promise > "u" ? x : Promise,
             "%Proxy%": typeof Proxy > "u" ? x : Proxy,
-            "%RangeError%": RangeError,
-            "%ReferenceError%": ReferenceError,
+            "%RangeError%": pr,
+            "%ReferenceError%": vr,
             "%Reflect%": typeof Reflect > "u" ? x : Reflect,
             "%RegExp%": RegExp,
             "%Set%": typeof Set > "u" ? x : Set,
             "%SetIteratorPrototype%": typeof Set > "u" || !ee || !j ? x : j(new Set()[Symbol.iterator]()),
             "%SharedArrayBuffer%": typeof SharedArrayBuffer > "u" ? x : SharedArrayBuffer,
             "%String%": String,
             "%StringIteratorPrototype%": ee && j ? j("" [Symbol.iterator]()) : x,
             "%Symbol%": ee ? Symbol : x,
             "%SyntaxError%": Q,
-            "%ThrowTypeError%": or,
-            "%TypedArray%": ir,
+            "%ThrowTypeError%": gr,
+            "%TypedArray%": mr,
             "%TypeError%": I,
             "%Uint8Array%": typeof Uint8Array > "u" ? x : Uint8Array,
             "%Uint8ClampedArray%": typeof Uint8ClampedArray > "u" ? x : Uint8ClampedArray,
             "%Uint16Array%": typeof Uint16Array > "u" ? x : Uint16Array,
             "%Uint32Array%": typeof Uint32Array > "u" ? x : Uint32Array,
-            "%URIError%": URIError,
+            "%URIError%": yr,
             "%WeakMap%": typeof WeakMap > "u" ? x : WeakMap,
             "%WeakRef%": typeof WeakRef > "u" ? x : WeakRef,
             "%WeakSet%": typeof WeakSet > "u" ? x : WeakSet
         };
     if (j) try {
         null.error
     } catch (e) {
-        var sr = j(j(e));
-        P["%Error.prototype%"] = sr
+        var wr = j(j(e));
+        P["%Error.prototype%"] = wr
     }
-    var ur = function e(t) {
+    var Sr = function e(t) {
             var r;
-            if (t === "%AsyncFunction%") r = _e("async function () {}");
-            else if (t === "%GeneratorFunction%") r = _e("function* () {}");
-            else if (t === "%AsyncGeneratorFunction%") r = _e("async function* () {}");
+            if (t === "%AsyncFunction%") r = Le("async function () {}");
+            else if (t === "%GeneratorFunction%") r = Le("function* () {}");
+            else if (t === "%AsyncGeneratorFunction%") r = Le("async function* () {}");
             else if (t === "%AsyncGenerator%") {
                 var n = e("%AsyncGeneratorFunction%");
                 n && (r = n.prototype)
             } else if (t === "%AsyncIteratorPrototype%") {
-                var i = e("%AsyncGenerator%");
-                i && j && (r = j(i.prototype))
+                var a = e("%AsyncGenerator%");
+                a && j && (r = j(a.prototype))
             }
             return P[t] = r, r
         },
-        gt = {
+        yt = {
+            __proto__: null,
             "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
             "%ArrayPrototype%": ["Array", "prototype"],
             "%ArrayProto_entries%": ["Array", "prototype", "entries"],
             "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
             "%ArrayProto_keys%": ["Array", "prototype", "keys"],
             "%ArrayProto_values%": ["Array", "prototype", "values"],
             "%AsyncFunctionPrototype%": ["AsyncFunction", "prototype"],
@@ -1087,898 +1099,885 @@
             "%Uint8ClampedArrayPrototype%": ["Uint8ClampedArray", "prototype"],
             "%Uint16ArrayPrototype%": ["Uint16Array", "prototype"],
             "%Uint32ArrayPrototype%": ["Uint32Array", "prototype"],
             "%URIErrorPrototype%": ["URIError", "prototype"],
             "%WeakMapPrototype%": ["WeakMap", "prototype"],
             "%WeakSetPrototype%": ["WeakSet", "prototype"]
         },
-        fe = nr,
-        ge = rr,
-        cr = fe.call(Function.call, Array.prototype.concat),
-        fr = fe.call(Function.apply, Array.prototype.splice),
-        mt = fe.call(Function.call, String.prototype.replace),
-        me = fe.call(Function.call, String.prototype.slice),
-        lr = fe.call(Function.call, RegExp.prototype.exec),
-        hr = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
-        pr = /\\(\\)?/g,
-        vr = function(t) {
-            var r = me(t, 0, 1),
-                n = me(t, -1);
+        fe = pt,
+        ge = fr,
+        Er = fe.call(Function.call, Array.prototype.concat),
+        Or = fe.call(Function.apply, Array.prototype.splice),
+        gt = fe.call(Function.call, String.prototype.replace),
+        de = fe.call(Function.call, String.prototype.slice),
+        br = fe.call(Function.call, RegExp.prototype.exec),
+        xr = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
+        kr = /\\(\\)?/g,
+        Tr = function(t) {
+            var r = de(t, 0, 1),
+                n = de(t, -1);
             if (r === "%" && n !== "%") throw new Q("invalid intrinsic syntax, expected closing `%`");
             if (n === "%" && r !== "%") throw new Q("invalid intrinsic syntax, expected opening `%`");
-            var i = [];
-            return mt(t, hr, function(h, v, u, a) {
-                i[i.length] = u ? mt(a, pr, "$1") : v || h
-            }), i
+            var a = [];
+            return gt(t, xr, function(l, v, u, i) {
+                a[a.length] = u ? gt(i, kr, "$1") : v || l
+            }), a
         },
-        yr = function(t, r) {
+        Rr = function(t, r) {
             var n = t,
-                i;
-            if (ge(gt, n) && (i = gt[n], n = "%" + i[0] + "%"), ge(P, n)) {
-                var h = P[n];
-                if (h === te && (h = ur(n)), typeof h > "u" && !r) throw new I("intrinsic " + t + " exists, but is not available. Please file an issue!");
+                a;
+            if (ge(yt, n) && (a = yt[n], n = "%" + a[0] + "%"), ge(P, n)) {
+                var l = P[n];
+                if (l === te && (l = Sr(n)), typeof l > "u" && !r) throw new I("intrinsic " + t + " exists, but is not available. Please file an issue!");
                 return {
-                    alias: i,
+                    alias: a,
                     name: n,
-                    value: h
+                    value: l
                 }
             }
             throw new Q("intrinsic " + t + " does not exist!")
         },
-        Fe = function(t, r) {
+        dt = function(t, r) {
             if (typeof t != "string" || t.length === 0) throw new I("intrinsic name must be a non-empty string");
             if (arguments.length > 1 && typeof r != "boolean") throw new I('"allowMissing" argument must be a boolean');
-            if (lr(/^%?[^%]*%?$/, t) === null) throw new Q("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
-            var n = vr(t),
-                i = n.length > 0 ? n[0] : "",
-                h = yr("%" + i + "%", r),
-                v = h.name,
-                u = h.value,
-                a = !1,
-                s = h.alias;
-            s && (i = s[0], fr(n, cr([0, 1], s)));
-            for (var c = 1, l = !0; c < n.length; c += 1) {
+            if (br(/^%?[^%]*%?$/, t) === null) throw new Q("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
+            var n = Tr(t),
+                a = n.length > 0 ? n[0] : "",
+                l = Rr("%" + a + "%", r),
+                v = l.name,
+                u = l.value,
+                i = !1,
+                s = l.alias;
+            s && (a = s[0], Or(n, Er([0, 1], s)));
+            for (var c = 1, h = !0; c < n.length; c += 1) {
                 var p = n[c],
-                    o = me(p, 0, 1),
-                    f = me(p, -1);
+                    o = de(p, 0, 1),
+                    f = de(p, -1);
                 if ((o === '"' || o === "'" || o === "`" || f === '"' || f === "'" || f === "`") && o !== f) throw new Q("property names with quotes must have matching quotes");
-                if ((p === "constructor" || !l) && (a = !0), i += "." + p, v = "%" + i + "%", ge(P, v)) u = P[v];
+                if ((p === "constructor" || !h) && (i = !0), a += "." + p, v = "%" + a + "%", ge(P, v)) u = P[v];
                 else if (u != null) {
                     if (!(p in u)) {
                         if (!r) throw new I("base intrinsic for " + t + " exists, but the property is not available.");
                         return
                     }
                     if (q && c + 1 >= n.length) {
                         var y = q(u, p);
-                        l = !!y, l && "get" in y && !("originalValue" in y.get) ? u = y.get : u = u[p]
-                    } else l = ge(u, p), u = u[p];
-                    l && !a && (P[v] = u)
+                        h = !!y, h && "get" in y && !("originalValue" in y.get) ? u = y.get : u = u[p]
+                    } else h = ge(u, p), u = u[p];
+                    h && !i && (P[v] = u)
                 }
             }
             return u
         },
-        dr = Fe,
-        Ue = dr("%Object.defineProperty%", !0),
-        Be = function() {
-            if (Ue) try {
-                return Ue({}, "a", {
-                    value: 1
-                }), !0
-            } catch {
-                return !1
-            }
-            return !1
-        };
-    Be.hasArrayLengthDefineBug = function() {
-        if (!Be()) return null;
-        try {
-            return Ue([], "length", {
-                value: 1
-            }).length !== 1
-        } catch {
-            return !0
-        }
-    };
-    var wt = Be,
-        We, St;
-
-    function gr() {
-        if (St) return We;
-        St = 1;
-        var e = Fe,
-            t = e("%Object.getOwnPropertyDescriptor%", !0);
-        if (t) try {
-            t([], "length")
-        } catch {
-            t = null
-        }
-        return We = t, We
-    }
-    var mr = wt(),
-        ze = Fe,
-        le = mr && ze("%Object.defineProperty%", !0);
-    if (le) try {
-        le({}, "a", {
+        Mr = dt,
+        me = Mr("%Object.defineProperty%", !0) || !1;
+    if (me) try {
+        me({}, "a", {
             value: 1
         })
     } catch {
-        le = !1
+        me = !1
+    }
+    var mt = me,
+        Dr = dt,
+        we = Dr("%Object.getOwnPropertyDescriptor%", !0);
+    if (we) try {
+        we([], "length")
+    } catch {
+        we = null
     }
-    var wr = ze("%SyntaxError%"),
-        ne = ze("%TypeError%"),
-        Et = gr(),
-        Sr = function(t, r, n) {
+    var jr = we,
+        wt = mt,
+        Cr = ct,
+        ne = ft,
+        St = jr,
+        _r = function(t, r, n) {
             if (!t || typeof t != "object" && typeof t != "function") throw new ne("`obj` must be an object or a function`");
             if (typeof r != "string" && typeof r != "symbol") throw new ne("`property` must be a string or a symbol`");
             if (arguments.length > 3 && typeof arguments[3] != "boolean" && arguments[3] !== null) throw new ne("`nonEnumerable`, if provided, must be a boolean or null");
             if (arguments.length > 4 && typeof arguments[4] != "boolean" && arguments[4] !== null) throw new ne("`nonWritable`, if provided, must be a boolean or null");
             if (arguments.length > 5 && typeof arguments[5] != "boolean" && arguments[5] !== null) throw new ne("`nonConfigurable`, if provided, must be a boolean or null");
             if (arguments.length > 6 && typeof arguments[6] != "boolean") throw new ne("`loose`, if provided, must be a boolean");
-            var i = arguments.length > 3 ? arguments[3] : null,
-                h = arguments.length > 4 ? arguments[4] : null,
+            var a = arguments.length > 3 ? arguments[3] : null,
+                l = arguments.length > 4 ? arguments[4] : null,
                 v = arguments.length > 5 ? arguments[5] : null,
                 u = arguments.length > 6 ? arguments[6] : !1,
-                a = !!Et && Et(t, r);
-            if (le) le(t, r, {
-                configurable: v === null && a ? a.configurable : !v,
-                enumerable: i === null && a ? a.enumerable : !i,
+                i = !!St && St(t, r);
+            if (wt) wt(t, r, {
+                configurable: v === null && i ? i.configurable : !v,
+                enumerable: a === null && i ? i.enumerable : !a,
                 value: n,
-                writable: h === null && a ? a.writable : !h
+                writable: l === null && i ? i.writable : !l
             });
-            else if (u || !i && !h && !v) t[r] = n;
-            else throw new wr("This environment does not support defining a property as non-configurable, non-writable, or non-enumerable.")
+            else if (u || !a && !l && !v) t[r] = n;
+            else throw new Cr("This environment does not support defining a property as non-configurable, non-writable, or non-enumerable.")
         },
-        Er = Vn,
-        Or = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
-        br = Object.prototype.toString,
-        xr = Array.prototype.concat,
-        Ot = Sr,
-        Tr = function(e) {
-            return typeof e == "function" && br.call(e) === "[object Function]"
+        Ue = mt,
+        Et = function() {
+            return !!Ue
+        };
+    Et.hasArrayLengthDefineBug = function() {
+        if (!Ue) return null;
+        try {
+            return Ue([], "length", {
+                value: 1
+            }).length !== 1
+        } catch {
+            return !0
+        }
+    };
+    var Lr = Et,
+        Fr = Vn,
+        Ur = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
+        Br = Object.prototype.toString,
+        $r = Array.prototype.concat,
+        Ot = _r,
+        Wr = function(e) {
+            return typeof e == "function" && Br.call(e) === "[object Function]"
         },
-        bt = wt(),
-        kr = function(e, t, r, n) {
+        bt = Lr(),
+        zr = function(e, t, r, n) {
             if (t in e) {
                 if (n === !0) {
                     if (e[t] === r) return
-                } else if (!Tr(n) || !n()) return
+                } else if (!Wr(n) || !n()) return
             }
             bt ? Ot(e, t, r, !0) : Ot(e, t, r)
         },
         xt = function(e, t) {
             var r = arguments.length > 2 ? arguments[2] : {},
-                n = Er(t);
-            Or && (n = xr.call(n, Object.getOwnPropertySymbols(t)));
-            for (var i = 0; i < n.length; i += 1) kr(e, n[i], t[n[i]], r[n[i]])
+                n = Fr(t);
+            Ur && (n = $r.call(n, Object.getOwnPropertySymbols(t)));
+            for (var a = 0; a < n.length; a += 1) zr(e, n[a], t[n[a]], r[n[a]])
         };
     xt.supportsDescriptors = !!bt;
-    var Tt = xt,
-        we = {
+    var kt = xt,
+        Se = {
             exports: {}
         };
-    typeof self < "u" ? we.exports = self : typeof window < "u" ? we.exports = window : we.exports = Function("return this")();
-    var kt = we.exports,
-        Rr = kt,
+    typeof self < "u" ? Se.exports = self : typeof window < "u" ? Se.exports = window : Se.exports = Function("return this")();
+    var Tt = Se.exports,
+        Gr = Tt,
         Rt = function() {
-            return typeof B != "object" || !B || B.Math !== Math || B.Array !== Array ? Rr : B
+            return typeof B != "object" || !B || B.Math !== Math || B.Array !== Array ? Gr : B
         },
-        Mr = Tt,
-        Dr = Rt,
-        jr = function() {
-            var t = Dr();
-            if (Mr.supportsDescriptors) {
+        Nr = kt,
+        Vr = Rt,
+        Kr = function() {
+            var t = Vr();
+            if (Nr.supportsDescriptors) {
                 var r = Object.getOwnPropertyDescriptor(t, "globalThis");
                 (!r || r.configurable && (r.enumerable || !r.writable || globalThis !== t)) && Object.defineProperty(t, "globalThis", {
                     configurable: !0,
                     enumerable: !1,
                     value: t,
                     writable: !0
                 })
             } else(typeof globalThis != "object" || globalThis !== t) && (t.globalThis = t);
             return t
         },
-        Cr = Tt,
-        _r = kt,
+        qr = kt,
+        Pr = Tt,
         Mt = Rt,
-        Lr = jr,
-        Fr = Mt(),
+        Xr = Kr,
+        Hr = Mt(),
         Dt = function() {
-            return Fr
+            return Hr
         };
-    Cr(Dt, {
+    qr(Dt, {
         getPolyfill: Mt,
-        implementation: _r,
-        shim: Lr
+        implementation: Pr,
+        shim: Xr
     });
-    var Ur = Dt;
-    const Br = it(Ur);
+    var Yr = Dt;
+    const Ar = rt(Yr);
 
     function jt(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
-            t && (n = n.filter(function(i) {
-                return Object.getOwnPropertyDescriptor(e, i).enumerable
+            t && (n = n.filter(function(a) {
+                return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function Wr(e) {
+    function Jr(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? jt(Object(r), !0).forEach(function(n) {
                 V(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : jt(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var z = Br(),
+    var W = Ar(),
         Ct = {
             vtkObject: function() {
                 return null
             }
         };
 
     function X(e) {
         if (e == null || e.isA) return e;
-        if (!e.vtkClass) return z.console && z.console.error && z.console.error("Invalid VTK object"), null;
+        if (!e.vtkClass) return W.console && W.console.error && W.console.error("Invalid VTK object"), null;
         var t = Ct[e.vtkClass];
-        if (!t) return z.console && z.console.error && z.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
-        var r = Wr({}, e);
-        Object.keys(r).forEach(function(i) {
-            r[i] && K(r[i]) === "object" && r[i].vtkClass && (r[i] = X(r[i]))
+        if (!t) return W.console && W.console.error && W.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
+        var r = Jr({}, e);
+        Object.keys(r).forEach(function(a) {
+            r[a] && K(r[a]) === "object" && r[a].vtkClass && (r[a] = X(r[a]))
         });
         var n = t(r);
         return n && n.modified && n.modified(), n
     }
 
-    function zr(e, t) {
+    function Zr(e, t) {
         Ct[e] = t
     }
-    X.register = zr;
+    X.register = Zr;
 
-    function $r(e, t) {
+    function Qr(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
 
     function _t(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
         }
     }
 
-    function Gr(e, t, r) {
+    function Ir(e, t, r) {
         return t && _t(e.prototype, t), r && _t(e, r), Object.defineProperty(e, "prototype", {
             writable: !1
         }), e
     }
 
     function H(e) {
         return H = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
             return r.__proto__ || Object.getPrototypeOf(r)
         }, H(e)
     }
 
-    function Nr(e, t) {
+    function eo(e, t) {
         for (; !Object.prototype.hasOwnProperty.call(e, t) && (e = H(e), e !== null););
         return e
     }
 
-    function Se() {
-        return typeof Reflect < "u" && Reflect.get ? Se = Reflect.get : Se = function(t, r, n) {
-            var i = Nr(t, r);
-            if (i) {
-                var h = Object.getOwnPropertyDescriptor(i, r);
-                return h.get ? h.get.call(arguments.length < 3 ? t : n) : h.value
+    function Ee() {
+        return typeof Reflect < "u" && Reflect.get ? Ee = Reflect.get : Ee = function(t, r, n) {
+            var a = eo(t, r);
+            if (a) {
+                var l = Object.getOwnPropertyDescriptor(a, r);
+                return l.get ? l.get.call(arguments.length < 3 ? t : n) : l.value
             }
-        }, Se.apply(this, arguments)
+        }, Ee.apply(this, arguments)
     }
 
-    function Vr(e, t) {
+    function to(e, t) {
         if (typeof t != "function" && t !== null) throw new TypeError("Super expression must either be null or a function");
         e.prototype = Object.create(t && t.prototype, {
             constructor: {
                 value: e,
                 writable: !0,
                 configurable: !0
             }
         }), Object.defineProperty(e, "prototype", {
             writable: !1
         }), t && ue(e, t)
     }
 
-    function Kr(e) {
+    function no(e) {
         if (e === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
-    function qr(e, t) {
+    function ro(e, t) {
         if (t && (K(t) === "object" || typeof t == "function")) return t;
         if (t !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
-        return Kr(e)
+        return no(e)
     }
 
-    function Pr(e) {
+    function oo(e) {
         return Function.toString.call(e).indexOf("[native code]") !== -1
     }
 
-    function $e(e) {
+    function Be(e) {
         var t = typeof Map == "function" ? new Map : void 0;
-        return $e = function(n) {
-            if (n === null || !Pr(n)) return n;
+        return Be = function(n) {
+            if (n === null || !oo(n)) return n;
             if (typeof n != "function") throw new TypeError("Super expression must either be null or a function");
             if (typeof t < "u") {
                 if (t.has(n)) return t.get(n);
-                t.set(n, i)
+                t.set(n, a)
             }
 
-            function i() {
+            function a() {
                 return ce(n, arguments, H(this).constructor)
             }
-            return i.prototype = Object.create(n.prototype, {
+            return a.prototype = Object.create(n.prototype, {
                 constructor: {
-                    value: i,
+                    value: a,
                     enumerable: !1,
                     writable: !0,
                     configurable: !0
                 }
-            }), ue(i, n)
-        }, $e(e)
+            }), ue(a, n)
+        }, Be(e)
     }
 
-    function Xr(e) {
-        var t = Hr();
+    function ao(e) {
+        var t = io();
         return function() {
             var n = H(e),
-                i;
+                a;
             if (t) {
-                var h = H(this).constructor;
-                i = Reflect.construct(n, arguments, h)
-            } else i = n.apply(this, arguments);
-            return qr(this, i)
+                var l = H(this).constructor;
+                a = Reflect.construct(n, arguments, l)
+            } else a = n.apply(this, arguments);
+            return ro(this, a)
         }
     }
 
-    function Hr() {
+    function io() {
         if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
         if (typeof Proxy == "function") return !0;
         try {
             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
         } catch {
             return !1
         }
     }
-    var Ge = function(e) {
-        Vr(r, e);
-        var t = Xr(r);
+    var $e = function(e) {
+        to(r, e);
+        var t = ao(r);
 
         function r() {
-            return $r(this, r), t.apply(this, arguments)
+            return Qr(this, r), t.apply(this, arguments)
         }
-        return Gr(r, [{
+        return Ir(r, [{
             key: "push",
             value: function() {
-                for (var i = 0; i < arguments.length; i++) this.includes(arguments[i]) || Se(H(r.prototype), "push", this).call(this, arguments[i]);
+                for (var a = 0; a < arguments.length; a++) this.includes(arguments[a]) || Ee(H(r.prototype), "push", this).call(this, arguments[a]);
                 return this.length
             }
         }]), r
-    }($e(Array));
+    }(Be(Array));
 
     function Lt(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
-            t && (n = n.filter(function(i) {
-                return Object.getOwnPropertyDescriptor(e, i).enumerable
+            t && (n = n.filter(function(a) {
+                return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function Ee(e) {
+    function Oe(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? Lt(Object(r), !0).forEach(function(n) {
                 V(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : Lt(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var Ne = 0,
-        Yr = Symbol("void");
+    var We = 0,
+        so = Symbol("void");
 
-    function Ar() {
-        return Ne
+    function uo() {
+        return We
     }
     var Ft = {};
 
     function Y() {}
-    var Jr = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
-    Jr.forEach(function(e) {
+    var co = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
+    co.forEach(function(e) {
         Ft[e] = Y
-    }), z.console = console.hasOwnProperty("log") ? console : Ft;
+    }), W.console = console.hasOwnProperty("log") ? console : Ft;
     var U = {
         debug: Y,
-        error: z.console.error || Y,
-        info: z.console.info || Y,
-        log: z.console.log || Y,
-        warn: z.console.warn || Y
+        error: W.console.error || Y,
+        info: W.console.info || Y,
+        log: W.console.log || Y,
+        warn: W.console.warn || Y
     };
 
-    function Zr(e, t) {
+    function fo(e, t) {
         U[e] && (U[e] = t || Y)
     }
 
-    function Qr() {
+    function lo() {
         U.log.apply(U, arguments)
     }
 
-    function Ir() {
+    function ho() {
         U.info.apply(U, arguments)
     }
 
-    function Ve() {
+    function ze() {
         U.debug.apply(U, arguments)
     }
 
     function C() {
         U.error.apply(U, arguments)
     }
 
     function Ut() {
         U.warn.apply(U, arguments)
     }
     var Bt = {};
 
-    function eo(e) {
+    function po(e) {
         Bt[e] || (U.error(e), Bt[e] = !0)
     }
     var F = Object.create(null);
     F.Float32Array = Float32Array, F.Float64Array = Float64Array, F.Uint8Array = Uint8Array, F.Int8Array = Int8Array, F.Uint16Array = Uint16Array, F.Int16Array = Int16Array, F.Uint32Array = Uint32Array, F.Int32Array = Int32Array, F.Uint8ClampedArray = Uint8ClampedArray;
     try {
         F.BigInt64Array = BigInt64Array, F.BigUint64Array = BigUint64Array
     } catch {}
 
-    function to(e) {
+    function vo(e) {
         for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
         return ce(F[e] || Float64Array, r)
     }
 
-    function no(e) {
-        for (var t, r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), i = 1; i < r; i++) n[i - 1] = arguments[i];
+    function yo(e) {
+        for (var t, r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) n[a - 1] = arguments[a];
         return (t = F[e] || Float64Array).from.apply(t, n)
     }
 
-    function Ke(e) {
+    function Ge(e) {
         return e.charAt(0).toUpperCase() + e.slice(1)
     }
 
     function D(e) {
-        return Ke(e[0] === "_" ? e.slice(1) : e)
+        return Ge(e[0] === "_" ? e.slice(1) : e)
     }
 
-    function ro(e) {
+    function go(e) {
         return e.charAt(0).toLowerCase() + e.slice(1)
     }
 
-    function oo(e) {
-        for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 2, r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1e3, n = ["TB", "GB", "MB", "KB"], i = Number(e), h = "B"; i > r;) i /= r, h = n.pop();
-        return "".concat(i.toFixed(t), " ").concat(h)
+    function mo(e) {
+        for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 2, r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1e3, n = ["TB", "GB", "MB", "KB"], a = Number(e), l = "B"; a > r;) a /= r, l = n.pop();
+        return "".concat(a.toFixed(t), " ").concat(l)
     }
 
-    function ao(e) {
+    function wo(e) {
         for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : " ", r = [], n = e; n > 1e3;) r.push("000".concat(n % 1e3).slice(-3)), n = Math.floor(n / 1e3);
         return n > 0 && r.push(n), r.reverse(), r.join(t)
     }
 
-    function Wt(e) {
+    function $t(e) {
         Object.keys(e).forEach(function(t) {
             Array.isArray(e[t]) && (e[t] = [].concat(e[t]))
         })
     }
 
-    function io(e, t) {
+    function So(e, t) {
         if (e === t) return !0;
         if (Array.isArray(e) && Array.isArray(t)) {
             if (e.length !== t.length) return !1;
             for (var r = 0; r < e.length; r++)
                 if (e[r] !== t[r]) return !1;
             return !0
         }
         return !1
     }
 
-    function so(e, t) {
+    function Eo(e, t) {
         return Object.keys(e).find(function(r) {
             return e[r] === t
         })
     }
 
-    function zt(e) {
+    function Wt(e) {
         return e && e.isA ? e.getState() : e
     }
 
-    function $t(e) {
+    function zt(e) {
         setTimeout(e, 0)
     }
 
-    function uo(e, t) {
+    function Oo(e, t) {
         var r = performance.now();
         e.finally(function() {
             var n = performance.now() - r;
             t(n)
         })
     }
 
-    function co() {
+    function bo() {
         var e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
             t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {};
-        Wt(t);
+        $t(t);
         var r = [];
-        if (Number.isInteger(t.mtime) || (t.mtime = ++Ne), !("classHierarchy" in t)) t.classHierarchy = new Ge("vtkObject");
-        else if (!(t.classHierarchy instanceof Ge)) {
-            for (var n = new Ge, i = 0; i < t.classHierarchy.length; i++) n.push(t.classHierarchy[i]);
+        if (Number.isInteger(t.mtime) || (t.mtime = ++We), !("classHierarchy" in t)) t.classHierarchy = new $e("vtkObject");
+        else if (!(t.classHierarchy instanceof $e)) {
+            for (var n = new $e, a = 0; a < t.classHierarchy.length; a++) n.push(t.classHierarchy[a]);
             t.classHierarchy = n
         }
 
-        function h(u) {
+        function l(u) {
             r[u] = null
         }
 
         function v(u) {
-            function a() {
-                h(u)
+            function i() {
+                l(u)
             }
             return Object.freeze({
-                unsubscribe: a
+                unsubscribe: i
             })
         }
         return e.isDeleted = function() {
             return !!t.deleted
         }, e.modified = function(u) {
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
-            u && u < e.getMTime() || (t.mtime = ++Ne, r.forEach(function(a) {
-                return a && a(e)
+            u && u < e.getMTime() || (t.mtime = ++We, r.forEach(function(i) {
+                return i && i(e)
             }))
         }, e.onModified = function(u) {
             if (t.deleted) return C("instance deleted - cannot call any method"), null;
-            var a = r.length;
-            return r.push(u), v(a)
+            var i = r.length;
+            return r.push(u), v(i)
         }, e.getMTime = function() {
             return t.mtime
         }, e.isA = function(u) {
-            for (var a = t.classHierarchy.length; a--;)
-                if (t.classHierarchy[a] === u) return !0;
+            for (var i = t.classHierarchy.length; i--;)
+                if (t.classHierarchy[i] === u) return !0;
             return !1
         }, e.getClassName = function() {
             var u = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.classHierarchy[t.classHierarchy.length - 1 - u]
         }, e.set = function() {
             var u = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-                a = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1,
+                i = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1,
                 s = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
                 c = !1;
-            return Object.keys(u).forEach(function(l) {
-                var p = s ? null : e["set".concat(Ke(l))];
-                p && Array.isArray(u[l]) && p.length > 1 ? c = p.apply(void 0, se(u[l])) || c : p ? c = p(u[l]) || c : (["mtime"].indexOf(l) === -1 && !a && Ut("Warning: Set value to model directly ".concat(l, ", ").concat(u[l])), c = t[l] !== u[l] || c, t[l] = u[l])
+            return Object.keys(u).forEach(function(h) {
+                var p = s ? null : e["set".concat(Ge(h))];
+                p && Array.isArray(u[h]) && p.length > 1 ? c = p.apply(void 0, se(u[h])) || c : p ? c = p(u[h]) || c : (["mtime"].indexOf(h) === -1 && !i && Ut("Warning: Set value to model directly ".concat(h, ", ").concat(u[h])), c = t[h] !== u[h] || c, t[h] = u[h])
             }), c
         }, e.get = function() {
-            for (var u = arguments.length, a = new Array(u), s = 0; s < u; s++) a[s] = arguments[s];
-            if (!a.length) return t;
+            for (var u = arguments.length, i = new Array(u), s = 0; s < u; s++) i[s] = arguments[s];
+            if (!i.length) return t;
             var c = {};
-            return a.forEach(function(l) {
-                c[l] = t[l]
+            return i.forEach(function(h) {
+                c[h] = t[h]
             }), c
         }, e.getReferenceByName = function(u) {
             return t[u]
         }, e.delete = function() {
             Object.keys(t).forEach(function(u) {
                 return delete t[u]
-            }), r.forEach(function(u, a) {
-                return h(a)
+            }), r.forEach(function(u, i) {
+                return l(i)
             }), t.deleted = !0
         }, e.getState = function() {
             if (t.deleted) return null;
-            var u = Ee(Ee({}, t), {}, {
+            var u = Oe(Oe({}, t), {}, {
                 vtkClass: e.getClassName()
             });
             Object.keys(u).forEach(function(s) {
-                u[s] === null || u[s] === void 0 || s[0] === "_" ? delete u[s] : u[s].isA ? u[s] = u[s].getState() : Array.isArray(u[s]) && (u[s] = u[s].map(zt))
+                u[s] === null || u[s] === void 0 || s[0] === "_" ? delete u[s] : u[s].isA ? u[s] = u[s].getState() : Array.isArray(u[s]) && (u[s] = u[s].map(Wt))
             });
-            var a = {};
+            var i = {};
             return Object.keys(u).sort().forEach(function(s) {
-                a[s] = u[s]
-            }), a.mtime && delete a.mtime, a
+                i[s] = u[s]
+            }), i.mtime && delete i.mtime, i
         }, e.shallowCopy = function(u) {
-            var a = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
+            var i = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
             if (u.getClassName() !== e.getClassName()) throw new Error("Cannot ShallowCopy ".concat(u.getClassName(), " into ").concat(e.getClassName()));
             var s = u.get(),
                 c = Object.keys(t).sort(),
-                l = Object.keys(s).sort();
-            l.forEach(function(p) {
+                h = Object.keys(s).sort();
+            h.forEach(function(p) {
                 var o = c.indexOf(p);
-                o === -1 ? a && Ve("add ".concat(p, " in shallowCopy")) : c.splice(o, 1), t[p] = s[p]
-            }), c.length && a && Ve("Untouched keys: ".concat(c.join(", "))), e.modified()
+                o === -1 ? i && ze("add ".concat(p, " in shallowCopy")) : c.splice(o, 1), t[p] = s[p]
+            }), c.length && i && ze("Untouched keys: ".concat(c.join(", "))), e.modified()
         }, e.toJSON = function() {
             return e.getState()
         }, e
     }
-    var fo = {
+    var xo = {
         object: function(t, r, n) {
             return function() {
-                return Ee({}, r[n.name])
+                return Oe({}, r[n.name])
             }
         }
     };
 
-    function Oe(e, t, r) {
+    function be(e, t, r) {
         r.forEach(function(n) {
             if (K(n) === "object") {
-                var i = fo[n.type];
-                i ? e["get".concat(D(n.name))] = i(e, t, n) : e["get".concat(D(n.name))] = function() {
+                var a = xo[n.type];
+                a ? e["get".concat(D(n.name))] = a(e, t, n) : e["get".concat(D(n.name))] = function() {
                     return t[n.name]
                 }
             } else e["get".concat(D(n))] = function() {
                 return t[n]
             }
         })
     }
-    var lo = {
+    var ko = {
         enum: function(t, r, n) {
-            var i = "_on".concat(D(n.name), "Changed");
-            return function(h) {
-                if (typeof h == "string") {
-                    if (n.enum[h] !== void 0) return r[n.name] !== n.enum[h] ? (r[n.name] = n.enum[h], t.modified(), !0) : !1;
-                    throw C("Set Enum with invalid argument ".concat(n, ", ").concat(h)), new RangeError("Set Enum with invalid string argument")
-                }
-                if (typeof h == "number") {
-                    if (r[n.name] !== h) {
-                        if (Object.keys(n.enum).map(function(a) {
-                                return n.enum[a]
-                            }).indexOf(h) !== -1) {
+            var a = "_on".concat(D(n.name), "Changed");
+            return function(l) {
+                if (typeof l == "string") {
+                    if (n.enum[l] !== void 0) return r[n.name] !== n.enum[l] ? (r[n.name] = n.enum[l], t.modified(), !0) : !1;
+                    throw C("Set Enum with invalid argument ".concat(n, ", ").concat(l)), new RangeError("Set Enum with invalid string argument")
+                }
+                if (typeof l == "number") {
+                    if (r[n.name] !== l) {
+                        if (Object.keys(n.enum).map(function(i) {
+                                return n.enum[i]
+                            }).indexOf(l) !== -1) {
                             var v, u = r[n.name];
-                            return r[n.name] = h, (v = r[i]) === null || v === void 0 || v.call(r, t, r, h, u), t.modified(), !0
+                            return r[n.name] = l, (v = r[a]) === null || v === void 0 || v.call(r, t, r, l, u), t.modified(), !0
                         }
-                        throw C("Set Enum outside numeric range ".concat(n, ", ").concat(h)), new RangeError("Set Enum outside numeric range")
+                        throw C("Set Enum outside numeric range ".concat(n, ", ").concat(l)), new RangeError("Set Enum outside numeric range")
                     }
                     return !1
                 }
-                throw C("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(h)), new TypeError("Set Enum with invalid argument (String/Number)")
+                throw C("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(l)), new TypeError("Set Enum with invalid argument (String/Number)")
             }
         },
         object: function(t, r, n) {
-            var i = "_on".concat(D(n.name), "Changed");
-            return function(h) {
-                if (!zn(r[n.name], h)) {
+            var a = "_on".concat(D(n.name), "Changed");
+            return function(l) {
+                if (!Wn(r[n.name], l)) {
                     var v, u = r[n.name];
-                    return r[n.name] = h, (v = r[i]) === null || v === void 0 || v.call(r, t, r, h, u), t.modified(), !0
+                    return r[n.name] = l, (v = r[a]) === null || v === void 0 || v.call(r, t, r, l, u), t.modified(), !0
                 }
                 return !1
             }
         }
     };
 
     function Gt(e) {
         if (K(e) === "object") {
-            var t = lo[e.type];
+            var t = ko[e.type];
             if (t) return function(r, n) {
                 return t(r, n, e)
             };
             throw C("No setter for field ".concat(e)), new TypeError("No setter for field")
         }
-        return function(n, i) {
-            var h = "_on".concat(D(e), "Changed");
+        return function(n, a) {
+            var l = "_on".concat(D(e), "Changed");
             return function(u) {
-                if (i.deleted) return C("instance deleted - cannot call any method"), !1;
-                if (i[e] !== u) {
-                    var a, s = i[e.name];
-                    return i[e] = u, (a = i[h]) === null || a === void 0 || a.call(i, n, i, u, s), n.modified(), !0
+                if (a.deleted) return C("instance deleted - cannot call any method"), !1;
+                if (a[e] !== u) {
+                    var i, s = a[e.name];
+                    return a[e] = u, (i = a[l]) === null || i === void 0 || i.call(a, n, a, u, s), n.modified(), !0
                 }
                 return !1
             }
         }
     }
 
     function Nt(e, t, r) {
         r.forEach(function(n) {
             K(n) === "object" ? e["set".concat(D(n.name))] = Gt(n)(e, t) : e["set".concat(D(n))] = Gt(n)(e, t)
         })
     }
 
     function Vt(e, t, r) {
-        Oe(e, t, r), Nt(e, t, r)
+        be(e, t, r), Nt(e, t, r)
     }
 
     function Kt(e, t, r) {
         r.forEach(function(n) {
             e["get".concat(D(n))] = function() {
                 return t[n] ? Array.from(t[n]) : t[n]
             }, e["get".concat(D(n), "ByReference")] = function() {
                 return t[n]
             }
         })
     }
 
     function qt(e, t, r, n) {
-        var i = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
-        r.forEach(function(h) {
-            if (t[h] && n && t[h].length !== n) throw new RangeError("Invalid initial number of values for array (".concat(h, ")"));
-            var v = "_on".concat(D(h), "Changed");
-            e["set".concat(D(h))] = function() {
+        var a = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
+        r.forEach(function(l) {
+            if (t[l] && n && t[l].length !== n) throw new RangeError("Invalid initial number of values for array (".concat(l, ")"));
+            var v = "_on".concat(D(l), "Changed");
+            e["set".concat(D(l))] = function() {
                 if (t.deleted) return C("instance deleted - cannot call any method"), !1;
-                for (var u = arguments.length, a = new Array(u), s = 0; s < u; s++) a[s] = arguments[s];
-                var c = a,
-                    l, p = !1;
-                if (c.length === 1 && (c[0] == null || c[0].length >= 0) && (c = c[0], p = !0), c == null) l = t[h] !== c;
+                for (var u = arguments.length, i = new Array(u), s = 0; s < u; s++) i[s] = arguments[s];
+                var c = i,
+                    h, p = !1;
+                if (c.length === 1 && (c[0] == null || c[0].length >= 0) && (c = c[0], p = !0), c == null) h = t[l] !== c;
                 else {
                     if (n && c.length !== n)
-                        if (c.length < n && i !== void 0)
-                            for (c = Array.from(c), p = !1; c.length < n;) c.push(i);
-                        else throw new RangeError("Invalid number of values for array setter (".concat(h, ")"));
-                    l = t[h] == null || t[h].length !== c.length;
-                    for (var o = 0; !l && o < c.length; ++o) l = t[h][o] !== c[o];
-                    l && p && (c = Array.from(c))
-                }
-                if (l) {
-                    var f, y = t[h.name];
-                    t[h] = c, (f = t[v]) === null || f === void 0 || f.call(t, e, t, c, y), e.modified()
-                }
-                return l
-            }, e["set".concat(D(h), "From")] = function(u) {
-                var a = t[h];
+                        if (c.length < n && a !== void 0)
+                            for (c = Array.from(c), p = !1; c.length < n;) c.push(a);
+                        else throw new RangeError("Invalid number of values for array setter (".concat(l, ")"));
+                    h = t[l] == null || t[l].length !== c.length;
+                    for (var o = 0; !h && o < c.length; ++o) h = t[l][o] !== c[o];
+                    h && p && (c = Array.from(c))
+                }
+                if (h) {
+                    var f, y = t[l.name];
+                    t[l] = c, (f = t[v]) === null || f === void 0 || f.call(t, e, t, c, y), e.modified()
+                }
+                return h
+            }, e["set".concat(D(l), "From")] = function(u) {
+                var i = t[l];
                 u.forEach(function(s, c) {
-                    a[c] = s
+                    i[c] = s
                 })
             }
         })
     }
 
-    function ho(e, t, r, n) {
-        var i = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
-        Kt(e, t, r), qt(e, t, r, n, i)
+    function To(e, t, r, n) {
+        var a = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
+        Kt(e, t, r), qt(e, t, r, n, a)
     }
 
-    function po(e, t, r) {
+    function Ro(e, t, r) {
         for (var n = 0; n < r.length; n++) {
-            var i = r[n];
-            t[i] !== void 0 && (t["_".concat(i)] = t[i], delete t[i])
+            var a = r[n];
+            t[a] !== void 0 && (t["_".concat(a)] = t[a], delete t[a])
         }
     }
 
-    function vo(e, t, r, n) {
+    function Mo(e, t, r, n) {
         t.inputData ? t.inputData = t.inputData.map(X) : t.inputData = [], t.inputConnection ? t.inputConnection = t.inputConnection.map(X) : t.inputConnection = [], t.output ? t.output = t.output.map(X) : t.output = [], t.inputArrayToProcess ? t.inputArrayToProcess = t.inputArrayToProcess.map(X) : t.inputArrayToProcess = [], t.numberOfInputs = r;
 
-        function i(f) {
+        function a(f) {
             var y = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
             if (y >= t.numberOfInputs) {
                 C("algorithm ".concat(e.getClassName(), " only has ").concat(t.numberOfInputs, " input ports. To add more input ports, use addInputData()"));
                 return
             }(t.inputData[y] !== f || t.inputConnection[y]) && (t.inputData[y] = f, t.inputConnection[y] = null, e.modified && e.modified())
         }
 
-        function h() {
+        function l() {
             var f = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.inputConnection[f] && (t.inputData[f] = t.inputConnection[f]()), t.inputData[f]
         }
 
         function v(f) {
             var y = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
             if (y >= t.numberOfInputs) {
-                var g = "algorithm ".concat(e.getClassName(), " only has ");
-                g += "".concat(t.numberOfInputs), g += " input ports. To add more input ports, use addInputConnection()", C(g);
+                var d = "algorithm ".concat(e.getClassName(), " only has ");
+                d += "".concat(t.numberOfInputs), d += " input ports. To add more input ports, use addInputConnection()", C(d);
                 return
             }
             t.inputData[y] = null, t.inputConnection[y] = f
         }
 
         function u() {
             var f = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.inputConnection[f]
         }
 
-        function a() {
+        function i() {
             for (var f = t.numberOfInputs; f && !t.inputData[f - 1] && !t.inputConnection[f - 1];) f--;
             return f === t.numberOfInputs && t.numberOfInputs++, f
         }
 
         function s(f) {
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
-            v(f, a())
+            v(f, i())
         }
 
         function c(f) {
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
-            i(f, a())
+            a(f, i())
         }
 
-        function l() {
+        function h() {
             var f = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.deleted ? (C("instance deleted - cannot call any method"), null) : (e.shouldUpdate() && e.update(), t.output[f])
         }
         e.shouldUpdate = function() {
-            for (var f = e.getMTime(), y = 1 / 0, g = n; g--;) {
-                if (!t.output[g] || t.output[g].isDeleted()) return !0;
-                var m = t.output[g].getMTime();
+            for (var f = e.getMTime(), y = 1 / 0, d = n; d--;) {
+                if (!t.output[d] || t.output[d].isDeleted()) return !0;
+                var m = t.output[d].getMTime();
                 if (m < f) return !0;
                 m < y && (y = m)
             }
-            for (g = t.numberOfInputs; g--;) {
-                var w, T;
-                if ((w = t.inputConnection[g]) !== null && w !== void 0 && w.filter.shouldUpdate() || ((T = e.getInputData(g)) === null || T === void 0 ? void 0 : T.getMTime()) > y) return !0
+            for (d = t.numberOfInputs; d--;) {
+                var w, k;
+                if ((w = t.inputConnection[d]) !== null && w !== void 0 && w.filter.shouldUpdate() || ((k = e.getInputData(d)) === null || k === void 0 ? void 0 : k.getMTime()) > y) return !0
             }
             return !1
         };
 
         function p() {
             var f = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
                 y = function() {
-                    return l(f)
+                    return h(f)
                 };
             return y.filter = e, y
         }
         if (t.numberOfInputs) {
             for (var o = t.numberOfInputs; o--;) t.inputData.push(null), t.inputConnection.push(null);
-            e.setInputData = i, e.setInputConnection = v, e.addInputData = c, e.addInputConnection = s, e.getInputData = h, e.getInputConnection = u
+            e.setInputData = a, e.setInputConnection = v, e.addInputData = c, e.addInputConnection = s, e.getInputData = l, e.getInputConnection = u
         }
-        n && (e.getOutputData = l, e.getOutputPort = p), e.update = function() {
+        n && (e.getOutputData = h, e.getOutputPort = p), e.update = function() {
             var f = [];
             if (t.numberOfInputs)
                 for (var y = 0; y < t.numberOfInputs;) f[y] = e.getInputData(y), y++;
             e.shouldUpdate() && e.requestData && e.requestData(f, t.output)
         }, e.getNumberOfInputPorts = function() {
             return t.numberOfInputs
         }, e.getNumberOfOutputPorts = function() {
             return n || t.output.length
         }, e.getInputArrayToProcess = function(f) {
             var y = t.inputArrayToProcess[f],
-                g = t.inputData[f];
-            return y && g ? g["get".concat(y.fieldAssociation)]().getArray(y.arrayName) : null
-        }, e.setInputArrayToProcess = function(f, y, g) {
+                d = t.inputData[f];
+            return y && d ? d["get".concat(y.fieldAssociation)]().getArray(y.arrayName) : null
+        }, e.setInputArrayToProcess = function(f, y, d) {
             for (var m = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : "Scalars"; t.inputArrayToProcess.length < f;) t.inputArrayToProcess.push(null);
             t.inputArrayToProcess[f] = {
                 arrayName: y,
-                fieldAssociation: g,
+                fieldAssociation: d,
                 attributeType: m
             }
         }
     }
     var Pt = Symbol("Event abort");
 
-    function yo(e, t, r) {
+    function Do(e, t, r) {
         var n = [],
-            i = e.delete,
-            h = 1;
+            a = e.delete,
+            l = 1;
 
         function v(s) {
             for (var c = 0; c < n.length; ++c) {
-                var l = De(n[c], 1),
-                    p = l[0];
+                var h = je(n[c], 1),
+                    p = h[0];
                 if (p === s) {
                     n.splice(c, 1);
                     return
                 }
             }
         }
 
@@ -1987,262 +1986,262 @@
                 v(s)
             }
             return Object.freeze({
                 unsubscribe: c
             })
         }
 
-        function a() {
+        function i() {
             var s = arguments;
             if (t.deleted) {
                 C("instance deleted - cannot call any method");
                 return
             }
-            for (var c = n.slice(), l = function(y) {
-                    var g = De(c[y], 3),
-                        m = g[1],
-                        w = g[2];
+            for (var c = n.slice(), h = function(y) {
+                    var d = je(c[y], 3),
+                        m = d[1],
+                        w = d[2];
                     if (!m) return "continue";
                     if (w < 0) setTimeout(function() {
                         return m.apply(e, s)
                     }, 1 - w);
                     else {
-                        var T = m.apply(e, s);
-                        if (T === Pt) return "break"
+                        var k = m.apply(e, s);
+                        if (k === Pt) return "break"
                     }
                 }, p = 0; p < c.length; ++p) {
-                var o = l(p);
+                var o = h(p);
                 if (o !== "continue" && o === "break") break
             }
         }
-        e["invoke".concat(D(r))] = a, e["on".concat(D(r))] = function(s) {
+        e["invoke".concat(D(r))] = i, e["on".concat(D(r))] = function(s) {
             var c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (!s.apply) return console.error("Invalid callback for event ".concat(r)), null;
             if (t.deleted) return C("instance deleted - cannot call any method"), null;
-            var l = h++;
-            return n.push([l, s, c]), n.sort(function(p, o) {
+            var h = l++;
+            return n.push([h, s, c]), n.sort(function(p, o) {
                 return o[2] - p[2]
-            }), u(l)
+            }), u(h)
         }, e.delete = function() {
-            i(), n.forEach(function(s) {
-                var c = De(s, 1),
-                    l = c[0];
-                return v(l)
+            a(), n.forEach(function(s) {
+                var c = je(s, 1),
+                    h = c[0];
+                return v(h)
             })
         }
     }
 
-    function go(e, t) {
+    function jo(e, t) {
         var r = function() {
-            var i = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-                h = {},
+            var a = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
+                l = {},
                 v = {};
-            return e(v, h, i), Object.freeze(v)
+            return e(v, l, a), Object.freeze(v)
         };
         return t && X.register(t, r), r
     }
 
-    function mo() {
+    function Co() {
         for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
         return function() {
-            for (var n = arguments.length, i = new Array(n), h = 0; h < n; h++) i[h] = arguments[h];
+            for (var n = arguments.length, a = new Array(n), l = 0; l < n; l++) a[l] = arguments[l];
             return t.filter(function(v) {
                 return !!v
             }).map(function(v) {
-                return v.apply(void 0, i)
+                return v.apply(void 0, a)
             })
         }
     }
 
     function Xt(e) {
         return e && e.isA && e.isA("vtkObject")
     }
 
-    function qe(e, t) {
+    function Ne(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : [],
             n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : [];
         if (Xt(e)) {
             if (n.indexOf(e) >= 0) return r;
             n.push(e);
-            var i = t(e);
-            i !== void 0 && r.push(i);
-            var h = e.get();
-            Object.keys(h).forEach(function(v) {
-                var u = h[v];
-                Array.isArray(u) ? u.forEach(function(a) {
-                    qe(a, t, r, n)
-                }) : qe(u, t, r, n)
+            var a = t(e);
+            a !== void 0 && r.push(a);
+            var l = e.get();
+            Object.keys(l).forEach(function(v) {
+                var u = l[v];
+                Array.isArray(u) ? u.forEach(function(i) {
+                    Ne(i, t, r, n)
+                }) : Ne(u, t, r, n)
             })
         }
         return r
     }
 
-    function wo(e, t, r) {
+    function _o(e, t, r) {
         var n = this,
-            i, h = function() {
-                for (var u = arguments.length, a = new Array(u), s = 0; s < u; s++) a[s] = arguments[s];
+            a, l = function() {
+                for (var u = arguments.length, i = new Array(u), s = 0; s < u; s++) i[s] = arguments[s];
                 var c = n,
-                    l = function() {
-                        i = null, r || e.apply(c, a)
+                    h = function() {
+                        a = null, r || e.apply(c, i)
                     },
-                    p = r && !i;
-                clearTimeout(i), i = setTimeout(l, t), p && e.apply(c, a)
+                    p = r && !a;
+                clearTimeout(a), a = setTimeout(h, t), p && e.apply(c, i)
             };
-        return h.cancel = function() {
-            return clearTimeout(i)
-        }, h
+        return l.cancel = function() {
+            return clearTimeout(a)
+        }, l
     }
 
-    function So(e, t) {
+    function Lo(e, t) {
         var r = !1,
             n = null;
 
-        function i() {
-            r = !1, n !== null && (h.apply(void 0, se(n)), n = null)
+        function a() {
+            r = !1, n !== null && (l.apply(void 0, se(n)), n = null)
         }
 
-        function h() {
-            for (var v = arguments.length, u = new Array(v), a = 0; a < v; a++) u[a] = arguments[a];
+        function l() {
+            for (var v = arguments.length, u = new Array(v), i = 0; i < v; i++) u[i] = arguments[i];
             if (r) {
                 n = u;
                 return
             }
-            r = !0, e.apply(void 0, u), setTimeout(i, t)
+            r = !0, e.apply(void 0, u), setTimeout(a, t)
         }
-        return h
+        return l
     }
 
     function Ht(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        t.keystore = Object.assign(t.keystore || {}, r), e.setKey = function(n, i) {
-            t.keystore[n] = i
+        t.keystore = Object.assign(t.keystore || {}, r), e.setKey = function(n, a) {
+            t.keystore[n] = a
         }, e.getKey = function(n) {
             return t.keystore[n]
         }, e.getAllKeys = function() {
             return Object.keys(t.keystore)
         }, e.deleteKey = function(n) {
             return delete t.keystore[n]
         }, e.clearKeystore = function() {
             return e.getAllKeys().forEach(function(n) {
                 return delete t.keystore[n]
             })
         }
     }
-    var Eo = 1,
-        be = "__root__";
+    var Fo = 1,
+        xe = "__root__";
 
-    function Oo(e, t) {
+    function Uo(e, t) {
         Ht(e, t);
         var r = e.delete;
-        t.proxyId = "".concat(Eo++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), Oe(e, t, ["proxyId", "proxyGroup", "proxyName"]), Vt(e, t, ["proxyManager"]);
+        t.proxyId = "".concat(Fo++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), be(e, t, ["proxyId", "proxyGroup", "proxyName"]), Vt(e, t, ["proxyManager"]);
         var n = {},
-            i = {};
+            a = {};
 
-        function h(s, c) {
-            i[c] || (i[c] = []);
-            for (var l = i[c], p = 0; p < s.length; p++) l.push(s[p].name), n[s[p].name] = s[p], s[p].children && s[p].children.length && h(s[p].children, s[p].name)
+        function l(s, c) {
+            a[c] || (a[c] = []);
+            for (var h = a[c], p = 0; p < s.length; p++) h.push(s[p].name), n[s[p].name] = s[p], s[p].children && s[p].children.length && l(s[p].children, s[p].name)
         }
-        h(t.ui, be), e.updateUI = function(s) {
+        l(t.ui, xe), e.updateUI = function(s) {
             t.ui = JSON.parse(JSON.stringify(s || [])), Object.keys(n).forEach(function(c) {
                 return delete n[c]
-            }), Object.keys(i).forEach(function(c) {
-                return delete i[c]
-            }), h(t.ui, be), e.modified()
+            }), Object.keys(a).forEach(function(c) {
+                return delete a[c]
+            }), l(t.ui, xe), e.modified()
         };
 
         function v() {
-            var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : be;
-            return i[s]
+            var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : xe;
+            return a[s]
         }
         e.updateProxyProperty = function(s, c) {
-            var l = n[s];
-            l ? Object.assign(l, c) : n[s] = Ee({}, c)
+            var h = n[s];
+            h ? Object.assign(h, c) : n[s] = Oe({}, c)
         }, e.activate = function() {
             if (t.proxyManager) {
                 var s = "setActive".concat(D(e.getProxyGroup().slice(0, -1)));
                 t.proxyManager[s] && t.proxyManager[s](e)
             }
         }, t.propertyLinkSubscribers = {}, e.registerPropertyLinkForGC = function(s, c) {
             c in t.propertyLinkSubscribers || (t.propertyLinkSubscribers[c] = []), t.propertyLinkSubscribers[c].push(s)
         }, e.gcPropertyLinks = function(s) {
             for (var c = t.propertyLinkSubscribers[s] || []; c.length;) c.pop().unbind(e)
         }, t.propertyLinkMap = {}, e.getPropertyLink = function(s) {
             var c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
             if (t.propertyLinkMap[s]) return t.propertyLinkMap[s];
-            var l = null,
+            var h = null,
                 p = [],
                 o = 0,
                 f = !1;
 
-            function y(d) {
+            function y(g) {
                 var S = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
                 if (f) return null;
                 var E = [],
                     O = null;
                 for (o = p.length; o--;) {
                     var b = p[o];
-                    b.instance === d ? O = b : E.push(b)
+                    b.instance === g ? O = b : E.push(b)
                 }
                 if (!O) return null;
                 var M = O.instance["get".concat(D(O.propertyName))]();
-                if (!io(M, l) || S) {
-                    for (l = M, f = !0; E.length;) {
+                if (!So(M, h) || S) {
+                    for (h = M, f = !0; E.length;) {
                         var _ = E.pop();
-                        _.instance.set(V({}, _.propertyName, l))
+                        _.instance.set(V({}, _.propertyName, h))
                     }
                     f = !1
                 }
                 return t.propertyLinkMap[s].persistent && (t.propertyLinkMap[s].value = M), M
             }
 
-            function g(d, S) {
+            function d(g, S) {
                 var E = [];
                 for (o = p.length; o--;) {
                     var O = p[o];
-                    O.instance === d && (O.propertyName === S || S === void 0) && (O.subscription.unsubscribe(), E.push(o))
+                    O.instance === g && (O.propertyName === S || S === void 0) && (O.subscription.unsubscribe(), E.push(o))
                 }
                 for (; E.length;) p.splice(E.pop(), 1)
             }
 
-            function m(d, S) {
+            function m(g, S) {
                 var E = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
-                    O = d.onModified(y),
+                    O = g.onModified(y),
                     b = p[0];
                 return p.push({
-                    instance: d,
+                    instance: g,
                     propertyName: S,
                     subscription: O
-                }), E && (t.propertyLinkMap[s].persistent && t.propertyLinkMap[s].value !== void 0 ? d.set(V({}, S, t.propertyLinkMap[s].value)) : b && y(b.instance, !0)), {
+                }), E && (t.propertyLinkMap[s].persistent && t.propertyLinkMap[s].value !== void 0 ? g.set(V({}, S, t.propertyLinkMap[s].value)) : b && y(b.instance, !0)), {
                     unsubscribe: function() {
-                        return g(d, S)
+                        return d(g, S)
                     }
                 }
             }
 
             function w() {
                 for (; p.length;) p.pop().subscription.unsubscribe()
             }
-            var T = {
+            var k = {
                 bind: m,
-                unbind: g,
+                unbind: d,
                 unsubscribe: w,
                 persistent: c
             };
-            return t.propertyLinkMap[s] = T, T
+            return t.propertyLinkMap[s] = k, k
         };
 
         function u() {
-            for (var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : be, c = [], l = t.proxyId, p = v(s) || [], o = 0; o < p.length; o++) {
+            for (var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : xe, c = [], h = t.proxyId, p = v(s) || [], o = 0; o < p.length; o++) {
                 var f = p[o],
                     y = e["get".concat(D(f))],
-                    g = y ? y() : void 0,
+                    d = y ? y() : void 0,
                     m = {
-                        id: l,
+                        id: h,
                         name: f,
-                        value: g
+                        value: d
                     },
                     w = u(f);
                 w.length && (m.children = w), c.push(m)
             }
             return c
         }
         e.listPropertyNames = function() {
@@ -2265,565 +2264,565 @@
         }, e.delete = function() {
             for (var s = Object.keys(t.propertyLinkMap), c = s.length; c--;) t.propertyLinkMap[s[c]].unsubscribe();
             Object.keys(t.propertyLinkSubscribers).forEach(e.gcPropertyLinks), r()
         }, e.getState = function() {
             return null
         };
 
-        function a() {
+        function i() {
             if (t.links)
                 for (var s = 0; s < t.links.length; s++) {
                     var c = t.links[s],
-                        l = c.link,
+                        h = c.link,
                         p = c.property,
                         o = c.persistent,
                         f = c.updateOnBind,
                         y = c.type;
                     if (y === "application") {
-                        var g = t.proxyManager.getPropertyLink(l, o);
-                        e.registerPropertyLinkForGC(g, "application"), g.bind(e, p, f)
+                        var d = t.proxyManager.getPropertyLink(h, o);
+                        e.registerPropertyLinkForGC(d, "application"), d.bind(e, p, f)
                     }
                 }
         }
-        $t(a)
+        zt(i)
     }
 
-    function bo(e, t, r) {
-        for (var n = e.delete, i = [], h = Object.keys(r), v = h.length; v--;) {
-            var u = h[v],
-                a = r[u],
-                s = a.modelKey,
-                c = a.property,
-                l = a.modified,
-                p = l === void 0 ? !0 : l,
+    function Bo(e, t, r) {
+        for (var n = e.delete, a = [], l = Object.keys(r), v = l.length; v--;) {
+            var u = l[v],
+                i = r[u],
+                s = i.modelKey,
+                c = i.property,
+                h = i.modified,
+                p = h === void 0 ? !0 : h,
                 o = D(c),
                 f = D(u);
-            e["get".concat(f)] = t[s]["get".concat(o)], e["set".concat(f)] = t[s]["set".concat(o)], p && i.push(t[s].onModified(e.modified))
+            e["get".concat(f)] = t[s]["get".concat(o)], e["set".concat(f)] = t[s]["set".concat(o)], p && a.push(t[s].onModified(e.modified))
         }
         e.delete = function() {
-            for (; i.length;) i.pop().unsubscribe();
+            for (; a.length;) a.pop().unsubscribe();
             n()
         }
     }
 
-    function xo(e, t) {
+    function $o(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
             n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : {};
         t.this = e;
 
-        function i(a) {
-            for (var s = Object.keys(a), c = s.length; c--;) {
-                var l = s[c];
-                t[l].set(a[l])
+        function a(i) {
+            for (var s = Object.keys(i), c = s.length; c--;) {
+                var h = s[c];
+                t[h].set(i[h])
             }
         }
-        for (var h = Object.keys(n), v = h.length, u = function() {
-                var s = h[v];
+        for (var l = Object.keys(n), v = l.length, u = function() {
+                var s = l[v];
                 t[s] = n[s];
                 var c = r[s];
-                e["set".concat(D(s))] = function(l) {
-                    if (l !== t[s]) {
-                        t[s] = l;
-                        var p = c[l];
-                        i(p), e.modified()
+                e["set".concat(D(s))] = function(h) {
+                    if (h !== t[s]) {
+                        t[s] = h;
+                        var p = c[h];
+                        a(p), e.modified()
                     }
                 }
             }; v--;) u();
-        h.length && Oe(e, t, h)
+        l.length && be(e, t, l)
     }
     var Yt = 10,
         At = 40,
         Jt = 800;
 
-    function To(e) {
+    function Wo(e) {
         var t = 0,
             r = 0,
             n = 0,
-            i = 0;
-        return "detail" in e && (r = e.detail), "wheelDelta" in e && (r = -e.wheelDelta / 120), "wheelDeltaY" in e && (r = -e.wheelDeltaY / 120), "wheelDeltaX" in e && (t = -e.wheelDeltaX / 120), "axis" in e && e.axis === e.HORIZONTAL_AXIS && (t = r, r = 0), n = t * Yt, i = r * Yt, "deltaY" in e && (i = e.deltaY), "deltaX" in e && (n = e.deltaX), (n || i) && e.deltaMode && (e.deltaMode === 1 ? (n *= At, i *= At) : (n *= Jt, i *= Jt)), n && !t && (t = n < 1 ? -1 : 1), i && !r && (r = i < 1 ? -1 : 1), {
+            a = 0;
+        return "detail" in e && (r = e.detail), "wheelDelta" in e && (r = -e.wheelDelta / 120), "wheelDeltaY" in e && (r = -e.wheelDeltaY / 120), "wheelDeltaX" in e && (t = -e.wheelDeltaX / 120), "axis" in e && e.axis === e.HORIZONTAL_AXIS && (t = r, r = 0), n = t * Yt, a = r * Yt, "deltaY" in e && (a = e.deltaY), "deltaX" in e && (n = e.deltaX), (n || a) && e.deltaMode && (e.deltaMode === 1 ? (n *= At, a *= At) : (n *= Jt, a *= Jt)), n && !t && (t = n < 1 ? -1 : 1), a && !r && (r = a < 1 ? -1 : 1), {
             spinX: t,
             spinY: r,
             pixelX: n,
-            pixelY: i
+            pixelY: a
         }
     }
-    var k = {
-            algo: vo,
-            capitalize: Ke,
-            chain: mo,
-            debounce: wo,
-            enumToString: so,
-            event: yo,
+    var T = {
+            algo: Mo,
+            capitalize: Ge,
+            chain: Co,
+            debounce: _o,
+            enumToString: Eo,
+            event: Do,
             EVENT_ABORT: Pt,
-            formatBytesToProperUnit: oo,
-            formatNumbersWithThousandSeparator: ao,
-            get: Oe,
+            formatBytesToProperUnit: mo,
+            formatNumbersWithThousandSeparator: wo,
+            get: be,
             getArray: Kt,
-            getCurrentGlobalMTime: Ar,
-            getStateArrayMapFunc: zt,
+            getCurrentGlobalMTime: uo,
+            getStateArrayMapFunc: Wt,
             isVtkObject: Xt,
             keystore: Ht,
-            measurePromiseExecution: uo,
-            moveToProtected: po,
-            newInstance: go,
-            newTypedArray: to,
-            newTypedArrayFrom: no,
-            normalizeWheel: To,
-            obj: co,
-            proxy: Oo,
-            proxyPropertyMapping: bo,
-            proxyPropertyState: xo,
-            safeArrays: Wt,
+            measurePromiseExecution: Oo,
+            moveToProtected: Ro,
+            newInstance: jo,
+            newTypedArray: vo,
+            newTypedArrayFrom: yo,
+            normalizeWheel: Wo,
+            obj: bo,
+            proxy: Uo,
+            proxyPropertyMapping: Bo,
+            proxyPropertyState: $o,
+            safeArrays: $t,
             set: Nt,
             setArray: qt,
             setGet: Vt,
-            setGetArray: ho,
-            setImmediate: $t,
-            setLoggerFunction: Zr,
-            throttle: So,
-            traverseInstanceTree: qe,
+            setGetArray: To,
+            setImmediate: zt,
+            setLoggerFunction: fo,
+            throttle: Lo,
+            traverseInstanceTree: Ne,
             TYPED_ARRAYS: F,
-            uncapitalize: ro,
-            VOID: Yr,
-            vtkDebugMacro: Ve,
+            uncapitalize: go,
+            VOID: so,
+            vtkDebugMacro: ze,
             vtkErrorMacro: C,
-            vtkInfoMacro: Ir,
-            vtkLogMacro: Qr,
-            vtkOnceErrorMacro: eo,
+            vtkInfoMacro: ho,
+            vtkLogMacro: lo,
+            vtkOnceErrorMacro: po,
             vtkWarningMacro: Ut
         },
-        Pe = {
+        Ve = {
             exports: {}
         };
-    Pe.exports,
+    Ve.exports,
         function(e) {
             (function(t, r, n) {
-                function i(a) {
+                function a(i) {
                     var s = this,
                         c = u();
                     s.next = function() {
-                        var l = 2091639 * s.s0 + s.c * 23283064365386963e-26;
-                        return s.s0 = s.s1, s.s1 = s.s2, s.s2 = l - (s.c = l | 0)
-                    }, s.c = 1, s.s0 = c(" "), s.s1 = c(" "), s.s2 = c(" "), s.s0 -= c(a), s.s0 < 0 && (s.s0 += 1), s.s1 -= c(a), s.s1 < 0 && (s.s1 += 1), s.s2 -= c(a), s.s2 < 0 && (s.s2 += 1), c = null
+                        var h = 2091639 * s.s0 + s.c * 23283064365386963e-26;
+                        return s.s0 = s.s1, s.s1 = s.s2, s.s2 = h - (s.c = h | 0)
+                    }, s.c = 1, s.s0 = c(" "), s.s1 = c(" "), s.s2 = c(" "), s.s0 -= c(i), s.s0 < 0 && (s.s0 += 1), s.s1 -= c(i), s.s1 < 0 && (s.s1 += 1), s.s2 -= c(i), s.s2 < 0 && (s.s2 += 1), c = null
                 }
 
-                function h(a, s) {
-                    return s.c = a.c, s.s0 = a.s0, s.s1 = a.s1, s.s2 = a.s2, s
+                function l(i, s) {
+                    return s.c = i.c, s.s0 = i.s0, s.s1 = i.s1, s.s2 = i.s2, s
                 }
 
-                function v(a, s) {
-                    var c = new i(a),
-                        l = s && s.state,
+                function v(i, s) {
+                    var c = new a(i),
+                        h = s && s.state,
                         p = c.next;
                     return p.int32 = function() {
                         return c.next() * 4294967296 | 0
                     }, p.double = function() {
                         return p() + (p() * 2097152 | 0) * 11102230246251565e-32
-                    }, p.quick = p, l && (typeof l == "object" && h(l, c), p.state = function() {
-                        return h(c, {})
+                    }, p.quick = p, h && (typeof h == "object" && l(h, c), p.state = function() {
+                        return l(c, {})
                     }), p
                 }
 
                 function u() {
-                    var a = 4022871197,
+                    var i = 4022871197,
                         s = function(c) {
                             c = String(c);
-                            for (var l = 0; l < c.length; l++) {
-                                a += c.charCodeAt(l);
-                                var p = .02519603282416938 * a;
-                                a = p >>> 0, p -= a, p *= a, a = p >>> 0, p -= a, a += p * 4294967296
+                            for (var h = 0; h < c.length; h++) {
+                                i += c.charCodeAt(h);
+                                var p = .02519603282416938 * i;
+                                i = p >>> 0, p -= i, p *= i, i = p >>> 0, p -= i, i += p * 4294967296
                             }
-                            return (a >>> 0) * 23283064365386963e-26
+                            return (i >>> 0) * 23283064365386963e-26
                         };
                     return s
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.alea = v
             })(B, e, !1)
-        }(Pe);
-    var ko = Pe.exports,
-        Xe = {
+        }(Ve);
+    var zo = Ve.exports,
+        Ke = {
             exports: {}
         };
-    Xe.exports,
+    Ke.exports,
         function(e) {
             (function(t, r, n) {
-                function i(u) {
-                    var a = this,
+                function a(u) {
+                    var i = this,
                         s = "";
-                    a.x = 0, a.y = 0, a.z = 0, a.w = 0, a.next = function() {
-                        var l = a.x ^ a.x << 11;
-                        return a.x = a.y, a.y = a.z, a.z = a.w, a.w ^= a.w >>> 19 ^ l ^ l >>> 8
-                    }, u === (u | 0) ? a.x = u : s += u;
-                    for (var c = 0; c < s.length + 64; c++) a.x ^= s.charCodeAt(c) | 0, a.next()
+                    i.x = 0, i.y = 0, i.z = 0, i.w = 0, i.next = function() {
+                        var h = i.x ^ i.x << 11;
+                        return i.x = i.y, i.y = i.z, i.z = i.w, i.w ^= i.w >>> 19 ^ h ^ h >>> 8
+                    }, u === (u | 0) ? i.x = u : s += u;
+                    for (var c = 0; c < s.length + 64; c++) i.x ^= s.charCodeAt(c) | 0, i.next()
                 }
 
-                function h(u, a) {
-                    return a.x = u.x, a.y = u.y, a.z = u.z, a.w = u.w, a
+                function l(u, i) {
+                    return i.x = u.x, i.y = u.y, i.z = u.z, i.w = u.w, i
                 }
 
-                function v(u, a) {
-                    var s = new i(u),
-                        c = a && a.state,
-                        l = function() {
+                function v(u, i) {
+                    var s = new a(u),
+                        c = i && i.state,
+                        h = function() {
                             return (s.next() >>> 0) / 4294967296
                         };
-                    return l.double = function() {
+                    return h.double = function() {
                         do var p = s.next() >>> 11,
                             o = (s.next() >>> 0) / 4294967296,
                             f = (p + o) / (1 << 21); while (f === 0);
                         return f
-                    }, l.int32 = s.next, l.quick = l, c && (typeof c == "object" && h(c, s), l.state = function() {
-                        return h(s, {})
-                    }), l
+                    }, h.int32 = s.next, h.quick = h, c && (typeof c == "object" && l(c, s), h.state = function() {
+                        return l(s, {})
+                    }), h
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.xor128 = v
             })(B, e, !1)
-        }(Xe);
-    var Ro = Xe.exports,
-        He = {
+        }(Ke);
+    var Go = Ke.exports,
+        qe = {
             exports: {}
         };
-    He.exports,
+    qe.exports,
         function(e) {
             (function(t, r, n) {
-                function i(u) {
-                    var a = this,
+                function a(u) {
+                    var i = this,
                         s = "";
-                    a.next = function() {
-                        var l = a.x ^ a.x >>> 2;
-                        return a.x = a.y, a.y = a.z, a.z = a.w, a.w = a.v, (a.d = a.d + 362437 | 0) + (a.v = a.v ^ a.v << 4 ^ (l ^ l << 1)) | 0
-                    }, a.x = 0, a.y = 0, a.z = 0, a.w = 0, a.v = 0, u === (u | 0) ? a.x = u : s += u;
-                    for (var c = 0; c < s.length + 64; c++) a.x ^= s.charCodeAt(c) | 0, c == s.length && (a.d = a.x << 10 ^ a.x >>> 4), a.next()
+                    i.next = function() {
+                        var h = i.x ^ i.x >>> 2;
+                        return i.x = i.y, i.y = i.z, i.z = i.w, i.w = i.v, (i.d = i.d + 362437 | 0) + (i.v = i.v ^ i.v << 4 ^ (h ^ h << 1)) | 0
+                    }, i.x = 0, i.y = 0, i.z = 0, i.w = 0, i.v = 0, u === (u | 0) ? i.x = u : s += u;
+                    for (var c = 0; c < s.length + 64; c++) i.x ^= s.charCodeAt(c) | 0, c == s.length && (i.d = i.x << 10 ^ i.x >>> 4), i.next()
                 }
 
-                function h(u, a) {
-                    return a.x = u.x, a.y = u.y, a.z = u.z, a.w = u.w, a.v = u.v, a.d = u.d, a
+                function l(u, i) {
+                    return i.x = u.x, i.y = u.y, i.z = u.z, i.w = u.w, i.v = u.v, i.d = u.d, i
                 }
 
-                function v(u, a) {
-                    var s = new i(u),
-                        c = a && a.state,
-                        l = function() {
+                function v(u, i) {
+                    var s = new a(u),
+                        c = i && i.state,
+                        h = function() {
                             return (s.next() >>> 0) / 4294967296
                         };
-                    return l.double = function() {
+                    return h.double = function() {
                         do var p = s.next() >>> 11,
                             o = (s.next() >>> 0) / 4294967296,
                             f = (p + o) / (1 << 21); while (f === 0);
                         return f
-                    }, l.int32 = s.next, l.quick = l, c && (typeof c == "object" && h(c, s), l.state = function() {
-                        return h(s, {})
-                    }), l
+                    }, h.int32 = s.next, h.quick = h, c && (typeof c == "object" && l(c, s), h.state = function() {
+                        return l(s, {})
+                    }), h
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.xorwow = v
             })(B, e, !1)
-        }(He);
-    var Mo = He.exports,
-        Ye = {
+        }(qe);
+    var No = qe.exports,
+        Pe = {
             exports: {}
         };
-    Ye.exports,
+    Pe.exports,
         function(e) {
             (function(t, r, n) {
-                function i(u) {
-                    var a = this;
-                    a.next = function() {
-                        var c = a.x,
-                            l = a.i,
+                function a(u) {
+                    var i = this;
+                    i.next = function() {
+                        var c = i.x,
+                            h = i.i,
                             p, o;
-                        return p = c[l], p ^= p >>> 7, o = p ^ p << 24, p = c[l + 1 & 7], o ^= p ^ p >>> 10, p = c[l + 3 & 7], o ^= p ^ p >>> 3, p = c[l + 4 & 7], o ^= p ^ p << 7, p = c[l + 7 & 7], p = p ^ p << 13, o ^= p ^ p << 9, c[l] = o, a.i = l + 1 & 7, o
+                        return p = c[h], p ^= p >>> 7, o = p ^ p << 24, p = c[h + 1 & 7], o ^= p ^ p >>> 10, p = c[h + 3 & 7], o ^= p ^ p >>> 3, p = c[h + 4 & 7], o ^= p ^ p << 7, p = c[h + 7 & 7], p = p ^ p << 13, o ^= p ^ p << 9, c[h] = o, i.i = h + 1 & 7, o
                     };
 
-                    function s(c, l) {
+                    function s(c, h) {
                         var p, o = [];
-                        if (l === (l | 0)) o[0] = l;
+                        if (h === (h | 0)) o[0] = h;
                         else
-                            for (l = "" + l, p = 0; p < l.length; ++p) o[p & 7] = o[p & 7] << 15 ^ l.charCodeAt(p) + o[p + 1 & 7] << 13;
+                            for (h = "" + h, p = 0; p < h.length; ++p) o[p & 7] = o[p & 7] << 15 ^ h.charCodeAt(p) + o[p + 1 & 7] << 13;
                         for (; o.length < 8;) o.push(0);
                         for (p = 0; p < 8 && o[p] === 0; ++p);
                         for (p == 8 ? o[7] = -1 : o[p], c.x = o, c.i = 0, p = 256; p > 0; --p) c.next()
                     }
-                    s(a, u)
+                    s(i, u)
                 }
 
-                function h(u, a) {
-                    return a.x = u.x.slice(), a.i = u.i, a
+                function l(u, i) {
+                    return i.x = u.x.slice(), i.i = u.i, i
                 }
 
-                function v(u, a) {
+                function v(u, i) {
                     u == null && (u = +new Date);
-                    var s = new i(u),
-                        c = a && a.state,
-                        l = function() {
+                    var s = new a(u),
+                        c = i && i.state,
+                        h = function() {
                             return (s.next() >>> 0) / 4294967296
                         };
-                    return l.double = function() {
+                    return h.double = function() {
                         do var p = s.next() >>> 11,
                             o = (s.next() >>> 0) / 4294967296,
                             f = (p + o) / (1 << 21); while (f === 0);
                         return f
-                    }, l.int32 = s.next, l.quick = l, c && (c.x && h(c, s), l.state = function() {
-                        return h(s, {})
-                    }), l
+                    }, h.int32 = s.next, h.quick = h, c && (c.x && l(c, s), h.state = function() {
+                        return l(s, {})
+                    }), h
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.xorshift7 = v
             })(B, e, !1)
-        }(Ye);
-    var Do = Ye.exports,
-        Ae = {
+        }(Pe);
+    var Vo = Pe.exports,
+        Xe = {
             exports: {}
         };
-    Ae.exports,
+    Xe.exports,
         function(e) {
             (function(t, r, n) {
-                function i(u) {
-                    var a = this;
-                    a.next = function() {
-                        var c = a.w,
-                            l = a.X,
-                            p = a.i,
+                function a(u) {
+                    var i = this;
+                    i.next = function() {
+                        var c = i.w,
+                            h = i.X,
+                            p = i.i,
                             o, f;
-                        return a.w = c = c + 1640531527 | 0, f = l[p + 34 & 127], o = l[p = p + 1 & 127], f ^= f << 13, o ^= o << 17, f ^= f >>> 15, o ^= o >>> 12, f = l[p] = f ^ o, a.i = p, f + (c ^ c >>> 16) | 0
+                        return i.w = c = c + 1640531527 | 0, f = h[p + 34 & 127], o = h[p = p + 1 & 127], f ^= f << 13, o ^= o << 17, f ^= f >>> 15, o ^= o >>> 12, f = h[p] = f ^ o, i.i = p, f + (c ^ c >>> 16) | 0
                     };
 
-                    function s(c, l) {
-                        var p, o, f, y, g, m = [],
+                    function s(c, h) {
+                        var p, o, f, y, d, m = [],
                             w = 128;
-                        for (l === (l | 0) ? (o = l, l = null) : (l = l + "\0", o = 0, w = Math.max(w, l.length)), f = 0, y = -32; y < w; ++y) l && (o ^= l.charCodeAt((y + 32) % l.length)), y === 0 && (g = o), o ^= o << 10, o ^= o >>> 15, o ^= o << 4, o ^= o >>> 13, y >= 0 && (g = g + 1640531527 | 0, p = m[y & 127] ^= o + g, f = p == 0 ? f + 1 : 0);
-                        for (f >= 128 && (m[(l && l.length || 0) & 127] = -1), f = 127, y = 4 * 128; y > 0; --y) o = m[f + 34 & 127], p = m[f = f + 1 & 127], o ^= o << 13, p ^= p << 17, o ^= o >>> 15, p ^= p >>> 12, m[f] = o ^ p;
-                        c.w = g, c.X = m, c.i = f
+                        for (h === (h | 0) ? (o = h, h = null) : (h = h + "\0", o = 0, w = Math.max(w, h.length)), f = 0, y = -32; y < w; ++y) h && (o ^= h.charCodeAt((y + 32) % h.length)), y === 0 && (d = o), o ^= o << 10, o ^= o >>> 15, o ^= o << 4, o ^= o >>> 13, y >= 0 && (d = d + 1640531527 | 0, p = m[y & 127] ^= o + d, f = p == 0 ? f + 1 : 0);
+                        for (f >= 128 && (m[(h && h.length || 0) & 127] = -1), f = 127, y = 4 * 128; y > 0; --y) o = m[f + 34 & 127], p = m[f = f + 1 & 127], o ^= o << 13, p ^= p << 17, o ^= o >>> 15, p ^= p >>> 12, m[f] = o ^ p;
+                        c.w = d, c.X = m, c.i = f
                     }
-                    s(a, u)
+                    s(i, u)
                 }
 
-                function h(u, a) {
-                    return a.i = u.i, a.w = u.w, a.X = u.X.slice(), a
+                function l(u, i) {
+                    return i.i = u.i, i.w = u.w, i.X = u.X.slice(), i
                 }
 
-                function v(u, a) {
+                function v(u, i) {
                     u == null && (u = +new Date);
-                    var s = new i(u),
-                        c = a && a.state,
-                        l = function() {
+                    var s = new a(u),
+                        c = i && i.state,
+                        h = function() {
                             return (s.next() >>> 0) / 4294967296
                         };
-                    return l.double = function() {
+                    return h.double = function() {
                         do var p = s.next() >>> 11,
                             o = (s.next() >>> 0) / 4294967296,
                             f = (p + o) / (1 << 21); while (f === 0);
                         return f
-                    }, l.int32 = s.next, l.quick = l, c && (c.X && h(c, s), l.state = function() {
-                        return h(s, {})
-                    }), l
+                    }, h.int32 = s.next, h.quick = h, c && (c.X && l(c, s), h.state = function() {
+                        return l(s, {})
+                    }), h
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.xor4096 = v
             })(B, e, !1)
-        }(Ae);
-    var jo = Ae.exports,
-        Je = {
+        }(Xe);
+    var Ko = Xe.exports,
+        He = {
             exports: {}
         };
-    Je.exports,
+    He.exports,
         function(e) {
             (function(t, r, n) {
-                function i(u) {
-                    var a = this,
+                function a(u) {
+                    var i = this,
                         s = "";
-                    a.next = function() {
-                        var l = a.b,
-                            p = a.c,
-                            o = a.d,
-                            f = a.a;
-                        return l = l << 25 ^ l >>> 7 ^ p, p = p - o | 0, o = o << 24 ^ o >>> 8 ^ f, f = f - l | 0, a.b = l = l << 20 ^ l >>> 12 ^ p, a.c = p = p - o | 0, a.d = o << 16 ^ p >>> 16 ^ f, a.a = f - l | 0
-                    }, a.a = 0, a.b = 0, a.c = -1640531527, a.d = 1367130551, u === Math.floor(u) ? (a.a = u / 4294967296 | 0, a.b = u | 0) : s += u;
-                    for (var c = 0; c < s.length + 20; c++) a.b ^= s.charCodeAt(c) | 0, a.next()
-                }
-
-                function h(u, a) {
-                    return a.a = u.a, a.b = u.b, a.c = u.c, a.d = u.d, a
-                }
-
-                function v(u, a) {
-                    var s = new i(u),
-                        c = a && a.state,
-                        l = function() {
+                    i.next = function() {
+                        var h = i.b,
+                            p = i.c,
+                            o = i.d,
+                            f = i.a;
+                        return h = h << 25 ^ h >>> 7 ^ p, p = p - o | 0, o = o << 24 ^ o >>> 8 ^ f, f = f - h | 0, i.b = h = h << 20 ^ h >>> 12 ^ p, i.c = p = p - o | 0, i.d = o << 16 ^ p >>> 16 ^ f, i.a = f - h | 0
+                    }, i.a = 0, i.b = 0, i.c = -1640531527, i.d = 1367130551, u === Math.floor(u) ? (i.a = u / 4294967296 | 0, i.b = u | 0) : s += u;
+                    for (var c = 0; c < s.length + 20; c++) i.b ^= s.charCodeAt(c) | 0, i.next()
+                }
+
+                function l(u, i) {
+                    return i.a = u.a, i.b = u.b, i.c = u.c, i.d = u.d, i
+                }
+
+                function v(u, i) {
+                    var s = new a(u),
+                        c = i && i.state,
+                        h = function() {
                             return (s.next() >>> 0) / 4294967296
                         };
-                    return l.double = function() {
+                    return h.double = function() {
                         do var p = s.next() >>> 11,
                             o = (s.next() >>> 0) / 4294967296,
                             f = (p + o) / (1 << 21); while (f === 0);
                         return f
-                    }, l.int32 = s.next, l.quick = l, c && (typeof c == "object" && h(c, s), l.state = function() {
-                        return h(s, {})
-                    }), l
+                    }, h.int32 = s.next, h.quick = h, c && (typeof c == "object" && l(c, s), h.state = function() {
+                        return l(s, {})
+                    }), h
                 }
                 r && r.exports ? r.exports = v : n && n.amd ? n(function() {
                     return v
                 }) : this.tychei = v
             })(B, e, !1)
-        }(Je);
-    var Co = Je.exports,
+        }(He);
+    var qo = He.exports,
         Zt = {
             exports: {}
         };
-    const _o = Bn(Object.freeze(Object.defineProperty({
+    const Po = Bn(Object.freeze(Object.defineProperty({
         __proto__: null,
         default: {}
     }, Symbol.toStringTag, {
         value: "Module"
     })));
     (function(e) {
         (function(t, r, n) {
-            var i = 256,
-                h = 6,
+            var a = 256,
+                l = 6,
                 v = 52,
                 u = "random",
-                a = n.pow(i, h),
+                i = n.pow(a, l),
                 s = n.pow(2, v),
                 c = s * 2,
-                l = i - 1,
+                h = a - 1,
                 p;
 
-            function o(d, S, E) {
+            function o(g, S, E) {
                 var O = [];
                 S = S == !0 ? {
                     entropy: !0
                 } : S || {};
-                var b = m(g(S.entropy ? [d, T(r)] : d ?? w(), 3), O),
+                var b = m(d(S.entropy ? [g, k(r)] : g ?? w(), 3), O),
                     M = new f(O),
                     _ = function() {
-                        for (var L = M.g(h), $ = a, W = 0; L < s;) L = (L + W) * i, $ *= i, W = M.g(1);
-                        for (; L >= c;) L /= 2, $ /= 2, W >>>= 1;
-                        return (L + W) / $
+                        for (var L = M.g(l), z = i, $ = 0; L < s;) L = (L + $) * a, z *= a, $ = M.g(1);
+                        for (; L >= c;) L /= 2, z /= 2, $ >>>= 1;
+                        return (L + $) / z
                     };
                 return _.int32 = function() {
                     return M.g(4) | 0
                 }, _.quick = function() {
                     return M.g(4) / 4294967296
-                }, _.double = _, m(T(M.S), r), (S.pass || E || function(L, $, W, N) {
+                }, _.double = _, m(k(M.S), r), (S.pass || E || function(L, z, $, N) {
                     return N && (N.S && y(N, M), L.state = function() {
                         return y(M, {})
-                    }), W ? (n[u] = L, $) : L
+                    }), $ ? (n[u] = L, z) : L
                 })(_, b, "global" in S ? S.global : this == n, S.state)
             }
 
-            function f(d) {
-                var S, E = d.length,
+            function f(g) {
+                var S, E = g.length,
                     O = this,
                     b = 0,
                     M = O.i = O.j = 0,
                     _ = O.S = [];
-                for (E || (d = [E++]); b < i;) _[b] = b++;
-                for (b = 0; b < i; b++) _[b] = _[M = l & M + d[b % E] + (S = _[b])], _[M] = S;
+                for (E || (g = [E++]); b < a;) _[b] = b++;
+                for (b = 0; b < a; b++) _[b] = _[M = h & M + g[b % E] + (S = _[b])], _[M] = S;
                 (O.g = function(L) {
-                    for (var $, W = 0, N = O.i, ae = O.j, J = O.S; L--;) $ = J[N = l & N + 1], W = W * i + J[l & (J[N] = J[ae = l & ae + $]) + (J[ae] = $)];
-                    return O.i = N, O.j = ae, W
-                })(i)
+                    for (var z, $ = 0, N = O.i, ae = O.j, J = O.S; L--;) z = J[N = h & N + 1], $ = $ * a + J[h & (J[N] = J[ae = h & ae + z]) + (J[ae] = z)];
+                    return O.i = N, O.j = ae, $
+                })(a)
             }
 
-            function y(d, S) {
-                return S.i = d.i, S.j = d.j, S.S = d.S.slice(), S
+            function y(g, S) {
+                return S.i = g.i, S.j = g.j, S.S = g.S.slice(), S
             }
 
-            function g(d, S) {
+            function d(g, S) {
                 var E = [],
-                    O = typeof d,
+                    O = typeof g,
                     b;
                 if (S && O == "object")
-                    for (b in d) try {
-                        E.push(g(d[b], S - 1))
+                    for (b in g) try {
+                        E.push(d(g[b], S - 1))
                     } catch {}
-                return E.length ? E : O == "string" ? d : d + "\0"
+                return E.length ? E : O == "string" ? g : g + "\0"
             }
 
-            function m(d, S) {
-                for (var E = d + "", O, b = 0; b < E.length;) S[l & b] = l & (O ^= S[l & b] * 19) + E.charCodeAt(b++);
-                return T(S)
+            function m(g, S) {
+                for (var E = g + "", O, b = 0; b < E.length;) S[h & b] = h & (O ^= S[h & b] * 19) + E.charCodeAt(b++);
+                return k(S)
             }
 
             function w() {
                 try {
-                    var d;
-                    return p && (d = p.randomBytes) ? d = d(i) : (d = new Uint8Array(i), (t.crypto || t.msCrypto).getRandomValues(d)), T(d)
+                    var g;
+                    return p && (g = p.randomBytes) ? g = g(a) : (g = new Uint8Array(a), (t.crypto || t.msCrypto).getRandomValues(g)), k(g)
                 } catch {
                     var S = t.navigator,
                         E = S && S.plugins;
-                    return [+new Date, t, E, t.screen, T(r)]
+                    return [+new Date, t, E, t.screen, k(r)]
                 }
             }
 
-            function T(d) {
-                return String.fromCharCode.apply(0, d)
+            function k(g) {
+                return String.fromCharCode.apply(0, g)
             }
             if (m(n.random(), r), e.exports) {
                 e.exports = o;
                 try {
-                    p = _o
+                    p = Po
                 } catch {}
             } else n["seed" + u] = o
         })(typeof self < "u" ? self : B, [], Math)
     })(Zt);
-    var Lo = Zt.exports,
-        Fo = ko,
-        Uo = Ro,
-        Bo = Mo,
-        Wo = Do,
-        zo = jo,
-        $o = Co,
-        re = Lo;
-    re.alea = Fo, re.xor128 = Uo, re.xorwow = Bo, re.xorshift7 = Wo, re.xor4096 = zo, re.tychei = $o;
+    var Xo = Zt.exports,
+        Ho = zo,
+        Yo = Go,
+        Ao = No,
+        Jo = Vo,
+        Zo = Ko,
+        Qo = qo,
+        re = Xo;
+    re.alea = Ho, re.xor128 = Yo, re.xorwow = Ao, re.xorshift7 = Jo, re.xor4096 = Zo, re.tychei = Qo;
 
     function Qt(e) {
         return e * 180 / Math.PI
     }
-    var Go = {
+    var Io = {
             Unknown: 0,
             LeftController: 1,
             RightController: 2
         },
-        No = {
+        ea = {
             Unknown: 0,
             Trigger: 1,
             TrackPad: 2,
             Grip: 3,
             Thumbstick: 4,
             A: 5,
             B: 6,
             ApplicationMenu: 7
         },
-        Vo = {
+        ta = {
             Unknown: 0,
             TouchpadX: 1,
             TouchpadY: 2,
             ThumbstickX: 3,
             ThumbstickY: 4
         },
-        Ze = {
-            Device: Go,
-            Input: No,
-            Axis: Vo
+        Ye = {
+            Device: Io,
+            Input: ea,
+            Axis: ta
         };
 
     function It(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
-            t && (n = n.filter(function(i) {
-                return Object.getOwnPropertyDescriptor(e, i).enumerable
+            t && (n = n.filter(function(a) {
+                return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
     function R(e) {
         for (var t = 1; t < arguments.length; t++) {
@@ -2832,151 +2831,151 @@
                 V(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : It(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var xe = Ze.Device,
-        A = Ze.Input,
-        Te = k.vtkWarningMacro,
-        ke = k.vtkErrorMacro,
-        Ko = k.normalizeWheel,
-        qo = k.vtkOnceErrorMacro,
+    var ke = Ye.Device,
+        A = Ye.Input,
+        Te = T.vtkWarningMacro,
+        Re = T.vtkErrorMacro,
+        na = T.normalizeWheel,
+        ra = T.vtkOnceErrorMacro,
         oe = new MouseEvent(""),
-        Qe = {
+        Ae = {
             "xr-standard": [A.Trigger, A.Grip, A.TrackPad, A.Thumbstick, A.A, A.B]
         },
-        Ie = ["StartAnimation", "Animation", "EndAnimation", "PointerEnter", "PointerLeave", "MouseEnter", "MouseLeave", "StartMouseMove", "MouseMove", "EndMouseMove", "LeftButtonPress", "LeftButtonRelease", "MiddleButtonPress", "MiddleButtonRelease", "RightButtonPress", "RightButtonRelease", "KeyPress", "KeyDown", "KeyUp", "StartMouseWheel", "MouseWheel", "EndMouseWheel", "StartPinch", "Pinch", "EndPinch", "StartPan", "Pan", "EndPan", "StartRotate", "Rotate", "EndRotate", "Button3D", "Move3D", "StartPointerLock", "EndPointerLock", "StartInteraction", "Interaction", "EndInteraction", "AnimationFrameRateUpdate"];
+        Je = ["StartAnimation", "Animation", "EndAnimation", "PointerEnter", "PointerLeave", "MouseEnter", "MouseLeave", "StartMouseMove", "MouseMove", "EndMouseMove", "LeftButtonPress", "LeftButtonRelease", "MiddleButtonPress", "MiddleButtonRelease", "RightButtonPress", "RightButtonRelease", "KeyPress", "KeyDown", "KeyUp", "StartMouseWheel", "MouseWheel", "EndMouseWheel", "StartPinch", "Pinch", "EndPinch", "StartPan", "Pan", "EndPan", "StartRotate", "Rotate", "EndRotate", "Button3D", "Move3D", "StartPointerLock", "EndPointerLock", "StartInteraction", "Interaction", "EndInteraction", "AnimationFrameRateUpdate"];
 
-    function he(e) {
+    function le(e) {
         e.cancelable && e.preventDefault()
     }
 
-    function Re(e) {
+    function Me(e) {
         var t = Object.create(null);
         return e.forEach(function(r) {
             var n = r.pointerId,
-                i = r.position;
-            t[n] = i
+                a = r.position;
+            t[n] = a
         }), t
     }
 
-    function Po(e, t) {
+    function oa(e, t) {
         t.classHierarchy.push("vtkRenderWindowInteractor");
         var r = new Set,
             n = new Map,
-            i = 1;
+            a = 1;
         e.start = function() {
             !t.initialized && (e.initialize(), !t.initialized) || e.startEventLoop()
         }, e.setRenderWindow = function(o) {
-            ke("you want to call setView(view) instead of setRenderWindow on a vtk.js interactor")
+            Re("you want to call setView(view) instead of setRenderWindow on a vtk.js interactor")
         }, e.setInteractorStyle = function(o) {
             t.interactorStyle !== o && (t.interactorStyle != null && t.interactorStyle.setInteractor(null), t.interactorStyle = o, t.interactorStyle != null && t.interactorStyle.getInteractor() !== e && t.interactorStyle.setInteractor(e))
         }, e.initialize = function() {
             t.initialized = !0, e.enable(), e.render()
         }, e.enable = function() {
             return e.setEnabled(!0)
         }, e.disable = function() {
             return e.setEnabled(!1)
         }, e.startEventLoop = function() {
             return Te("empty event loop")
         };
 
-        function h(o, f) {
+        function l(o, f) {
             t._forcedRenderer || (t.currentRenderer = e.findPokedRenderer(o, f))
         }
         e.getCurrentRenderer = function() {
-            return t.currentRenderer || h(0, 0), t.currentRenderer
+            return t.currentRenderer || l(0, 0), t.currentRenderer
         };
 
         function v(o) {
             var f = t._view.getCanvas(),
                 y = f.getBoundingClientRect(),
-                g = f.width / y.width,
+                d = f.width / y.width,
                 m = f.height / y.height,
                 w = {
-                    x: g * (o.clientX - y.left),
+                    x: d * (o.clientX - y.left),
                     y: m * (y.height - o.clientY + y.top),
                     z: 0
                 };
-            return (n.size <= 1 || !t.currentRenderer) && h(w.x, w.y), w
+            return (n.size <= 1 || !t.currentRenderer) && l(w.x, w.y), w
         }
         var u = t._getScreenEventPositionFor || v;
 
-        function a(o) {
+        function i(o) {
             return {
                 controlKey: o.ctrlKey,
                 altKey: o.altKey,
                 shiftKey: o.shiftKey
             }
         }
 
         function s(o) {
-            var f = a(o),
+            var f = i(o),
                 y = R({
                     key: o.key,
                     keyCode: o.charCode
                 }, f);
             return y
         }
 
         function c(o) {
             return o.pointerType || ""
         }
         e.bindEvents = function(o) {
-            t.container = o, o.addEventListener("contextmenu", he), o.addEventListener("wheel", e.handleWheel), o.addEventListener("DOMMouseScroll", e.handleWheel), o.addEventListener("pointerenter", e.handlePointerEnter), o.addEventListener("pointerleave", e.handlePointerLeave), o.addEventListener("pointermove", e.handlePointerMove, {
+            t.container = o, o.addEventListener("contextmenu", le), o.addEventListener("wheel", e.handleWheel), o.addEventListener("DOMMouseScroll", e.handleWheel), o.addEventListener("pointerenter", e.handlePointerEnter), o.addEventListener("pointerleave", e.handlePointerLeave), o.addEventListener("pointermove", e.handlePointerMove, {
                 passive: !1
             }), o.addEventListener("pointerdown", e.handlePointerDown, {
                 passive: !1
             }), o.addEventListener("pointerup", e.handlePointerUp), o.addEventListener("pointercancel", e.handlePointerCancel), document.addEventListener("keypress", e.handleKeyPress), document.addEventListener("keydown", e.handleKeyDown), document.addEventListener("keyup", e.handleKeyUp), document.addEventListener("pointerlockchange", e.handlePointerLockChange), o.style.touchAction = "none", o.style.userSelect = "none", o.style.webkitTapHighlightColor = "rgba(0,0,0,0)"
         }, e.unbindEvents = function() {
             var o = t.container;
-            o.removeEventListener("contextmenu", he), o.removeEventListener("wheel", e.handleWheel), o.removeEventListener("DOMMouseScroll", e.handleWheel), o.removeEventListener("pointerenter", e.handlePointerEnter), o.removeEventListener("pointerleave", e.handlePointerLeave), o.removeEventListener("pointermove", e.handlePointerMove, {
+            o.removeEventListener("contextmenu", le), o.removeEventListener("wheel", e.handleWheel), o.removeEventListener("DOMMouseScroll", e.handleWheel), o.removeEventListener("pointerenter", e.handlePointerEnter), o.removeEventListener("pointerleave", e.handlePointerLeave), o.removeEventListener("pointermove", e.handlePointerMove, {
                 passive: !1
             }), o.removeEventListener("pointerdown", e.handlePointerDown, {
                 passive: !1
             }), o.removeEventListener("pointerup", e.handlePointerUp), o.removeEventListener("pointercancel", e.handlePointerCancel), document.removeEventListener("keypress", e.handleKeyPress), document.removeEventListener("keydown", e.handleKeyDown), document.removeEventListener("keyup", e.handleKeyUp), document.removeEventListener("pointerlockchange", e.handlePointerLockChange), t.container = null, n.clear()
         }, e.handleKeyPress = function(o) {
             var f = s(o);
             e.keyPressEvent(f)
         }, e.handleKeyDown = function(o) {
             var f = s(o);
             e.keyDownEvent(f)
         }, e.handleKeyUp = function(o) {
             var f = s(o);
             e.keyUpEvent(f)
         }, e.handlePointerEnter = function(o) {
-            var f = R(R({}, a(o)), {}, {
+            var f = R(R({}, i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
             e.pointerEnterEvent(f), f.deviceType === "mouse" && e.mouseEnterEvent(f)
         }, e.handlePointerLeave = function(o) {
-            var f = R(R({}, a(o)), {}, {
+            var f = R(R({}, i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
             e.pointerLeaveEvent(f), f.deviceType === "mouse" && e.mouseLeaveEvent(f)
         }, e.handlePointerDown = function(o) {
-            if (!(o.button > 2 || e.isPointerLocked())) switch (t.preventDefaultOnPointerDown && he(o), o.target.hasPointerCapture(o.pointerId) && o.target.releasePointerCapture(o.pointerId), t.container.setPointerCapture(o.pointerId), n.has(o.pointerId) && Te("[RenderWindowInteractor] duplicate pointerId detected"), n.set(o.pointerId, {
+            if (!(o.button > 2 || e.isPointerLocked())) switch (t.preventDefaultOnPointerDown && le(o), o.target.hasPointerCapture(o.pointerId) && o.target.releasePointerCapture(o.pointerId), t.container.setPointerCapture(o.pointerId), n.has(o.pointerId) && Te("[RenderWindowInteractor] duplicate pointerId detected"), n.set(o.pointerId, {
                     pointerId: o.pointerId,
                     position: u(o)
                 }), o.pointerType) {
                 case "pen":
                 case "touch":
                     e.handleTouchStart(o);
                     break;
                 case "mouse":
                 default:
                     e.handleMouseDown(o);
                     break
             }
         }, e.handlePointerUp = function(o) {
-            if (n.has(o.pointerId)) switch (t.preventDefaultOnPointerUp && he(o), n.delete(o.pointerId), t.container.releasePointerCapture(o.pointerId), o.pointerType) {
+            if (n.has(o.pointerId)) switch (t.preventDefaultOnPointerUp && le(o), n.delete(o.pointerId), t.container.releasePointerCapture(o.pointerId), o.pointerType) {
                 case "pen":
                 case "touch":
                     e.handleTouchEnd(o);
                     break;
                 case "mouse":
                 default:
                     e.handleMouseUp(o);
@@ -3005,49 +3004,49 @@
                     break;
                 case "mouse":
                 default:
                     e.handleMouseMove(o);
                     break
             }
         }, e.handleMouseDown = function(o) {
-            var f = R(R({}, a(o)), {}, {
+            var f = R(R({}, i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
             switch (o.button) {
                 case 0:
                     e.leftButtonPressEvent(f);
                     break;
                 case 1:
                     e.middleButtonPressEvent(f);
                     break;
                 case 2:
                     e.rightButtonPressEvent(f);
                     break;
                 default:
-                    ke("Unknown mouse button pressed: ".concat(o.button));
+                    Re("Unknown mouse button pressed: ".concat(o.button));
                     break
             }
         }, e.requestPointerLock = function() {
             t.container && t.container.requestPointerLock()
         }, e.exitPointerLock = function() {
             var o, f;
             return (o = (f = document).exitPointerLock) === null || o === void 0 ? void 0 : o.call(f)
         }, e.isPointerLocked = function() {
             return !!t.container && document.pointerLockElement === t.container
         }, e.handlePointerLockChange = function() {
             e.isPointerLocked() ? e.startPointerLockEvent() : e.endPointerLockEvent()
         };
 
-        function l() {
+        function h() {
             t._view && t.enabled && t.enableRender && (t.inRender = !0, t._view.traverseAllPasses(), t.inRender = !1), e.invokeRenderEvent()
         }
         e.requestAnimation = function(o) {
             if (o === void 0) {
-                ke("undefined requester, can not start animating");
+                Re("undefined requester, can not start animating");
                 return
             }
             if (r.has(o)) {
                 Te("requester is already registered for animating");
                 return
             }
             r.add(o), !t.animationRequest && r.size === 1 && !t.xrAnimation && (t._animationStartTime = Date.now(), t._animationFrameCount = 0, t.animationRequest = requestAnimationFrame(e.handleAnimation), e.startAnimationEvent())
@@ -3067,174 +3066,174 @@
             }
             r.delete(o), t.animationRequest && r.size === 0 && Date.now() > t._animationExtendedEnd && (cancelAnimationFrame(t.animationRequest), t.animationRequest = null, e.endAnimationEvent(), e.render())
         }, e.switchToXRAnimation = function() {
             t.animationRequest && (cancelAnimationFrame(t.animationRequest), t.animationRequest = null), t.xrAnimation = !0
         }, e.returnFromXRAnimation = function() {
             t.xrAnimation = !1, r.size !== 0 && (t.recentAnimationFrameRate = 10, t.animationRequest = requestAnimationFrame(e.handleAnimation))
         }, e.updateXRGamepads = function(o, f, y) {
-            o.inputSources.forEach(function(g) {
-                var m = g.gripSpace == null ? null : f.getPose(g.gripSpace, y),
-                    w = g.gamepad,
-                    T = g.handedness;
+            o.inputSources.forEach(function(d) {
+                var m = d.gripSpace == null ? null : f.getPose(d.gripSpace, y),
+                    w = d.gamepad,
+                    k = d.handedness;
                 if (w) {
                     w.index in t.lastGamepadValues || (t.lastGamepadValues[w.index] = {
                         left: {
                             buttons: {}
                         },
                         right: {
                             buttons: {}
                         },
                         none: {
                             buttons: {}
                         }
                     });
-                    for (var d = 0; d < w.buttons.length; ++d) d in t.lastGamepadValues[w.index][T].buttons || (t.lastGamepadValues[w.index][T].buttons[d] = !1), t.lastGamepadValues[w.index][T].buttons[d] !== w.buttons[d].pressed && m != null && (e.button3DEvent({
+                    for (var g = 0; g < w.buttons.length; ++g) g in t.lastGamepadValues[w.index][k].buttons || (t.lastGamepadValues[w.index][k].buttons[g] = !1), t.lastGamepadValues[w.index][k].buttons[g] !== w.buttons[g].pressed && m != null && (e.button3DEvent({
                         gamepad: w,
                         position: m.transform.position,
                         orientation: m.transform.orientation,
-                        pressed: w.buttons[d].pressed,
-                        device: g.handedness === "left" ? xe.LeftController : xe.RightController,
-                        input: Qe[w.mapping] && Qe[w.mapping][d] ? Qe[w.mapping][d] : A.Trigger
-                    }), t.lastGamepadValues[w.index][T].buttons[d] = w.buttons[d].pressed), t.lastGamepadValues[w.index][T].buttons[d] && m != null && e.move3DEvent({
+                        pressed: w.buttons[g].pressed,
+                        device: d.handedness === "left" ? ke.LeftController : ke.RightController,
+                        input: Ae[w.mapping] && Ae[w.mapping][g] ? Ae[w.mapping][g] : A.Trigger
+                    }), t.lastGamepadValues[w.index][k].buttons[g] = w.buttons[g].pressed), t.lastGamepadValues[w.index][k].buttons[g] && m != null && e.move3DEvent({
                         gamepad: w,
                         position: m.transform.position,
                         orientation: m.transform.orientation,
-                        device: g.handedness === "left" ? xe.LeftController : xe.RightController
+                        device: d.handedness === "left" ? ke.LeftController : ke.RightController
                     })
                 }
             })
         }, e.handleMouseMove = function(o) {
-            var f = R(R({}, a(o)), {}, {
+            var f = R(R({}, i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
             t.moveTimeoutID === 0 ? e.startMouseMoveEvent(f) : (e.mouseMoveEvent(f), clearTimeout(t.moveTimeoutID)), t.moveTimeoutID = setTimeout(function() {
                 e.endMouseMoveEvent(), t.moveTimeoutID = 0
             }, 200)
         }, e.handleAnimation = function() {
             var o = Date.now();
-            t._animationFrameCount++, o - t._animationStartTime > 1e3 && t._animationFrameCount > 1 && (t.recentAnimationFrameRate = 1e3 * (t._animationFrameCount - 1) / (o - t._animationStartTime), t.lastFrameTime = 1 / t.recentAnimationFrameRate, e.animationFrameRateUpdateEvent(), t._animationStartTime = o, t._animationFrameCount = 1), e.animationEvent(), l(), r.size > 0 || Date.now() < t._animationExtendedEnd ? t.animationRequest = requestAnimationFrame(e.handleAnimation) : (cancelAnimationFrame(t.animationRequest), t.animationRequest = null, e.endAnimationEvent(), e.render())
+            t._animationFrameCount++, o - t._animationStartTime > 1e3 && t._animationFrameCount > 1 && (t.recentAnimationFrameRate = 1e3 * (t._animationFrameCount - 1) / (o - t._animationStartTime), t.lastFrameTime = 1 / t.recentAnimationFrameRate, e.animationFrameRateUpdateEvent(), t._animationStartTime = o, t._animationFrameCount = 1), e.animationEvent(), h(), r.size > 0 || Date.now() < t._animationExtendedEnd ? t.animationRequest = requestAnimationFrame(e.handleAnimation) : (cancelAnimationFrame(t.animationRequest), t.animationRequest = null, e.endAnimationEvent(), e.render())
         }, e.handleWheel = function(o) {
-            he(o);
-            var f = R(R(R({}, Ko(o)), a(o)), {}, {
+            le(o);
+            var f = R(R(R({}, na(o)), i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
-            t.wheelTimeoutID === 0 && (Math.abs(f.spinY) >= .3 ? i = Math.abs(f.spinY) : i = 1), f.spinY /= i, t.wheelTimeoutID === 0 ? (e.startMouseWheelEvent(f), e.mouseWheelEvent(f)) : (e.mouseWheelEvent(f), clearTimeout(t.wheelTimeoutID)), t.mouseScrollDebounceByPass ? (e.extendAnimation(600), e.endMouseWheelEvent(), t.wheelTimeoutID = 0) : t.wheelTimeoutID = setTimeout(function() {
+            t.wheelTimeoutID === 0 && (Math.abs(f.spinY) >= .3 ? a = Math.abs(f.spinY) : a = 1), f.spinY /= a, t.wheelTimeoutID === 0 ? (e.startMouseWheelEvent(f), e.mouseWheelEvent(f)) : (e.mouseWheelEvent(f), clearTimeout(t.wheelTimeoutID)), t.mouseScrollDebounceByPass ? (e.extendAnimation(600), e.endMouseWheelEvent(), t.wheelTimeoutID = 0) : t.wheelTimeoutID = setTimeout(function() {
                 e.extendAnimation(600), e.endMouseWheelEvent(), t.wheelTimeoutID = 0
             }, 200)
         }, e.handleMouseUp = function(o) {
-            var f = R(R({}, a(o)), {}, {
+            var f = R(R({}, i(o)), {}, {
                 position: u(o),
                 deviceType: c(o)
             });
             switch (o.button) {
                 case 0:
                     e.leftButtonReleaseEvent(f);
                     break;
                 case 1:
                     e.middleButtonReleaseEvent(f);
                     break;
                 case 2:
                     e.rightButtonReleaseEvent(f);
                     break;
                 default:
-                    ke("Unknown mouse button released: ".concat(o.button));
+                    Re("Unknown mouse button released: ".concat(o.button));
                     break
             }
         }, e.handleTouchStart = function(o) {
             var f = se(n.values());
             if (t.recognizeGestures && f.length > 1) {
-                var y = Re(n);
+                var y = Me(n);
                 if (f.length === 2) {
-                    var g = R(R({}, a(oe)), {}, {
+                    var d = R(R({}, i(oe)), {}, {
                         position: f[0].position,
                         deviceType: c(o)
                     });
-                    e.leftButtonReleaseEvent(g)
+                    e.leftButtonReleaseEvent(d)
                 }
                 e.recognizeGesture("TouchStart", y)
             } else if (f.length === 1) {
-                var m = R(R({}, a(oe)), {}, {
+                var m = R(R({}, i(oe)), {}, {
                     position: u(o),
                     deviceType: c(o)
                 });
                 e.leftButtonPressEvent(m)
             }
         }, e.handleTouchMove = function(o) {
             var f = se(n.values());
             if (t.recognizeGestures && f.length > 1) {
-                var y = Re(n);
+                var y = Me(n);
                 e.recognizeGesture("TouchMove", y)
             } else if (f.length === 1) {
-                var g = R(R({}, a(oe)), {}, {
+                var d = R(R({}, i(oe)), {}, {
                     position: f[0].position,
                     deviceType: c(o)
                 });
-                e.mouseMoveEvent(g)
+                e.mouseMoveEvent(d)
             }
         }, e.handleTouchEnd = function(o) {
             var f = se(n.values());
             if (t.recognizeGestures)
                 if (f.length === 0) {
-                    var y = R(R({}, a(oe)), {}, {
+                    var y = R(R({}, i(oe)), {}, {
                         position: u(o),
                         deviceType: c(o)
                     });
                     e.leftButtonReleaseEvent(y)
                 } else if (f.length === 1) {
-                var g = Re(n);
-                e.recognizeGesture("TouchEnd", g);
-                var m = R(R({}, a(oe)), {}, {
+                var d = Me(n);
+                e.recognizeGesture("TouchEnd", d);
+                var m = R(R({}, i(oe)), {}, {
                     position: f[0].position,
                     deviceType: c(o)
                 });
                 e.leftButtonPressEvent(m)
             } else {
-                var w = Re(n);
+                var w = Me(n);
                 e.recognizeGesture("TouchMove", w)
             } else if (f.length === 1) {
-                var T = R(R({}, a(oe)), {}, {
+                var k = R(R({}, i(oe)), {}, {
                     position: f[0].position,
                     deviceType: c(o)
                 });
-                e.leftButtonReleaseEvent(T)
+                e.leftButtonReleaseEvent(k)
             }
         }, e.setView = function(o) {
             t._view !== o && (t._view = o, t._view.getRenderable().setInteractor(e), e.modified())
         }, e.getFirstRenderer = function() {
             var o, f, y;
             return (o = t._view) === null || o === void 0 || (f = o.getRenderable()) === null || f === void 0 || (y = f.getRenderersByReference()) === null || y === void 0 ? void 0 : y[0]
         }, e.findPokedRenderer = function() {
             var o, f, y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
-                g = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
+                d = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (!t._view) return null;
             var m = (o = t._view) === null || o === void 0 || (f = o.getRenderable()) === null || f === void 0 ? void 0 : f.getRenderers();
             if (!m || m.length === 0) return null;
             m.sort(function(O, b) {
                 return O.getLayer() - b.getLayer()
             });
-            for (var w = null, T = null, d = null, S = m.length; S--;) {
+            for (var w = null, k = null, g = null, S = m.length; S--;) {
                 var E = m[S];
-                if (t._view.isInViewport(y, g, E) && E.getInteractive()) {
-                    d = E;
+                if (t._view.isInViewport(y, d, E) && E.getInteractive()) {
+                    g = E;
                     break
                 }
-                w === null && E.getInteractive() && (w = E), T === null && t._view.isInViewport(y, g, E) && (T = E)
+                w === null && E.getInteractive() && (w = E), k === null && t._view.isInViewport(y, d, E) && (k = E)
             }
-            return d === null && (d = w), d === null && (d = T), d == null && (d = m[0]), d
+            return g === null && (g = w), g === null && (g = k), g == null && (g = m[0]), g
         }, e.render = function() {
-            !e.isAnimating() && !t.inRender && l()
-        }, Ie.forEach(function(o) {
+            !e.isAnimating() && !t.inRender && h()
+        }, Je.forEach(function(o) {
             var f = o.charAt(0).toLowerCase() + o.slice(1);
             e["".concat(f, "Event")] = function(y) {
                 if (t.enabled) {
-                    var g = e.getCurrentRenderer();
-                    if (!g) {
-                        qo(`
+                    var d = e.getCurrentRenderer();
+                    if (!d) {
+                        ra(`
           Can not forward events without a current renderer on the interactor.
         `);
                         return
                     }
                     var m = R({
                         type: o,
                         pokedRenderer: t.currentRenderer,
@@ -3242,57 +3241,57 @@
                     }, y);
                     e["invoke".concat(o)](m)
                 }
             }
         }), e.recognizeGesture = function(o, f) {
             if (!(Object.keys(f).length > 2)) {
                 if (t.startingEventPositions || (t.startingEventPositions = {}), o === "TouchStart") {
-                    Object.keys(f).forEach(function(ye) {
-                        t.startingEventPositions[ye] = f[ye]
+                    Object.keys(f).forEach(function(ve) {
+                        t.startingEventPositions[ve] = f[ve]
                     }), t.currentGesture = "Start";
                     return
                 }
                 if (o === "TouchEnd") {
                     t.currentGesture === "Pinch" && (e.render(), e.endPinchEvent()), t.currentGesture === "Rotate" && (e.render(), e.endRotateEvent()), t.currentGesture === "Pan" && (e.render(), e.endPanEvent()), t.currentGesture = "Start", t.startingEventPositions = {};
                     return
                 }
                 var y = 0,
-                    g = [],
+                    d = [],
                     m = [];
-                Object.keys(f).forEach(function(ye) {
-                    g[y] = f[ye], m[y] = t.startingEventPositions[ye], y++
+                Object.keys(f).forEach(function(ve) {
+                    d[y] = f[ve], m[y] = t.startingEventPositions[ve], y++
                 });
                 var w = Math.sqrt((m[0].x - m[1].x) * (m[0].x - m[1].x) + (m[0].y - m[1].y) * (m[0].y - m[1].y)),
-                    T = Math.sqrt((g[0].x - g[1].x) * (g[0].x - g[1].x) + (g[0].y - g[1].y) * (g[0].y - g[1].y)),
-                    d = Qt(Math.atan2(m[1].y - m[0].y, m[1].x - m[0].x)),
-                    S = Qt(Math.atan2(g[1].y - g[0].y, g[1].x - g[0].x)),
-                    E = S - d;
-                S = S + 180 >= 360 ? S - 180 : S + 180, d = d + 180 >= 360 ? d - 180 : d + 180, Math.abs(S - d) < Math.abs(E) && (E = S - d);
+                    k = Math.sqrt((d[0].x - d[1].x) * (d[0].x - d[1].x) + (d[0].y - d[1].y) * (d[0].y - d[1].y)),
+                    g = Qt(Math.atan2(m[1].y - m[0].y, m[1].x - m[0].x)),
+                    S = Qt(Math.atan2(d[1].y - d[0].y, d[1].x - d[0].x)),
+                    E = S - g;
+                S = S + 180 >= 360 ? S - 180 : S + 180, g = g + 180 >= 360 ? g - 180 : g + 180, Math.abs(S - g) < Math.abs(E) && (E = S - g);
                 var O = [];
-                if (O[0] = (g[0].x - m[0].x + g[1].x - m[1].x) / 2, O[1] = (g[0].y - m[0].y + g[1].y - m[1].y) / 2, o === "TouchMove")
+                if (O[0] = (d[0].x - m[0].x + d[1].x - m[1].x) / 2, O[1] = (d[0].y - m[0].y + d[1].y - m[1].y) / 2, o === "TouchMove")
                     if (t.currentGesture === "Start") {
                         var b = .01 * Math.sqrt(t.container.clientWidth * t.container.clientWidth + t.container.clientHeight * t.container.clientHeight);
                         b < 15 && (b = 15);
-                        var M = Math.abs(T - w),
-                            _ = T * 3.1415926 * Math.abs(E) / 360,
+                        var M = Math.abs(k - w),
+                            _ = k * 3.1415926 * Math.abs(E) / 360,
                             L = Math.sqrt(O[0] * O[0] + O[1] * O[1]);
                         if (M > b && M > _ && M > L) {
                             t.currentGesture = "Pinch";
-                            var $ = {
+                            var z = {
                                 scale: 1,
                                 touches: f
                             };
-                            e.startPinchEvent($)
+                            e.startPinchEvent(z)
                         } else if (_ > b && _ > L) {
                             t.currentGesture = "Rotate";
-                            var W = {
+                            var $ = {
                                 rotation: 0,
                                 touches: f
                             };
-                            e.startRotateEvent(W)
+                            e.startRotateEvent($)
                         } else if (L > b) {
                             t.currentGesture = "Pan";
                             var N = {
                                 translation: [0, 0],
                                 touches: f
                             };
                             e.startPanEvent(N)
@@ -3303,40 +3302,40 @@
                                 rotation: E,
                                 touches: f
                             };
                             e.rotateEvent(ae)
                         }
                         if (t.currentGesture === "Pinch") {
                             var J = {
-                                scale: T / w,
+                                scale: k / w,
                                 touches: f
                             };
                             e.pinchEvent(J)
                         }
                         if (t.currentGesture === "Pan") {
-                            var ma = {
+                            var Ca = {
                                 translation: O,
                                 touches: f
                             };
-                            e.panEvent(ma)
+                            e.panEvent(Ca)
                         }
                     }
             }
         }, e.handleVisibilityChange = function() {
             t._animationStartTime = Date.now(), t._animationFrameCount = 0
         }, e.setCurrentRenderer = function(o) {
             t._forcedRenderer = !!o, t.currentRenderer = o
         };
         var p = e.delete;
         e.delete = function() {
             for (; r.size;) e.cancelAnimation(r.values().next().value);
             typeof document.hidden < "u" && document.removeEventListener("visibilitychange", e.handleVisibilityChange), t.container && e.unbindEvents(), p()
         }, typeof document.hidden < "u" && document.addEventListener("visibilitychange", e.handleVisibilityChange, !1)
     }
-    var Xo = {
+    var aa = {
         renderWindow: null,
         interactorStyle: null,
         picker: null,
         pickingManager: null,
         initialized: !1,
         enabled: !1,
         enableRender: !0,
@@ -3356,31 +3355,31 @@
         preventDefaultOnPointerDown: !1,
         preventDefaultOnPointerUp: !1,
         mouseScrollDebounceByPass: !1
     };
 
     function en(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, Xo, r), k.obj(e, t), t._animationExtendedEnd = 0, k.event(e, t, "RenderEvent"), Ie.forEach(function(n) {
-            return k.event(e, t, n)
-        }), k.get(e, t, ["initialized", "container", "interactorStyle", "lastFrameTime", "recentAnimationFrameRate", "_view"]), k.setGet(e, t, ["lightFollowCamera", "enabled", "enableRender", "recognizeGestures", "desiredUpdateRate", "stillUpdateRate", "picker", "preventDefaultOnPointerDown", "preventDefaultOnPointerUp", "mouseScrollDebounceByPass"]), k.moveToProtected(e, t, ["view"]), Po(e, t)
+        Object.assign(t, aa, r), T.obj(e, t), t._animationExtendedEnd = 0, T.event(e, t, "RenderEvent"), Je.forEach(function(n) {
+            return T.event(e, t, n)
+        }), T.get(e, t, ["initialized", "container", "interactorStyle", "lastFrameTime", "recentAnimationFrameRate", "_view"]), T.setGet(e, t, ["lightFollowCamera", "enabled", "enableRender", "recognizeGestures", "desiredUpdateRate", "stillUpdateRate", "picker", "preventDefaultOnPointerDown", "preventDefaultOnPointerUp", "mouseScrollDebounceByPass"]), T.moveToProtected(e, t, ["view"]), oa(e, t)
     }
-    var Ho = k.newInstance(en, "vtkRenderWindowInteractor"),
+    var ia = T.newInstance(en, "vtkRenderWindowInteractor"),
         tn = R({
-            newInstance: Ho,
+            newInstance: ia,
             extend: en,
-            handledEvents: Ie
-        }, Ze);
+            handledEvents: Je
+        }, Ye);
 
     function nn(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
-            t && (n = n.filter(function(i) {
-                return Object.getOwnPropertyDescriptor(e, i).enumerable
+            t && (n = n.filter(function(a) {
+                return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
     function rn(e) {
         for (var t = 1; t < arguments.length; t++) {
@@ -3389,220 +3388,220 @@
                 V(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : nn(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var Yo = k.vtkErrorMacro,
-        Ao = k.VOID;
+    var sa = T.vtkErrorMacro,
+        ua = T.VOID;
 
-    function Jo(e, t, r, n) {
-        var i = e.getRenderWindow().getViews()[0];
-        return i.worldToDisplay(t, r, n, e)
+    function ca(e, t, r, n) {
+        var a = e.getRenderWindow().getViews()[0];
+        return a.worldToDisplay(t, r, n, e)
     }
 
-    function Zo(e, t, r, n) {
-        var i = e.getRenderWindow().getViews()[0];
-        return i.displayToWorld(t, r, n, e)
+    function fa(e, t, r, n) {
+        var a = e.getRenderWindow().getViews()[0];
+        return a.displayToWorld(t, r, n, e)
     }
-    var Qo = {
-        computeWorldToDisplay: Jo,
-        computeDisplayToWorld: Zo
+    var la = {
+        computeWorldToDisplay: ca,
+        computeDisplayToWorld: fa
     };
 
-    function Io(e, t) {
+    function ha(e, t) {
         t.classHierarchy.push("vtkInteractorObserver");
         var r = rn({}, e);
 
         function n() {
             for (; t.subscribedEvents.length;) t.subscribedEvents.pop().unsubscribe()
         }
 
-        function i() {
-            tn.handledEvents.forEach(function(h) {
-                e["handle".concat(h)] && t.subscribedEvents.push(t._interactor["on".concat(h)](function(v) {
-                    return t.processEvents ? e["handle".concat(h)](v) : Ao
+        function a() {
+            tn.handledEvents.forEach(function(l) {
+                e["handle".concat(l)] && t.subscribedEvents.push(t._interactor["on".concat(l)](function(v) {
+                    return t.processEvents ? e["handle".concat(l)](v) : ua
                 }, t.priority))
             })
         }
-        e.setInteractor = function(h) {
-            h !== t._interactor && (n(), t._interactor = h, h && t.enabled && i(), e.modified())
-        }, e.setEnabled = function(h) {
-            h !== t.enabled && (n(), h && (t._interactor ? i() : Yo(`
+        e.setInteractor = function(l) {
+            l !== t._interactor && (n(), t._interactor = l, l && t.enabled && a(), e.modified())
+        }, e.setEnabled = function(l) {
+            l !== t.enabled && (n(), l && (t._interactor ? a() : sa(`
           The interactor must be set before subscribing to events
-        `)), t.enabled = h, e.modified())
-        }, e.computeDisplayToWorld = function(h, v, u, a) {
-            return h ? t._interactor.getView().displayToWorld(v, u, a, h) : null
-        }, e.computeWorldToDisplay = function(h, v, u, a) {
-            return h ? t._interactor.getView().worldToDisplay(v, u, a, h) : null
-        }, e.setPriority = function(h) {
-            var v = r.setPriority(h);
-            v && t._interactor && (n(), i())
+        `)), t.enabled = l, e.modified())
+        }, e.computeDisplayToWorld = function(l, v, u, i) {
+            return l ? t._interactor.getView().displayToWorld(v, u, i, l) : null
+        }, e.computeWorldToDisplay = function(l, v, u, i) {
+            return l ? t._interactor.getView().worldToDisplay(v, u, i, l) : null
+        }, e.setPriority = function(l) {
+            var v = r.setPriority(l);
+            v && t._interactor && (n(), a())
         }
     }
-    var ea = {
+    var pa = {
         enabled: !0,
         priority: 0,
         processEvents: !0,
         subscribedEvents: []
     };
 
     function on(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, ea, r), k.obj(e, t), k.event(e, t, "InteractionEvent"), k.event(e, t, "StartInteractionEvent"), k.event(e, t, "EndInteractionEvent"), k.get(e, t, ["_interactor", "enabled"]), k.setGet(e, t, ["priority", "processEvents"]), k.moveToProtected(e, t, ["interactor"]), Io(e, t)
+        Object.assign(t, pa, r), T.obj(e, t), T.event(e, t, "InteractionEvent"), T.event(e, t, "StartInteractionEvent"), T.event(e, t, "EndInteractionEvent"), T.get(e, t, ["_interactor", "enabled"]), T.setGet(e, t, ["priority", "processEvents"]), T.moveToProtected(e, t, ["interactor"]), ha(e, t)
     }
-    var ta = k.newInstance(on, "vtkInteractorObserver"),
-        na = rn({
-            newInstance: ta,
+    var va = T.newInstance(on, "vtkInteractorObserver"),
+        ya = rn({
+            newInstance: va,
             extend: on
-        }, Qo),
-        ra = {
+        }, la),
+        ga = {
             IS_START: 0,
             IS_NONE: 0,
             IS_ROTATE: 1,
             IS_PAN: 2,
             IS_SPIN: 3,
             IS_DOLLY: 4,
             IS_CAMERA_POSE: 11,
             IS_WINDOW_LEVEL: 1024,
             IS_SLICE: 1025
         },
         an = {
-            States: ra
+            States: ga
         };
 
     function sn(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
-            t && (n = n.filter(function(i) {
-                return Object.getOwnPropertyDescriptor(e, i).enumerable
+            t && (n = n.filter(function(a) {
+                return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function oa(e) {
+    function da(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? sn(Object(r), !0).forEach(function(n) {
                 V(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : sn(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
     var G = an.States,
-        et = {
+        Ze = {
             Rotate: G.IS_ROTATE,
             Pan: G.IS_PAN,
             Spin: G.IS_SPIN,
             Dolly: G.IS_DOLLY,
             CameraPose: G.IS_CAMERA_POSE,
             WindowLevel: G.IS_WINDOW_LEVEL,
             Slice: G.IS_SLICE
         };
 
-    function aa(e, t) {
-        t.classHierarchy.push("vtkInteractorStyle"), Object.keys(et).forEach(function(r) {
-            k.event(e, t, "Start".concat(r, "Event")), e["start".concat(r)] = function() {
-                t.state === G.IS_NONE && (t.state = et[r], t._interactor.requestAnimation(e), e.invokeStartInteractionEvent({
+    function ma(e, t) {
+        t.classHierarchy.push("vtkInteractorStyle"), Object.keys(Ze).forEach(function(r) {
+            T.event(e, t, "Start".concat(r, "Event")), e["start".concat(r)] = function() {
+                t.state === G.IS_NONE && (t.state = Ze[r], t._interactor.requestAnimation(e), e.invokeStartInteractionEvent({
                     type: "StartInteractionEvent"
                 }), e["invokeStart".concat(r, "Event")]({
                     type: "Start".concat(r, "Event")
                 }))
-            }, k.event(e, t, "End".concat(r, "Event")), e["end".concat(r)] = function() {
-                t.state === et[r] && (t.state = G.IS_NONE, t._interactor.cancelAnimation(e), e.invokeEndInteractionEvent({
+            }, T.event(e, t, "End".concat(r, "Event")), e["end".concat(r)] = function() {
+                t.state === Ze[r] && (t.state = G.IS_NONE, t._interactor.cancelAnimation(e), e.invokeEndInteractionEvent({
                     type: "EndInteractionEvent"
                 }), e["invokeEnd".concat(r, "Event")]({
                     type: "End".concat(r, "Event")
                 }), t._interactor.render())
             }
         }), e.handleKeyPress = function(r) {
             var n = t._interactor,
-                i = null;
+                a = null;
             switch (r.key) {
                 case "r":
                 case "R":
                     r.pokedRenderer.resetCamera(), n.render();
                     break;
                 case "w":
                 case "W":
-                    i = r.pokedRenderer.getActors(), i.forEach(function(h) {
-                        var v = h.getProperty();
+                    a = r.pokedRenderer.getActors(), a.forEach(function(l) {
+                        var v = l.getProperty();
                         v.setRepresentationToWireframe && v.setRepresentationToWireframe()
                     }), n.render();
                     break;
                 case "s":
                 case "S":
-                    i = r.pokedRenderer.getActors(), i.forEach(function(h) {
-                        var v = h.getProperty();
+                    a = r.pokedRenderer.getActors(), a.forEach(function(l) {
+                        var v = l.getProperty();
                         v.setRepresentationToSurface && v.setRepresentationToSurface()
                     }), n.render();
                     break;
                 case "v":
                 case "V":
-                    i = r.pokedRenderer.getActors(), i.forEach(function(h) {
-                        var v = h.getProperty();
+                    a = r.pokedRenderer.getActors(), a.forEach(function(l) {
+                        var v = l.getProperty();
                         v.setRepresentationToPoints && v.setRepresentationToPoints()
                     }), n.render();
                     break
             }
         }
     }
-    var ia = {
+    var wa = {
         state: G.IS_NONE,
         handleObservers: 1,
         autoAdjustCameraClippingRange: 1
     };
 
     function un(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, ia, r), na.extend(e, t, r), aa(e, t)
+        Object.assign(t, wa, r), ya.extend(e, t, r), ma(e, t)
     }
-    var sa = k.newInstance(un, "vtkInteractorStyle"),
-        ua = oa({
-            newInstance: sa,
+    var Sa = T.newInstance(un, "vtkInteractorStyle"),
+        Ea = da({
+            newInstance: Sa,
             extend: un
         }, an);
-    const pe = {
+    const he = {
             type: "StartInteractionEvent"
         },
         cn = {
             type: "InteractionEvent"
         },
-        ve = {
+        pe = {
             type: "EndInteractionEvent"
         };
 
-    function ca(e, t) {
+    function Oa(e, t) {
         t.classHierarchy.push("vtkInteractorStyleRemoteMouse");
 
         function r(n) {
             const {
-                buttonLeft: i,
-                buttonMiddle: h,
+                buttonLeft: a,
+                buttonMiddle: l,
                 buttonRight: v
-            } = t, u = n.shiftKey ? 1 : 0, a = n.controlKey ? 1 : 0, s = n.altKey ? 1 : 0, c = n.metaKey ? 1 : 0, l = i || h || v ? "down" : "up";
+            } = t, u = n.shiftKey ? 1 : 0, i = n.controlKey ? 1 : 0, s = n.altKey ? 1 : 0, c = n.metaKey ? 1 : 0, h = a || l || v ? "down" : "up";
             let {
                 x: p,
                 y: o
             } = n.position;
             return {
-                action: l,
+                action: h,
                 x: p,
                 y: o,
-                buttonLeft: i,
-                buttonMiddle: h,
+                buttonLeft: a,
+                buttonMiddle: l,
                 buttonRight: v,
                 shiftKey: u,
                 altKey: s,
-                ctrlKey: a,
+                ctrlKey: i,
                 metaKey: c,
                 ...t.remoteEventAddOn
             }
         }
         e.handleLeftButtonPress = n => {
             t.previousPosition = n.position, t.buttonLeft = 1, e.onButtonDown(1, n)
         }, e.handleMiddleButtonPress = n => {
@@ -3611,127 +3610,127 @@
             t.previousPosition = n.position, t.buttonRight = 1, e.onButtonDown(3, n)
         }, e.handleLeftButtonRelease = n => {
             t.buttonLeft = 0, e.onButtonUp(1, n)
         }, e.handleMiddleButtonRelease = n => {
             t.buttonMiddle = 0, e.onButtonUp(2, n)
         }, e.handleRightButtonRelease = n => {
             t.buttonRight = 0, e.onButtonUp(3, n)
-        }, e.onButtonDown = (n, i) => {
-            e.invokeStartInteractionEvent(pe);
-            let h = "";
-            n == 1 ? h = "LeftButtonPress" : n == 2 ? h = "MiddleButtonPress" : n == 3 && (h = "RightButtonPress"), e.invokeRemoteMouseEvent({
-                type: h,
-                ...r(i)
-            })
-        }, e.onButtonUp = (n, i) => {
-            let h = "";
-            n == 1 ? h = "LeftButtonRelease" : n == 2 ? h = "MiddleButtonRelease" : n == 3 && (h = "RightButtonRelease"), e.invokeRemoteMouseEvent({
-                type: h,
-                ...r(i)
-            }), e.invokeEndInteractionEvent(ve)
+        }, e.onButtonDown = (n, a) => {
+            e.invokeStartInteractionEvent(he);
+            let l = "";
+            n == 1 ? l = "LeftButtonPress" : n == 2 ? l = "MiddleButtonPress" : n == 3 && (l = "RightButtonPress"), e.invokeRemoteMouseEvent({
+                type: l,
+                ...r(a)
+            })
+        }, e.onButtonUp = (n, a) => {
+            let l = "";
+            n == 1 ? l = "LeftButtonRelease" : n == 2 ? l = "MiddleButtonRelease" : n == 3 && (l = "RightButtonRelease"), e.invokeRemoteMouseEvent({
+                type: l,
+                ...r(a)
+            }), e.invokeEndInteractionEvent(pe)
         }, e.handleStartMouseWheel = n => {
-            e.invokeStartInteractionEvent(pe), e.invokeRemoteWheelEvent({
+            e.invokeStartInteractionEvent(he), e.invokeRemoteWheelEvent({
                 type: "StartMouseWheel",
                 ...r(n),
                 spinY: n.spinY
             })
         }, e.handleMouseWheel = n => {
-            let i = !0;
+            let a = !0;
             if (t.wheelThrottleDelay) {
-                const h = Date.now();
-                i = t.wheelThrottleDelay < h - t.wheelLastThrottleTime, i && (t.wheelLastThrottleTime = h)
+                const l = Date.now();
+                a = t.wheelThrottleDelay < l - t.wheelLastThrottleTime, a && (t.wheelLastThrottleTime = l)
             }
-            i && (e.invokeRemoteWheelEvent({
+            a && (e.invokeRemoteWheelEvent({
                 type: "MouseWheel",
                 ...r(n),
                 spinY: n.spinY
             }), e.invokeInteractionEvent(cn))
         }, e.handleEndMouseWheel = () => {
             e.invokeRemoteWheelEvent({
                 type: "EndMouseWheel",
                 ...t.remoteEventAddOn
-            }), e.invokeEndInteractionEvent(ve)
+            }), e.invokeEndInteractionEvent(pe)
         }, e.handleMouseMove = n => {
-            const i = Date.now();
-            t.throttleDelay < i - t.lastThrottleTime && (t.sendMouseMove || t.buttonLeft || t.buttonMiddle || t.buttonRight) && (t.lastThrottleTime = i, e.invokeRemoteMouseEvent({
+            const a = Date.now();
+            t.throttleDelay < a - t.lastThrottleTime && (t.sendMouseMove || t.buttonLeft || t.buttonMiddle || t.buttonRight) && (t.lastThrottleTime = a, e.invokeRemoteMouseEvent({
                 type: "MouseMove",
                 ...r(n)
             })), e.invokeInteractionEvent(cn)
         }, e.handleKeyPress = () => {}, e.handleStartPinch = n => {
             e.startDolly();
             const {
-                scale: i
+                scale: a
             } = n;
-            e.invokeStartInteractionEvent(pe), e.invokeRemoteGestureEvent({
+            e.invokeStartInteractionEvent(he), e.invokeRemoteGestureEvent({
                 type: "StartPinch",
-                scale: i,
+                scale: a,
                 ...t.remoteEventAddOn
             })
         }, e.handlePinch = n => {
             const {
-                scale: i
+                scale: a
             } = n;
             e.invokeRemoteGestureEvent({
                 type: "Pinch",
-                scale: i,
+                scale: a,
                 ...t.remoteEventAddOn
             })
         }, e.handleEndPinch = () => {
             e.endDolly(), e.invokeRemoteGestureEvent({
                 type: "EndPinch",
                 ...t.remoteEventAddOn
-            }), e.invokeEndInteractionEvent(ve)
+            }), e.invokeEndInteractionEvent(pe)
         }, e.handleStartRotate = n => {
             e.startRotate();
             const {
-                rotation: i
+                rotation: a
             } = n;
-            e.invokeStartInteractionEvent(pe), e.invokeRemoteGestureEvent({
+            e.invokeStartInteractionEvent(he), e.invokeRemoteGestureEvent({
                 type: "StartRotate",
-                rotation: i,
+                rotation: a,
                 ...t.remoteEventAddOn
             })
         }, e.handleRotate = n => {
             const {
-                rotation: i
+                rotation: a
             } = n;
             e.invokeRemoteGestureEvent({
                 type: "Rotate",
-                rotation: i,
+                rotation: a,
                 ...t.remoteEventAddOn
             })
         }, e.handleEndRotate = () => {
             e.endRotate(), e.invokeRemoteGestureEvent({
                 type: "EndRotate",
                 ...t.remoteEventAddOn
-            }), e.invokeEndInteractionEvent(ve)
+            }), e.invokeEndInteractionEvent(pe)
         }, e.handleStartPan = n => {
             e.startPan();
             const {
-                translation: i
+                translation: a
             } = n;
-            e.invokeStartInteractionEvent(pe), e.invokeRemoteGestureEvent({
+            e.invokeStartInteractionEvent(he), e.invokeRemoteGestureEvent({
                 type: "StartPan",
-                translation: i,
+                translation: a,
                 ...t.remoteEventAddOn
             })
         }, e.handlePan = n => {
             const {
-                translation: i
+                translation: a
             } = n;
             e.invokeRemoteGestureEvent({
                 type: "Pan",
-                translation: i,
+                translation: a,
                 ...t.remoteEventAddOn
             })
         }, e.handleEndPan = () => {
             e.endPan(), e.invokeRemoteGestureEvent({
                 type: "EndPan",
                 ...t.remoteEventAddOn
-            }), e.invokeEndInteractionEvent(ve)
+            }), e.invokeEndInteractionEvent(pe)
         }, e.handleKeyPress = n => {
             e.invokeRemoteKeyEvent({
                 type: "keyPress",
                 ...n
             })
         }, e.handleKeyDown = n => {
             e.invokeRemoteKeyEvent({
@@ -3741,45 +3740,45 @@
         }, e.handleKeyUp = n => {
             e.invokeRemoteKeyEvent({
                 type: "keyUp",
                 ...n
             })
         }
     }
-    const fa = {
+    const ba = {
         buttonLeft: 0,
         buttonMiddle: 0,
         buttonRight: 0,
         sendMouseMove: !1,
         throttleDelay: 33.3,
         lastThrottleTime: 0,
         wheelThrottleDelay: 0,
         wheelLastThrottleTime: 0
     };
 
     function fn(e, t, r = {}) {
-        Object.assign(t, fa, r), ua.extend(e, t, r), k.setGet(e, t, ["sendMouseMove", "remoteEventAddOn", "throttleDelay", "wheelThrottleDelay"]), k.event(e, t, "RemoteMouseEvent"), k.event(e, t, "RemoteWheelEvent"), k.event(e, t, "RemoteGestureEvent"), k.event(e, t, "RemoteKeyEvent"), ca(e, t)
+        Object.assign(t, ba, r), Ea.extend(e, t, r), T.setGet(e, t, ["sendMouseMove", "remoteEventAddOn", "throttleDelay", "wheelThrottleDelay"]), T.event(e, t, "RemoteMouseEvent"), T.event(e, t, "RemoteWheelEvent"), T.event(e, t, "RemoteGestureEvent"), T.event(e, t, "RemoteKeyEvent"), Oa(e, t)
     }
-    const la = {
-            newInstance: k.newInstance(fn, "vtkInteractorStyleRemoteMouse"),
+    const xa = {
+            newInstance: T.newInstance(fn, "vtkInteractorStyleRemoteMouse"),
             extend: fn
         },
         {
-            inject: ha,
-            provide: pa,
+            inject: ka,
+            provide: Ta,
             ref: ln,
-            toRefs: va,
-            onMounted: ya,
-            onBeforeUnmount: da
+            toRefs: Ra,
+            onMounted: Ma,
+            onBeforeUnmount: Da
         } = window.Vue,
         hn = Promise.resolve(!0),
         pn = {
-            DisplayArea: Tn,
+            DisplayArea: kn,
             StatisticsDisplay: Mn,
-            ImageDisplayArea: tt,
+            ImageDisplayArea: Qe,
             RemoteControlledArea: {
                 props: {
                     name: {
                         type: String,
                         default: "default"
                     },
                     origin: {
@@ -3790,118 +3789,118 @@
                         type: String,
                         default: "image"
                     }
                 },
                 setup(e) {
                     const t = ln(null),
                         r = ln(hn),
-                        n = ha("trame");
-                    let i = !0,
-                        h = null,
+                        n = ka("trame");
+                    let a = !0,
+                        l = null,
                         v = 0,
                         u = [0, 0],
-                        a = {
+                        i = {
                             w: 10,
                             h: 10,
                             p: window.devicePixelRatio
                         },
                         s = !0,
                         c = hn,
-                        l = 0;
+                        h = 0;
 
-                    function p(d) {
-                        return d.preventDefault(), {
-                            x: d.clientX - u[0],
-                            y: a.h - d.clientY + u[1],
+                    function p(g) {
+                        return g.preventDefault(), {
+                            x: g.clientX - u[0],
+                            y: i.h - g.clientY + u[1],
                             z: 0
                         }
                     }
                     const o = tn.newInstance({
                             _getScreenEventPositionFor: p,
                             currentRenderer: 1
                         }),
-                        f = la.newInstance();
-                    o.setInteractorStyle(f), f.onRemoteMouseEvent(d => {
+                        f = xa.newInstance();
+                    o.setInteractorStyle(f), f.onRemoteMouseEvent(g => {
                         y(Object.assign({
-                            w: a.w,
-                            h: a.h
-                        }, d))
-                    }), f.onRemoteWheelEvent(d => {
+                            w: i.w,
+                            h: i.h
+                        }, g))
+                    }), f.onRemoteWheelEvent(g => {
                         y(Object.assign({
-                            w: a.w,
-                            h: a.h
-                        }, d))
-                    }), f.onRemoteGestureEvent(d => {
+                            w: i.w,
+                            h: i.h
+                        }, g))
+                    }), f.onRemoteGestureEvent(g => {
                         y(Object.assign({
-                            w: a.w,
-                            h: a.h
-                        }, d))
-                    }), f.onRemoteKeyEvent(d => {
+                            w: i.w,
+                            h: i.h
+                        }, g))
+                    }), f.onRemoteKeyEvent(g => {
                         y(Object.assign({
-                            w: a.w,
-                            h: a.h
-                        }, d))
-                    }), f.onStartInteractionEvent(d => {
-                        y(d)
-                    }), f.onEndInteractionEvent(d => {
-                        y(d)
+                            w: i.w,
+                            h: i.h
+                        }, g))
+                    }), f.onStartInteractionEvent(g => {
+                        y(g)
+                    }), f.onEndInteractionEvent(g => {
+                        y(g)
                     });
 
-                    function y(d) {
-                        n && (i ? (i = !1, h = d, r.value = n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, h]), c.finally(g)) : h.type !== d.type && (v = 0, n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, h]), n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, d]), h = d))
+                    function y(g) {
+                        n && (a ? (a = !1, l = g, r.value = n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, l]), c.finally(d)) : l.type !== g.type && (v = 0, n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, l]), n.client.getConnection().getSession().call("trame.rca.event", [e.name, e.origin, g]), l = g))
                     }
 
-                    function g() {
-                        i = !0, v && (v = 0, y(h))
+                    function d() {
+                        a = !0, v && (v = 0, y(l))
                     }
 
                     function m() {
-                        s = !0, l && (l = 0, T())
+                        s = !0, h && (h = 0, k())
                     }
                     const w = new ResizeObserver(() => {
                         if (!t.value) return;
-                        const d = t.value.getBoundingClientRect(),
+                        const g = t.value.getBoundingClientRect(),
                             {
                                 top: S,
                                 left: E
-                            } = d;
-                        a.w = d.width, a.h = d.height, a.p = window.devicePixelRatio, u = [E, S], T()
+                            } = g;
+                        i.w = g.width, i.h = g.height, i.p = window.devicePixelRatio, u = [E, S], k()
                     });
 
-                    function T(d) {
-                        n && (s ? (s = !1, d ? c = n.client.getConnection().getSession().call("trame.rca.size", [e.name, e.origin, {
-                            ...a,
-                            ...d
-                        }]) : c = n.client.getConnection().getSession().call("trame.rca.size", [e.name, e.origin, a]), c.finally(m)) : l++)
+                    function k(g) {
+                        n && (s ? (s = !1, g ? c = n.client.getConnection().getSession().call("trame.rca.size", [e.name, e.origin, {
+                            ...i,
+                            ...g
+                        }]) : c = n.client.getConnection().getSession().call("trame.rca.size", [e.name, e.origin, i]), c.finally(m)) : h++)
                     }
-                    return pa("rcaPushSize", T), ya(() => {
+                    return Ta("rcaPushSize", k), Ma(() => {
                         w.observe(t.value), o.initialize(), o.bindEvents(t.value)
-                    }), da(() => {
+                    }), Da(() => {
                         w.unobserve(t.value), o.unbindEvents(t.value)
                     }), {
                         rootElem: t,
-                        ...va(e)
+                        ...Ra(e)
                     }
                 },
                 template: `
     <div ref="rootElem" style="margin: 0; padding: 0; position: relative; width: 100%; height: 100%;">
       <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
         <display-area :display="display" :name="name" :origin="origin" />
         <slot></slot>
       </div>
     </div>
   `
             },
-            MediaSourceDisplayArea: nt,
-            VideoDecoderDisplayArea: rt,
-            RawImageDisplayArea: ot
+            MediaSourceDisplayArea: Ie,
+            VideoDecoderDisplayArea: et,
+            RawImageDisplayArea: tt
         };
 
-    function ga(e) {
+    function ja(e) {
         Object.keys(pn).forEach(t => {
             e.component(t, pn[t])
         })
     }
-    Z.install = ga, Object.defineProperty(Z, Symbol.toStringTag, {
+    Z.install = ja, Object.defineProperty(Z, Symbol.toStringTag, {
         value: "Module"
     })
 });
```

### Comparing `trame-rca-0.4.1/trame_rca/protocol.py` & `trame-rca-0.4.2/trame_rca/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-rca-0.4.1/trame_rca/widgets/rca.py` & `trame-rca-0.4.2/trame_rca/widgets/rca.py`

 * *Files identical despite different names*

### Comparing `trame-rca-0.4.1/trame_rca.egg-info/PKG-INFO` & `trame-rca-0.4.2/trame_rca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-rca
-Version: 0.4.1
+Version: 0.4.2
 Summary: Remote Controlled Area widget for trame
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

