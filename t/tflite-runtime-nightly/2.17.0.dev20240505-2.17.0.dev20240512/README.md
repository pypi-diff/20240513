# Comparing `tmp/tflite_runtime_nightly-2.17.0.dev20240505-cp39-cp39-manylinux_2_34_armv7l.whl.zip` & `tmp/tflite_runtime_nightly-2.17.0.dev20240512-cp39-cp39-manylinux_2_34_armv7l.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1918902 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 24-May-06 05:15 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  5250476 b- defN 24-May-06 05:20 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    39490 b- defN 24-May-06 05:15 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 24-May-06 05:15 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 24-May-06 05:15 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1439 b- defN 24-May-06 05:20 tflite_runtime_nightly-2.17.0.dev20240505.dist-info/METADATA
--rw-rw-r--  2.0 unx      112 b- defN 24-May-06 05:20 tflite_runtime_nightly-2.17.0.dev20240505.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 24-May-06 05:20 tflite_runtime_nightly-2.17.0.dev20240505.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 24-May-06 05:20 tflite_runtime_nightly-2.17.0.dev20240505.dist-info/RECORD
-9 files, 5296080 bytes uncompressed, 1917356 bytes compressed:  63.8%
+Zip file size: 1918900 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 24-May-13 05:18 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  5250476 b- defN 24-May-13 05:23 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    39490 b- defN 24-May-13 05:18 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 24-May-13 05:18 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 24-May-13 05:18 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1439 b- defN 24-May-13 05:23 tflite_runtime_nightly-2.17.0.dev20240512.dist-info/METADATA
+-rw-rw-r--  2.0 unx      112 b- defN 24-May-13 05:23 tflite_runtime_nightly-2.17.0.dev20240512.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 24-May-13 05:23 tflite_runtime_nightly-2.17.0.dev20240512.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 24-May-13 05:23 tflite_runtime_nightly-2.17.0.dev20240512.dist-info/RECORD
+9 files, 5296080 bytes uncompressed, 1917354 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240505.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.17.0.dev20240512.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240505.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.17.0.dev20240512.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240505.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.17.0.dev20240512.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.17.0.dev20240505.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.17.0.dev20240512.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.17.0dev20240505'
-__git_version__ = '0.6.0-163834-gf77a4bd9bed'
+__version__ = '2.17.0dev20240512'
+__git_version__ = '0.6.0-164240-g6c172a96279'
```

## tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -475462,15 +475462,15 @@
 	ldr	r3, [r3]
 	sub	r3, r3, #2
 	cmp	r3, #1
 	bls	27682c <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x60>
 	ldr	r1, [pc, #1048]	@ 276c14 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x448>
 	mov	r0, r4
 	ldr	r2, [pc, #1044]	@ 276c18 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x44c>
-	mov	r3, #216	@ 0xd8
+	mov	r3, #215	@ 0xd7
 	add	r1, pc, r1
 	ldr	r4, [r4, #20]
 	str	r1, [sp]
 	add	r2, pc, r2
 	ldr	r1, [pc, #1024]	@ 276c1c <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x450>
 	add	r1, pc, r1
 	blx	r4
@@ -475483,15 +475483,15 @@
 	beq	276898 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0xcc>
 	ldr	r6, [r2]
 	cmp	r6, #1
 	beq	2768a0 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0xd4>
 	ldr	r1, [pc, #976]	@ 276c20 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x454>
 	mov	r0, r4
 	ldr	r2, [pc, #972]	@ 276c24 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x458>
-	mov	r3, #217	@ 0xd9
+	mov	r3, #216	@ 0xd8
 	ldr	r5, [r4, #20]
 	add	r1, pc, r1
 	add	r2, pc, r2
 	str	r1, [sp, #4]
 	str	r2, [sp]
 	mov	r4, #1
 	ldr	r2, [pc, #944]	@ 276c28 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x45c>
@@ -475582,15 +475582,15 @@
 	mov	r0, r4
 	add	r1, sp, #20
 	bl	a69ac <tflite::ops::builtin::pad::ResizeOutputTensor(TfLiteContext*, tflite::ops::builtin::pad::PadContext*)@plt>
 	b	276824 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x58>
 	ldr	r1, [pc, #596]	@ 276c30 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x464>
 	mov	r0, r4
 	ldr	r2, [pc, #592]	@ 276c34 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x468>
-	mov	r3, #234	@ 0xea
+	mov	r3, #233	@ 0xe9
 	add	r1, pc, r1
 	ldr	r4, [r4, #20]
 	str	r1, [sp]
 	add	r2, pc, r2
 	ldr	r1, [pc, #572]	@ 276c38 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x46c>
 	add	r1, pc, r1
 	blx	r4
@@ -475600,15 +475600,15 @@
 	bl	ab668 <TfLiteTypeGetName@plt>
 	ldr	r3, [sp, #20]
 	mov	r6, r0
 	ldr	r0, [r3]
 	bl	ab668 <TfLiteTypeGetName@plt>
 	ldr	r1, [pc, #532]	@ 276c3c <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x470>
 	ldr	r2, [pc, #532]	@ 276c40 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x474>
-	mov	r3, #229	@ 0xe5
+	mov	r3, #228	@ 0xe4
 	add	r1, pc, r1
 	str	r1, [sp, #4]
 	add	r2, pc, r2
 	ldr	r1, [pc, #516]	@ 276c44 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x478>
 	str	r2, [sp]
 	ldr	r2, [pc, #512]	@ 276c48 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x47c>
 	add	r1, pc, r1
@@ -475688,15 +475688,15 @@
 	bl	ab668 <TfLiteTypeGetName@plt>
 	ldr	r3, [sp, #32]
 	mov	r6, r0
 	ldr	r0, [r3]
 	bl	ab668 <TfLiteTypeGetName@plt>
 	ldr	r1, [pc, #204]	@ 276c54 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x488>
 	ldr	r2, [pc, #204]	@ 276c58 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x48c>
-	mov	r3, #226	@ 0xe2
+	mov	r3, #225	@ 0xe1
 	add	r1, pc, r1
 	str	r1, [sp, #4]
 	add	r2, pc, r2
 	ldr	r1, [pc, #188]	@ 276c5c <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x490>
 	str	r2, [sp]
 	ldr	r2, [pc, #184]	@ 276c60 <tflite::ops::builtin::pad::Prepare(TfLiteContext*, TfLiteNode*)+0x494>
 	add	r1, pc, r1
@@ -478240,15 +478240,15 @@
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, r5
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, #0
 	add	sp, sp, #204	@ 0xcc
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	ldr	r1, [pc, #1584]	@ 279918 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x714>
-	movw	r3, #263	@ 0x107
+	movw	r3, #262	@ 0x106
 	str	r2, [sp, #8]
 	str	ip, [sp, #12]
 	add	r1, pc, r1
 	ldr	r5, [r0, #20]
 	ldr	r4, [pc, #1564]	@ 27991c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x718>
 	str	r1, [sp]
 	ldr	r2, [pc, #1560]	@ 279920 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x71c>
@@ -478263,15 +478263,15 @@
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	cmp	r2, #0
 	blt	279858 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x654>
 	cmp	r2, #255	@ 0xff
 	uxtble	r2, r2
 	ble	279250 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x4c>
 	ldr	r1, [pc, #1508]	@ 279928 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x724>
-	movw	r3, #257	@ 0x101
+	mov	r3, #256	@ 0x100
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #1496]	@ 27992c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x728>
 	str	r1, [sp]
 	ldr	r1, [pc, #1492]	@ 279930 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x72c>
 	add	r2, pc, r2
 	add	r1, pc, r1
@@ -478572,15 +478572,15 @@
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, #0
 	add	sp, sp, #204	@ 0xcc
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	vcvt.f64.f32	d17, s14
 	ldr	r1, [pc, #288]	@ 279934 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x730>
 	ldr	r2, [pc, #288]	@ 279938 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x734>
-	movw	r3, #265	@ 0x109
+	mov	r3, #264	@ 0x108
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	add	r2, pc, r2
 	str	r1, [sp, #4]
 	str	r2, [sp]
 	ldr	r1, [pc, #264]	@ 27993c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x738>
 	ldr	r2, [pc, #264]	@ 279940 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x73c>
@@ -478590,15 +478590,15 @@
 	vstr	d17, [sp, #16]
 	vstr	d16, [sp, #8]
 	blx	r4
 	mov	r0, #1
 	add	sp, sp, #204	@ 0xcc
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	ldr	r1, [pc, #228]	@ 279944 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x740>
-	mov	r3, #255	@ 0xff
+	mov	r3, #254	@ 0xfe
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #216]	@ 279948 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x744>
 	str	r1, [sp]
 	ldr	r1, [pc, #212]	@ 27994c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<unsigned char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x748>
 	add	r2, pc, r2
 	add	r1, pc, r1
@@ -479218,15 +479218,15 @@
 	mov	r0, r7
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, #0
 	add	sp, sp, #284	@ 0x11c
 	vpop	{d8-d9}
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	ldr	r1, [pc, #1856]	@ 27a94c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x824>
-	movw	r3, #263	@ 0x107
+	movw	r3, #262	@ 0x106
 	str	r2, [sp, #8]
 	str	ip, [sp, #12]
 	add	r1, pc, r1
 	ldr	r5, [r0, #20]
 	ldr	r4, [pc, #1836]	@ 27a950 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x828>
 	str	r1, [sp]
 	ldr	r2, [pc, #1832]	@ 27a954 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x82c>
@@ -479242,27 +479242,27 @@
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	cmn	r2, #128	@ 0x80
 	blt	27a294 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x16c>
 	cmp	r2, #127	@ 0x7f
 	sxtble	r2, r2
 	ble	27a178 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x50>
 	ldr	r1, [pc, #1776]	@ 27a95c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x834>
-	movw	r3, #257	@ 0x101
+	mov	r3, #256	@ 0x100
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #1764]	@ 27a960 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x838>
 	str	r1, [sp]
 	ldr	r1, [pc, #1760]	@ 27a964 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x83c>
 	add	r2, pc, r2
 	add	r1, pc, r1
 	blx	r4
 	mov	r0, #1
 	b	27a1f8 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0xd0>
 	ldr	r1, [pc, #1740]	@ 27a968 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x840>
-	mov	r3, #255	@ 0xff
+	mov	r3, #254	@ 0xfe
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #1728]	@ 27a96c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x844>
 	str	r1, [sp]
 	ldr	r1, [pc, #1724]	@ 27a970 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x848>
 	add	r2, pc, r2
 	add	r1, pc, r1
@@ -479648,15 +479648,15 @@
 	mov	r0, #0
 	add	sp, sp, #284	@ 0x11c
 	vpop	{d8-d9}
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	vcvt.f64.f32	d17, s14
 	ldr	r1, [pc, #180]	@ 27a974 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x84c>
 	ldr	r2, [pc, #180]	@ 27a978 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x850>
-	movw	r3, #265	@ 0x109
+	mov	r3, #264	@ 0x108
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	add	r2, pc, r2
 	str	r1, [sp, #4]
 	str	r2, [sp]
 	ldr	r1, [pc, #156]	@ 27a97c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x854>
 	ldr	r2, [pc, #156]	@ 27a980 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<signed char>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x858>
@@ -480317,15 +480317,15 @@
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, r7
 	bl	a6b98 <tflite::RuntimeShape::~RuntimeShape()@plt>
 	mov	r0, #0
 	add	sp, sp, #300	@ 0x12c
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	ldr	r1, [pc, #2160]	@ 27bb84 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x94c>
-	movw	r3, #263	@ 0x107
+	movw	r3, #262	@ 0x106
 	str	r2, [sp, #8]
 	str	ip, [sp, #12]
 	add	r1, pc, r1
 	ldr	r5, [r0, #20]
 	ldr	r4, [pc, #2140]	@ 27bb88 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x950>
 	str	r1, [sp]
 	ldr	r2, [pc, #2136]	@ 27bb8c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x954>
@@ -480340,27 +480340,27 @@
 	pop	{r4, r5, r6, r7, r8, r9, sl, fp, pc}
 	cmn	r2, #32768	@ 0x8000
 	blt	27b398 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x160>
 	cmp	r2, #32768	@ 0x8000
 	sxthlt	r2, r2
 	blt	27b284 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x4c>
 	ldr	r1, [pc, #2084]	@ 27bb94 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x95c>
-	movw	r3, #257	@ 0x101
+	mov	r3, #256	@ 0x100
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #2072]	@ 27bb98 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x960>
 	str	r1, [sp]
 	ldr	r1, [pc, #2068]	@ 27bb9c <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x964>
 	add	r2, pc, r2
 	add	r1, pc, r1
 	blx	r4
 	mov	r0, #1
 	b	27b304 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0xcc>
 	ldr	r1, [pc, #2048]	@ 27bba0 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x968>
-	mov	r3, #255	@ 0xff
+	mov	r3, #254	@ 0xfe
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	ldr	r2, [pc, #2036]	@ 27bba4 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x96c>
 	str	r1, [sp]
 	ldr	r1, [pc, #2032]	@ 27bba8 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x970>
 	add	r2, pc, r2
 	add	r1, pc, r1
@@ -480824,15 +480824,15 @@
 	bgt	27ba94 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x85c>
 	cmp	r0, r2
 	bgt	27ba10 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x7d8>
 	b	27b800 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x5c8>
 	vcvt.f64.f32	d17, s14
 	ldr	r1, [pc, #176]	@ 27bbac <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x974>
 	ldr	r2, [pc, #176]	@ 27bbb0 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x978>
-	movw	r3, #265	@ 0x109
+	mov	r3, #264	@ 0x108
 	ldr	r4, [r0, #20]
 	add	r1, pc, r1
 	add	r2, pc, r2
 	str	r1, [sp, #4]
 	str	r2, [sp]
 	ldr	r1, [pc, #152]	@ 27bbb4 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x97c>
 	ldr	r2, [pc, #152]	@ 27bbb8 <TfLiteStatus tflite::ops::builtin::pad::EvalInt<short>(TfLiteContext*, tflite::ops::builtin::pad::PadContext const&, tflite::PadParams const&)+0x980>
@@ -480973,15 +480973,15 @@
 	ldr	r1, [pc, #2976]	@ 27c8d0 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd14>
 	mov	r0, r4
 	strd	r2, [sp, #8]
 	mov	r4, #1
 	add	r1, pc, r1
 	ldr	ip, [pc, #2960]	@ 27c8d4 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd18>
 	str	r1, [sp]
-	movw	r3, #295	@ 0x127
+	movw	r3, #294	@ 0x126
 	ldr	r2, [pc, #2952]	@ 27c8d8 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd1c>
 	add	ip, pc, ip
 	ldr	r1, [pc, #2948]	@ 27c8dc <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd20>
 	str	ip, [sp, #4]
 	add	r2, pc, r2
 	str	r4, [sp, #16]
 	add	r1, pc, r1
@@ -480996,15 +480996,15 @@
 	beq	27befc <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0x340>
 	ldr	r3, [sp, #288]	@ 0x120
 	cmp	r3, #5
 	ble	27be94 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0x2d8>
 	ldr	r1, [pc, #2884]	@ 27c8e0 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd24>
 	mov	r0, r4
 	ldr	r2, [pc, #2880]	@ 27c8e4 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd28>
-	mov	r3, #304	@ 0x130
+	movw	r3, #303	@ 0x12f
 	ldr	r4, [r4, #20]
 	add	r1, pc, r1
 	str	r1, [sp]
 	add	r2, pc, r2
 	ldr	r1, [pc, #2860]	@ 27c8e8 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)0>(TfLiteContext*, TfLiteNode*)+0xd2c>
 	add	r1, pc, r1
 	blx	r4
@@ -483112,15 +483112,15 @@
 	ldr	r1, [pc, #2464]	@ 27e830 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb0c>
 	mov	r0, r4
 	strd	r2, [sp, #8]
 	mov	r4, #1
 	add	r1, pc, r1
 	ldr	ip, [pc, #2448]	@ 27e834 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb10>
 	str	r1, [sp]
-	movw	r3, #295	@ 0x127
+	movw	r3, #294	@ 0x126
 	ldr	r2, [pc, #2440]	@ 27e838 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb14>
 	add	ip, pc, ip
 	ldr	r1, [pc, #2436]	@ 27e83c <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb18>
 	str	ip, [sp, #4]
 	add	r2, pc, r2
 	str	r4, [sp, #16]
 	add	r1, pc, r1
@@ -483134,15 +483134,15 @@
 	beq	27e050 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0x32c>
 	ldr	r3, [sp, #116]	@ 0x74
 	cmp	r3, #5
 	ble	27dfe8 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0x2c4>
 	ldr	r1, [pc, #2376]	@ 27e840 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb1c>
 	mov	r0, r4
 	ldr	r2, [pc, #2372]	@ 27e844 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb20>
-	mov	r3, #304	@ 0x130
+	movw	r3, #303	@ 0x12f
 	ldr	r4, [r4, #20]
 	add	r1, pc, r1
 	str	r1, [sp]
 	add	r2, pc, r2
 	ldr	r1, [pc, #2352]	@ 27e848 <TfLiteStatus tflite::ops::builtin::pad::Eval<(tflite::ops::builtin::pad::KernelType)1>(TfLiteContext*, TfLiteNode*)+0xb24>
 	add	r1, pc, r1
 	blx	r4
```

## Comparing `tflite_runtime_nightly-2.17.0.dev20240505.dist-info/METADATA` & `tflite_runtime_nightly-2.17.0.dev20240512.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.17.0.dev20240505
+Version: 2.17.0.dev20240512
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

