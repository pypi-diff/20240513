# Comparing `tmp/dghs_imgutils-0.4.4.tar.gz` & `tmp/dghs_imgutils-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs_imgutils-0.4.4.tar", last modified: Fri May 10 14:49:50 2024, max compression
+gzip compressed data, was "dghs_imgutils-0.4.5.tar", last modified: Mon May 13 13:27:35 2024, max compression
```

## Comparing `dghs_imgutils-0.4.4.tar` & `dghs_imgutils-0.4.5.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.436571 dghs_imgutils-0.4.4/imgutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ascii/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/censor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/halfbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/ccip.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/dbaesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/censor_.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/emoji_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/heart_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/imgcensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/smile_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/squeeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/dwpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/resource/background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/restore/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/nafnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/scunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/sd/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/upscale/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/upscale/cdc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/onnxruntime.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/tqdm_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/bangumi_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/dbrating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/nsfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/portrait.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/real.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/style_age.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/teen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-model.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.603784 dghs_imgutils-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 13:26:46.000000 dghs_imgutils-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-13 13:26:46.000000 dghs_imgutils-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-13 13:27:35.603784 dghs_imgutils-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-13 13:26:46.000000 dghs_imgutils-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.595784 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-13 13:27:35.000000 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-13 13:27:35.000000 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:27:35.000000 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-13 13:27:35.000000 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 13:27:35.000000 dghs_imgutils-0.4.5/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.583784 dghs_imgutils-0.4.5/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.583784 dghs_imgutils-0.4.5/imgutils/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ascii/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.583784 dghs_imgutils-0.4.5/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.587784 dghs_imgutils-0.4.5/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.587784 dghs_imgutils-0.4.5/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/halfbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.587784 dghs_imgutils-0.4.5/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.587784 dghs_imgutils-0.4.5/imgutils/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/generic/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/generic/enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.587784 dghs_imgutils-0.4.5/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/dbaesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ocr/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ocr/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/ocr/recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/pose/dwpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/pose/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/pose/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/resource/background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/restore/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/restore/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/restore/nafnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/restore/scunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/sd/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/sd/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.591784 dghs_imgutils-0.4.5/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.595784 dghs_imgutils-0.4.5/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.595784 dghs_imgutils-0.4.5/imgutils/upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/upscale/cdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.595784 dghs_imgutils-0.4.5/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/onnxruntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/utils/tqdm_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:27:35.595784 dghs_imgutils-0.4.5/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/bangumi_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/dbrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/nsfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/portrait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/style_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/teen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements-model.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:27:35.603784 dghs_imgutils-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-13 13:26:47.000000 dghs_imgutils-0.4.5/setup.py
```

### Comparing `dghs_imgutils-0.4.4/LICENSE` & `dghs_imgutils-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/PKG-INFO` & `dghs_imgutils-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.4
+Version: 0.4.5
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs_imgutils-0.4.4/README.md` & `dghs_imgutils-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/PKG-INFO` & `dghs_imgutils-0.4.5/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.4
+Version: 0.4.5
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/SOURCES.txt` & `dghs_imgutils-0.4.5/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 imgutils/tagging/order.py
 imgutils/tagging/overlap.py
 imgutils/tagging/wd14.py
 imgutils/upscale/__init__.py
 imgutils/upscale/cdc.py
 imgutils/utils/__init__.py
 imgutils/utils/area.py
+imgutils/utils/format.py
 imgutils/utils/onnxruntime.py
 imgutils/utils/storage.py
 imgutils/utils/tqdm_.py
 imgutils/validate/__init__.py
 imgutils/validate/aicheck.py
 imgutils/validate/bangumi_char.py
 imgutils/validate/classify.py
```

### Comparing `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/requires.txt` & `dghs_imgutils-0.4.5/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/ascii/drawing.py` & `dghs_imgutils-0.4.5/imgutils/ascii/drawing.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/config/meta.py` & `dghs_imgutils-0.4.5/imgutils/config/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.4.4'
+__VERSION__ = '0.4.5'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d7'
```

### Comparing `dghs_imgutils-0.4.4/imgutils/data/background.py` & `dghs_imgutils-0.4.5/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/data/decode.py` & `dghs_imgutils-0.4.5/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/data/encode.py` & `dghs_imgutils-0.4.5/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/data/image.py` & `dghs_imgutils-0.4.5/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/data/layer.py` & `dghs_imgutils-0.4.5/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/__init__.py` & `dghs_imgutils-0.4.5/imgutils/detect/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/_yolo.py` & `dghs_imgutils-0.4.5/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/censor.py` & `dghs_imgutils-0.4.5/imgutils/detect/censor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/eye.py` & `dghs_imgutils-0.4.5/imgutils/detect/eye.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/face.py` & `dghs_imgutils-0.4.5/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/halfbody.py` & `dghs_imgutils-0.4.5/imgutils/detect/halfbody.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/hand.py` & `dghs_imgutils-0.4.5/imgutils/detect/hand.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/head.py` & `dghs_imgutils-0.4.5/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/person.py` & `dghs_imgutils-0.4.5/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/text.py` & `dghs_imgutils-0.4.5/imgutils/detect/text.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/detect/visual.py` & `dghs_imgutils-0.4.5/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/edge/__init__.py` & `dghs_imgutils-0.4.5/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/edge/_base.py` & `dghs_imgutils-0.4.5/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/edge/canny.py` & `dghs_imgutils-0.4.5/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/edge/lineart.py` & `dghs_imgutils-0.4.5/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/edge/lineart_anime.py` & `dghs_imgutils-0.4.5/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/generic/classify.py` & `dghs_imgutils-0.4.5/imgutils/generic/classify.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/generic/enhance.py` & `dghs_imgutils-0.4.5/imgutils/generic/enhance.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/aesthetic.py` & `dghs_imgutils-0.4.5/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/ccip.py` & `dghs_imgutils-0.4.5/imgutils/metrics/ccip.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/dbaesthetic.py` & `dghs_imgutils-0.4.5/imgutils/metrics/dbaesthetic.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 """
 from typing import Dict, Optional, Tuple
 
 import numpy as np
 from huggingface_hub import hf_hub_download
 
-from imgutils.data import ImageTyping
-from imgutils.generic import ClassifyModel
+from ..data import ImageTyping
+from ..generic import ClassifyModel
+from ..utils import vreplace
 
 __all__ = [
     'anime_dbaesthetic',
 ]
 
 _DEFAULT_MODEL_NAME = 'swinv2pv3_v0_448_ls0.2_x'
 _REPO_ID = 'deepghs/anime_aesthetic'
@@ -36,38 +37,14 @@
     'good': 0.5,
     'normal': 0.25,
     'low': 0.1,
     'worst': 0.0,
 }
 
 
-def _value_replace(v, mapping):
-    """
-    Replaces values in a data structure using a mapping dictionary.
-
-    :param v: The input data structure.
-    :type v: Any
-    :param mapping: A dictionary mapping values to replacement values.
-    :type mapping: Dict
-    :return: The modified data structure.
-    :rtype: Any
-    """
-    if isinstance(v, (list, tuple)):
-        return type(v)([_value_replace(vitem, mapping) for vitem in v])
-    elif isinstance(v, dict):
-        return type(v)({key: _value_replace(value, mapping) for key, value in v.items()})
-    else:
-        try:
-            _ = hash(v)
-        except TypeError:  # pragma: no cover
-            return v
-        else:
-            return mapping.get(v, v)
-
-
 class AestheticModel:
     """
     A model for assessing the aesthetic quality of anime images.
     """
 
     def __init__(self, repo_id: str):
         """
@@ -167,15 +144,15 @@
         :type fmt: Tuple[str, ...]
         :return: A dictionary containing the aesthetic assessment results.
         :rtype: Dict[str, float]
         """
         score, confidence = self.get_aesthetic_score(image, model_name)
         percentile = self.score_to_percentile(score, model_name)
         label = self.percentile_to_label(percentile)
-        return _value_replace(
+        return vreplace(
             v=fmt,
             mapping={
                 'label': label,
                 'percentile': percentile,
                 'score': score,
                 'confidence': confidence,
             }
```

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/laplacian.py` & `dghs_imgutils-0.4.5/imgutils/metrics/laplacian.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/lpips.py` & `dghs_imgutils-0.4.5/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/metrics/psnr_.py` & `dghs_imgutils-0.4.5/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/ocr/__init__.py` & `dghs_imgutils-0.4.5/imgutils/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/ocr/detect.py` & `dghs_imgutils-0.4.5/imgutils/ocr/detect.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/ocr/entry.py` & `dghs_imgutils-0.4.5/imgutils/ocr/entry.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/ocr/recognize.py` & `dghs_imgutils-0.4.5/imgutils/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/align.py` & `dghs_imgutils-0.4.5/imgutils/operate/align.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/censor_.py` & `dghs_imgutils-0.4.5/imgutils/operate/censor_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/emoji_censor.png` & `dghs_imgutils-0.4.5/imgutils/operate/emoji_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/heart_censor.png` & `dghs_imgutils-0.4.5/imgutils/operate/heart_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/imgcensor.py` & `dghs_imgutils-0.4.5/imgutils/operate/imgcensor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/smile_censor.png` & `dghs_imgutils-0.4.5/imgutils/operate/smile_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/operate/squeeze.py` & `dghs_imgutils-0.4.5/imgutils/operate/squeeze.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/pose/dwpose.py` & `dghs_imgutils-0.4.5/imgutils/pose/dwpose.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/pose/format.py` & `dghs_imgutils-0.4.5/imgutils/pose/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/pose/visual.py` & `dghs_imgutils-0.4.5/imgutils/pose/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/resource/background.py` & `dghs_imgutils-0.4.5/imgutils/resource/background.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/restore/adversarial.py` & `dghs_imgutils-0.4.5/imgutils/restore/adversarial.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/restore/nafnet.py` & `dghs_imgutils-0.4.5/imgutils/restore/nafnet.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/restore/scunet.py` & `dghs_imgutils-0.4.5/imgutils/restore/scunet.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/sd/metadata.py` & `dghs_imgutils-0.4.5/imgutils/sd/metadata.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/sd/model.py` & `dghs_imgutils-0.4.5/imgutils/sd/model.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/segment/isnetis.py` & `dghs_imgutils-0.4.5/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/__init__.py` & `dghs_imgutils-0.4.5/imgutils/tagging/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/blacklist.py` & `dghs_imgutils-0.4.5/imgutils/tagging/blacklist.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/character.py` & `dghs_imgutils-0.4.5/imgutils/tagging/character.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/deepdanbooru.py` & `dghs_imgutils-0.4.5/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/format.py` & `dghs_imgutils-0.4.5/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/match.py` & `dghs_imgutils-0.4.5/imgutils/tagging/match.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/mldanbooru.py` & `dghs_imgutils-0.4.5/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/order.py` & `dghs_imgutils-0.4.5/imgutils/tagging/order.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/overlap.py` & `dghs_imgutils-0.4.5/imgutils/tagging/overlap.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/tagging/wd14.py` & `dghs_imgutils-0.4.5/imgutils/tagging/wd14.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 Overview:
     Tagging utils based on wd14 v2, inspired by
     `SmilingWolf/wd-v1-4-tags <https://huggingface.co/spaces/SmilingWolf/wd-v1-4-tags>`_ .
 """
 from functools import lru_cache
 from typing import List, Tuple
 
-import huggingface_hub
 import numpy as np
 import onnxruntime
 import pandas as pd
 from PIL import Image
 from hbutils.testing.requires.version import VersionInfo
+from huggingface_hub import hf_hub_download
 
 from .format import remove_underline
 from .overlap import drop_overlap_tags
 from ..data import load_image, ImageTyping
-from ..utils import open_onnx_model
+from ..utils import open_onnx_model, vreplace
 
 SWIN_MODEL_REPO = "SmilingWolf/wd-v1-4-swinv2-tagger-v2"
 CONV_MODEL_REPO = "SmilingWolf/wd-v1-4-convnext-tagger-v2"
 CONV2_MODEL_REPO = "SmilingWolf/wd-v1-4-convnextv2-tagger-v2"
 VIT_MODEL_REPO = "SmilingWolf/wd-v1-4-vit-tagger-v2"
 MOAT_MODEL_REPO = "SmilingWolf/wd-v1-4-moat-tagger-v2"
 CONV_V3_MODEL_REPO = 'SmilingWolf/wd-convnext-tagger-v3'
@@ -60,30 +60,33 @@
 
     :param model_name: The name of the model.
     :type model_name: str
     :return: The loaded ONNX model.
     :rtype: ONNXModel
     """
     _version_support_check(model_name)
-    return open_onnx_model(huggingface_hub.hf_hub_download(MODEL_NAMES[model_name], MODEL_FILENAME))
+    return open_onnx_model(hf_hub_download(
+        repo_id='deepghs/wd14_tagger_with_embeddings',
+        filename=f'{MODEL_NAMES[model_name]}/model.onnx',
+    ))
 
 
 @lru_cache()
 def _get_wd14_labels(model_name, no_underline: bool = False) -> Tuple[List[str], List[int], List[int], List[int]]:
     """
     Get labels for the WD14 model.
 
     :param model_name: The name of the model.
     :type model_name: str
     :param no_underline: If True, replaces underscores in tag names with spaces.
     :type no_underline: bool
     :return: A tuple containing the list of tag names, and lists of indexes for rating, general, and character categories.
     :rtype: Tuple[List[str], List[int], List[int], List[int]]
     """
-    path = huggingface_hub.hf_hub_download(MODEL_NAMES[model_name], LABEL_FILENAME)
+    path = hf_hub_download(MODEL_NAMES[model_name], LABEL_FILENAME)
     df = pd.read_csv(path)
     name_series = df["name"]
     if no_underline:
         name_series = name_series.map(remove_underline)
     tag_names = name_series.tolist()
 
     rating_indexes = list(np.where(df["category"] == 9)[0])
@@ -129,14 +132,15 @@
         model_name: str = _DEFAULT_MODEL_NAME,
         general_threshold: float = 0.35,
         general_mcut_enabled: bool = False,
         character_threshold: float = 0.85,
         character_mcut_enabled: bool = False,
         no_underline: bool = False,
         drop_overlap: bool = False,
+        fmt=('rating', 'general', 'character'),
 ):
     """
     Overview:
         Get tags for an image with wd14 taggers.
         Similar to `SmilingWolf/wd-v1-4-tags <https://huggingface.co/spaces/SmilingWolf/wd-v1-4-tags>`_ .
 
     :param image: The input image.
@@ -151,14 +155,17 @@
     :type character_threshold: float
     :param character_mcut_enabled: If True, applies MCut thresholding to character tags.
     :type character_mcut_enabled: bool
     :param no_underline: If True, replaces underscores in tag names with spaces.
     :type no_underline: bool
     :param drop_overlap: If True, drops overlapping tags.
     :type drop_overlap: bool
+    :param fmt: Return format, default is ``('rating', 'general', 'character')``.
+        ``embedding`` is also supported for feature extraction.
+    :type fmt: Any
     :return: A tuple containing dictionaries for rating, general, and character tags with their probabilities.
     :rtype: Tuple[Dict[str, float], Dict[str, float], Dict[str, float]]
 
     Example:
         Here are some images for example
 
         .. image:: tagging_demo.plot.py.svg
@@ -185,16 +192,18 @@
     """
     tag_names, rating_indexes, general_indexes, character_indexes = _get_wd14_labels(model_name, no_underline)
     model = _get_wd14_model(model_name)
     _, target_size, _, _ = model.get_inputs()[0].shape
     image = _prepare_image_for_tagging(image, target_size)
 
     input_name = model.get_inputs()[0].name
+    assert len(model.get_outputs()) == 2
     label_name = model.get_outputs()[0].name
-    preds = model.run([label_name], {input_name: image})[0]
+    emb_name = model.get_outputs()[1].name
+    preds, embeddings = model.run([label_name, emb_name], {input_name: image})
     labels = list(zip(tag_names, preds[0].astype(float)))
 
     ratings_names = [labels[i] for i in rating_indexes]
     rating = dict(ratings_names)
 
     general_names = [labels[i] for i in general_indexes]
     if general_mcut_enabled:
@@ -211,8 +220,17 @@
         character_probs = np.array([x[1] for x in character_names])
         character_threshold = _mcut_threshold(character_probs)
         character_threshold = max(0.15, character_threshold)
 
     character_res = [x for x in character_names if x[1] > character_threshold]
     character_res = dict(character_res)
 
-    return rating, general_res, character_res
+    return vreplace(
+        fmt,
+        {
+            'rating': rating,
+            'general': general_res,
+            'character': character_res,
+            'tag': {**general_res, **character_res},
+            'embedding': embeddings[0],
+        }
+    )
```

### Comparing `dghs_imgutils-0.4.4/imgutils/upscale/cdc.py` & `dghs_imgutils-0.4.5/imgutils/upscale/cdc.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/utils/area.py` & `dghs_imgutils-0.4.5/imgutils/utils/area.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/utils/onnxruntime.py` & `dghs_imgutils-0.4.5/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/utils/tqdm_.py` & `dghs_imgutils-0.4.5/imgutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/aicheck.py` & `dghs_imgutils-0.4.5/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/bangumi_char.py` & `dghs_imgutils-0.4.5/imgutils/validate/bangumi_char.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/classify.py` & `dghs_imgutils-0.4.5/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/color.py` & `dghs_imgutils-0.4.5/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/completeness.py` & `dghs_imgutils-0.4.5/imgutils/validate/completeness.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/dbrating.py` & `dghs_imgutils-0.4.5/imgutils/validate/dbrating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/monochrome.py` & `dghs_imgutils-0.4.5/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/nsfw.py` & `dghs_imgutils-0.4.5/imgutils/validate/nsfw.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/portrait.py` & `dghs_imgutils-0.4.5/imgutils/validate/portrait.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/rating.py` & `dghs_imgutils-0.4.5/imgutils/validate/rating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/real.py` & `dghs_imgutils-0.4.5/imgutils/validate/real.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/safe.py` & `dghs_imgutils-0.4.5/imgutils/validate/safe.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/style_age.py` & `dghs_imgutils-0.4.5/imgutils/validate/style_age.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/teen.py` & `dghs_imgutils-0.4.5/imgutils/validate/teen.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/imgutils/validate/truncate.py` & `dghs_imgutils-0.4.5/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.4/setup.py` & `dghs_imgutils-0.4.5/setup.py`

 * *Files identical despite different names*

