# Comparing `tmp/nxswriter-3.8.2.tar.gz` & `tmp/nxswriter-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxswriter-3.8.2.tar", last modified: Thu May 25 04:43:37 2023, max compression
+gzip compressed data, was "nxswriter-3.9.0.tar", last modified: Wed Oct 11 06:52:09 2023, max compression
```

## Comparing `nxswriter-3.8.2.tar` & `nxswriter-3.9.0.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.338563 nxswriter-3.8.2/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian10_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3518 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian10_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian10_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3593 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian10_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian11_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3587 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian11_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian8_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2554 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian8_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian8_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2763 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian8_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian9_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3521 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian9_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/debian9_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3524 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/debian9_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)     3292 2023-05-24 13:07:50.000000 nxswriter-3.8.2/.ci/install.sh
--rw-r--r--   0 jkotan   (15949) irc         (39)      460 2023-05-24 13:07:50.000000 nxswriter-3.8.2/.ci/run.sh
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/ubuntu16.04_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2598 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/ubuntu16.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/ubuntu16.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2603 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/ubuntu16.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/ubuntu18.04_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3273 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/ubuntu18.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/ubuntu18.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3326 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/ubuntu18.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.ci/ubuntu20.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3737 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.ci/ubuntu20.04_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)      175 2022-11-22 20:26:35.000000 nxswriter-3.8.2/.flake8
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.github/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.310563 nxswriter-3.8.2/.github/workflows/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2058 2023-05-24 13:07:50.000000 nxswriter-3.8.2/.github/workflows/tests.yml
--rw-r--r--   0 jkotan   (15949) irc         (39)       83 2018-09-14 10:01:58.000000 nxswriter-3.8.2/.gitignore
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-09-14 10:01:58.000000 nxswriter-3.8.2/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)    17504 2023-05-25 04:43:04.000000 nxswriter-3.8.2/ChangeLog
--rw-r--r--   0 jkotan   (15949) irc         (39)      114 2022-11-22 20:26:35.000000 nxswriter-3.8.2/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      918 2022-11-22 20:26:35.000000 nxswriter-3.8.2/NXSDataWriter
--rw-r--r--   0 jkotan   (15949) irc         (39)    18108 2023-03-08 10:18:04.000000 nxswriter-3.8.2/NXSDataWriter.xmi
--rw-r--r--   0 jkotan   (15949) irc         (39)    10752 2023-05-25 04:43:37.338563 nxswriter-3.8.2/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     7582 2023-04-24 15:16:46.000000 nxswriter-3.8.2/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.314563 nxswriter-3.8.2/XMLExamples/
--rw-r--r--   0 jkotan   (15949) irc         (39)   104154 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/MNI.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      915 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/encodedImage.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      904 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/encodedImage4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1593 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/scan.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1645 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/scan2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1594 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/scan3.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     7606 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/test.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     7539 2018-09-14 10:01:58.000000 nxswriter-3.8.2/XMLExamples/trigger.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.314563 nxswriter-3.8.2/doc/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6774 2022-11-22 20:26:35.000000 nxswriter-3.8.2/doc/Makefile
--rw-r--r--   0 jkotan   (15949) irc         (39)    14053 2022-11-22 20:26:35.000000 nxswriter-3.8.2/doc/conf.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      448 2022-11-22 20:26:35.000000 nxswriter-3.8.2/doc/index.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     6707 2022-11-22 20:26:35.000000 nxswriter-3.8.2/doc/make.bat
--rw-r--r--   0 jkotan   (15949) irc         (39)     4318 2022-11-22 20:26:35.000000 nxswriter-3.8.2/doc/nxswriter.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.314563 nxswriter-3.8.2/doc_html/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3757 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrCanFail.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3732 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrCurrentFileId.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3656 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrErrors.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3956 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrFileName.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3882 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrJSONRecord.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3839 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrSkipAcquisition.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3968 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrStepsPerFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3914 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/AttrXMLSettings.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     3053 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/Attributes.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1861 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/ClassDescription.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1249 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdCloseEntry.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1288 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdCloseEntryAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1231 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdCloseFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1272 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdOpenEntry.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1311 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdOpenEntryAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1232 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdOpenFile.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1292 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdRecord.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1331 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdRecordAsynch.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1253 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdState.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1266 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/CmdStatus.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     2701 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/Commands.html
--rw-r--r--   0 jkotan   (15949) irc         (39)    51670 2023-03-08 10:18:44.000000 nxswriter-3.8.2/doc_html/FullDocument.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1756 2023-03-08 10:18:53.000000 nxswriter-3.8.2/doc_html/Properties.html
--rw-r--r--   0 jkotan   (15949) irc         (39)     1003 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/States.html
--rw-r--r--   0 jkotan   (15949) irc         (39)      903 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/TitleBanner.html
--rw-r--r--   0 jkotan   (15949) irc         (39)      979 2023-03-02 11:49:57.000000 nxswriter-3.8.2/doc_html/index.html
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.314563 nxswriter-3.8.2/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      991 2022-11-22 20:26:35.000000 nxswriter-3.8.2/man/NXSDataWriter.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2209 2023-02-28 13:19:57.000000 nxswriter-3.8.2/man/nxsfromxml.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    86849 2023-03-08 09:00:26.000000 nxswriter-3.8.2/man/nxswriter.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       74 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxsfromxml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.318563 nxswriter-3.8.2/nxswriter/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3889 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/ClientSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9068 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/DBaseSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6156 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/DataHolder.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4683 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/DataSourceFactory.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4574 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/DataSourcePool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5295 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/DataSources.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15052 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/DecoderPool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8599 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/EAttribute.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    26261 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/EField.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/EGroup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8816 2023-05-25 04:43:04.000000 nxswriter-3.8.2/nxswriter/ELink.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4000 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/EStrategy.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3011 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/Element.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2099 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/ElementThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1660 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/Errors.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20455 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/FElement.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6821 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/FetchNameHandler.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6035 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/H5Elements.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4493 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/InnerXMLParser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3668 2022-12-12 12:16:40.000000 nxswriter-3.8.2/nxswriter/Metadata.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9077 2023-02-28 13:17:59.000000 nxswriter-3.8.2/nxswriter/NXSFromXML.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    31313 2023-03-02 11:51:13.000000 nxswriter-3.8.2/nxswriter/NXSWriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13805 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/NexusXMLHandler.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11230 2023-03-02 09:03:40.000000 nxswriter-3.8.2/nxswriter/PyEvalSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-05-24 13:07:50.000000 nxswriter-3.8.2/nxswriter/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 13:11:43.000000 nxswriter-3.8.2/nxswriter/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    27784 2023-03-08 09:00:26.000000 nxswriter-3.8.2/nxswriter/TangoDataWriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29378 2023-03-09 13:11:43.000000 nxswriter-3.8.2/nxswriter/TangoSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6031 2023-03-08 09:00:26.000000 nxswriter-3.8.2/nxswriter/ThreadPool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7676 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/Types.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1760 2022-11-22 20:26:35.000000 nxswriter-3.8.2/nxswriter/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.318563 nxswriter-3.8.2/nxswriter.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)    10752 2023-05-25 04:43:37.000000 nxswriter-3.8.2/nxswriter.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     5577 2023-05-25 04:43:37.000000 nxswriter-3.8.2/nxswriter.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-05-25 04:43:37.000000 nxswriter-3.8.2/nxswriter.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 20:30:29.000000 nxswriter-3.8.2/nxswriter.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       28 2023-05-25 04:43:37.000000 nxswriter-3.8.2/nxswriter.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       10 2023-05-25 04:43:37.000000 nxswriter-3.8.2/nxswriter.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      203 2023-05-25 04:43:37.338563 nxswriter-3.8.2/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4121 2023-05-24 13:07:50.000000 nxswriter-3.8.2/setup.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 04:43:37.338563 nxswriter-3.8.2/test/
--rw-r--r--   0 jkotan   (15949) irc         (39)    52501 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/Checkers.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5501 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5490 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4684 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4771 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   105723 2023-03-02 07:45:36.000000 nxswriter-3.8.2/test/ClientFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   105064 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20281 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ClientSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5954 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/Converters_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5612 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5598 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4882 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    87899 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    87520 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16850 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DBaseSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    30489 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DataHolder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10182 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DataSourceDecoders_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15976 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DataSourceFactory_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10560 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DataSourcePool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5859 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DataSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12848 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/DecoderPool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   108465 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EAttributeH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   107896 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EAttributeH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    18366 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDimH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    18395 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDimH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7839 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDimensionsH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7832 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDimensionsH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6412 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDocH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6409 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EDocH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   285119 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFieldH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   285230 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFieldH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   171438 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFieldReshapeH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   170929 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFieldReshapeH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5329 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFileH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5321 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EFileH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    42448 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EGroupH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    42416 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EGroupH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    72274 2023-05-24 13:07:50.000000 nxswriter-3.8.2/test/ELinkH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    71745 2023-05-24 13:07:50.000000 nxswriter-3.8.2/test/ELinkH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11340 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EStrategyH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11349 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/EStrategyH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7030 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ESymbolH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7120 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ESymbolH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ElementH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3204 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ElementH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5386 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ElementThread_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3629 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/Element_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4471 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/Errors_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45152 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FElementH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45164 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FElementH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    34938 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FElementWithAttrH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35205 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FElementWithAttrH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22964 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FetchNameHandler_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   344148 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FileWriterH5CppH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   179717 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FileWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/FileWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   215225 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/H5CppWriter_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   178444 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/H5PYWriter_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15547 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/InnerXMLParser_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    15418 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/MYSQLSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    46174 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/NTP_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   211886 2023-02-28 12:37:21.000000 nxswriter-3.8.2/test/NXSDataWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   211039 2023-02-28 12:37:21.000000 nxswriter-3.8.2/test/NXSDataWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    41359 2023-02-28 13:17:59.000000 nxswriter-3.8.2/test/NXSFromXMLH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    41371 2023-02-28 13:17:59.000000 nxswriter-3.8.2/test/NXSFromXMLH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   125101 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/NexusXMLHandlerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   125171 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/NexusXMLHandlerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14694 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ORACLESource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13061 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/PGSQLSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1652 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ProxyHelper.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5053 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ProxyTools_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    25478 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/PyEvalSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    54033 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/PyEvalTangoSourceH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    53808 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/PyEvalTangoSourceH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4886 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    52123 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/SimpleServer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5851 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/SimpleServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    21946 2023-03-09 13:11:43.000000 nxswriter-3.8.2/test/StreamSet_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7488 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TNObject_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      252 2018-09-14 10:01:58.000000 nxswriter-3.8.2/test/TangoClassID.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)    35756 2023-03-02 09:03:40.000000 nxswriter-3.8.2/test/TangoDataWriterH5CppH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   250238 2023-02-28 12:37:21.000000 nxswriter-3.8.2/test/TangoDataWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   250237 2023-02-28 12:37:21.000000 nxswriter-3.8.2/test/TangoDataWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5627 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TangoFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5618 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TangoFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4851 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TangoFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4841 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TangoFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   112661 2023-03-02 09:03:40.000000 nxswriter-3.8.2/test/TangoFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   112655 2023-03-02 09:03:40.000000 nxswriter-3.8.2/test/TangoFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   161008 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TangoSource_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11581 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TgDevice_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    33398 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TgGroup_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    27676 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TgMember_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10508 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/ThreadPool_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4264 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/TstDataSource.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8163 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/UINT32decoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5434 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/UTF8decoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9237 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/VDEOdecoder_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5365 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagAsynchH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5354 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagAsynchH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4712 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagServerH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4702 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagServerH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35614 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35619 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/XMLFieldTagWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      923 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      945 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/__main__.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    20511 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/main.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1458 2018-09-14 10:01:58.000000 nxswriter-3.8.2/test/mydb.pgsql
--rw-r--r--   0 jkotan   (15949) irc         (39)     1646 2022-11-22 20:26:35.000000 nxswriter-3.8.2/test/sttest.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.957426 nxswriter-3.9.0/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian10_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3518 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian10_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian10_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3593 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian10_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian11_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3587 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian11_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian8_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2554 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian8_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian8_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2763 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian8_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian9_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3521 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian9_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/debian9_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3524 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/debian9_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3342 2023-06-19 13:39:32.000000 nxswriter-3.9.0/.ci/install.sh
+-rw-r--r--   0 jkotan   (15949) irc         (39)      243 2023-06-19 13:39:32.000000 nxswriter-3.9.0/.ci/run.sh
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.921427 nxswriter-3.9.0/.ci/ubuntu16.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2598 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/ubuntu16.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/.ci/ubuntu16.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2603 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/ubuntu16.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/.ci/ubuntu18.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3273 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/ubuntu18.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/.ci/ubuntu18.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3326 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/ubuntu18.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/.ci/ubuntu20.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3737 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.ci/ubuntu20.04_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)      175 2022-11-22 20:26:35.000000 nxswriter-3.9.0/.flake8
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.917427 nxswriter-3.9.0/.github/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/.github/workflows/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2068 2023-06-19 13:39:32.000000 nxswriter-3.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       83 2018-09-14 10:01:58.000000 nxswriter-3.9.0/.gitignore
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-09-14 10:01:58.000000 nxswriter-3.9.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17608 2023-10-11 05:46:51.000000 nxswriter-3.9.0/ChangeLog
+-rw-r--r--   0 jkotan   (15949) irc         (39)      114 2022-11-22 20:26:35.000000 nxswriter-3.9.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      918 2022-11-22 20:26:35.000000 nxswriter-3.9.0/NXSDataWriter
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18108 2023-03-08 10:18:04.000000 nxswriter-3.9.0/NXSDataWriter.xmi
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10773 2023-10-11 06:52:09.957426 nxswriter-3.9.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7603 2023-06-19 13:40:54.000000 nxswriter-3.9.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.925427 nxswriter-3.9.0/XMLExamples/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   104154 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/MNI.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      915 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/encodedImage.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      904 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/encodedImage4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1593 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/scan.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1645 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/scan2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1594 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/scan3.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7606 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/test.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7539 2018-09-14 10:01:58.000000 nxswriter-3.9.0/XMLExamples/trigger.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.929427 nxswriter-3.9.0/doc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6774 2022-11-22 20:26:35.000000 nxswriter-3.9.0/doc/Makefile
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14053 2022-11-22 20:26:35.000000 nxswriter-3.9.0/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      448 2022-11-22 20:26:35.000000 nxswriter-3.9.0/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6707 2022-11-22 20:26:35.000000 nxswriter-3.9.0/doc/make.bat
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4318 2022-11-22 20:26:35.000000 nxswriter-3.9.0/doc/nxswriter.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.937427 nxswriter-3.9.0/doc_html/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3757 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrCanFail.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3732 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrCurrentFileId.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3656 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrErrors.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3956 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrFileName.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3882 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrJSONRecord.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3839 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrSkipAcquisition.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3968 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrStepsPerFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3914 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/AttrXMLSettings.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3053 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/Attributes.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1861 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/ClassDescription.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1249 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdCloseEntry.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1288 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdCloseEntryAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1231 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdCloseFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1272 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdOpenEntry.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1311 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdOpenEntryAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1232 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdOpenFile.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1292 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdRecord.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1331 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdRecordAsynch.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1253 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdState.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1266 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/CmdStatus.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2701 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/Commands.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)    51670 2023-03-08 10:18:44.000000 nxswriter-3.9.0/doc_html/FullDocument.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1756 2023-03-08 10:18:53.000000 nxswriter-3.9.0/doc_html/Properties.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1003 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/States.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)      903 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/TitleBanner.html
+-rw-r--r--   0 jkotan   (15949) irc         (39)      979 2023-03-02 11:49:57.000000 nxswriter-3.9.0/doc_html/index.html
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.937427 nxswriter-3.9.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      991 2022-11-22 20:26:35.000000 nxswriter-3.9.0/man/NXSDataWriter.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2209 2023-02-28 13:19:57.000000 nxswriter-3.9.0/man/nxsfromxml.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    86864 2023-06-19 13:48:14.000000 nxswriter-3.9.0/man/nxswriter.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       74 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxsfromxml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.941427 nxswriter-3.9.0/nxswriter/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3889 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/ClientSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9068 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/DBaseSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6156 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/DataHolder.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4683 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/DataSourceFactory.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4574 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/DataSourcePool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5295 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/DataSources.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15052 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/DecoderPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8430 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/EAttribute.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27649 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/EField.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/EGroup.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8816 2023-05-25 04:43:04.000000 nxswriter-3.9.0/nxswriter/ELink.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3988 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/EStrategy.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3011 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/Element.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2099 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/ElementThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1660 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/Errors.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20455 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/FElement.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6821 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/FetchNameHandler.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7396 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/H5Elements.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4493 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/InnerXMLParser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3668 2022-12-12 12:16:40.000000 nxswriter-3.9.0/nxswriter/Metadata.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9077 2023-02-28 13:17:59.000000 nxswriter-3.9.0/nxswriter/NXSFromXML.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    31313 2023-03-02 11:51:13.000000 nxswriter-3.9.0/nxswriter/NXSWriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13833 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/NexusXMLHandler.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11230 2023-03-02 09:03:40.000000 nxswriter-3.9.0/nxswriter/PyEvalSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-10-11 05:46:51.000000 nxswriter-3.9.0/nxswriter/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 13:11:43.000000 nxswriter-3.9.0/nxswriter/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27784 2023-03-08 09:00:26.000000 nxswriter-3.9.0/nxswriter/TangoDataWriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29378 2023-03-09 13:11:43.000000 nxswriter-3.9.0/nxswriter/TangoSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6031 2023-03-08 09:00:26.000000 nxswriter-3.9.0/nxswriter/ThreadPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7676 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/Types.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1760 2022-11-22 20:26:35.000000 nxswriter-3.9.0/nxswriter/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.941427 nxswriter-3.9.0/nxswriter.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10773 2023-10-11 06:52:09.000000 nxswriter-3.9.0/nxswriter.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5577 2023-10-11 06:52:09.000000 nxswriter-3.9.0/nxswriter.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-10-11 06:52:09.000000 nxswriter-3.9.0/nxswriter.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 20:30:29.000000 nxswriter-3.9.0/nxswriter.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       39 2023-10-11 06:52:09.000000 nxswriter-3.9.0/nxswriter.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       10 2023-10-11 06:52:09.000000 nxswriter-3.9.0/nxswriter.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      203 2023-10-11 06:52:09.957426 nxswriter-3.9.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4115 2023-10-11 05:46:51.000000 nxswriter-3.9.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-10-11 06:52:09.957426 nxswriter-3.9.0/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52500 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/Checkers.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5501 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ClientFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5490 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ClientFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4684 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ClientFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4771 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ClientFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   105728 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/ClientFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   105069 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/ClientFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20281 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ClientSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5954 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/Converters_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5612 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DBFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5598 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DBFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4896 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DBFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4882 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DBFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    87901 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/DBFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    87522 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/DBFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16850 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DBaseSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    30470 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/DataHolder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10182 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DataSourceDecoders_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15976 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DataSourceFactory_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10560 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DataSourcePool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5859 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DataSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12848 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/DecoderPool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   108481 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EAttributeH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   107912 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EAttributeH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18366 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDimH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    18395 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDimH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7839 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDimensionsH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7832 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDimensionsH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6412 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDocH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6409 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EDocH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   285147 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EFieldH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   285258 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EFieldH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   171466 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EFieldReshapeH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   170957 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EFieldReshapeH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5329 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EFileH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5321 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EFileH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    42448 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EGroupH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    42416 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/EGroupH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    72274 2023-05-24 13:07:50.000000 nxswriter-3.9.0/test/ELinkH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    71745 2023-05-24 13:07:50.000000 nxswriter-3.9.0/test/ELinkH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11342 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EStrategyH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11351 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/EStrategyH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7030 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ESymbolH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7120 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ESymbolH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3208 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ElementH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3204 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ElementH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5386 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ElementThread_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3629 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/Element_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4471 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/Errors_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45152 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FElementH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45164 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FElementH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    34938 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FElementWithAttrH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35205 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FElementWithAttrH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22964 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FetchNameHandler_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   344154 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/FileWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   179723 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/FileWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/FileWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   215245 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/H5CppWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   178444 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/H5PYWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15547 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/InnerXMLParser_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15418 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/MYSQLSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46174 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/NTP_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   211886 2023-02-28 12:37:21.000000 nxswriter-3.9.0/test/NXSDataWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   211039 2023-02-28 12:37:21.000000 nxswriter-3.9.0/test/NXSDataWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    41359 2023-02-28 13:17:59.000000 nxswriter-3.9.0/test/NXSFromXMLH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    41371 2023-02-28 13:17:59.000000 nxswriter-3.9.0/test/NXSFromXMLH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   125145 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/NexusXMLHandlerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   125215 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/NexusXMLHandlerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14694 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ORACLESource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13061 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/PGSQLSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1652 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ProxyHelper.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5053 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ProxyTools_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25478 2023-10-09 11:20:04.000000 nxswriter-3.9.0/test/PyEvalSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    54033 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/PyEvalTangoSourceH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    53808 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/PyEvalTangoSourceH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4886 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52123 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/SimpleServer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5851 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/SimpleServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    21946 2023-03-09 13:11:43.000000 nxswriter-3.9.0/test/StreamSet_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7488 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TNObject_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      252 2018-09-14 10:01:58.000000 nxswriter-3.9.0/test/TangoClassID.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35756 2023-03-02 09:03:40.000000 nxswriter-3.9.0/test/TangoDataWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   250238 2023-02-28 12:37:21.000000 nxswriter-3.9.0/test/TangoDataWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   250237 2023-02-28 12:37:21.000000 nxswriter-3.9.0/test/TangoDataWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5627 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TangoFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5618 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TangoFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4851 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TangoFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4841 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TangoFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   112731 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/TangoFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   112725 2023-10-11 05:46:51.000000 nxswriter-3.9.0/test/TangoFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   161008 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TangoSource_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11581 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TgDevice_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    33398 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TgGroup_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27676 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TgMember_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10508 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/ThreadPool_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4264 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/TstDataSource.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8163 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/UINT32decoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5434 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/UTF8decoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9237 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/VDEOdecoder_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5365 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagAsynchH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5354 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagAsynchH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4712 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagServerH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4702 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagServerH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35614 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35619 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/XMLFieldTagWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      923 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      945 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/__main__.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    20511 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/main.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1458 2018-09-14 10:01:58.000000 nxswriter-3.9.0/test/mydb.pgsql
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1646 2022-11-22 20:26:35.000000 nxswriter-3.9.0/test/sttest.py
```

### Comparing `nxswriter-3.8.2/.ci/debian10_py2/Dockerfile` & `nxswriter-3.9.0/.ci/debian10_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian10_py3/Dockerfile` & `nxswriter-3.9.0/.ci/debian10_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian11_py3/Dockerfile` & `nxswriter-3.9.0/.ci/debian11_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian8_py2/Dockerfile` & `nxswriter-3.9.0/.ci/debian8_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian8_py3/Dockerfile` & `nxswriter-3.9.0/.ci/debian8_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian9_py2/Dockerfile` & `nxswriter-3.9.0/.ci/debian9_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/debian9_py3/Dockerfile` & `nxswriter-3.9.0/.ci/debian9_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/install.sh` & `nxswriter-3.9.0/.ci/install.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 
 # restart mysqldb
-if [ "$1" = "debian11" ]; then
+if [ "$1" = "debian11" ] || [ "$1" = "debian12" ]; then
     docker exec --user root ndts service mariadb restart
 else
     # workaround for a bug in debian9, i.e. starting mysql hangs
     docker exec --user root ndts service mysql stop
     if [ "$1" = "ubuntu20.04" ] || [ "$1" = "ubuntu20.10" ] || [ "$1" = "ubuntu21.04" ] || [ "$1" = "ubuntu22.04" ] || [ "$1" = "ubuntu23.04" ]; then
 	# docker exec --user root ndts /bin/bash -c 'mkdir -p /var/lib/mysql'
 	# docker exec --user root ndts /bin/bash -c 'chown mysql:mysql /var/lib/mysql'
@@ -39,15 +39,15 @@
 docker exec  --user root ndts chown -R tango:tango .
 
 if [ "$2" = "2" ]; then
     echo "install python-pytango"
     docker exec  --user root ndts /bin/sh -c 'apt-get -qq update; apt-get -qq install -y   python-pytango nxsconfigserver-db python-nxstools'
 else
     echo "install python3-pytango"
-    if [ "$1" = "ubuntu20.04" ] || [ "$1" = "ubuntu20.10" ] || [ "$1" = "ubuntu21.04" ] || [ "$1" = "ubuntu23.04" ] || [ "$1" = "ubuntu22.04" ] || [ "$1" = "debian11" ]; then
+    if [ "$1" = "ubuntu20.04" ] || [ "$1" = "ubuntu20.10" ] || [ "$1" = "ubuntu21.04" ] || [ "$1" = "ubuntu23.04" ] || [ "$1" = "ubuntu22.04" ] || [ "$1" = "debian11" ] || [ "$1" = "debian12" ]; then
 	docker exec  --user root ndts /bin/sh -c 'apt-get -qq update; apt-get -qq install -y   python3-tango nxsconfigserver-db python3-nxstools'
     else
 	docker exec  --user root ndts /bin/sh -c 'apt-get -qq update; apt-get -qq install -y   python3-pytango nxsconfigserver-db python3-nxstools'
     fi
 fi
 if [ "$?" != "0" ]; then exit 255; fi
```

### Comparing `nxswriter-3.8.2/.ci/ubuntu16.04_py2/Dockerfile` & `nxswriter-3.9.0/.ci/ubuntu16.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/ubuntu16.04_py3/Dockerfile` & `nxswriter-3.9.0/.ci/ubuntu16.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/ubuntu18.04_py2/Dockerfile` & `nxswriter-3.9.0/.ci/ubuntu18.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/ubuntu18.04_py3/Dockerfile` & `nxswriter-3.9.0/.ci/ubuntu18.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.ci/ubuntu20.04_py3/Dockerfile` & `nxswriter-3.9.0/.ci/ubuntu20.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/.github/workflows/tests.yml` & `nxswriter-3.9.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - name: Run flake8
         run: flake8 .
 
   python3_tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        os: [debian11, debian10, ubuntu23.04, ubuntu22.04, ubuntu20.04]
+        os: [debian12, debian11, debian10, ubuntu23.04, ubuntu22.04, ubuntu20.04]
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
       - name: Update bash files
         run: |
           chmod +x .ci/run.sh
           chmod +x .ci/install.sh
```

### Comparing `nxswriter-3.8.2/COPYRIGHT` & `nxswriter-3.9.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/ChangeLog` & `nxswriter-3.9.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-10-11 Jan Kotanski <jankotan@gmail.com>
+	* add support for a filter tag (#154)
+	* tagged as 3.9.0
+
 2023-05-24 Jan Kotanski <jankotan@gmail.com>
 	* add support for ':/' in the link target (#147)
 	* tagged as 3.8.2
 
 2023-03-07 Jan Kotanski <jankotan@gmail.com>
 	* add timestamps to stderr and stdout logs (#142)
 	* tagged as 3.8.1
```

### Comparing `nxswriter-3.8.2/NXSDataWriter` & `nxswriter-3.9.0/NXSDataWriter`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/NXSDataWriter.xmi` & `nxswriter-3.9.0/NXSDataWriter.xmi`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/PKG-INFO` & `nxswriter-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxswriter
-Version: 3.8.2
+Version: 3.9.0
 Summary: Nexus Data writer implemented as a Tango Server
 Home-page: https://github.com/nexdatas/nxsdatawriter
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to NXSDataWriter's documentation!
         =========================================
@@ -68,30 +68,30 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         """""""""""""""
         
-        Debian `bullseye`, `buster`  or Ubuntu `focal`, `bionic` packages can be found in the HDRI repository.
+        Debian `bookworm`, `bullseye`, `buster`  or Ubuntu `lunar`, `jammy`, `focal`  packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ curl -s http://repos.pni-hdri.de/debian_repo.pub.gpg | gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/debian-hdri-repo.gpg --import
         	  $ chmod 644 /etc/apt/trusted.gpg.d/debian-hdri-repo.gpg
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         To install tango server
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install nxswriter
```

### Comparing `nxswriter-3.8.2/README.rst` & `nxswriter-3.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,30 @@
 .. code-block:: console
 
 	  $ python setup.py install
 
 Debian packages
 """""""""""""""
 
-Debian `bullseye`, `buster`  or Ubuntu `focal`, `bionic` packages can be found in the HDRI repository.
+Debian `bookworm`, `bullseye`, `buster`  or Ubuntu `lunar`, `jammy`, `focal`  packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
 	  $ curl -s http://repos.pni-hdri.de/debian_repo.pub.gpg | gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/debian-hdri-repo.gpg --import
 	  $ chmod 644 /etc/apt/trusted.gpg.d/debian-hdri-repo.gpg
 
 and then download the corresponding source list
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
 
 To install tango server
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install nxswriter
```

### Comparing `nxswriter-3.8.2/XMLExamples/MNI.xml` & `nxswriter-3.9.0/XMLExamples/MNI.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/encodedImage.xml` & `nxswriter-3.9.0/XMLExamples/encodedImage.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/encodedImage4.xml` & `nxswriter-3.9.0/XMLExamples/encodedImage4.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/scan.xml` & `nxswriter-3.9.0/XMLExamples/scan.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/scan2.xml` & `nxswriter-3.9.0/XMLExamples/scan2.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/scan3.xml` & `nxswriter-3.9.0/XMLExamples/scan3.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/test.xml` & `nxswriter-3.9.0/XMLExamples/test.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/XMLExamples/trigger.xml` & `nxswriter-3.9.0/XMLExamples/trigger.xml`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc/Makefile` & `nxswriter-3.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc/conf.py` & `nxswriter-3.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc/make.bat` & `nxswriter-3.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc/nxswriter.rst` & `nxswriter-3.9.0/doc/nxswriter.rst`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrCanFail.html` & `nxswriter-3.9.0/doc_html/AttrCanFail.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrCurrentFileId.html` & `nxswriter-3.9.0/doc_html/AttrCurrentFileId.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrErrors.html` & `nxswriter-3.9.0/doc_html/AttrErrors.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrFileName.html` & `nxswriter-3.9.0/doc_html/AttrFileName.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrJSONRecord.html` & `nxswriter-3.9.0/doc_html/AttrJSONRecord.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrSkipAcquisition.html` & `nxswriter-3.9.0/doc_html/AttrSkipAcquisition.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrStepsPerFile.html` & `nxswriter-3.9.0/doc_html/AttrStepsPerFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/AttrXMLSettings.html` & `nxswriter-3.9.0/doc_html/AttrXMLSettings.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/Attributes.html` & `nxswriter-3.9.0/doc_html/Attributes.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/ClassDescription.html` & `nxswriter-3.9.0/doc_html/ClassDescription.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdCloseEntry.html` & `nxswriter-3.9.0/doc_html/CmdCloseEntry.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdCloseEntryAsynch.html` & `nxswriter-3.9.0/doc_html/CmdCloseEntryAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdCloseFile.html` & `nxswriter-3.9.0/doc_html/CmdCloseFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdOpenEntry.html` & `nxswriter-3.9.0/doc_html/CmdOpenEntry.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdOpenEntryAsynch.html` & `nxswriter-3.9.0/doc_html/CmdOpenEntryAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdOpenFile.html` & `nxswriter-3.9.0/doc_html/CmdOpenFile.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdRecord.html` & `nxswriter-3.9.0/doc_html/CmdRecord.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdRecordAsynch.html` & `nxswriter-3.9.0/doc_html/CmdRecordAsynch.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdState.html` & `nxswriter-3.9.0/doc_html/CmdState.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/CmdStatus.html` & `nxswriter-3.9.0/doc_html/CmdStatus.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/Commands.html` & `nxswriter-3.9.0/doc_html/Commands.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/FullDocument.html` & `nxswriter-3.9.0/doc_html/FullDocument.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/Properties.html` & `nxswriter-3.9.0/doc_html/Properties.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/States.html` & `nxswriter-3.9.0/doc_html/States.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/TitleBanner.html` & `nxswriter-3.9.0/doc_html/TitleBanner.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/doc_html/index.html` & `nxswriter-3.9.0/doc_html/index.html`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/man/NXSDataWriter.1` & `nxswriter-3.9.0/man/NXSDataWriter.1`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/man/nxsfromxml.1` & `nxswriter-3.9.0/man/nxsfromxml.1`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/man/nxswriter.1` & `nxswriter-3.9.0/man/nxswriter.1`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 $ python setup.py install
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Debian packages
 .sp
-Debian \fIbullseye\fP, \fIbuster\fP, \fIstretch\fP  or Ubuntu \fIfocal\fP, \fIbionic\fP packages can be found in the HDRI repository.
+Debian \fIbookworm\fP,  \fIbullseye\fP, \fIbuster\fP  or Ubuntu \fIlunar\fP,  \fIjammy\fP, \fIfocal\fP packages can be found in the HDRI repository.
 .sp
 To install the debian packages, add the PGP repository key
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
@@ -98,15 +98,15 @@
 and then download the corresponding source list
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 $ cd /etc/apt/sources.list.d
-$ wget http://repos.pni\-hdri.de/bullseye\-pni\-hdri.list
+$ wget http://repos.pni\-hdri.de/bookworm\-pni\-hdri.list
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 To install tango server
 .INDENT 0.0
```

### Comparing `nxswriter-3.8.2/nxswriter/ClientSource.py` & `nxswriter-3.9.0/nxswriter/ClientSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DBaseSource.py` & `nxswriter-3.9.0/nxswriter/DBaseSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DataHolder.py` & `nxswriter-3.9.0/nxswriter/DataHolder.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DataSourceFactory.py` & `nxswriter-3.9.0/nxswriter/DataSourceFactory.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DataSourcePool.py` & `nxswriter-3.9.0/nxswriter/DataSourcePool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DataSources.py` & `nxswriter-3.9.0/nxswriter/DataSources.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/DecoderPool.py` & `nxswriter-3.9.0/nxswriter/DecoderPool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/EAttribute.py` & `nxswriter-3.9.0/nxswriter/EAttribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,22 +160,19 @@
         if self.name and not self.h5Object:
             self.h5Object = self.last.h5Attribute(self.name)
         shape = list(self.h5Object.shape)
 
         nptype = self.h5Object.dtype
         value = ''
 
-        if nptype != "string":
+        if nptype == "bool":
+            value = False
+        elif nptype != "string":
             try:
-                # workaround for bug #5618 in numpy for 1.8 < ver < 1.9.2
-                #
-                if nptype == 'uint64':
-                    value = numpy.iinfo(getattr(numpy, 'int64')).max
-                else:
-                    value = numpy.iinfo(getattr(numpy, nptype)).max
+                value = numpy.iinfo(getattr(numpy, nptype)).max
             except Exception:
                 try:
                     try:
                         value = numpy.finfo(getattr(numpy, nptype)).max.item()
                     except Exception:
                         value = numpy.asscalar(
                             numpy.finfo(getattr(numpy, nptype)).max)
```

### Comparing `nxswriter-3.8.2/nxswriter/EField.py` & `nxswriter-3.9.0/nxswriter/EField.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
         FElementWithAttr.__init__(self, "field", attrs, last, streams=streams,
                                   reloadmode=reloadmode)
         #: (:obj:`str`) rank of the field
         self.rank = "0"
         #: (:obj:`dict` <:obj:`str`, :obj:`str`>) \
         #:        shape of the field, i.e. {index: length}
         self.lengths = {}
+        #: (:obj:`dict` <:obj:`int`, \
+        #:        (:obj:`int`, :obj:`str`, :obj:`str`, :obj:`str`) >) \
+        #:        index filter lists, i.e. \
+        #:        {index: (filter_id, name, id, cd_values, availability)}
+        self.filters = {}
         #: (:obj:`bool`) True if field is stored in STEP mode
         self.__extraD = False
         #: (:obj:`str`) strategy, i.e. INIT, STEP, FINAL, POSTRUN
         self.strategy = 'INIT'
         #: (:obj:`str`) trigger for asynchronous writing
         self.trigger = None
         #: (:obj:`int`) growing dimension
@@ -154,20 +159,49 @@
                 return f
 
         chunk = [s if s > 0 else 1 for s in shape]
         minshape = [1 if s > 0 else 0 for s in shape]
         datafilter = None
         # create Filter
 
-        if self.compression:
+        datafilters = []
+        if (self.compression and self.rate) or self.shuffle:
             datafilter = FileWriter.data_filter(self._lastObject())
-            datafilter.rate = self.rate
-            datafilter.shuffle = self.shuffle
-            datafilter.options = tuple(self.compression_opts)
-            datafilter.filterid = self.compression
+            if (self.compression and self.rate):
+                datafilter.rate = self.rate
+                datafilter.options = tuple(self.compression_opts)
+                datafilter.shuffle = self.shuffle
+                datafilter.filterid = self.compression
+            if self.shuffle:
+                datafilter.shuffle = self.shuffle
+            datafilters.append(datafilter)
+        if self.filters:
+            mindex = max(self.filters.keys())
+            for ind in range(mindex):
+                if ind in self.filters:
+                    (filter_id, fname, cd_values, availability) = \
+                        self.filters[ind]
+                    datafilter = FileWriter.data_filter(self._lastObject())
+
+                    datafilter.name = fname
+                    datafilter.filterid = filter_id
+                    datafilter.availability = availability
+                    try:
+                        if cd_values:
+                            options = [int(vl) for vl in cd_values.split(",")]
+                            datafilter.options = tuple(options)
+                    except Exception:
+                        if self._streams:
+                            self._streams.error(
+                                "EField::__createObject() - "
+                                "Wrong filter cd_values ",
+                                std=False)
+
+                            raise Exception("Wrong filter cd_values")
+                    datafilters.append(datafilter)
 
         if sys.version_info < (3,):
             name = name.encode()
             dtype = dtype.encode()
 
         try:
             if shape:
@@ -189,17 +223,17 @@
                     f = self._lastObject().create_field(
                         name, dtype)
                 else:
                     if self.strategy in ['INIT', 'FINAL', None]:
                         mshape = [1]
                     else:
                         mshape = [0]
-                    if datafilter:
+                    if datafilters:
                         f = self._lastObject().create_field(
-                            name, dtype, mshape, [1], datafilter)
+                            name, dtype, mshape, [1], datafilters)
                     else:
                         f = self._lastObject().create_field(
                             name, dtype, mshape, [1])
         except Exception:
             info = sys.exc_info()
             import traceback
             message = str(info[1].__str__()) + "\n " + (" ").join(
@@ -601,20 +635,15 @@
         shape = [s if s > 0 else 1 for s in shape]
         self.__growshape(shape)
 
         if nptype == "bool":
             value = False
         elif nptype != "string":
             try:
-                # workaround for bug #5618 in numpy for 1.8 < ver < 1.9.2
-                #
-                if nptype == 'uint64':
-                    value = numpy.iinfo(getattr(numpy, 'int64')).max
-                else:
-                    value = numpy.iinfo(getattr(numpy, nptype)).max
+                value = numpy.iinfo(getattr(numpy, nptype)).max
             except Exception:
                 try:
                     try:
                         value = numpy.finfo(getattr(numpy, nptype)).max.item()
                     except Exception:
                         value = numpy.asscalar(
                             numpy.finfo(getattr(numpy, nptype)).max)
```

### Comparing `nxswriter-3.8.2/nxswriter/EGroup.py` & `nxswriter-3.9.0/nxswriter/EGroup.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/ELink.py` & `nxswriter-3.9.0/nxswriter/ELink.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/EStrategy.py` & `nxswriter-3.9.0/nxswriter/EStrategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,17 +72,17 @@
                          for vl in attrs["compression_opts"].split(",")]
                 if "rate" in attrs.keys() and hasattr(self.last, "rate"):
                     self.last.rate = int(attrs["rate"])
                     if self.last.rate < 0:
                         self.last.rate = 0
                     if self.last.rate > 9:
                         self.last.rate = 9
-                if "shuffle" in attrs.keys() and hasattr(self.last, "shuffle"):
-                    self.last.shuffle = False \
-                        if attrs["shuffle"].upper() == "FALSE" else True
+            if "shuffle" in attrs.keys() and hasattr(self.last, "shuffle"):
+                self.last.shuffle = False \
+                    if attrs["shuffle"].upper() == "FALSE" else True
 
     def store(self, xml=None, globalJSON=None):
         """ stores the tag content
 
         :param xml: xml setting
         :type xml: :obj:`str`
         :param globalJSON: global JSON string
```

### Comparing `nxswriter-3.8.2/nxswriter/Element.py` & `nxswriter-3.9.0/nxswriter/Element.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/ElementThread.py` & `nxswriter-3.9.0/nxswriter/ElementThread.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/Errors.py` & `nxswriter-3.9.0/nxswriter/Errors.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/FElement.py` & `nxswriter-3.9.0/nxswriter/FElement.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/FetchNameHandler.py` & `nxswriter-3.9.0/nxswriter/FetchNameHandler.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/H5Elements.py` & `nxswriter-3.9.0/nxswriter/H5Elements.py`

 * *Files 23% similar despite different names*

```diff
@@ -167,7 +167,53 @@
         if self.__index is not None and self.source:
             dt = self.source.getData()
             if dt and isinstance(dt, dict):
                 dh = DataHolder(streams=self._streams, **dt)
                 if dh:
                     self._beforeLast().lengths[self.__index] = str(
                         dh.cast("string"))
+
+
+class EFilter(Element):
+
+    """ filter tag element
+    """
+
+    def __init__(self, attrs, last, streams=None):
+        """ constructor
+
+        :param attrs: dictionary of the tag attributes
+        :type attrs: :obj:`dict` <:obj:`str`, :obj:`str`>
+        :param last: the last element from the stack
+        :type last: :class:`nxswriter.Element.Element`
+        :param streams: tango-like steamset class
+        :type streams: :class:`StreamSet` or :class:`tango.Device_4Impl`
+        """
+        Element.__init__(self, "filter", attrs, last, streams=streams)
+        index = 0
+        try:
+            if ("index" in attrs.keys()):
+                index = int(attrs["index"])
+        except Exception:
+            pass
+        try:
+            filter_id = int(attrs["id"])
+        except Exception:
+            filter_id = 0
+        try:
+            name = attrs["name"]
+        except Exception:
+            name = ""
+        try:
+            cd_values = attrs["cd_values"]
+        except Exception:
+            cd_values = ""
+        try:
+            availability = attrs["availability"]
+        except Exception:
+            availability = ""
+
+        if filter_id or name:
+            self._beforeLast().filters[index] = (
+                filter_id, name, cd_values, availability)
+        #: (:obj:`int`) index attribute
+        self.__index = index
```

### Comparing `nxswriter-3.8.2/nxswriter/InnerXMLParser.py` & `nxswriter-3.9.0/nxswriter/InnerXMLParser.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/Metadata.py` & `nxswriter-3.9.0/nxswriter/Metadata.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/NXSFromXML.py` & `nxswriter-3.9.0/nxswriter/NXSFromXML.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/NXSWriter.py` & `nxswriter-3.9.0/nxswriter/NXSWriter.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/NexusXMLHandler.py` & `nxswriter-3.9.0/nxswriter/NexusXMLHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from .FElement import FElement
 from .EGroup import EGroup
 from .EField import EField
 from .EAttribute import EAttribute
 from .EStrategy import EStrategy
 from .ELink import ELink
 from .H5Elements import (
-    EDoc, ESymbol, EDimensions, EDim, EFile)
+    EDoc, ESymbol, EDimensions, EDim, EFile, EFilter)
 from .DataSourceFactory import DataSourceFactory
 from .ThreadPool import ThreadPool
 from .InnerXMLParser import InnerXMLHandler
 from .Errors import UnsupportedTagError
 from .FetchNameHandler import TNObject
 
 
@@ -117,15 +117,15 @@
         #: map of tag names to related classes
         self.elementClass = {
             'group': EGroup, 'field': EField,
             'attribute': EAttribute, 'link': ELink,
             'symbols': Element, 'symbol': ESymbol,
             'dimensions': EDimensions, 'dim': EDim,
             'enumeration': Element, 'item': Element,
-            'strategy': EStrategy
+            'strategy': EStrategy, 'filter': EFilter
         }
 
         #: (:obj:`list` <:obj:`dict` <:obj:`str`, :obj:`str` > >) \
         #: list of entry group attributes
         self.entryAttrs = []
 
         #: (:obj:`dict` <:obj:`str`, :obj:`type` > ) \
```

### Comparing `nxswriter-3.8.2/nxswriter/PyEvalSource.py` & `nxswriter-3.9.0/nxswriter/PyEvalSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/Release.py` & `nxswriter-3.9.0/nxswriter/Release.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """ Tango Data Writer realease"""
 
 
 #: package version
-__version__ = "3.8.2"
+__version__ = "3.9.0"
```

### Comparing `nxswriter-3.8.2/nxswriter/StreamSet.py` & `nxswriter-3.9.0/nxswriter/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/TangoDataWriter.py` & `nxswriter-3.9.0/nxswriter/TangoDataWriter.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/TangoSource.py` & `nxswriter-3.9.0/nxswriter/TangoSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/ThreadPool.py` & `nxswriter-3.9.0/nxswriter/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/Types.py` & `nxswriter-3.9.0/nxswriter/Types.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter/__init__.py` & `nxswriter-3.9.0/nxswriter/__init__.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/nxswriter.egg-info/PKG-INFO` & `nxswriter-3.9.0/nxswriter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxswriter
-Version: 3.8.2
+Version: 3.9.0
 Summary: Nexus Data writer implemented as a Tango Server
 Home-page: https://github.com/nexdatas/nxsdatawriter
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to NXSDataWriter's documentation!
         =========================================
@@ -68,30 +68,30 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         """""""""""""""
         
-        Debian `bullseye`, `buster`  or Ubuntu `focal`, `bionic` packages can be found in the HDRI repository.
+        Debian `bookworm`, `bullseye`, `buster`  or Ubuntu `lunar`, `jammy`, `focal`  packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ curl -s http://repos.pni-hdri.de/debian_repo.pub.gpg | gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/debian-hdri-repo.gpg --import
         	  $ chmod 644 /etc/apt/trusted.gpg.d/debian-hdri-repo.gpg
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
         
         To install tango server
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install nxswriter
```

### Comparing `nxswriter-3.8.2/nxswriter.egg-info/SOURCES.txt` & `nxswriter-3.9.0/nxswriter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/setup.py` & `nxswriter-3.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 
 #: required python packages
 install_requires = [
     'pytz',
     'lxml',
     'numpy>1.6.0',
-    'fabio',
-    # 'nxstools',  # '>=3.30.0'
+    # 'fabio',
+    'nxstools>=3.50.0',
     # 'h5py',
     # 'pymysqldb',
     # 'psycopg2-binary'
     # 'psycopg2'
     # 'cx-oracle',
     # 'pytango',
     # 'pninexus',
```

### Comparing `nxswriter-3.8.2/test/Checkers.py` & `nxswriter-3.9.0/test/Checkers.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
                 else:
                     self._tc.assertEqual(values[i], value[i])
         for i in range(len(values)):
             cv = cnt[i]
             #            if self._isNumeric(cnt[i]):
             if self._isNumeric(cv):
                 if nxtype == "NX_BOOLEAN":
-                    #    print "BOOL: ", values[i] ,cnt[i]
+                    # print( "BOOL: ", values[i] ,cnt[i])
                     self._tc.assertEqual(
                         Types.Converters.toBool(values[i]), cnt[i])
                 else:
                     self._tc.assertTrue(abs(values[i] - cnt[i]) <= error)
             else:
                 # print("ONE")
                 # print(values)
```

### Comparing `nxswriter-3.8.2/test/ClientFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.9.0/test/ClientFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ClientFieldTagAsynchH5PY_test.py` & `nxswriter-3.9.0/test/ClientFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ClientFieldTagServerH5Cpp_test.py` & `nxswriter-3.9.0/test/ClientFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ClientFieldTagServerH5PY_test.py` & `nxswriter-3.9.0/test/ClientFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ClientFieldTagWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/ClientFieldTagWriterH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             det, "mclient_ucounter32", "uint32", "NX_UINT32",
             [abs(c) for c in self._counter])
         self._sc.checkScalarField(det, "ucounter64", "uint64", "NX_UINT64",
                                   [abs(c) for c in self._counter])
         self._sc.checkScalarField(
             det, "ucounter64_canfail", "uint64", "NX_UINT64",
             [self._counter[i] if not i % 2 else
-             numpy.iinfo(getattr(numpy, 'int64')).max
+             numpy.iinfo(getattr(numpy, 'uint64')).max
              for i in range(len(self._counter))],
             attrs={
                 "type": "NX_UINT64", "units": "m", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP",
                 "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkSingleScalarField(
@@ -1732,22 +1732,22 @@
         print(field.read(), logical)
         self._sc.checkSpectrumAttribute(
             field, "flag_spectrum_string", "string",
             logical)
 
         self._sc.checkSpectrumAttribute(
             det, "spectrum_uint64_canfail", "uint64",
-            [numpy.iinfo(getattr(numpy, 'int64')).max] * 1024)
+            [numpy.iinfo(getattr(numpy, 'uint64')).max] * 1024)
         self._sc.checkSpectrumAttribute(
             det, "spectrum_bool_canfail", "bool",
             [False] * 8)
 
         self._sc.checkSpectrumAttribute(
             field, "final_spectrum_uint64_canfail", "uint64",
-            [numpy.iinfo(getattr(numpy, 'int64')).max] * 256)
+            [numpy.iinfo(getattr(numpy, 'uint64')).max] * 256)
         self._sc.checkSpectrumAttribute(
             field, "init_spectrum_bool_canfail", "bool",
             [False] * 8)
 
         self._sc.checkScalarAttribute(
             det, "nexdatas_canfail", "string", "FAILED")
         self._sc.checkScalarAttribute(
@@ -2016,15 +2016,15 @@
              for rpco in self._pco1[0]],
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkSingleImageField(
             det, "final_pco_uint_canfail", "uint64", "NX_UINT",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max for el in rpco]
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max for el in rpco]
              for rpco in self._pco1[0]],
             attrs={"type": "NX_UINT", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "FINAL", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkImageField(
             det, "pco_uint8_canfail", "uint8", "NX_UINT8",
@@ -2822,15 +2822,15 @@
             field, "image_uint32", "uint32", self._pco1[steps - 1])
         self._sc.checkImageAttribute(
             field, "image_uint64", "uint64", self._pco1[0])
         self._sc.checkImageAttribute(field, "image_bool", "bool", logical)
 
         self._sc.checkImageAttribute(
             field, "image_uint64_canfail", "uint64",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max] *
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max] *
              len(self._pco1[0][0])] * len(self._pco1[0]))
         self._sc.checkImageAttribute(
             field, "image_bool_canfail", "bool",
             [[False] * len(logical[0])] * len(logical))
         self._sc.checkImageAttribute(
             det, "image_float_canfail", "float64",
             [[numpy.finfo(getattr(numpy, 'float64')).max] * 30] * 20)
```

### Comparing `nxswriter-3.8.2/test/ClientFieldTagWriterH5PY_test.py` & `nxswriter-3.9.0/test/ClientFieldTagWriterH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             det, "mclient_ucounter32", "uint32", "NX_UINT32",
             [abs(c) for c in self._counter])
         self._sc.checkScalarField(det, "ucounter64", "uint64", "NX_UINT64",
                                   [abs(c) for c in self._counter])
         self._sc.checkScalarField(
             det, "ucounter64_canfail", "uint64", "NX_UINT64",
             [self._counter[i] if not i % 2 else
-             numpy.iinfo(getattr(numpy, 'int64')).max
+             numpy.iinfo(getattr(numpy, 'uint64')).max
              for i in range(len(self._counter))],
             attrs={
                 "type": "NX_UINT64", "units": "m", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP",
                 "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkSingleScalarField(
@@ -1710,21 +1710,21 @@
             field, "init_spectrum_bool", "bool", logical)
         # NOT SUPPORTED BY PNINX
 # self._sc.checkSpectrumAttribute(field, "flag_spectrum_string", "string",
 # logical)
 
         self._sc.checkSpectrumAttribute(
             det, "spectrum_uint64_canfail", "uint64",
-            [numpy.iinfo(getattr(numpy, 'int64')).max] * 1024)
+            [numpy.iinfo(getattr(numpy, 'uint64')).max] * 1024)
         self._sc.checkSpectrumAttribute(det, "spectrum_bool_canfail", "bool",
                                         [False] * 8)
 
         self._sc.checkSpectrumAttribute(
             field, "final_spectrum_uint64_canfail", "uint64",
-            [numpy.iinfo(getattr(numpy, 'int64')).max] * 256)
+            [numpy.iinfo(getattr(numpy, 'uint64')).max] * 256)
         self._sc.checkSpectrumAttribute(
             field, "init_spectrum_bool_canfail", "bool",
             [False] * 8)
 
         self._sc.checkScalarAttribute(
             det, "nexdatas_canfail", "string", "FAILED")
         self._sc.checkScalarAttribute(
@@ -1992,15 +1992,15 @@
              for rpco in self._pco1[0]],
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkSingleImageField(
             det, "final_pco_uint_canfail", "uint64", "NX_UINT",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max for el in rpco]
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max for el in rpco]
              for rpco in self._pco1[0]],
             attrs={"type": "NX_UINT", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "FINAL",
                    "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkImageField(
@@ -2796,15 +2796,15 @@
             field, "image_uint32", "uint32", self._pco1[steps - 1])
         self._sc.checkImageAttribute(
             field, "image_uint64", "uint64", self._pco1[0])
         self._sc.checkImageAttribute(field, "image_bool", "bool", logical)
 
         self._sc.checkImageAttribute(
             field, "image_uint64_canfail", "uint64",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max] *
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max] *
              len(self._pco1[0][0])] * len(self._pco1[0]))
         self._sc.checkImageAttribute(
             field, "image_bool_canfail", "bool",
             [[False] * len(logical[0])] * len(logical))
         self._sc.checkImageAttribute(
             det, "image_float_canfail", "float64",
             [[numpy.finfo(getattr(numpy, 'float64')).max] * 30] * 20)
```

### Comparing `nxswriter-3.8.2/test/ClientSource_test.py` & `nxswriter-3.9.0/test/ClientSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/Converters_test.py` & `nxswriter-3.9.0/test/Converters_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DBFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.9.0/test/DBFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DBFieldTagAsynchH5PY_test.py` & `nxswriter-3.9.0/test/DBFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DBFieldTagServerH5Cpp_test.py` & `nxswriter-3.9.0/test/DBFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DBFieldTagServerH5PY_test.py` & `nxswriter-3.9.0/test/DBFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DBFieldTagWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/DBFieldTagWriterH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,15 +733,15 @@
         self._sc.checkScalarField(
             det, "pid_scalar4_string", "string", "NX_CHAR", [''] * 3,
             attrs={"type": "NX_CHAR", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "pid_scalar_uint", "uint64", "NX_UINT", [
-                numpy.iinfo(getattr(numpy, 'int64')).max] * 3,
+                numpy.iinfo(getattr(numpy, 'uint64')).max] * 3,
             attrs={"type": "NX_UINT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "pid_scalar_int64", "int64", "NX_INT64", [
                 numpy.iinfo(getattr(numpy, 'int64')).max] * 3,
             attrs={"type": "NX_INT64", "units": "m", "nexdatas_source": None,
@@ -2414,15 +2414,15 @@
             attrs={"type": "NX_FLOAT", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkImageField(
             det, "pid_image_uint", "uint64", "NX_UINT",
             [[[numpy.iinfo(
-                getattr(numpy, 'int64')).max]]] * 3,
+                getattr(numpy, 'uint64')).max]]] * 3,
             attrs={
                 "type": "NX_UINT", "units": "", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkSingleImageField(
             det, "final_pid_image_float", "float64", "NX_FLOAT",
             [[numpy.finfo(
```

### Comparing `nxswriter-3.8.2/test/DBFieldTagWriterH5PY_test.py` & `nxswriter-3.9.0/test/DBFieldTagWriterH5PY_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,15 +734,15 @@
         self._sc.checkScalarField(
             det, "pid_scalar4_string", "string", "NX_CHAR", [''] * 3,
             attrs={"type": "NX_CHAR", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "pid_scalar_uint", "uint64", "NX_UINT", [
-                numpy.iinfo(getattr(numpy, 'int64')).max] * 3,
+                numpy.iinfo(getattr(numpy, 'uint64')).max] * 3,
             attrs={"type": "NX_UINT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "pid_scalar_int64", "int64", "NX_INT64", [
                 numpy.iinfo(getattr(numpy, 'int64')).max] * 3,
             attrs={"type": "NX_INT64", "units": "m", "nexdatas_source": None,
@@ -2420,15 +2420,15 @@
                 getattr(numpy, 'float64')).max]],
             attrs={"type": "NX_FLOAT", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
 
         self._sc.checkImageField(
             det, "pid_image_uint", "uint64", "NX_UINT",
-            [[[numpy.iinfo(getattr(numpy, 'int64')).max]]] * 3,
+            [[[numpy.iinfo(getattr(numpy, 'uint64')).max]]] * 3,
             attrs={
                 "type": "NX_UINT", "units": "", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkSingleImageField(
             det, "final_pid_image_float", "float64", "NX_FLOAT",
             [[numpy.finfo(
```

### Comparing `nxswriter-3.8.2/test/DBaseSource_test.py` & `nxswriter-3.9.0/test/DBaseSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DataHolder_test.py` & `nxswriter-3.9.0/test/DataHolder_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             "ScalarShort": ["int16", "DevShort", -123],
             "ScalarUShort": ["uint16", "DevUShort", 1234],
             "ScalarLong": ["int64", "DevLong", -124],
             "ScalarULong": ["uint64", "DevULong", 234],
             "ScalarLong64": ["int64", "DevLong64", 234],
             "ScalarULong64": ["uint64", "DevULong64", 23],
             "ScalarFloat": ["float32", "DevFloat", 12.234, 1e-5],
-            "ScalarDouble": ["float64", "DevDouble", -2.456673e+02, 1e-14],
+            "ScalarDouble": ["float64", "DevDouble", -2.456673e+01, 1e-14],
             "ScalarString": ["string", "DevString", "MyTrue"],
             # "State":[ "string", "DevState", tango._tango.DevState.ON],
         }
 
         for a in arr:
 
             data = {"rank": "SCALAR",
@@ -384,29 +384,29 @@
         arrs = {}
 
         arrs["b"] = {
             "ScalarBoolean": ["bool", "DevBoolean", True],
         }
 
         arrs["i"] = {
-            "ScalarShort": ["int16", "DevShort", -123],
-            "ScalarLong": ["int64", "DevLong", -124],
+            "ScalarShort": ["int16", "DevShort", 123],
+            "ScalarLong": ["int64", "DevLong", 124],
             "ScalarLong64": ["int64", "DevLong64", 234],
         }
 
         arrs["u"] = {
             "ScalarUChar": ["uint8", "DevUChar", 23],
             "ScalarUShort": ["uint16", "DevUShort", 1234],
             "ScalarULong": ["uint64", "DevULong", 234],
             "ScalarULong64": ["uint64", "DevULong64", 23],
         }
 
         arrs["f"] = {
             "ScalarFloat": ["float32", "DevFloat", 12.234, 1e-5],
-            "ScalarDouble": ["float64", "DevDouble", -2.456673e+02, 1e-14],
+            "ScalarDouble": ["float64", "DevDouble", 2.456673e+02, 1e-14],
         }
 
         arrs["s"] = {
             "ScalarString": ["string", "DevString", "MyTrue"],
             # "State":[ "string", "DevState", tango._tango.DevState.ON],
         }
 
@@ -543,29 +543,29 @@
         arrs = {}
 
         arrs["b"] = {
             "SpectrumBoolean": ["bool", "DevBoolean", True, [1, 0]],
         }
 
         arrs["i"] = {
-            "SpectrumShort": ["int16", "DevShort", -13, [1, 0]],
-            "SpectrumLong": ["int64", "DevLong", -14, [1, 0]],
-            "SpectrumLong64": ["int64", "DevLong64", -24, [1, 0]],
+            "SpectrumShort": ["int16", "DevShort", 3, [1, 0]],
+            "SpectrumLong": ["int64", "DevLong", 4, [1, 0]],
+            "SpectrumLong64": ["int64", "DevLong64", 4, [1, 0]],
         }
 
         arrs["u"] = {
-            "SpectrumUChar": ["uint8", "DevUChar", 23, [1, 0]],
+            "SpectrumUChar": ["uint8", "DevUChar", 3, [1, 0]],
             "SpectrumULong": ["uint64", "DevULong", 2, [1, 0]],
             "SpectrumUShort": ["uint16", "DevUShort", 1, [1, 0]],
             "SpectrumULong64": ["uint64", "DevULong64", 3, [1, 0]],
         }
 
         arrs["f"] = {
             "SpectrumFloat": ["float32", "DevFloat", 12.234, [1, 0], 1e-5],
-            "SpectrumDouble": ["float64", "DevDouble", -2.456673e+02, [1, 0],
+            "SpectrumDouble": ["float64", "DevDouble", 2.156673e+01, [1, 0],
                                1e-14],
         }
 
         arrs["s"] = {
             "SpectrumString": ["string", "DevString", "MyTrue", [1, 0]],
             #  "State":[ "string", "DevState", tango._tango.DevState.ON],
         }
@@ -592,15 +592,15 @@
             arr = arrs[s]
             for k in arr:
 
                 if arr[k][1] != "DevBoolean":
                     mlen = [
                         self.__rnd.randint(1, 10), self.__rnd.randint(0, 3)]
                     arr[k][2] = [
-                        arr[k][2] * self.__rnd.randint(1, 3)
+                        arr[k][2] * self.__rnd.randint(1, 2)
                         for c in range(mlen[0])]
                 else:
                     mlen = [self.__rnd.randint(1, 10)]
                     arr[k][2] = [(True if self.__rnd.randint(0, 1) else False)
                                  for c in range(mlen[0])]
 
                 arr[k][3] = [mlen[0], 0]
@@ -650,29 +650,29 @@
         arrs = {}
 
         arrs["b"] = {
             "SpectrumBoolean": ["bool", "DevBoolean", True, [1, 0]],
         }
 
         arrs["i"] = {
-            "SpectrumShort": ["int16", "DevShort", -13, [1, 0]],
-            "SpectrumLong": ["int64", "DevLong", -14, [1, 0]],
-            "SpectrumLong64": ["int64", "DevLong64", -24, [1, 0]],
+            "SpectrumShort": ["int16", "DevShort", 3, [1, 0]],
+            "SpectrumLong": ["int64", "DevLong", 4, [1, 0]],
+            "SpectrumLong64": ["int64", "DevLong64", 5, [1, 0]],
         }
 
         arrs["u"] = {
-            "SpectrumUChar": ["uint8", "DevUChar", 23, [1, 0]],
+            "SpectrumUChar": ["uint8", "DevUChar", 7, [1, 0]],
             "SpectrumULong": ["uint64", "DevULong", 2, [1, 0]],
             "SpectrumUShort": ["uint16", "DevUShort", 1, [1, 0]],
             "SpectrumULong64": ["uint64", "DevULong64", 3, [1, 0]],
         }
 
         arrs["f"] = {
             "SpectrumFloat": ["float32", "DevFloat", 12.234, [1, 0], 1e-5],
-            "SpectrumDouble": ["float64", "DevDouble", -2.456673e+02, [1, 0],
+            "SpectrumDouble": ["float64", "DevDouble", 2.456673e+01, [1, 0],
                                1e-14],
         }
 
         arrs["s"] = {
             "SpectrumString": ["string", "DevString", "MyTrue", [1, 0]],
             #  "State":[ "string", "DevState", tango._tango.DevState.ON],
         }
@@ -699,15 +699,15 @@
             arr = arrs[s]
 
             for k in arr:
 
                 mlen = [self.__rnd.randint(1, 10), self.__rnd.randint(
                     1, 10), self.__rnd.randint(0, 3)]
                 if arr[k][1] != "DevBoolean":
-                    arr[k][2] = [[arr[k][2] * self.__rnd.randint(0, 3)
+                    arr[k][2] = [[arr[k][2] * self.__rnd.randint(0, 2)
                                   for r in range(mlen[1])]
                                  for c in range(mlen[0])]
                 else:
                     mlen = [
                         self.__rnd.randint(1, 10), self.__rnd.randint(1, 10)]
                     if arr[k][1] == 'DevBoolean':
                         arr[k][2] = [[(True if self.__rnd.randint(0, 1)
```

### Comparing `nxswriter-3.8.2/test/DataSourceDecoders_test.py` & `nxswriter-3.9.0/test/DataSourceDecoders_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DataSourceFactory_test.py` & `nxswriter-3.9.0/test/DataSourceFactory_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DataSourcePool_test.py` & `nxswriter-3.9.0/test/DataSourcePool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DataSource_test.py` & `nxswriter-3.9.0/test/DataSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/DecoderPool_test.py` & `nxswriter-3.9.0/test/DecoderPool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EAttributeH5Cpp_test.py` & `nxswriter-3.9.0/test/EAttributeH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1111,27 +1111,27 @@
                      "NX_INT8", "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", 1.e-5],
@@ -1294,27 +1294,27 @@
                      "NX_INT8", "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", 1.e-5],
@@ -1479,25 +1479,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1675,25 +1675,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1877,25 +1877,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2081,25 +2081,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2290,25 +2290,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2507,25 +2507,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
```

### Comparing `nxswriter-3.8.2/test/EAttributeH5PY_test.py` & `nxswriter-3.9.0/test/EAttributeH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1092,27 +1092,27 @@
                      "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", 1.e-5],
@@ -1275,27 +1275,27 @@
                      "NX_INT8", "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", 1.e-5],
@@ -1459,25 +1459,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1656,25 +1656,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT64",
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT64",
                        "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1857,25 +1857,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2060,25 +2060,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2262,25 +2262,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max, "NX_UINT8",
                       "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max, "NX_UINT16",
                        "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max, "NX_UINT32",
                        "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT64",
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT64",
                        "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2483,25 +2483,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
```

### Comparing `nxswriter-3.8.2/test/EDimH5Cpp_test.py` & `nxswriter-3.9.0/test/EDimH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EDimH5PY_test.py` & `nxswriter-3.9.0/test/EDimH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EDimensionsH5Cpp_test.py` & `nxswriter-3.9.0/test/EDimensionsH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EDimensionsH5PY_test.py` & `nxswriter-3.9.0/test/EDimensionsH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EDocH5Cpp_test.py` & `nxswriter-3.9.0/test/EDocH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EDocH5PY_test.py` & `nxswriter-3.9.0/test/EDocH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EFieldH5Cpp_test.py` & `nxswriter-3.9.0/test/EFieldH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2676,25 +2676,25 @@
                      "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
@@ -2920,25 +2920,25 @@
             "int16": [-223, "NX_INT16", "int16",
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [13235, "NX_INT32", "int32",
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12425, "NX_INT64", "int64",
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64",
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64",
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [65, "NX_UINT8", "uint8",
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [453, "NX_UINT16", "uint16",
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12235, "NX_UINT32", "uint32",
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [14345, "NX_UINT64", "uint64",
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[14345,"NX_UINT64",
             # "uint64",numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-16.345, "NX_FLOAT", "float64",
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-2.345e+2, "NX_NUMBER", "float64",
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-4.355e-1, "NX_FLOAT32", "float32",
@@ -3175,27 +3175,27 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max, "NX_UINT8",
                       "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", (1,), 1.e-5],
@@ -3467,25 +3467,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -3860,25 +3860,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -4144,25 +4144,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -4427,27 +4427,27 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", (1,), 1.e-5],
@@ -4714,27 +4714,27 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
                         numpy.finfo(getattr(numpy, 'float32')).max, 1.e-5],
             "float64": [-12.345, "NX_FLOAT64", "float64", (1,),
@@ -4994,25 +4994,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -5283,23 +5283,23 @@
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,), 1.e-14,
                       numpy.finfo(getattr(numpy, 'float64')).max],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,), 1.e-14,
                        numpy.finfo(getattr(numpy, 'float64')).max],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,), 1.e-5,
@@ -5566,25 +5566,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #  "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,"NX_UINT",
             # "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             # "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,"NX_UINT64",
             #      "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -5847,25 +5847,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -6132,25 +6132,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -6421,25 +6421,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64",
             # (1,), numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
```

### Comparing `nxswriter-3.8.2/test/EFieldH5PY_test.py` & `nxswriter-3.9.0/test/EFieldH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2683,25 +2683,25 @@
                      "NX_INT8", "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
@@ -2926,25 +2926,25 @@
             "int16": [-223, "NX_INT16", "int16",
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [13235, "NX_INT32", "int32",
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12425, "NX_INT64", "int64",
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64",
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT",
             # "uint64",numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [65, "NX_UINT8", "uint8",
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [453, "NX_UINT16", "uint16",
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12235, "NX_UINT32", "uint32",
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [14345, "NX_UINT64", "uint64",
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[14345,"NX_UINT64",
             #  "uint64",numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-16.345, "NX_FLOAT", "float64",
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-2.345e+2, "NX_NUMBER", "float64",
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-4.355e-1, "NX_FLOAT32", "float32",
@@ -3182,27 +3182,27 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", (1,), 1.e-5],
@@ -3478,25 +3478,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -3873,25 +3873,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -4157,25 +4157,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -4437,27 +4437,27 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
             "float32": [numpy.finfo(getattr(numpy, 'float32')).max,
                         "NX_FLOAT32", "float32", (1,), 1.e-5],
@@ -4724,27 +4724,27 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
                         numpy.finfo(getattr(numpy, 'float32')).max, 1.e-5],
             "float64": [-12.345, "NX_FLOAT64", "float64", (1,),
@@ -5005,25 +5005,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -5287,23 +5287,23 @@
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,), 1.e-14,
                       numpy.finfo(getattr(numpy, 'float64')).max],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,), 1.e-14,
                        numpy.finfo(getattr(numpy, 'float64')).max],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,), 1.e-5,
@@ -5564,25 +5564,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
 
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
@@ -5844,25 +5844,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -6130,25 +6130,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -6416,25 +6416,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
```

### Comparing `nxswriter-3.8.2/test/EFieldReshapeH5Cpp_test.py` & `nxswriter-3.9.0/test/EFieldReshapeH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,25 +244,25 @@
                      "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
@@ -486,25 +486,25 @@
             "int16": [-223, "NX_INT16", "int16",
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [13235, "NX_INT32", "int32",
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12425, "NX_INT64", "int64",
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64",
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64",
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [65, "NX_UINT8", "uint8",
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [453, "NX_UINT16", "uint16",
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12235, "NX_UINT32", "uint32",
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [14345, "NX_UINT64", "uint64",
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[14345,"NX_UINT64", "uint64",
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-16.345, "NX_FLOAT", "float64",
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-2.345e+2, "NX_NUMBER", "float64",
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-4.355e-1, "NX_FLOAT32", "float32",
@@ -735,25 +735,25 @@
                      "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max, "NX_INT16",
                       "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max, "NX_INT32",
                       "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_INT64",
                       "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max, "NX_UINT8",
                       "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max, "NX_UINT16",
                        "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max, "NX_UINT32",
                        "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT64",
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT64",
                        "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1023,25 +1023,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #   numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -1292,25 +1292,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1570,25 +1570,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -1846,25 +1846,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #       "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #      "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2129,25 +2129,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -2407,25 +2407,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2688,25 +2688,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #   numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,), 1.e-14,
                       numpy.finfo(getattr(numpy, 'float64')).max],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,), 1.e-14,
                        numpy.finfo(getattr(numpy, 'float64')).max],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,), 1.e-5,
@@ -2970,25 +2970,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #  "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -3238,25 +3238,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -3522,25 +3522,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -3799,27 +3799,27 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
                         numpy.finfo(getattr(numpy, 'float32')).max, 1.e-5],
             "float64": [-12.345, "NX_FLOAT64", "float64", (1,),
```

### Comparing `nxswriter-3.8.2/test/EFieldReshapeH5PY_test.py` & `nxswriter-3.9.0/test/EFieldReshapeH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,25 +245,25 @@
                      "NX_INT8", "int8"],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16"],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32"],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64"],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64"],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64"],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8"],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16"],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32"],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64"],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64"],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", 1.e-14],
@@ -488,25 +488,25 @@
             "int16": [-223, "NX_INT16", "int16",
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [13235, "NX_INT32", "int32",
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12425, "NX_INT64", "int64",
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64",
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64",
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [65, "NX_UINT8", "uint8",
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [453, "NX_UINT16", "uint16",
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12235, "NX_UINT32", "uint32",
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [14345, "NX_UINT64", "uint64",
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[14345,"NX_UINT64",
             # "uint64",numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-16.345, "NX_FLOAT", "float64",
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-2.345e+2, "NX_NUMBER", "float64",
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-4.355e-1, "NX_FLOAT32", "float32",
@@ -736,25 +736,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #   "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1021,25 +1021,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -1290,25 +1290,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #        "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -1567,25 +1567,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -1843,25 +1843,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2124,25 +2124,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -2402,25 +2402,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max, "NX_UINT",
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max, "NX_UINT",
                      "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             # "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -2679,25 +2679,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #      numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #   numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,), 1.e-14,
                       numpy.finfo(getattr(numpy, 'float64')).max],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,), 1.e-14,
                        numpy.finfo(getattr(numpy, 'float64')).max],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,), 1.e-5,
@@ -2960,25 +2960,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #            "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #             "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #            "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #            "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -3228,25 +3228,25 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             # numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
@@ -3512,25 +3512,25 @@
                      "NX_INT8", "int8", (1,)],
             "int16": [numpy.iinfo(getattr(numpy, 'int16')).max,
                       "NX_INT16", "int16", (1,)],
             "int32": [numpy.iinfo(getattr(numpy, 'int32')).max,
                       "NX_INT32", "int32", (1,)],
             "int64": [numpy.iinfo(getattr(numpy, 'int64')).max,
                       "NX_INT64", "int64", (1,)],
-            "uint": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                      "NX_UINT", "uint64", (1,)],
             #      "uint":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #             "NX_UINT", "uint64", (1,)],
             "uint8": [numpy.iinfo(getattr(numpy, 'uint8')).max,
                       "NX_UINT8", "uint8", (1,)],
             "uint16": [numpy.iinfo(getattr(numpy, 'uint16')).max,
                        "NX_UINT16", "uint16", (1,)],
             "uint32": [numpy.iinfo(getattr(numpy, 'uint32')).max,
                        "NX_UINT32", "uint32", (1,)],
-            "uint64": [numpy.iinfo(getattr(numpy, 'int64')).max,
+            "uint64": [numpy.iinfo(getattr(numpy, 'uint64')).max,
                        "NX_UINT64", "uint64", (1,)],
             #        "uint64":[numpy.iinfo(getattr(numpy, 'uint64')).max,
             #          "NX_UINT64", "uint64", (1,)],
             "float": [numpy.finfo(getattr(numpy, 'float64')).max,
                       "NX_FLOAT", "float64", (1,), 1.e-14],
             "number": [numpy.finfo(getattr(numpy, 'float64')).max,
                        "NX_NUMBER", "float64", (1,), 1.e-14],
@@ -3793,27 +3793,27 @@
             "int16": [-123, "NX_INT16", "int16", (1,),
                       numpy.iinfo(getattr(numpy, 'int16')).max],
             "int32": [12345, "NX_INT32", "int32", (1,),
                       numpy.iinfo(getattr(numpy, 'int32')).max],
             "int64": [-12345, "NX_INT64", "int64", (1,),
                       numpy.iinfo(getattr(numpy, 'int64')).max],
             "uint": [123, "NX_UINT", "uint64", (1,),
-                     numpy.iinfo(getattr(numpy, 'int64')).max],
+                     numpy.iinfo(getattr(numpy, 'uint64')).max],
             #            "uint":[123,"NX_UINT", "uint64", (1,),
             #       numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint8": [12, "NX_UINT8", "uint8", (1,),
                       numpy.iinfo(getattr(numpy, 'uint8')).max],
             "uint16": [123, "NX_UINT16", "uint16", (1,),
                        numpy.iinfo(getattr(numpy, 'uint16')).max],
             "uint32": [12345, "NX_UINT32", "uint32", (1,),
                        numpy.iinfo(getattr(numpy, 'uint32')).max],
             #            "uint64":[12345,"NX_UINT64", "uint64", (1,),
             #  numpy.iinfo(getattr(numpy, 'uint64')).max],
             "uint64": [12345, "NX_UINT64", "uint64", (1,),
-                       numpy.iinfo(getattr(numpy, 'int64')).max],
+                       numpy.iinfo(getattr(numpy, 'uint64')).max],
             "float": [-12.345, "NX_FLOAT", "float64", (1,),
                       numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "number": [-12.345e+2, "NX_NUMBER", "float64", (1,),
                        numpy.finfo(getattr(numpy, 'float64')).max, 1.e-14],
             "float32": [-12.345e-1, "NX_FLOAT32", "float32", (1,),
                         numpy.finfo(getattr(numpy, 'float32')).max, 1.e-5],
             "float64": [-12.345, "NX_FLOAT64", "float64", (1,),
```

### Comparing `nxswriter-3.8.2/test/EFileH5Cpp_test.py` & `nxswriter-3.9.0/test/EFileH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EFileH5PY_test.py` & `nxswriter-3.9.0/test/EFileH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EGroupH5Cpp_test.py` & `nxswriter-3.9.0/test/EGroupH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EGroupH5PY_test.py` & `nxswriter-3.9.0/test/EGroupH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ELinkH5Cpp_test.py` & `nxswriter-3.9.0/test/ELinkH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ELinkH5PY_test.py` & `nxswriter-3.9.0/test/ELinkH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/EStrategyH5Cpp_test.py` & `nxswriter-3.9.0/test/EStrategyH5Cpp_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,16 +178,16 @@
             el.grows, int(attrs["grows"]) if int(attrs["grows"]) > 0 else 1)
         self.assertEqual(
             st.last.compression, Converters.toBool(attrs["compression"]))
         self.assertEqual(
             el.compression, Converters.toBool(attrs["compression"]))
         self.assertEqual(st.last.rate, 2)
         self.assertEqual(el.rate, 2)
-        self.assertEqual(st.last.shuffle, True)
-        self.assertEqual(el.shuffle, True)
+        self.assertEqual(st.last.shuffle, False)
+        self.assertEqual(el.shuffle, False)
 
     # first constructor test
     # \brief It tests default settings
     def test_constructor_3(self):
         print("Run: %s.test_constructor() " % self.__class__.__name__)
         attrs = {}
         attrs["mode"] = "STEP"
```

### Comparing `nxswriter-3.8.2/test/EStrategyH5PY_test.py` & `nxswriter-3.9.0/test/EStrategyH5PY_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,16 @@
             el.grows, int(attrs["grows"]) if int(attrs["grows"]) > 0 else 1)
         self.assertEqual(
             st.last.compression, Converters.toBool(attrs["compression"]))
         self.assertEqual(
             el.compression, Converters.toBool(attrs["compression"]))
         self.assertEqual(st.last.rate, 2)
         self.assertEqual(el.rate, 2)
-        self.assertEqual(st.last.shuffle, True)
-        self.assertEqual(el.shuffle, True)
+        self.assertEqual(st.last.shuffle, False)
+        self.assertEqual(el.shuffle, False)
 
     # first constructor test
     # \brief It tests default settings
     def test_constructor_3(self):
         print("Run: %s.test_constructor() " % self.__class__.__name__)
         attrs = {}
         attrs["mode"] = "STEP"
```

### Comparing `nxswriter-3.8.2/test/ESymbolH5Cpp_test.py` & `nxswriter-3.9.0/test/ESymbolH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ESymbolH5PY_test.py` & `nxswriter-3.9.0/test/ESymbolH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ElementH5Cpp_test.py` & `nxswriter-3.9.0/test/ElementH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ElementH5PY_test.py` & `nxswriter-3.9.0/test/ElementH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ElementThread_test.py` & `nxswriter-3.9.0/test/ElementThread_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/Element_test.py` & `nxswriter-3.9.0/test/Element_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/Errors_test.py` & `nxswriter-3.9.0/test/Errors_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FElementH5Cpp_test.py` & `nxswriter-3.9.0/test/FElementH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FElementH5PY_test.py` & `nxswriter-3.9.0/test/FElementH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FElementWithAttrH5Cpp_test.py` & `nxswriter-3.9.0/test/FElementWithAttrH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FElementWithAttrH5PY_test.py` & `nxswriter-3.9.0/test/FElementWithAttrH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FetchNameHandler_test.py` & `nxswriter-3.9.0/test/FetchNameHandler_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/FileWriterH5CppH5PY_test.py` & `nxswriter-3.9.0/test/FileWriterH5CppH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4569,23 +4569,23 @@
             det.create_field(
                 "intvec", "uint32", [0, 2, 30], dfilter=df2)
 
             self.assertEqual(df0.rate, 0)
             self.assertEqual(df0.shuffle, False)
             self.assertEqual(df0.parent, None)
             print(df0.h5object)
-            self.assertTrue(isinstance(df0.h5object, h5cpp.filter.Filter))
+            # self.assertTrue(isinstance(df0.h5object, h5cpp.filter.Filter))
             self.assertEqual(df1.rate, 2)
             self.assertEqual(df1.shuffle, False)
             self.assertEqual(df1.parent, None)
-            self.assertTrue(isinstance(df1.h5object, h5cpp.filter.Filter))
+            # self.assertTrue(isinstance(df1.h5object, h5cpp.filter.Filter))
             self.assertEqual(df2.rate, 4)
             self.assertEqual(df2.shuffle, True)
             self.assertEqual(df2.parent, None)
-            self.assertTrue(isinstance(df2.h5object, h5cpp.filter.Filter))
+            # self.assertTrue(isinstance(df2.h5object, h5cpp.filter.Filter))
         finally:
             os.remove(self._fname)
 
     # default createfile test
     # \brief It tests default settings
     def test_h5pydeflate(self):
         fun = sys._getframe().f_code.co_name
```

### Comparing `nxswriter-3.8.2/test/FileWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/FileWriterH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2730,23 +2730,23 @@
             # intvec =
             det.create_field(
                 "intvec", "uint32", [0, 2, 30], dfilter=df2)
 
             self.assertEqual(df0.rate, 0)
             self.assertEqual(df0.shuffle, False)
             self.assertEqual(df0.parent, None)
-            self.assertTrue(isinstance(df0.h5object, h5cpp._filter.Deflate))
+            # self.assertTrue(isinstance(df0.h5object, h5cpp._filter.Deflate))
             self.assertEqual(df1.rate, 2)
             self.assertEqual(df1.shuffle, False)
             self.assertEqual(df1.parent, None)
-            self.assertTrue(isinstance(df1.h5object, h5cpp._filter.Deflate))
+            # self.assertTrue(isinstance(df1.h5object, h5cpp._filter.Deflate))
             self.assertEqual(df2.rate, 4)
             self.assertEqual(df2.shuffle, True)
             self.assertEqual(df2.parent, None)
-            self.assertTrue(isinstance(df2.h5object, h5cpp._filter.Deflate))
+            # self.assertTrue(isinstance(df2.h5object, h5cpp._filter.Deflate))
         finally:
             os.remove(self._fname)
 
     # default createfile test
     # \brief It tests default settings
     def test_h5cppattributemanager(self):
         fun = sys._getframe().f_code.co_name
```

### Comparing `nxswriter-3.8.2/test/FileWriterH5PY_test.py` & `nxswriter-3.9.0/test/FileWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/H5CppWriter_test.py` & `nxswriter-3.9.0/test/H5CppWriter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2321,24 +2321,24 @@
                 "floatvec", "float64", [1, 20, 10], [1, 10, 10], dfilter=df1)
             det.create_field(
                 "intvec", "uint32", [0, 2, 30], dfilter=df2)
 
             self.assertEqual(df0.rate, 0)
             self.assertEqual(df0.shuffle, False)
             self.assertEqual(df0.parent, None)
-            print(type(df0.h5object))
-            self.assertTrue(isinstance(df0.h5object, h5cpp._filter.Deflate))
+            # print(type(df0.h5object))
+            # self.assertTrue(isinstance(df0.h5object, h5cpp._filter.Deflate))
             self.assertEqual(df1.rate, 2)
             self.assertEqual(df1.shuffle, False)
             self.assertEqual(df1.parent, None)
-            self.assertTrue(isinstance(df1.h5object, h5cpp._filter.Deflate))
+            # self.assertTrue(isinstance(df1.h5object, h5cpp._filter.Deflate))
             self.assertEqual(df2.rate, 4)
             self.assertEqual(df2.shuffle, True)
             self.assertEqual(df2.parent, None)
-            self.assertTrue(isinstance(df2.h5object, h5cpp._filter.Deflate))
+            # self.assertTrue(isinstance(df2.h5object, h5cpp._filter.Deflate))
         finally:
             os.remove(self._fname)
 
     # default createfile test
     # \brief It tests default settings
     def test_h5cppbitshuffle(self):
         fun = sys._getframe().f_code.co_name
@@ -2384,26 +2384,26 @@
                     dfilter=df1)
                 det.create_field(
                     "intvec", "uint32", [0, 2, 30], dfilter=df2)
 
                 self.assertEqual(df0.rate, 0)
                 self.assertEqual(df0.shuffle, False)
                 self.assertEqual(df0.parent, None)
-                self.assertTrue(isinstance(df0.h5object,
-                                           h5cpp._filter.Deflate))
+                # self.assertTrue(isinstance(df0.h5object,
+                #                            h5cpp._filter.Deflate))
                 self.assertEqual(df1.rate, 0)
                 self.assertEqual(df1.shuffle, False)
                 self.assertEqual(df1.parent, None)
-                self.assertTrue(isinstance(df1.h5object,
-                                           h5cpp._filter.Deflate))
+                # self.assertTrue(isinstance(df1.h5object,
+                #                            h5cpp._filter.Deflate))
                 self.assertEqual(df2.rate, 0)
                 self.assertEqual(df2.shuffle, True)
                 self.assertEqual(df2.parent, None)
-                self.assertTrue(isinstance(df2.h5object,
-                                           h5cpp._filter.Deflate))
+                # self.assertTrue(isinstance(df2.h5object,
+                #                            h5cpp._filter.Deflate))
             finally:
                 os.remove(self._fname)
         else:
             print("Skip: %s.%s() " % (self.__class__.__name__, fun))
 
     # default createfile test
     # \brief It tests default settings
```

### Comparing `nxswriter-3.8.2/test/H5PYWriter_test.py` & `nxswriter-3.9.0/test/H5PYWriter_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/InnerXMLParser_test.py` & `nxswriter-3.9.0/test/InnerXMLParser_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/MYSQLSource_test.py` & `nxswriter-3.9.0/test/MYSQLSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NTP_test.py` & `nxswriter-3.9.0/test/NTP_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NXSDataWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/NXSDataWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NXSDataWriterH5PY_test.py` & `nxswriter-3.9.0/test/NXSDataWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NXSFromXMLH5Cpp_test.py` & `nxswriter-3.9.0/test/NXSFromXMLH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NXSFromXMLH5PY_test.py` & `nxswriter-3.9.0/test/NXSFromXMLH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/NexusXMLHandlerH5Cpp_test.py` & `nxswriter-3.9.0/test/NexusXMLHandlerH5Cpp_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from nxswriter.EGroup import EGroup
 from nxswriter.EField import EField
 from nxswriter.EAttribute import EAttribute
 from nxswriter.ELink import ELink
 from nxswriter.EStrategy import EStrategy
 from nxswriter.FElement import FElement
 from nxswriter.H5Elements import (
-    EDoc, ESymbol, EDimensions, EDim, EFile)
+    EDoc, ESymbol, EDimensions, EDim, EFile, EFilter)
 from nxswriter.DataSourceFactory import DataSourceFactory
 from nxswriter.Errors import UnsupportedTagError
 from nxswriter.FetchNameHandler import TNObject
 
 from nxstools import filewriter as FileWriter
 from nxstools import h5cppwriter as H5CppWriter
 
@@ -564,15 +564,16 @@
         self.assertEqual(
             nh.elementClass, {
                 'group': EGroup, 'field': EField, 'attribute': EAttribute,
                 'link': ELink,
                 'symbols': Element, 'symbol': ESymbol,
                 'dimensions': EDimensions,
                 'dim': EDim, 'enumeration': Element, 'item': Element,
-                'strategy': EStrategy
+                'strategy': EStrategy,
+                'filter': EFilter
             })
         self.assertEqual(nh.transparentTags, ['definition'])
         self.assertEqual(nh.close(), None)
 
         self._nxFile.close()
         os.remove(self._fname)
```

### Comparing `nxswriter-3.8.2/test/NexusXMLHandlerH5PY_test.py` & `nxswriter-3.9.0/test/NexusXMLHandlerH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from nxswriter.EGroup import EGroup
 from nxswriter.EField import EField
 from nxswriter.EAttribute import EAttribute
 from nxswriter.ELink import ELink
 from nxswriter.EStrategy import EStrategy
 from nxswriter.FElement import FElement
 from nxswriter.H5Elements import (
-    EDoc, ESymbol, EDimensions, EDim, EFile)
+    EDoc, ESymbol, EDimensions, EDim, EFile, EFilter)
 from nxswriter.DataSourceFactory import DataSourceFactory
 from nxswriter.Errors import UnsupportedTagError
 from nxswriter.FetchNameHandler import TNObject
 
 from nxstools import filewriter as FileWriter
 from nxstools import h5pywriter as H5PYWriter
 
@@ -563,15 +563,16 @@
         self.assertEqual(
             nh.elementClass, {
                 'group': EGroup, 'field': EField, 'attribute': EAttribute,
                 'link': ELink,
                 'symbols': Element, 'symbol': ESymbol,
                 'dimensions': EDimensions,
                 'dim': EDim, 'enumeration': Element, 'item': Element,
-                'strategy': EStrategy
+                'strategy': EStrategy,
+                'filter': EFilter
             })
         self.assertEqual(nh.transparentTags, ['definition'])
         self.assertEqual(nh.close(), None)
 
         self._nxFile.close()
         os.remove(self._fname)
```

### Comparing `nxswriter-3.8.2/test/ORACLESource_test.py` & `nxswriter-3.9.0/test/ORACLESource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/PGSQLSource_test.py` & `nxswriter-3.9.0/test/PGSQLSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ProxyHelper.py` & `nxswriter-3.9.0/test/ProxyHelper.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ProxyTools_test.py` & `nxswriter-3.9.0/test/ProxyTools_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/PyEvalSource_test.py` & `nxswriter-3.9.0/test/PyEvalSource_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     # setup test
     # \brief It tests default settings
     def test_getData_global_scalar(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
 
         script = """
-if type(ds.inp) == type(ds.inp2):
+if type(ds.inp) is type(ds.inp2):
     ds.res = ds.inp + ds.inp2
 else:
     ds.res = unicode(ds.inp) + unicode(ds.inp2)
 """
         if sys.version_info > (3,):
             script = script.replace("unicode", "str")
         dp = DataSourcePool()
@@ -391,27 +391,27 @@
                 self.assertEqual(
                     ds.setJSON(json.loads(gjson), json.loads(gjson2)), None)
                 dt = ds.getData()
                 v1 = Converters.toBool(arr[a][0]) if arr[
                     a][2] == "DevBoolean" else arr[a][0]
                 v2 = Converters.toBool(arr2[a2][0]) if arr2[
                     a2][2] == "DevBoolean" else arr2[a2][0]
-                vv = v1 + v2 if type(v1) == type(
+                vv = v1 + v2 if type(v1) is type(
                     v2) else unicode(v1) + unicode(v2)
                 self.checkData(
                     dt, arr[a][1], vv, NTP.pTt[type(vv).__name__], arr[a][3])
 
     # setup test
     # \brief It tests default settings
     def test_getData_global_spectrum(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
 
         script = """
-if type(ds.inp[0]) == type(ds.inp2[0]):
+if type(ds.inp[0]) is type(ds.inp2[0]):
     ds.res = ds.inp + ds.inp2
 else:
     ds.res = [str(i) for i in ds.inp] + [str(i2) for i2 in ds.inp2]
 """
 
         dp = DataSourcePool()
         arr = {
@@ -519,15 +519,15 @@
     # getData test
     # \brief It tests default settings with global json string
     def test_getData_global_image(self):
         fun = sys._getframe().f_code.co_name
         print("Run: %s.%s() " % (self.__class__.__name__, fun))
 
         script = """
-if type(ds.inp[0][0]) == type(ds.inp2[0][0]):
+if type(ds.inp[0][0]) is type(ds.inp2[0][0]):
     ds.res = ds.inp + ds.inp2
 else:
     ds.res = [[str(j) for j in i] for i in ds.inp] + """ \
         """[[str(j2) for j2 in i2] for i2 in ds.inp2]
 """
 
         dp = DataSourcePool()
```

### Comparing `nxswriter-3.8.2/test/PyEvalTangoSourceH5Cpp_test.py` & `nxswriter-3.9.0/test/PyEvalTangoSourceH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/PyEvalTangoSourceH5PY_test.py` & `nxswriter-3.9.0/test/PyEvalTangoSourceH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ServerSetUp.py` & `nxswriter-3.9.0/test/ServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/SimpleServer.py` & `nxswriter-3.9.0/test/SimpleServer.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/SimpleServerSetUp.py` & `nxswriter-3.9.0/test/SimpleServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/StreamSet_test.py` & `nxswriter-3.9.0/test/StreamSet_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TNObject_test.py` & `nxswriter-3.9.0/test/TNObject_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoDataWriterH5CppH5PY_test.py` & `nxswriter-3.9.0/test/TangoDataWriterH5CppH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoDataWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/TangoDataWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoDataWriterH5PY_test.py` & `nxswriter-3.9.0/test/TangoDataWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.9.0/test/TangoFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoFieldTagAsynchH5PY_test.py` & `nxswriter-3.9.0/test/TangoFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoFieldTagServerH5Cpp_test.py` & `nxswriter-3.9.0/test/TangoFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoFieldTagServerH5PY_test.py` & `nxswriter-3.9.0/test/TangoFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TangoFieldTagWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/TangoFieldTagWriterH5Cpp_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,16 +645,16 @@
 
         # tdw = self.openWriter(fname, xml, json='{ ' + decoder + ' }')
 
         steps = min(len(self._counter), len(self._fcounter), len(self._bools))
         for i in range(steps):
 
             self._simps.dp.ScalarBoolean = Types.Converters.toBool(
-                self._bools[0])
-            self._simps.dp.ScalarUChar = abs(self._counter[0])
+                self._bools[i])
+            self._simps.dp.ScalarUChar = abs(self._counter[i])
             self._simps.dp.ScalarShort = self._counter[0]
             self._simps.dp.ScalarUShort = abs(self._counter[0])
             self._simps.dp.ScalarLong = self._counter[0]
             self._simps.dp.ScalarULong = abs(self._counter[i])
             self._simps.dp.ScalarLong64 = self._counter[i]
             self._simps.dp.ScalarFloat = self._fcounter[i]
             self._simps.dp.ScalarDouble = self._dcounter[i]
@@ -985,15 +985,15 @@
              for i in range(steps)],
             attrs={"type": "NX_INT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarULong", "uint64", "NX_UINT",
             [(abs(self._counter[i]) if i % 2
-              else numpy.iinfo(getattr(numpy, 'int64')).max)
+              else numpy.iinfo(getattr(numpy, 'uint64')).max)
              for i in range(steps)],
             attrs={"type": "NX_UINT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarLong64", "int64", "NX_INT64",
             [(self._counter[i] if i % 2
@@ -1001,15 +1001,15 @@
              for i in range(steps)],
             attrs={"type": "NX_INT64", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": None, "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarULong64", "uint64", "NX_UINT",
             [(abs(self._counter[i]) if i % 2
-              else numpy.iinfo(getattr(numpy, 'int64')).max)
+              else numpy.iinfo(getattr(numpy, 'uint64')).max)
              for i in range(steps)],
             attrs={
                 "type": "NX_UINT64", "units": "m", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarFloat", "float32", "NX_FLOAT32",
@@ -1398,15 +1398,15 @@
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
         self._sc.checkSpectrumField(
             det, "SpectrumULong64", "uint64", "NX_UINT64",
             [(self._mca2[i] if not i % 2
-              else [numpy.iinfo(getattr(numpy, 'int64')).max] *
+              else [numpy.iinfo(getattr(numpy, 'uint64')).max] *
               len(self._mca2[i]))
              for i in range(steps)],
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
 
@@ -2268,17 +2268,18 @@
            <device member="attribute"
  name="stestp09/testss/s1r228" port="10000" />
            <record name="ImageUShort"/>
           </datasource>
         </field>
 
        <field units="" type="NX_INT32" name="ImageLong">
-          <strategy mode="STEP"  compression="32008"
- compression_opts="0,2"  grows="2"
- shuffle="true"  />
+          <strategy mode="STEP" grows="2">
+            <filter index="0" name="shuffle" />
+            <filter index="1" id="32008" cd_values="0,2" />
+          </strategy>
           <dimensions rank="2" />
           <datasource type="TANGO">
            <device member="attribute"
  name="stestp09/testss/s1r228" port="10000" />
            <record name="ImageLong"/>
           </datasource>
         </field>
@@ -2958,15 +2959,15 @@
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=1)
         self._sc.checkImageField(
             det, "ImageULong64", "uint64", "NX_UINT64",
             [(self._pco1[i] if not i % 2 else
-              [[numpy.iinfo(getattr(numpy, 'int64')).max] *
+              [[numpy.iinfo(getattr(numpy, 'uint64')).max] *
                len(self._pco1[i][0])] * len(self._pco1[i]))
              for i in range(steps)],
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
 
@@ -3025,15 +3026,15 @@
                     "type": "NX_UINT8", "units": "", "nexdatas_source": None,
                     "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                     "nexdatas_canfail_error": None},
                 grows=3)
 
         self._sc.checkSingleImageField(
             det, "InitImageULong64", "uint64", "NX_UINT64",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max] * len(
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max] * len(
                 self._pco1[0][0])] * len(self._pco1[0]),
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkSingleImageField(
             det, "FinalImageFloat", "float32", "NX_FLOAT32",
             [[numpy.finfo(getattr(numpy, 'float32')).max] * len(
```

### Comparing `nxswriter-3.8.2/test/TangoFieldTagWriterH5PY_test.py` & `nxswriter-3.9.0/test/TangoFieldTagWriterH5PY_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,17 +641,17 @@
 
         # tdw = self.openWriter(fname, xml, json='{ ' + decoder + ' }')
 
         steps = min(len(self._counter), len(self._fcounter), len(self._bools))
         for i in range(steps):
 
             self._simps.dp.ScalarBoolean = Types.Converters.toBool(
-                self._bools[0])
-            self._simps.dp.ScalarUChar = abs(self._counter[0])
-            self._simps.dp.ScalarShort = self._counter[0]
+                self._bools[i])
+            self._simps.dp.ScalarUChar = abs(self._counter[i])
+            self._simps.dp.ScalarShort = self._counter[i]
             self._simps.dp.ScalarUShort = abs(self._counter[0])
             self._simps.dp.ScalarLong = self._counter[0]
             self._simps.dp.ScalarULong = abs(self._counter[i])
             self._simps.dp.ScalarLong64 = self._counter[i]
             self._simps.dp.ScalarFloat = self._fcounter[i]
             self._simps.dp.ScalarDouble = self._dcounter[i]
             self._simps.dp.ScalarString = self._bools[i]
@@ -789,17 +789,18 @@
            <device member="attribute"
  name="stestp09/testss/s1r228" port="10000" />
            <record name="ImageUShort"/>
           </datasource>
         </field>
 
        <field units="" type="NX_INT32" name="ImageLong">
-          <strategy mode="STEP"  compression="32008"
- compression_opts="0,2"  grows="2"
- shuffle="true"  />
+          <strategy mode="STEP" grows="2">
+            <filter index="0" name="shuffle" />
+            <filter index="1" id="32008" cd_values="0,2" />
+          </strategy>
           <dimensions rank="2" />
           <datasource type="TANGO">
            <device member="attribute"
  name="stestp09/testss/s1r228" port="10000" />
            <record name="ImageLong"/>
           </datasource>
         </field>
@@ -1239,15 +1240,15 @@
              for i in range(steps)],
             attrs={"type": "NX_INT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarULong", "uint64", "NX_UINT",
             [(abs(self._counter[i]) if i % 2
-              else numpy.iinfo(getattr(numpy, 'int64')).max)
+              else numpy.iinfo(getattr(numpy, 'uint64')).max)
              for i in range(steps)],
             attrs={"type": "NX_UINT", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarLong64", "int64", "NX_INT64",
             [(self._counter[i] if i % 2
@@ -1255,15 +1256,15 @@
              for i in range(steps)],
             attrs={"type": "NX_INT64", "units": "m", "nexdatas_source": None,
                    "nexdatas_strategy": None, "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarULong64", "uint64", "NX_UINT",
             [(abs(self._counter[i]) if i % 2
-              else numpy.iinfo(getattr(numpy, 'int64')).max)
+              else numpy.iinfo(getattr(numpy, 'uint64')).max)
              for i in range(steps)],
             attrs={
                 "type": "NX_UINT64", "units": "m", "nexdatas_source": None,
                 "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                 "nexdatas_canfail_error": None})
         self._sc.checkScalarField(
             det, "ScalarFloat", "float32", "NX_FLOAT32",
@@ -1652,15 +1653,15 @@
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
         self._sc.checkSpectrumField(
             det, "SpectrumULong64", "uint64", "NX_UINT64",
             [(self._mca2[i] if not i % 2
-              else [numpy.iinfo(getattr(numpy, 'int64')).max] *
+              else [numpy.iinfo(getattr(numpy, 'uint64')).max] *
               len(self._mca2[i]))
              for i in range(steps)],
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
 
@@ -2954,15 +2955,15 @@
             attrs={"type": "NX_INT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=1)
         self._sc.checkImageField(
             det, "ImageULong64", "uint64", "NX_UINT64",
             [(self._pco1[i] if not i % 2 else
-              [[numpy.iinfo(getattr(numpy, 'int64')).max] *
+              [[numpy.iinfo(getattr(numpy, 'uint64')).max] *
                len(self._pco1[i][0])] * len(self._pco1[i]))
              for i in range(steps)],
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None},
             grows=2)
 
@@ -3021,15 +3022,15 @@
                     "type": "NX_UINT8", "units": "", "nexdatas_source": None,
                     "nexdatas_strategy": "STEP", "nexdatas_canfail": "FAILED",
                     "nexdatas_canfail_error": None},
                 grows=3)
 
         self._sc.checkSingleImageField(
             det, "InitImageULong64", "uint64", "NX_UINT64",
-            [[numpy.iinfo(getattr(numpy, 'int64')).max] * len(
+            [[numpy.iinfo(getattr(numpy, 'uint64')).max] * len(
                 self._pco1[0][0])] * len(self._pco1[0]),
             attrs={"type": "NX_UINT64", "units": "", "nexdatas_source": None,
                    "nexdatas_strategy": "INIT", "nexdatas_canfail": "FAILED",
                    "nexdatas_canfail_error": None})
         self._sc.checkSingleImageField(
             det, "FinalImageFloat", "float32", "NX_FLOAT32",
             [[numpy.finfo(getattr(numpy, 'float32')).max] * len(
```

### Comparing `nxswriter-3.8.2/test/TangoSource_test.py` & `nxswriter-3.9.0/test/TangoSource_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TgDevice_test.py` & `nxswriter-3.9.0/test/TgDevice_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TgGroup_test.py` & `nxswriter-3.9.0/test/TgGroup_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TgMember_test.py` & `nxswriter-3.9.0/test/TgMember_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/ThreadPool_test.py` & `nxswriter-3.9.0/test/ThreadPool_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/TstDataSource.py` & `nxswriter-3.9.0/test/TstDataSource.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/UINT32decoder_test.py` & `nxswriter-3.9.0/test/UINT32decoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/UTF8decoder_test.py` & `nxswriter-3.9.0/test/UTF8decoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/VDEOdecoder_test.py` & `nxswriter-3.9.0/test/VDEOdecoder_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagAsynchH5Cpp_test.py` & `nxswriter-3.9.0/test/XMLFieldTagAsynchH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagAsynchH5PY_test.py` & `nxswriter-3.9.0/test/XMLFieldTagAsynchH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagServerH5Cpp_test.py` & `nxswriter-3.9.0/test/XMLFieldTagServerH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagServerH5PY_test.py` & `nxswriter-3.9.0/test/XMLFieldTagServerH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagWriterH5Cpp_test.py` & `nxswriter-3.9.0/test/XMLFieldTagWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/XMLFieldTagWriterH5PY_test.py` & `nxswriter-3.9.0/test/XMLFieldTagWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/__init__.py` & `nxswriter-3.9.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/__main__.py` & `nxswriter-3.9.0/test/__main__.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/main.py` & `nxswriter-3.9.0/test/main.py`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/mydb.pgsql` & `nxswriter-3.9.0/test/mydb.pgsql`

 * *Files identical despite different names*

### Comparing `nxswriter-3.8.2/test/sttest.py` & `nxswriter-3.9.0/test/sttest.py`

 * *Files identical despite different names*

