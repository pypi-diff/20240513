# Comparing `tmp/c4m_flexio-0.4.2.post2.tar.gz` & `tmp/c4m_flexio-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexio-0.4.2.post2.tar", last modified: Fri May  3 12:54:42 2024, max compression
+gzip compressed data, was "c4m_flexio-0.4.3.tar", last modified: Mon May 13 15:31:32 2024, max compression
```

## Comparing `c4m_flexio-0.4.2.post2.tar` & `c4m_flexio-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      992 2024-04-29 12:19:56.775201 c4m_flexio-0.4.2.post2/LICENSE.md
--rw-r--r--   0        0        0     2611 2024-05-03 11:33:55.090498 c4m_flexio-0.4.2.post2/README.md
--rw-r--r--   0        0        0      170 2024-04-29 09:44:39.473491 c4m_flexio-0.4.2.post2/c4m/flexio/__init__.py
--rw-r--r--   0        0        0    18938 2024-04-29 09:49:22.507719 c4m_flexio-0.4.2.post2/c4m/flexio/_helpers.py
--rw-r--r--   0        0        0   104325 2024-04-29 09:48:37.619999 c4m_flexio-0.4.2.post2/c4m/flexio/cell.py
--rw-r--r--   0        0        0   236159 2024-04-29 09:49:02.035846 c4m_flexio-0.4.2.post2/c4m/flexio/factory.py
--rw-r--r--   0        0        0    37990 2024-04-29 09:49:14.995766 c4m_flexio-0.4.2.post2/c4m/flexio/specification.py
--rw-r--r--   0        0        0      712 2024-05-03 12:54:42.446697 c4m_flexio-0.4.2.post2/pyproject.toml
--rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 c4m_flexio-0.4.2.post2/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:19:56.775201 c4m_flexio-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0     2813 2024-05-13 15:26:22.107061 c4m_flexio-0.4.3/README.md
+-rw-r--r--   0        0        0      170 2024-04-29 09:44:39.473491 c4m_flexio-0.4.3/c4m/flexio/__init__.py
+-rw-r--r--   0        0        0    18938 2024-04-29 09:49:22.507719 c4m_flexio-0.4.3/c4m/flexio/_helpers.py
+-rw-r--r--   0        0        0   106512 2024-05-13 14:44:22.044766 c4m_flexio-0.4.3/c4m/flexio/cell.py
+-rw-r--r--   0        0        0   236164 2024-05-08 14:45:54.124023 c4m_flexio-0.4.3/c4m/flexio/factory.py
+-rw-r--r--   0        0        0    37990 2024-04-29 09:49:14.995766 c4m_flexio-0.4.3/c4m/flexio/specification.py
+-rw-r--r--   0        0        0      706 2024-05-13 15:31:32.425533 c4m_flexio-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 c4m_flexio-0.4.3/PKG-INFO
```

### Comparing `c4m_flexio-0.4.2.post2/LICENSE.md` & `c4m_flexio-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.2.post2/README.md` & `c4m_flexio-0.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
+  * Critical fix for IOPadVdd layout.
+  * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
   suport, prefix all cell names.
 * v0.4.1:
   Implement layout without the bond pad included and pin that connects to the bond located at the
   bottom of the cell. This also implements ESD using diodes between pad and iovdd/iovdd net.
   This was done during development of IO library for the IHP sg13g2 process.
```

### Comparing `c4m_flexio-0.4.2.post2/c4m/flexio/_helpers.py` & `c4m_flexio-0.4.3/c4m/flexio/_helpers.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.2.post2/c4m/flexio/cell.py` & `c4m_flexio-0.4.3/c4m/flexio/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1879,38 +1879,39 @@
         insts = ckt.instances
 
         metal = comp.metal
         metal1 = metal[1].prim
         metal1pin = metal1.pin
         metal2 = metal[2].prim
         metal2pin = metal2.pin
+        metal3 = metal[3].prim
         via1 = comp.vias[1]
         via2 = comp.vias[2]
 
         iovss_trackspec = self.track_specs["iovss"]
         iovdd_trackspec = self.track_specs["iovdd"]
 
         padm2_bounds = self.pad_bb(prim=metal2)
 
         # Place nclamp + connect to pad + pad guard ring
         l_nclamp = layouter.place(insts.nclamp, x=0.0, y=iovss_trackspec.bottom)
         for polygon in l_nclamp.filter_polygons(
-            net=nets.iovdd, mask=metal2pin.mask, split=True,
+            net=pad, mask=metal2pin.mask, split=True,
         ):
             bb = polygon.bounds
             shape = _geo.Rect.from_rect(
                 rect=bb,
                 top=max(bb.top, padm2_bounds.bottom),
                 bottom=min(bb.bottom, padm2_bounds.top),
             )
-            layouter.add_wire(wire=metal2, net=nets.iovdd, shape=shape)
+            layouter.add_wire(wire=metal2, net=pad, shape=shape)
 
             y = bb.top
             layouter.add_wire(
-                net=nets.iovdd, wire=via1, y=y,
+                net=pad, wire=via1, y=y,
                 bottom_left=shape.left, bottom_right=shape.right, bottom_enclosure="tall",
                 top_left=shape.left, top_right=shape.right, top_enclosure="tall",
             )
 
         # Draw guardring around pad and connect to iovdd track
         bottom = cast(_geo._Rectangular, l_nclamp.boundary).top
         top = iovdd_trackspec.bottom - comp.guardring_space
@@ -1939,33 +1940,85 @@
                 y=(
                     tech.on_grid(0.5*(nclamp_m1bb.top + iovdd_trackspec.bottom))
                     - _bb.center.y
                 ),
             )
         l_rcres = layouter.place(_l, origin=o)
 
-        # Connect supply of inv to iovdd track
+        # Connect supply of inv to track with same net as pad
         net = pad
         m1pinbb = l_rcinv.bounds(mask=metal1pin.mask, net=net, depth=1)
 
-        w = m1pinbb.width
-        _l = layouter.wire_layout(
-            net=net, wire=via1,
-            bottom_width=w, bottom_enclosure="tall",
-            top_width=w, top_enclosure="tall",
-        )
-        _m1bb = _l.bounds(mask=metal1.mask)
-        x = m1pinbb.center.x
-        y = m1pinbb.bottom - _m1bb.bottom
-        layouter.place(_l, x=x, y=y)
-        layouter.add_wire(
-            net=net, wire=via2, x=x, y=y,
-            bottom_width=w, bottom_enclosure="tall",
-            top_width=w, top_enclosure="tall",
-        )
+        if net == nets["iovdd"]:
+            w = m1pinbb.width
+            _l = layouter.wire_layout(
+                net=net, wire=via1,
+                bottom_width=w, bottom_enclosure="tall",
+                top_width=w, top_enclosure="tall",
+            )
+            _m1bb = _l.bounds(mask=metal1.mask)
+            x = m1pinbb.center.x
+            y = m1pinbb.bottom - _m1bb.bottom
+            layouter.place(_l, x=x, y=y)
+
+            layouter.add_wire(
+                net=net, wire=via2, x=x, y=y,
+                bottom_width=w, bottom_enclosure="tall",
+                top_width=w, top_enclosure="tall",
+            )
+        elif net == nets["vdd"]:
+            w = m1pinbb.width
+            _l = layouter.wire_layout(
+                net=net, wire=via1,
+                bottom_width=w, bottom_enclosure="tall",
+                top_width=w, top_enclosure="tall",
+            )
+            _m1bb = _l.bounds(mask=metal1.mask)
+            x = m1pinbb.center.x
+            y = m1pinbb.bottom - _m1bb.bottom
+            l = layouter.place(_l, x=x, y=y)
+            m2bb1 = l.bounds(mask=metal2.mask)
+
+            metal3spec = comp.metal[3]
+            trackseg = self._track_segments["vddvss"][1]
+            m3connect_bottom = trackseg.bottom + 0.5*metal3spec.tracksegment_space
+
+            _l = layouter.wire_layout(
+                net=net, wire=via2, rows=2,
+                bottom_width=w, bottom_enclosure="tall",
+                top_width=w, top_enclosure="tall",
+            )
+            _m3bb = _l.bounds(mask=metal3.mask)
+            # x = x
+            y = m3connect_bottom - _m3bb.bottom
+            l = layouter.place(_l, x=x, y=y)
+            m2bb2 = l.bounds(mask=metal2.mask)
+
+            w = m2bb1.width
+            max_pitch = self.tracksegment_maxpitch
+            # Take space from M3
+            space = comp.track_metalspecs[0].tracksegment_space
+            fingers = floor((w + space + _geo.epsilon)/max_pitch) + 1
+            pitch = tech.on_grid(w/fingers, mult=2, rounding="floor")
+            w_finger = pitch - space
+            bottom = m2bb1.bottom
+            top = m2bb2.top
+            for n in range(fingers):
+                if n < fingers - 1:
+                    left = m2bb1.left + n*pitch
+                    right = left + w_finger
+                else:
+                    right = m2bb1.right
+                    left = right - w_finger
+                shape = _geo.Rect(left=left, bottom=bottom, right=right, top=top)
+                layouter.add_wire(
+                    net=net, wire=metal2, shape=shape,
+                )
+        else: # pragma: no cover
+            raise NotImplementedError(f"net '{net.name} for RCClampInverter supply")
 
         # Connect res output to inv input
         net = nets.res_cap
         res_m1pinbb = l_rcres.bounds(mask=metal1pin.mask, net=net, depth=1)
         inv_m2pinbb = l_rcinv.bounds(mask=metal2pin.mask, net=net, depth=1)
 
         w = inv_m2pinbb.right - res_m1pinbb.left
```

### Comparing `c4m_flexio-0.4.2.post2/c4m/flexio/factory.py` & `c4m_flexio-0.4.3/c4m/flexio/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -5361,19 +5361,19 @@
         if frame.has_pad or (spec.invvdd_n_mosfet is None):
             frame.add_nclamp_inst(
                 ckt=ckt, n_trans=spec.clampcount, n_drive=0, pad=vdd,
             )
             frame.add_pclamp_inst(
                 ckt=ckt, n_trans=spec.clampcount, n_drive=0, pad=vdd,
             )
+
+            frame.add_dcdiodes_inst(ckt=ckt, pad=vdd)
         else:
             frame.add_rcclamp_insts(ckt=ckt, pad=vdd)
 
-        frame.add_dcdiodes_inst(ckt=ckt, pad=vdd)
-
     def _create_layout(self):
         fab = self.fab
         spec = fab.spec
         frame = fab.frame
         tech = self.tech
         comp = fab.computed
 
@@ -5415,15 +5415,15 @@
             )
 
             l_padconn = frame.connect_pad2track(
                 layouter=layouter, pad=nets.vdd, track="vdd",
                 pclamp_lay=l_pclamp, ndio_lay=l_ndio, pdio_lay=l_pdio,
             )
 
-            # connec DCDiodes
+            # connect DCDiodes
             frame.connect_dcdiodes(
                 layouter=layouter, pad=nets.vdd,
                 nclamp_lay = l_nclamp, pclamp_lay=l_pclamp,
                 ndio_lay=l_ndio, pdio_lay=l_pdio,
                 padconn_lay=l_padconn,
             )
         else:
```

### Comparing `c4m_flexio-0.4.2.post2/c4m/flexio/specification.py` & `c4m_flexio-0.4.3/c4m/flexio/specification.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.2.post2/pyproject.toml` & `c4m_flexio-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "PDKMaster>=0.10.2,<0.12.0",
     "c4m-flexcell~=0.4.2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.4.2.post2"
+version = "0.4.3"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `c4m_flexio-0.4.2.post2/PKG-INFO` & `c4m_flexio-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexio
-Version: 0.4.2.post2
+Version: 0.4.3
 Summary: PDKMaster based scalable IO library
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster<0.12.0,>=0.10.2
 Requires-Dist: c4m-flexcell~=0.4.2
 Description-Content-Type: text/markdown
@@ -13,14 +13,17 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
+  * Critical fix for IOPadVdd layout.
+  * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
   suport, prefix all cell names.
 * v0.4.1:
   Implement layout without the bond pad included and pin that connects to the bond located at the
   bottom of the cell. This also implements ESD using diodes between pad and iovdd/iovdd net.
   This was done during development of IO library for the IHP sg13g2 process.
```

