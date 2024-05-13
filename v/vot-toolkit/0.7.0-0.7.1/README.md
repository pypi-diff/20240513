# Comparing `tmp/vot-toolkit-0.7.0.tar.gz` & `tmp/vot-toolkit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.7.0.tar", last modified: Sun Apr 21 18:30:28 2024, max compression
+gzip compressed data, was "vot-toolkit-0.7.1.tar", last modified: Mon May 13 09:00:38 2024, max compression
```

## Comparing `vot-toolkit-0.7.0.tar` & `vot-toolkit-0.7.1.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    35149 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/LICENSE
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      205 2024-04-21 18:27:03.000000 vot-toolkit-0.7.0/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2919 2024-04-18 08:40:54.000000 vot-toolkit-0.7.0/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.7.0/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4545 2024-04-21 09:13:18.000000 vot-toolkit-0.7.0/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      254 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24213 2024-04-20 20:32:32.000000 vot-toolkit-0.7.0/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17333 2024-04-21 16:09:08.000000 vot-toolkit-0.7.0/vot/analysis/accuracy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3872 2024-04-21 13:51:39.000000 vot-toolkit-0.7.0/vot/analysis/failures.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29495 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/analysis/longterm.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17775 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30789 2024-04-20 20:39:42.000000 vot-toolkit-0.7.0/vot/analysis/processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14055 2024-04-21 14:36:12.000000 vot-toolkit-0.7.0/vot/analysis/supervised.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      591 2024-04-21 16:05:33.000000 vot-toolkit-0.7.0/vot/analysis/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    39096 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12821 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/dataset/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.7.0/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3545 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11383 2024-04-20 20:38:34.000000 vot-toolkit-0.7.0/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14274 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3828 2024-04-12 12:03:00.000000 vot-toolkit-0.7.0/vot/dataset/trackingnet.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13889 2024-04-21 16:38:01.000000 vot-toolkit-0.7.0/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1702 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/experiment/helpers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10048 2024-01-16 15:51:12.000000 vot-toolkit-0.7.0/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4945 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6040 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3728 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10604 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15220 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16612 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4202 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/report/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24824 2024-04-21 18:05:49.000000 vot-toolkit-0.7.0/vot/report/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9966 2024-04-21 17:02:49.000000 vot-toolkit-0.7.0/vot/report/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7543 2024-04-21 17:09:49.000000 vot-toolkit-0.7.0/vot/report/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6753 2024-04-21 09:38:48.000000 vot-toolkit-0.7.0/vot/report/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2160 2024-04-21 10:45:44.000000 vot-toolkit-0.7.0/vot/report/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4125 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/video.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3929 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      249 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      247 2024-03-18 10:30:36.000000 vot-toolkit-0.7.0/vot/stack/otb50.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/tests/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      184 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/tests/basic.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.7.0/vot/stack/tests/multiobject.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/tests/segmentation.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      969 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2014.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2015/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2015/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2015/tir.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2016/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      542 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2016/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      303 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2016/tir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2017.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2018/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2018/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2018/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2019/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2020/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2021/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2021/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2021/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2021/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.7.0/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/shortterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/shorttermbox.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.7.0/vot/stack/vots2023.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vots2024/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vots2024/main.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/stack/vots2024/votst.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      688 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/stack/vots2024/votstval.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    33466 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      808 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9417 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      631 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29426 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21476 2024-04-21 16:29:00.000000 vot-toolkit-0.7.0/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    22345 2024-04-21 09:12:45.000000 vot-toolkit-0.7.0/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5740 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10476 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4351 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7113 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10059 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7922 2024-04-21 16:18:22.000000 vot-toolkit-0.7.0/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13864 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1840 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2565 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    35149 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/LICENSE
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      205 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2919 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1401 2024-05-13 09:00:34.000000 vot-toolkit-0.7.1/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.805887 vot-toolkit-0.7.1/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4690 2024-04-23 11:03:41.000000 vot-toolkit-0.7.1/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      254 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.805887 vot-toolkit-0.7.1/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24339 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17630 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3872 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29495 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17775 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    31034 2024-04-24 21:09:39.000000 vot-toolkit-0.7.1/vot/analysis/processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14055 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/supervised.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      591 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/analysis/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.805887 vot-toolkit-0.7.1/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    39182 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12821 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/dataset/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.7.1/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3545 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11337 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14274 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3917 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/dataset/trackingnet.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.805887 vot-toolkit-0.7.1/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13926 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1702 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10048 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4945 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6040 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.805887 vot-toolkit-0.7.1/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3728 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10604 2024-04-18 08:34:19.000000 vot-toolkit-0.7.1/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15220 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16612 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4210 2024-05-13 08:52:50.000000 vot-toolkit-0.7.1/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/report/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    23359 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/report/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9966 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/report/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7543 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/report/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6753 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/report/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2160 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/report/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/report/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4125 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/report/video.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3939 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      249 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      247 2024-03-18 10:30:36.000000 vot-toolkit-0.7.1/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      184 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.7.1/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      969 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      542 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      303 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.809887 vot-toolkit-0.7.1/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2021/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2021/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.7.1/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2022/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.7.1/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2022/shortterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/stack/vot2022/shorttermbox.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.7.1/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/stack/vots2024/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/stack/vots2024/main.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/stack/vots2024/votst.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      688 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/stack/vots2024/votstval.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    33499 2024-04-24 17:32:46.000000 vot-toolkit-0.7.1/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      808 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9417 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      631 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29426 2024-04-12 12:01:42.000000 vot-toolkit-0.7.1/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    20836 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21866 2024-04-23 21:25:51.000000 vot-toolkit-0.7.1/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5740 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10476 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1541 2024-04-23 10:08:18.000000 vot-toolkit-0.7.1/vot/utilities/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4351 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7113 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10059 2024-05-13 08:59:47.000000 vot-toolkit-0.7.1/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2024-05-13 08:57:46.000000 vot-toolkit-0.7.1/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8958 2024-04-23 12:07:07.000000 vot-toolkit-0.7.1/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13864 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1840 2023-06-14 09:31:05.000000 vot-toolkit-0.7.1/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-05-13 09:00:38.813887 vot-toolkit-0.7.1/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2585 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2024-05-13 09:00:38.000000 vot-toolkit-0.7.1/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.7.0/LICENSE` & `vot-toolkit-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/PKG-INFO` & `vot-toolkit-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vot-toolkit-0.7.0/README.md` & `vot-toolkit-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/setup.py` & `vot-toolkit-0.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 
 from os.path import join, dirname, abspath, isfile
-from distutils.core import setup
-from setuptools import find_packages
+from setuptools import find_packages, setup
 
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 install_requires = []
 if isfile(join(this_directory, "requirements.txt")):
```

### Comparing `vot-toolkit-0.7.0/vot/__init__.py` & `vot-toolkit-0.7.1/vot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         local_version = packaging.parse(__version__)
 
         return remote_version > local_version, groups.group(1)
 
     else:
         return False, None
 
-from attributee import Attributee, Integer, Boolean
+from attributee import Attributee, Integer, Boolean, List, String
 
 class GlobalConfiguration(Attributee):
     """Global configuration object for the toolkit. It is used to store global configuration options. It can be initialized
     from environment variables. The following options are supported:
 
     - ``VOT_DEBUG_MODE``: Enables debug mode for the toolkit.
     - ``VOT_SEQUENCE_CACHE_SIZE``: Maximum number of sequences to keep in cache.
@@ -72,14 +72,15 @@
 
     debug_mode = Boolean(default=False, description="Enables debug mode for the toolkit.")
     sequence_cache_size = Integer(default=100, description="Maximum number of sequences to keep in cache.")
     results_binary = Boolean(default=True, description="Enables binary results format.")
     mask_optimize_read = Boolean(default=True, description="Enables mask optimization when reading masks.")
     worker_pool_size = Integer(default=1, description="Number of workers to use for parallel processing.")
     persistent_cache = Boolean(default=True, description="Enables persistent cache for analysis results in workspace.")
+    registry = List(String(), default="", separator=os.pathsep, description="List of directories to search for tracker metadata.")
 
     def __init__(self):
         """Initializes the global configuration object. It reads the configuration from environment variables.
         
         Raises:
             ValueError: When an invalid value is provided for an attribute.
         """
```

### Comparing `vot-toolkit-0.7.0/vot/analysis/__init__.py` & `vot-toolkit-0.7.1/vot/analysis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,19 @@
         raise NotImplementedError()
 
     @property
     def axes(self) -> Axes:
         """ Returns axes semantic description for the result grid """
         raise NotImplementedError()
 
+    @property
+    def cached(self) -> bool:
+        """Returns whether the analysis should be cached."""
+        return True
+
     def commit(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence]):
         """Commits the analysis for execution on default processor."""
         return AnalysisProcessor.commit_default(self, experiment, trackers, sequences)
 
     def run(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence]):
         """Runs the analysis on default processor."""
         return AnalysisProcessor.run_default(self, experiment, trackers, sequences)
```

### Comparing `vot-toolkit-0.7.0/vot/analysis/accuracy.py` & `vot-toolkit-0.7.1/vot/analysis/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,48 +312,62 @@
         bounds = (sequence.size) if self.bounded else None
 
         axis_x = np.linspace(0, 1, self.resolution)
         axis_y = np.zeros_like(axis_x)
 
         ignore_masks = sequence.object(self.ignore_masks)
 
+        valid_objects = 0
+
         for object in objects:
             trajectories = experiment.gather(tracker, sequence, objects=[object])
             if len(trajectories) == 0:
                 raise MissingResultsException()
 
             object_y = np.zeros_like(axis_x) 
 
             if self.filter_tag is not None:
                 frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
             else:
                 frame_mask = None
 
+            valid_trajectories = 0
+
             for trajectory in trajectories:
                 if frame_mask is not None:
                     trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
                     groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m] 
                     masks = [region for region, m in zip(ignore_masks, frame_mask) if m]
                 else:
                     groundtruth = sequence.object(object)
                     masks = ignore_masks
         
                 overlaps, _ = gather_overlaps(trajectory, groundtruth, burnin=self.burnin, ignore_unknown=self.ignore_unknown, 
                                             ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold, ignore_masks=masks)
 
+                if len(overlaps) == 0:
+                    continue
+
+                valid_trajectories += 1
+
                 for i, threshold in enumerate(axis_x):
                     if threshold == 1:
                         # Nicer handling of the edge case
                         object_y[i] += np.sum(overlaps >= threshold) / len(overlaps)
                     else:
                         object_y[i] += np.sum(overlaps > threshold) / len(overlaps)
 
-            axis_y += object_y / len(trajectories)
+            if valid_trajectories == 0:
+                continue
+            
+            valid_objects += 1
+            
+            axis_y += object_y / valid_trajectories
 
-        axis_y /= len(objects)
+        axis_y /= valid_objects
 
         return [(x, y) for x, y in zip(axis_x, axis_y)],
 
 
 @analysis_registry.register("average_success_plot")
 class AverageSuccessPlot(SequenceAggregator):
     """Average success plot analysis. Computes the average success plot of the tracker."""
```

### Comparing `vot-toolkit-0.7.0/vot/analysis/failures.py` & `vot-toolkit-0.7.1/vot/analysis/failures.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/analysis/longterm.py` & `vot-toolkit-0.7.1/vot/analysis/longterm.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/analysis/multistart.py` & `vot-toolkit-0.7.1/vot/analysis/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/analysis/processor.py` & `vot-toolkit-0.7.1/vot/analysis/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -487,21 +487,16 @@
         """Initializes a new instance of the AnalysisFuture class.
 
         Args:
             key (str): The key of the analysis.
         """
 
         super().__init__()
-        self._key = key
-
-    @property
-    def key(self):
-        """Gets the key of the analysis."""
-        return self._key
-
+        self.key = key
+        
     def __repr__(self) -> str:
         """Gets a string representation of the future."""
         return "<AnalysisFuture key={}>".format(self._key)
 
 class AnalysisProcessor(object):
     """A processor that computes analyses."""
 
@@ -541,15 +536,15 @@
 
         key = hashkey(analysis, experiment, trackers, sequences)
 
         with self._lock:
 
             promise = self._exists(key)
 
-            if not promise is None:
+            if not promise is None and analysis.cached:
                 return promise
     
             promise = AnalysisFuture(key)
             promise.add_done_callback(self._promise_cancelled)
 
             dependencies = [self.commit(dependency, experiment, trackers, sequences) for dependency in analysis.dependencies()]
 
@@ -565,33 +560,36 @@
                 parts = analysis.separate(trackers, sequences)
                 partpromises = []
 
                 for part in parts:
                     partkey = hashkey(analysis, experiment, unwrap(part.trackers), unwrap(part.sequences))
                 
                     partpromise = self._exists(partkey)
-                    if not partpromise is None:
+                    if not partpromise is None and analysis.cached:
                         partpromises.append(partpromise)
                         continue
                 
                     partpromise = AnalysisFuture(partkey)
                     partpromises.append(partpromise)
 
                     executorpromise = self._executor.submit(AnalysisPartTask(analysis, experiment, part.trackers, part.sequences), *dependencies, 
                         mapping=partial(select_dependencies, analysis, part.tid, part.sid))
                     self._promises[partkey] = [partpromise]
+                    executorpromise.cached = analysis.cached
                     self._pending[partkey] = executorpromise
                     executorpromise.add_done_callback(self._future_done)
 
                 executorpromise = self._executor.submit(AnalysisJoinTask(analysis, experiment, trackers, sequences),
                         *partpromises, mapping=lambda *x: [list(x)])
+                executorpromise.cached = analysis.cached
                 self._pending[key] = executorpromise
             else:
                 task = AnalysisTask(analysis, experiment, trackers, sequences)
                 executorpromise = self._executor.submit(task, *dependencies, mapping=lambda *x: [list(x)])
+                executorpromise.cached = analysis.cached
                 self._pending[key] = executorpromise
 
             self._promises[key] = [promise]
             executorpromise.add_done_callback(self._future_done)
             logger.debug("Adding analysis task %s", key)
 
             return promise
@@ -633,15 +631,16 @@
             if future.cancelled():
                 del self._pending[key]
                 del self._promises[key]
                 return
 
             try:
                 result = future.result()
-                self._cache[key] = result
+                if self._cache is not None and getattr(future, "cached", False):
+                    self._cache[key] = result
                 error = None
             except (AnalysisError, RuntimeError) as e:
                 error = e
 
             if key not in self._promises:
                 return
 
@@ -765,15 +764,15 @@
         Returns: 
             AnalysisProcessor: The default analysis processor for the current thread.
         """
 
         processor = getattr(AnalysisProcessor._context, 'analysis_processor', None)
 
         if processor is None:
-            logger.warning("Default analysis processor not set for thread %s, using a simple one.", threading.current_thread().name)
+            logger.debug("Default analysis processor not set for thread %s, using a simple one.", threading.current_thread().name)
             from vot.utilities import ThreadPoolExecutor
             from cachetools import LRUCache
             executor = ThreadPoolExecutor(1)
             cache = LRUCache(1000)
             processor = AnalysisProcessor(executor, cache)
             AnalysisProcessor._context.analysis_processor = processor
 
@@ -846,22 +845,22 @@
             container (dict): The container to insert the result into.
             key (Analysis): The analysis to insert the result for.
         """
         def insert(future: Future):
             """Inserts the result of a computation into a container."""
             try:
                 container[key] = future.result()
-            except AnalysisError as e:
-                errors.append(e)
             except Exception as e:
-                logger.exception(e)
+                errors.append(e)
             with condition:
                 condition.notify()
         return insert
 
+    if isinstance(trackers, Tracker): trackers = [trackers]
+
     for experiment in workspace.stack:
 
         logger.debug("Traversing experiment %s", experiment.identifier)
 
         experiment_results = dict()
 
         results[experiment] = experiment_results
@@ -888,14 +887,15 @@
     with Progress("Running analysis", processor.total) as progress:
         try:
 
             while True:
 
                 progress.absolute(processor.total - processor.pending)
                 if processor.pending == 0:
+                    progress.absolute(processor.total)
                     break
 
                 with condition:
                     condition.wait(1)
 
         except KeyboardInterrupt:
             processor.cancel()
@@ -903,12 +903,12 @@
             logger.info("Analysis interrupted by user, aborting.")
             return None
 
     if len(errors) > 0:
         logger.info("Errors occured during analysis, incomplete.")
         for e in errors:
             logger.info("Failed task {}: {}".format(e.task, e.root_cause))
-            if logger.isEnabledFor(logging.DEBUG):
-                e.print(logger)
+            #if logger.isEnabledFor(logging.DEBUG):
+            #    e.print(logger)
         return None
 
     return results
```

### Comparing `vot-toolkit-0.7.0/vot/analysis/supervised.py` & `vot-toolkit-0.7.1/vot/analysis/supervised.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/analysis/tests.py` & `vot-toolkit-0.7.1/vot/analysis/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/__init__.py` & `vot-toolkit-0.7.1/vot/dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Dataset module provides an interface for accessing the datasets and sequences. It also provides a set of utility functions for downloading and extracting datasets."""
 
 import os
-import logging
 
 from numbers import Number
 from collections import namedtuple
 from abc import abstractmethod, ABC
 from typing import List, Mapping, Optional, Set, Tuple, Iterator
 
 from PIL.Image import Image
@@ -15,16 +14,14 @@
 
 from vot.region import Region
 from vot import ToolkitException
 from vot.utilities import Registry
 
 import cv2
 
-logger = logging.getLogger("vot")
-
 dataset_downloader = Registry("vot_downloader")
 sequence_indexer = Registry("vot_indexer")
 sequence_reader = Registry("vot_sequence")
 
 class DatasetException(ToolkitException):
     """Dataset and sequence related exceptions
     """
@@ -1153,19 +1150,20 @@
         path (str, optional): Destination directory. Defaults to ".".
 
     Raises:
         DatasetException: If the bundle cannot be downloaded or is not supported.
     """
 
     from vot.utilities.net import download_uncompress, NetworkException
+    from vot import get_logger
 
     if not url.endswith(".zip"):
         raise DatasetException("Unknown bundle format")
 
-    logger.info('Downloading sequence bundle from "%s". This may take a while ...', url)
+    get_logger().info('Downloading sequence bundle from "%s". This may take a while ...', url)
 
     try:
         download_uncompress(url, path)
     except NetworkException as e:
         raise DatasetException("Unable do download dataset bundle, Please try to download the bundle manually from {} and uncompress it to {}'".format(url, path))
     except IOError as e:
         raise DatasetException("Unable to extract dataset bundle, is the target directory writable and do you have enough space?")
@@ -1210,16 +1208,19 @@
         DatasetException: When a folder does not exist or the format is not recognized.
 
     Returns:
         Dataset: Dataset object
     """
 
     from collections import OrderedDict
+    from vot import get_logger
 
     sequence_list = None
+    
+    logger = get_logger()
 
     for _, indexer in sequence_indexer.items():
         logger.debug("Attempting to index sequences with {}.{}".format(indexer.__module__, indexer.__name__))
         sequence_list = indexer(path)
         if sequence_list is not None:
             break
         
@@ -1249,19 +1250,20 @@
 
     Raises:
         DatasetException: If an loading error occures, unsupported format or other issues.
 
     Returns:
         Sequence: Sequence object
     """
+    from vot import get_logger
 
     for _, loader in sequence_reader.items():
         sequence = loader(path)
         if sequence is not None:
-            logger.debug("Loaded sequence with {}.{}".format(loader.__module__, loader.__name__))
+            get_logger().debug("Loaded sequence with {}.{}".format(loader.__module__, loader.__name__))
             return sequence
 
     raise DatasetException("Unable to load sequence, unknown format or unsupported sequence: {}".format(path))
 
 import importlib
 for module in [".common", ".otb", ".got10k", ".trackingnet"]:
     importlib.import_module(module, package="vot.dataset")
```

### Comparing `vot-toolkit-0.7.0/vot/dataset/common.py` & `vot-toolkit-0.7.1/vot/dataset/common.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/cow.png` & `vot-toolkit-0.7.1/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/dummy.py` & `vot-toolkit-0.7.1/vot/dataset/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/got10k.py` & `vot-toolkit-0.7.1/vot/dataset/got10k.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/otb.py` & `vot-toolkit-0.7.1/vot/dataset/otb.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from vot import get_logger
 from vot.dataset import BasedSequence, DatasetException, PatternFileListChannel, SequenceData
 from vot.utilities import Progress
 from vot.region.io import parse_region
 
 logger = get_logger()
 
-_BASE_URL = "https://web.archive.org/web/20221118171918/http://cvlab.hanyang.ac.kr/tracker_benchmark/   seq/"
+_BASE_URL = "http://cvlab.hanyang.ac.kr/tracker_benchmark/seq/"
 
 _OTB50_SUBSET = ["Basketball", "Biker", "Bird1", "BlurBody", "BlurCar2", "BlurFace", "BlurOwl", "Bolt", "Box",
     "Car1", "Car4", "CarDark", "CarScale", "ClifBar", "Couple", "Crowds", "David", "Deer", "Diving",
     "DragonBaby", "Dudek", "Football", "Freeman4", "Girl", "Human3", "Human4", "Human6", "Human9",
     "Ironman", "Jump", "Jumping", "Liquor", "Matrix", "MotorRolling", "Panda", "RedTeam", "Shaking",
     "Singer2", "Skating1", "Skating2_1", "Skating2_2", "Skiing", "Soccer", "Surfer", "Sylvester", "Tiger2",
     "Trellis", "Walking", "Walking2", "Woman"]
```

### Comparing `vot-toolkit-0.7.0/vot/dataset/proxy.py` & `vot-toolkit-0.7.1/vot/dataset/proxy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/dataset/trackingnet.py` & `vot-toolkit-0.7.1/vot/dataset/trackingnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """ Dataset adapter for the TrackingNet dataset. Note that the dataset is organized a different way than the VOT datasets,
 annotated frames are stored in a separate directory. The dataset also contains train and test splits. The loader 
 assumes that only one of the splits is used at a time and that the path is given to this part of the dataset. """
 
 import os
 import glob
 import logging
+from collections import OrderedDict
 
 import six
 
-from vot.dataset import BasedSequence, PatternFileListChannel, SequenceData, \
+from vot.dataset import Dataset, DatasetException, \
+    BasedSequence, PatternFileListChannel, SequenceData, \
     Sequence
-from vot import get_logger
 from vot.region import Special
 from vot.region.io import read_trajectory
+from vot.utilities import Progress
 
-logger = get_logger()
+logger = logging.getLogger("vot")
 
 def load_channel(source):
     """ Load channel from the given source.
     
     Args:
         source (str): Path to the source. If the source is a directory, it is
             assumed to be a pattern file list. If the source is a file, it is
```

### Comparing `vot-toolkit-0.7.0/vot/experiment/__init__.py` & `vot-toolkit-0.7.1/vot/experiment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from datetime import datetime
 from abc import abstractmethod
 
 from class_registry import ClassRegistry
 
 from attributee import Attributee, Object, Integer, Float, Nested, List, Boolean
 
-from vot import get_logger
 from vot.tracker import TrackerException
 from vot.utilities import Progress, to_number, import_class, ObjectResolver
 from vot.dataset.proxy import IgnoreSpecialObjects
 
 experiment_registry = ClassRegistry("vot_experiment")
 transformer_registry = ClassRegistry("vot_transformer")
 
@@ -270,14 +269,16 @@
             sequences (typing.List[Sequence]): List of sequences to transform
 
         Returns:
             typing.List[Sequence]: List of transformed sequences. The number of sequences may be larger than the input as some transformers may split sequences.
         """
         from vot.dataset import Sequence
         from vot.experiment.transformer import SingleObject
+        from vot import get_logger
+        
         if isinstance(sequences, Sequence):
             sequences = [sequences]
         
         transformers = list(self.transformers)
 
         if not self._multiobject:
             get_logger().debug("Adding single object transformer since experiment is not multi-object")
@@ -345,27 +346,29 @@
             self._finished = self._finished + 1
             self.bar.absolute(self._finished)
 
         def close(self):
             """Close the progress bar."""
             self.bar.close()
 
-    logger = logging.getLogger("vot")
+    from vot import get_logger
+
+    logger = get_logger()
 
     transformed = []
     for sequence in sequences:
         transformed.extend(experiment.transform(sequence))
     sequences = transformed
 
     progress = EvaluationProgress("{}/{}".format(tracker.identifier, experiment.identifier), len(sequences))
     for sequence in sequences:
         try:
             experiment.execute(tracker, sequence, force=force, callback=progress)
         except TrackerException as te:
-            logger.error("Tracker %s encountered an error on sequence %s: %s", te.tracker.identifier, sequence.name, te)
+            logger.error("Tracker %s encountered an error at sequence %s: %s", te.tracker.identifier, sequence.name, te)
             logger.debug(te, exc_info=True)
             if not te.log is None:
                 with experiment.log(te.tracker.identifier) as flog:
                     flog.write(te.log)
                     logger.error("Tracker output written to file: %s", flog.name)
             if not persist:
                 raise TrackerException("Experiment interrupted", te, tracker=tracker)
```

### Comparing `vot-toolkit-0.7.0/vot/experiment/helpers.py` & `vot-toolkit-0.7.1/vot/experiment/helpers.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/experiment/multirun.py` & `vot-toolkit-0.7.1/vot/experiment/multirun.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/experiment/multistart.py` & `vot-toolkit-0.7.1/vot/experiment/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/experiment/transformer.py` & `vot-toolkit-0.7.1/vot/experiment/transformer.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/region/__init__.py` & `vot-toolkit-0.7.1/vot/region/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/region/io.py` & `vot-toolkit-0.7.1/vot/region/io.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/region/raster.py` & `vot-toolkit-0.7.1/vot/region/raster.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/region/shapes.py` & `vot-toolkit-0.7.1/vot/region/shapes.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/region/tests.py` & `vot-toolkit-0.7.1/vot/region/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     def test_ignore_mask(self):
         """Tests if the mask ignore works correctly."""
         from vot.region import Mask
 
         r1 = Mask(np.ones((100, 100), dtype=np.uint8))
         r2 = Mask(np.ones((100, 100), dtype=np.uint8))
         ignore = Mask(np.zeros((100, 100), dtype=np.uint8))
-        self.assertEqual(calculate_overlap(r1, r2, ignore=ignore), 0)
-
-        ignore = Mask(np.ones((100, 100), dtype=np.uint8))
         self.assertEqual(calculate_overlap(r1, r2, ignore=ignore), 1)
 
+        ignore = Mask(np.ones((100, 100), dtype=np.uint8))
+        self.assertEqual(calculate_overlap(r1, r2, ignore=ignore), 0)
+        
     def test_empty_mask(self):
         """Tests if the empty mask is correctly detected."""
         from vot.region import Mask
 
         mask = Mask(np.zeros((100, 100), dtype=np.uint8))
         self.assertTrue(mask.is_empty())
```

### Comparing `vot-toolkit-0.7.0/vot/report/__init__.py` & `vot-toolkit-0.7.1/vot/report/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,57 +228,20 @@
 
             handle.style(**style.region_style())
             regions[frame].draw(handle)
 
         return handle.array
 
 
-class ResultsJSONEncoder(json.JSONEncoder):
-    """ JSON encoder for results. """
-
-    def default(self, o):
-        """ Default encoder. """
-        if isinstance(o, Grid):
-            return list(o)
-        elif isinstance(o, datetime.date):
-            return o.strftime('%Y/%m/%d')
-        elif isinstance(o, np.ndarray):
-            return o.tolist()
-        else:
-            return super().default(o)
-
-class ResultsYAMLEncoder(yaml.Dumper):
-    """ YAML encoder for results."""
-
-    def represent_tuple(self, data):
-        """ Represents a tuple. """
-        return self.represent_list(list(data))
-
-
-    def represent_object(self, o):
-        """ Represents an object. """
-        if isinstance(o, Grid):
-            return self.represent_list(list(o))
-        elif isinstance(o, datetime.date):
-            return o.strftime('%Y/%m/%d')
-        elif isinstance(o, np.ndarray):
-            return self.represent_list(o.tolist())
-        else:
-            return super().represent_object(o)
-
-ResultsYAMLEncoder.add_representer(collections.OrderedDict, ResultsYAMLEncoder.represent_dict)
-ResultsYAMLEncoder.add_representer(tuple, ResultsYAMLEncoder.represent_tuple)
-ResultsYAMLEncoder.add_representer(Grid, ResultsYAMLEncoder.represent_object)
-ResultsYAMLEncoder.add_representer(np.ndarray, ResultsYAMLEncoder.represent_object)
-ResultsYAMLEncoder.add_multi_representer(np.integer, ResultsYAMLEncoder.represent_int)
-ResultsYAMLEncoder.add_multi_representer(np.inexact, ResultsYAMLEncoder.represent_float)
 
 def generate_serialized(trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage", serializer: str, name: str):
     """ Generates a serialized report of the results.  """
 
+    from vot.utilities.io import JSONEncoder, YAMLEncoder
+
     doc = dict()
     doc["toolkit"] = version
     doc["timestamp"] = datetime.datetime.now().isoformat()
     doc["trackers"] = {t.reference : t.describe() for t in trackers}
     doc["sequences"] = {s.name : s.describe() for s in sequences}
 
     doc["results"] = dict()
@@ -288,18 +251,18 @@
         exp["results"] = []
         for _, data in analyses.items():
             exp["results"].append(data)
         doc["results"][experiment.identifier] = exp
 
     if serializer == "json":
         with storage.write(name + "." + serializer) as handle:
-            json.dump(doc, handle, indent=2, cls=ResultsJSONEncoder)
+            json.dump(doc, handle, indent=2, cls=JSONEncoder)
     elif serializer == "yaml":
         with storage.write(name + "." + serializer) as handle:
-            yaml.dump(doc, handle, Dumper=ResultsYAMLEncoder)
+            yaml.dump(doc, handle, Dumper=YAMLEncoder)
     else:
         raise RuntimeError("Unknown serializer")
 
 def configure_axes(figure, rect=None, _=None):
     """ Configures the axes of the plot. """
 
     axes = PlotAxes(figure, rect or [0, 0, 1, 1])
```

### Comparing `vot-toolkit-0.7.0/vot/report/common.py` & `vot-toolkit-0.7.1/vot/report/common.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/html.py` & `vot-toolkit-0.7.1/vot/report/html.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/jquery.js` & `vot-toolkit-0.7.1/vot/report/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/latex.py` & `vot-toolkit-0.7.1/vot/report/latex.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/pure.css` & `vot-toolkit-0.7.1/vot/report/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/report.css` & `vot-toolkit-0.7.1/vot/report/report.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/report.js` & `vot-toolkit-0.7.1/vot/report/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/table.js` & `vot-toolkit-0.7.1/vot/report/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/report/video.py` & `vot-toolkit-0.7.1/vot/report/video.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/__init__.py` & `vot-toolkit-0.7.1/vot/stack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     url = String(default="")
     deprecated = Boolean(default=False)
     experiments = Map(Object(experiment_resolver))
 
     @property
     def name(self):
         """Returns the name of the stack."""
-        return self.get("_name", None)
+        return getattr(self, "_name", None)
 
     def __iter__(self):
         """Iterates over experiments in the stack."""
         return iter(self.experiments.values())
 
     def __len__(self):
         """Returns the number of experiments in the stack."""
@@ -70,14 +70,15 @@
             identifier (str): Identifier of the experiment
         
         Returns:
             Experiment: Experiment object
 
         """
         return self.experiments[identifier]
+    
 
 def resolve_stack(name: str, *directories: List[str]) -> str:
     """Searches for stack file in the given directories and returns its absolute path. If given an absolute path as input
     it simply returns it.
 
     Args:
         name (str): Name of the stack
```

### Comparing `vot-toolkit-0.7.0/vot/stack/tests/multiobject.yaml` & `vot-toolkit-0.7.1/vot/stack/tests/multiobject.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/tests/segmentation.yaml` & `vot-toolkit-0.7.1/vot/stack/tests/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/tests.py` & `vot-toolkit-0.7.1/vot/stack/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2016/rgb.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2016/rgb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2017.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2017.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2018/shortterm.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2018/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2019/shortterm.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2019/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2020/shortterm.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2020/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2021/shortterm.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2021/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2022/shortterm.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2022/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vot2022/shorttermbox.yaml` & `vot-toolkit-0.7.1/vot/stack/vot2022/shorttermbox.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/stack/vots2024/votstval.yaml` & `vot-toolkit-0.7.1/vot/stack/vots2024/votstval.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/tracker/__init__.py` & `vot-toolkit-0.7.1/vot/tracker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """ This module contains the base classes for trackers and the registry of known trackers. """
 
 import os
 import re
 import configparser
-import logging
 import copy
 from typing import Tuple, List, Union
 from collections import OrderedDict, namedtuple
 from abc import abstractmethod, ABC
 
 import yaml
 
 from vot import ToolkitException
 from vot.dataset import Frame
 from vot.region import Region
 from vot.utilities import to_string
 
-logger = logging.getLogger("vot")
-
 class TrackerException(ToolkitException):
     """ Base class for all tracker related exceptions."""
 
     def __init__(self, *args, tracker, tracker_log=None):
         """ Initialize the exception.
 
         Args:
@@ -101,14 +98,18 @@
     def __init__(self, directories, root=os.getcwd()):
         """ Initialize the registry.
 
         Args:
             directories (list): List of directories to scan for trackers.
             root (str, optional): The root directory of the workspace. Defaults to os.getcwd().
         """
+        from vot import get_logger
+        
+        logger = get_logger()
+        
         trackers = dict()
         registries = []
 
         for directory in directories:
             if not os.path.isabs(directory):
                 directory = os.path.normpath(os.path.abspath(os.path.join(root, directory)))
```

### Comparing `vot-toolkit-0.7.0/vot/tracker/dummy.py` & `vot-toolkit-0.7.1/vot/tracker/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/tracker/results.py` & `vot-toolkit-0.7.1/vot/tracker/results.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/tracker/tests.py` & `vot-toolkit-0.7.1/vot/tracker/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/tracker/trax.py` & `vot-toolkit-0.7.1/vot/tracker/trax.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/utilities/__init__.py` & `vot-toolkit-0.7.1/vot/utilities/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import sys
 import csv
 import re
 import hashlib
 import logging
 import inspect
+import threading
 import time
 import concurrent.futures as futures
 from logging import Formatter, LogRecord
 
 from numbers import Number
 from typing import Any, Mapping, Tuple
 import typing
@@ -109,66 +110,49 @@
         nested_list: The nested list to flatten.
 
     Returns:
         The flattened list.
     """
     return [item for sublist in nested_list for item in sublist]
 
-from vot.utilities.notebook import is_notebook
-
-if is_notebook():
-    try:
-        from ipywidgets import IntProgress
-        from tqdm._tqdm_notebook import tqdm_notebook as tqdm
-    except ImportError:
-        from tqdm import tqdm
-else:
-    from tqdm import tqdm
 
 class Progress(object):
     """Wrapper around tqdm progress bar, enables silecing the progress output and some more
     costumizations.
     """
 
-    class StreamProxy(object):
-        """Proxy class for tqdm to enable silent mode."""
-
-        def write(self, x):
-            """Write function used by tqdm."""
-            # Avoid print() second call (useless \n)
-            if len(x.rstrip()) > 0:
-                tqdm.write(x)
-
-        def flush(self):
-            """Flush function used by tqdm."""
-            #return getattr(self.file, "flush", lambda: None)()
-            pass
-
-    @staticmethod
-    def logstream():
-        """Returns a stream proxy that can be used to redirect output to the progress bar."""
-        return Progress.StreamProxy()
-
     def __init__(self, description="Processing", total=100):
         """Creates a new progress bar.
 
         Args:
             description: The description of the progress bar.
             total: The total number of steps.
         """
+        
+        from vot.utilities.notebook import is_notebook
+        
         from vot import get_logger
+        
+        if is_notebook():
+            try:
+                from tqdm._tqdm_notebook import tqdm_notebook as tqdm
+            except ImportError:
+                from tqdm import tqdm
+        else:
+            from tqdm import tqdm
+        
         silent = get_logger().level > logging.INFO
 
         if not silent:
-            self._tqdm = tqdm(disable=False if is_notebook() else None, 
+            self._bar = tqdm(disable=None, 
                 bar_format=" {desc:20.20} |{bar}| {percentage:3.0f}% [{elapsed}<{remaining}]", file=sys.stdout, leave=False)
-            self._tqdm.desc = description
-            self._tqdm.total = total
-        if silent or self._tqdm.disable:
-            self._tqdm = None
+            self._bar.desc = description
+            self._bar.total = total
+        if silent or self._bar.disable:
+            self._bar = None
             self._value = 0
             self._total = total if not silent else 0
 
     def _percent(self, n):
         """Returns the percentage of the given value.
 
         Args:
@@ -181,68 +165,67 @@
 
     def absolute(self, value):
         """Sets the progress to the given value.
 
         Args:
             value: The value to set the progress to.
         """
-        if self._tqdm is None:
+        if self._bar is None:
             if self._total == 0:
                 return
             prev = self._value
             self._value = max(0, min(value, self._total))
             if self._percent(prev) != self._percent(self._value):
                 print("%d %%" % self._percent(self._value))
         else:
-            self._tqdm.update(value - self._tqdm.n)  # will also set self.n = b * bsize
+            self._bar.update(value - self._bar.n)  # will also set self.n = b * bsize
         
     def relative(self, n):
         """Increments the progress by the given value.
 
         Args:
             n: The value to increment the progress by.
         """
-        if self._tqdm is None:
+        if self._bar is None:
             if self._total == 0:
                 return
             prev = self._value
             self._value = max(0, min(self._value + n, self._total))
             if self._percent(prev) != self._percent(self._value):
                 print("%d %%" % self._percent(self._value))
         else:
-            self._tqdm.update(n)  # will also set self.n = b * bsize 
+            self._bar.update(n)  # will also set self.n = b * bsize 
 
     def total(self, t):
         """Sets the total number of steps.
 
         Args:
             t: The total number of steps.
         """
-        if self._tqdm is None:
+        if self._bar is None:
             if self._total == 0:
                 return
             self._total = t
         else:
-            if self._tqdm.total == t:
+            if self._bar.total == t:
                 return
-            self._tqdm.total = t
-            self._tqdm.refresh()
+            self._bar.total = t
+            self._bar.refresh()
 
+    def close(self):
+        """Closes the progress bar."""
+        if self._bar:
+            self._bar.close()
+            
     def __enter__(self):
-        """Enters the context manager."""
         return self
-
+    
     def __exit__(self, exc_type, exc_value, traceback):
-        """Exits the context manager."""
         self.close()
-
-    def close(self):
-        """Closes the progress bar."""
-        if self._tqdm:
-            self._tqdm.close()
+        
 
 def extract_files(archive, destination, callback = None):
     """Extracts all files from the given archive to the given destination.
 
     Args:
         archive: The archive to extract the files from.
         destination: The destination to extract the files to.
```

### Comparing `vot-toolkit-0.7.0/vot/utilities/cli.py` & `vot-toolkit-0.7.1/vot/utilities/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import argparse
 import logging
 import yaml
 from datetime import datetime
 
-from .. import check_updates, toolkit_version, get_logger
+from .. import check_updates, toolkit_version, get_logger, check_debug
 from . import Progress, normalize_path
 
 logger = get_logger()
 
 class EnvDefault(argparse.Action):
     """Argparse action that resorts to a value in a specified envvar if no value is provided via program arguments.
     """
@@ -41,16 +41,17 @@
         config (argparse.Namespace): Configuration
     """
     from vot.dataset.dummy import generate_dummy
     from vot.dataset import load_sequence, Frame
     from vot.tracker import ObjectStatus, Registry, TrackerException
     from vot.experiment.helpers import MultiObjectHelper
     from vot.dataset.proxy import ObjectsHideFilterSequence
+    from vot import config as global_config
 
-    trackers = Registry(config.registry)
+    trackers = Registry(global_config.registry)
 
     if not config.tracker:
         logger.error("Unable to continue without a tracker")
         logger.error("List of found trackers: ")
         for k in trackers.identifiers():
             logger.error(" * %s", k)
         return
@@ -224,33 +225,27 @@
     """Run an evaluation for a tracker on an experiment stack and a set of sequences.
     
     Args:
         config (argparse.Namespace): Configuration    
     """
 
     from vot.experiment import run_experiment
-    from ..tracker import Registry, TrackerException
+    from ..tracker import TrackerException
     from ..workspace import Workspace
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
-    global_registry = [os.path.abspath(x) for x in config.registry]
-
-    registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
-
-    logger.debug("Found data for %d trackers", len(registry))
-
-    trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
+    trackers = workspace.registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if len(trackers) == 0:
         logger.error("Unable to continue without at least on tracker")
         logger.error("List of available found trackers: ")
-        for k in registry.identifiers():
+        for k in workspace.registry.identifiers():
             logger.error(" * %s", k)
         return
 
     # Filter experiments
     if config.experiments:
         experiments = [v for k, v in workspace.stack.experiments.items() if k in config.experiments.split(",")]
     else:
@@ -280,32 +275,25 @@
     Args:
         args (argparse.Namespace): Configuration
     """
     from vot import config
 
     from vot.analysis import AnalysisProcessor, process_stack_analyses
     from vot.report import generate_serialized
-    from ..tracker import Registry
     from ..workspace import Workspace
     from ..workspace.storage import Cache
 
     workspace = Workspace.load(args.workspace)
 
     logger.debug("Loaded workspace in '%s'", args.workspace)
 
-    global_registry = [os.path.abspath(x) for x in args.registry]
-
-    registry = Registry(list(workspace.registry) + global_registry, root=args.workspace)
-
-    logger.debug("Found data for %d trackers", len(registry))
-
     if not args.trackers:
-        trackers = workspace.list_results(registry)
+        trackers = workspace.list_results(workspace.registry)
     else:
-        trackers = registry.resolve(*args.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
+        trackers = workspace.registry.resolve(*args.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if not trackers:
         logger.warning("No trackers resolved, stopping.")
         return
 
     logger.debug("Running analysis for %d trackers", len(trackers))
 
@@ -362,67 +350,59 @@
     """Generate a report for a one or multiple trackers on an experiment stack and a set of sequences.
 
     Args:
         config (argparse.Namespace): Configuration
     """
 
     from vot.report import generate_document
-    from ..tracker import Registry
     from ..workspace import Workspace
 
 
     if config.name is None:
         name = "{:%Y-%m-%dT%H-%M-%S.%f%z}".format(datetime.now())
     else:
         name = config.name
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
-    global_registry = [os.path.abspath(x) for x in config.registry]
-
-    registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
-
-    logger.debug("Found data for %d trackers", len(registry))
-
     if not config.trackers:
-        trackers = workspace.list_results(registry)
+        trackers = workspace.list_results(workspace.registry)
     else:
-        trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
+        trackers = workspace.registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if not trackers:
         logger.warning("No trackers resolved, stopping.")
         return
 
-    logger.debug("Running analysis for %d trackers", len(trackers))
+    logger.debug("Running report generation for %d trackers", len(trackers))
 
     generate_document(workspace, trackers, config.format, name, config.sequences, config.experiments)
     
+    logger.info("Report generation successful, document available as %s", name)
+    
     
 def do_pack(config: argparse.Namespace):
     """Package results to a ZIP file so that they can be submitted to a challenge.
 
     Args:
         config (argparse.Namespace): Configuration
     """
 
     import zipfile, io
     from shutil import copyfileobj
-
-    from ..tracker import Registry
     from ..workspace import Workspace
+    from vot.utilities.io import YAMLEncoder
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
-    registry = Registry(list(workspace.registry) + config.registry, root=config.workspace)
-
-    tracker = registry[config.tracker]
+    tracker = workspace.registry[config.tracker]
 
     logger.info("Packaging results for tracker %s", tracker.identifier)
 
     all_files = []
     can_finish = True
 
     with Progress("Scanning", len(workspace.dataset) * len(workspace.stack)) as progress:
@@ -447,40 +427,39 @@
 
     archive_name = "{}_{:%Y-%m-%dT%H-%M-%S.%f%z}.zip".format(tracker.identifier, timestamp)
 
     with Progress("Compressing", len(all_files)) as progress:
 
         manifest = dict(identifier=tracker.identifier, configuration=tracker.describe(),
             timestamp="{:%Y-%m-%dT%H-%M-%S.%f%z}".format(timestamp), platform=sys.platform,
-            python=sys.version, toolkit=toolkit_version(), stack=workspace.stack.dump())
+            python=sys.version, toolkit=toolkit_version(), stack=workspace.dump()["stack"])
 
         with zipfile.ZipFile(workspace.storage.write(archive_name, binary=True), mode="w") as archive:
             for f in all_files:
                 info = zipfile.ZipInfo(filename=os.path.join(f[1], f[2], f[0]), date_time=timestamp.timetuple())
                 with archive.open(info, mode="w") as fout, f[3].read(f[0]) as fin:
                     if isinstance(fin, io.TextIOBase):
                         copyfileobj(fin, io.TextIOWrapper(fout))
                     else:
                         copyfileobj(fin, fout)
                 progress.relative(1)
 
             info = zipfile.ZipInfo(filename="manifest.yml", date_time=timestamp.timetuple())
             with io.TextIOWrapper(archive.open(info, mode="w")) as fout:
-                yaml.dump(manifest, fout)
+                yaml.dump(manifest, fout, Dumper=YAMLEncoder)
 
     logger.info("Result packaging successful, archive available in %s", archive_name)
 
 def main():
     """Entrypoint to the toolkit Command Line Interface utility, should be executed as a program and provided with arguments.
     """
 
     parser = argparse.ArgumentParser(description='VOT Toolkit Command Line Interface', prog="vot")
     parser.add_argument("--debug", "-d", default=False, help="Backup backend", required=False, action='store_true')
-    parser.add_argument("--registry", default=".", help='Tracker registry paths', required=False, action=EnvDefault, \
-        separator=os.path.pathsep, envvar='VOT_REGISTRY')
+    parser.add_argument("--registry", default=".", help='Tracker registry paths', required=False)
 
     subparsers = parser.add_subparsers(help='commands', dest='action', title="Commands")
 
     test_parser = subparsers.add_parser('test', help='Test a tracker integration on a synthetic sequence')
     test_parser.add_argument("tracker", help='Tracker identifier', nargs="?")
     test_parser.add_argument("--visualize", "-g", default=False, required=False, help='Visualize results of the test session', action='store_true')
     test_parser.add_argument("--sequence", "-s", required=False, help='Path to sequence to use instead of dummy')
@@ -518,14 +497,17 @@
 
     from vot import print_config
 
     try:
 
         args = parser.parse_args()
 
+        if args.registry:
+            os.environ["VOT_REGISTRY"] = os.pathsep.join(os.environ.get("VOT_REGISTRY", "").split(os.pathsep) + [args.registry])
+
         if args.debug:
             os.environ["VOT_DEBUG_MODE"] = "1"
             logger.setLevel(logging.DEBUG)
         else:
             logger.setLevel(logging.INFO)
 
         print_config()
@@ -557,11 +539,11 @@
         else:
             parser.print_help()
 
     except argparse.ArgumentError as e:
         logger.error(e)
         exit(-1)
     except Exception as e:
-        logger.exception(e)
+        logger.exception(e, exc_info=check_debug())
         exit(1)
 
     exit(0)
```

### Comparing `vot-toolkit-0.7.0/vot/utilities/data.py` & `vot-toolkit-0.7.1/vot/utilities/data.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/utilities/draw.py` & `vot-toolkit-0.7.1/vot/utilities/draw.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/utilities/migration.py` & `vot-toolkit-0.7.1/vot/utilities/migration.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/utilities/net.py` & `vot-toolkit-0.7.1/vot/utilities/net.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/utilities/notebook.py` & `vot-toolkit-0.7.1/vot/utilities/notebook.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/workspace/__init__.py` & `vot-toolkit-0.7.1/vot/workspace/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,20 +64,44 @@
             str: Dumped value
         """
         if value.name is None:
             return value.dump()
         else:
             return value.name
 
+class RegistryLoader(Attribute):
+    """Special attribute that converts a list of strings input to a Registry object. The paths are appended to
+    the global registry search paths.
+    """
+    
+    def coerce(self, value, context: typing.Optional[CoerceContext]):
+        
+        from vot import config, get_logger
+        
+        # Workspace registry paths are relative to the workspace directory
+        paths = list(List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory))).coerce(value, context))
+
+        # Combine the paths with the global registry search paths (relative to the current directory)
+        registry = Registry(paths + [normalize_path(x, os.curdir) for x in config.registry], root=context.parent.directory)
+        registry._paths = paths
+ 
+        get_logger().debug("Found data for %d trackers", len(registry))
+
+        return registry
+
+    def dump(self, value: "Registry") -> typing.List[str]:
+        assert isinstance(value, Registry)
+        return value._paths
+
 class Workspace(Attributee):
     """Workspace class represents the main junction of trackers, datasets and experiments. Each workspace performs 
     given experiments on a provided dataset.
     """
 
-    registry = List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory)))
+    registry = RegistryLoader() # List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory)))
     stack = StackLoader()
     sequences = String(default="sequences")
     report = Nested(ReportConfiguration)
 
     @staticmethod
     def exists(directory: str) -> bool:
         """Check if a workspace exists in a given directory.
```

### Comparing `vot-toolkit-0.7.0/vot/workspace/storage.py` & `vot-toolkit-0.7.1/vot/workspace/storage.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot/workspace/tests.py` & `vot-toolkit-0.7.1/vot/workspace/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.7.0/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.7.1/vot_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vot-toolkit-0.7.0/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.7.1/vot_toolkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 vot/tracker/results.py
 vot/tracker/tests.py
 vot/tracker/trax.py
 vot/utilities/__init__.py
 vot/utilities/cli.py
 vot/utilities/data.py
 vot/utilities/draw.py
+vot/utilities/io.py
 vot/utilities/migration.py
 vot/utilities/net.py
 vot/utilities/notebook.py
 vot/workspace/__init__.py
 vot/workspace/storage.py
 vot/workspace/tests.py
 vot_toolkit.egg-info/PKG-INFO
```

