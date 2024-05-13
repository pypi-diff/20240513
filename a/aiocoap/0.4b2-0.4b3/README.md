# Comparing `tmp/aiocoap-0.4b2.tar.gz` & `tmp/aiocoap-0.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiocoap-0.4b2.tar", last modified: Tue Jan 28 13:09:22 2020, max compression
+gzip compressed data, was "dist/aiocoap-0.4b3.tar", last modified: Thu Jun 18 09:54:06 2020, max compression
```

## Comparing `aiocoap-0.4b2.tar` & `aiocoap-0.4b3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1174 2017-11-14 16:20:02.000000 aiocoap-0.4b2/LICENSE
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)       74 2017-11-14 16:20:02.000000 aiocoap-0.4b2/MANIFEST.in
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    12307 2020-01-28 10:34:02.000000 aiocoap-0.4b2/NEWS
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      903 2020-01-28 13:09:22.000000 aiocoap-0.4b2/PKG-INFO
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6666 2020-01-28 11:00:48.000000 aiocoap-0.4b2/README.rst
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1158 2018-10-08 17:57:23.000000 aiocoap-0.4b2/aiocoap/__init__.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/cli/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      748 2018-04-13 13:10:52.000000 aiocoap-0.4b2/aiocoap/cli/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    14550 2020-01-28 13:06:21.000000 aiocoap-0.4b2/aiocoap/cli/client.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4047 2018-05-02 23:29:23.000000 aiocoap-0.4b2/aiocoap/cli/common.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8126 2019-07-16 13:13:44.000000 aiocoap-0.4b2/aiocoap/cli/fileserver.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3977 2018-09-16 17:20:36.000000 aiocoap-0.4b2/aiocoap/cli/proxy.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    20600 2019-09-11 20:30:35.000000 aiocoap-0.4b2/aiocoap/cli/rd.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11014 2020-01-28 10:07:06.000000 aiocoap-0.4b2/aiocoap/credentials.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5781 2018-10-08 17:52:08.000000 aiocoap-0.4b2/aiocoap/defaults.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6356 2019-12-11 14:49:12.000000 aiocoap-0.4b2/aiocoap/error.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11253 2019-10-01 13:14:33.000000 aiocoap-0.4b2/aiocoap/interfaces.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    24148 2019-07-16 11:35:48.000000 aiocoap-0.4b2/aiocoap/message.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    20340 2019-10-01 13:14:33.000000 aiocoap-0.4b2/aiocoap/messagemanager.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      897 2020-01-28 13:07:05.000000 aiocoap-0.4b2/aiocoap/meta.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/numbers/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3414 2019-04-16 13:56:36.000000 aiocoap-0.4b2/aiocoap/numbers/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4690 2018-09-30 15:50:46.000000 aiocoap-0.4b2/aiocoap/numbers/codes.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4321 2019-06-19 19:13:46.000000 aiocoap-0.4b2/aiocoap/numbers/constants.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6688 2020-01-28 11:01:23.000000 aiocoap-0.4b2/aiocoap/numbers/optionnumbers.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      759 2017-11-14 16:20:02.000000 aiocoap-0.4b2/aiocoap/numbers/types.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8722 2020-01-28 10:07:06.000000 aiocoap-0.4b2/aiocoap/options.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6332 2018-12-05 16:10:18.000000 aiocoap-0.4b2/aiocoap/optiontypes.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    38563 2020-01-28 10:07:06.000000 aiocoap-0.4b2/aiocoap/oscore.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    47619 2020-01-28 09:41:28.000000 aiocoap-0.4b2/aiocoap/protocol.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/proxy/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      475 2017-11-14 16:20:02.000000 aiocoap-0.4b2/aiocoap/proxy/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3006 2018-05-02 23:29:24.000000 aiocoap-0.4b2/aiocoap/proxy/client.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13287 2018-10-27 15:49:52.000000 aiocoap-0.4b2/aiocoap/proxy/server.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    16524 2019-09-11 20:45:00.000000 aiocoap-0.4b2/aiocoap/resource.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/resourcedirectory/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      615 2018-04-13 13:10:52.000000 aiocoap-0.4b2/aiocoap/resourcedirectory/__init__.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/resourcedirectory/client/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      537 2018-04-13 13:10:52.000000 aiocoap-0.4b2/aiocoap/resourcedirectory/client/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13839 2019-03-23 16:24:35.000000 aiocoap-0.4b2/aiocoap/resourcedirectory/client/register.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    12218 2019-10-01 13:14:33.000000 aiocoap-0.4b2/aiocoap/tokenmanager.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/transports/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1061 2018-04-13 13:10:52.000000 aiocoap-0.4b2/aiocoap/transports/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2190 2018-06-27 08:00:45.000000 aiocoap-0.4b2/aiocoap/transports/generic_udp.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8828 2020-01-28 10:07:06.000000 aiocoap-0.4b2/aiocoap/transports/oscore.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     9269 2019-09-11 19:26:26.000000 aiocoap-0.4b2/aiocoap/transports/simple6.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5760 2020-01-28 11:12:50.000000 aiocoap-0.4b2/aiocoap/transports/simplesocketserver.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    17462 2019-07-16 11:53:50.000000 aiocoap-0.4b2/aiocoap/transports/tcp.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13330 2019-09-03 20:00:28.000000 aiocoap-0.4b2/aiocoap/transports/tinydtls.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1254 2018-05-02 23:29:24.000000 aiocoap-0.4b2/aiocoap/transports/tls.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    16248 2020-01-28 11:12:40.000000 aiocoap-0.4b2/aiocoap/transports/udp6.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/util/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3108 2018-10-27 15:49:52.000000 aiocoap-0.4b2/aiocoap/util/__init__.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap/util/asyncio/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      476 2018-09-26 12:56:11.000000 aiocoap-0.4b2/aiocoap/util/asyncio/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1232 2018-07-31 18:23:48.000000 aiocoap-0.4b2/aiocoap/util/asyncio/peekqueue.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1075 2018-07-31 18:23:48.000000 aiocoap-0.4b2/aiocoap/util/asyncio/pre35.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5504 2019-10-01 08:36:13.000000 aiocoap-0.4b2/aiocoap/util/asyncio/recvmsg.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4001 2018-10-08 17:52:08.000000 aiocoap-0.4b2/aiocoap/util/cli.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4856 2018-10-05 11:33:39.000000 aiocoap-0.4b2/aiocoap/util/linkformat.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1442 2018-10-08 21:58:43.000000 aiocoap-0.4b2/aiocoap/util/linkformat_pygments.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4838 2019-07-16 12:23:09.000000 aiocoap-0.4b2/aiocoap/util/prettyprint.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      692 2018-04-13 13:10:53.000000 aiocoap-0.4b2/aiocoap/util/secrets.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1176 2019-10-17 06:29:42.000000 aiocoap-0.4b2/aiocoap/util/socknumbers.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1063 2018-05-02 23:29:24.000000 aiocoap-0.4b2/aiocoap/util/uri.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      903 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/PKG-INFO
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2455 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/SOURCES.txt
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)        1 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/dependency_links.txt
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      245 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/entry_points.txt
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      380 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/requires.txt
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)       14 2020-01-28 13:09:22.000000 aiocoap-0.4b2/aiocoap.egg-info/top_level.txt
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1193 2019-03-31 17:47:19.000000 aiocoap-0.4b2/clientGET-observe.py
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1092 2019-09-12 06:18:39.000000 aiocoap-0.4b2/clientGET.py
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1318 2018-06-27 08:00:40.000000 aiocoap-0.4b2/clientPUT.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/contrib/
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1695 2019-09-11 20:31:18.000000 aiocoap-0.4b2/contrib/aiocoap-kivy-widget
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     3689 2019-09-11 20:31:50.000000 aiocoap-0.4b2/contrib/aiocoap-widgets
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1808 2019-11-25 21:43:23.000000 aiocoap-0.4b2/contrib/oscore-key-derivation~
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     5916 2019-09-11 20:33:24.000000 aiocoap-0.4b2/contrib/rd-relay
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/doc/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)       41 2017-11-14 16:20:02.000000 aiocoap-0.4b2/doc/LICENSE.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1491 2018-04-13 13:10:53.000000 aiocoap-0.4b2/doc/README.doc
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5178 2019-07-16 13:10:31.000000 aiocoap-0.4b2/doc/aiocoap_index.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2191 2019-03-23 16:49:38.000000 aiocoap-0.4b2/doc/api.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6599 2020-01-28 13:07:15.000000 aiocoap-0.4b2/doc/conf.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6600 2020-01-28 13:07:13.000000 aiocoap-0.4b2/doc/conf.py~
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1082 2018-05-02 23:29:24.000000 aiocoap-0.4b2/doc/examples.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     9616 2019-06-19 19:22:34.000000 aiocoap-0.4b2/doc/guidedtour.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      150 2018-05-02 23:29:24.000000 aiocoap-0.4b2/doc/index.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3243 2019-07-20 18:48:29.000000 aiocoap-0.4b2/doc/installation.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     7263 2018-05-02 23:29:24.000000 aiocoap-0.4b2/doc/logo-square.svg
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    26760 2018-05-02 23:29:24.000000 aiocoap-0.4b2/doc/logo.svg
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      244 2017-11-14 16:20:02.000000 aiocoap-0.4b2/doc/news.rst
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      498 2019-09-12 06:22:05.000000 aiocoap-0.4b2/doc/release-checklist
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2797 2019-07-16 13:13:44.000000 aiocoap-0.4b2/doc/tools.rst
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     3932 2019-11-08 10:35:53.000000 aiocoap-0.4b2/server.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)       38 2020-01-28 13:09:22.000000 aiocoap-0.4b2/setup.cfg
--rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     4523 2020-01-28 13:07:23.000000 aiocoap-0.4b2/setup.py
-drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-01-28 13:09:22.000000 aiocoap-0.4b2/tests/
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)      549 2018-04-13 13:10:53.000000 aiocoap-0.4b2/tests/__init__.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2741 2018-09-26 12:56:11.000000 aiocoap-0.4b2/tests/common.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    10320 2019-09-11 19:26:26.000000 aiocoap-0.4b2/tests/fixtures.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4339 2019-06-19 20:24:40.000000 aiocoap-0.4b2/tests/test_blockwise.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4968 2018-10-27 15:49:52.000000 aiocoap-0.4b2/tests/test_client.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6422 2018-12-05 15:57:36.000000 aiocoap-0.4b2/tests/test_commandline.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2368 2020-01-28 10:07:06.000000 aiocoap-0.4b2/tests/test_credentials.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1153 2019-09-07 11:01:49.000000 aiocoap-0.4b2/tests/test_doctest.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11113 2018-12-05 16:10:18.000000 aiocoap-0.4b2/tests/test_encoding.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5940 2019-10-01 13:14:33.000000 aiocoap-0.4b2/tests/test_noncoap_client.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     7095 2018-09-26 12:56:11.000000 aiocoap-0.4b2/tests/test_noncoap_tcp_client.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13929 2019-09-11 20:45:00.000000 aiocoap-0.4b2/tests/test_observe.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11600 2020-01-28 10:37:15.000000 aiocoap-0.4b2/tests/test_oscore.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8396 2020-01-28 11:14:54.000000 aiocoap-0.4b2/tests/test_oscore_plugtest.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3262 2018-09-24 14:29:06.000000 aiocoap-0.4b2/tests/test_proxy.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3466 2018-10-09 16:35:07.000000 aiocoap-0.4b2/tests/test_rd_examples.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4452 2018-05-02 23:29:24.000000 aiocoap-0.4b2/tests/test_reverseproxy.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)    12646 2019-10-01 10:29:39.000000 aiocoap-0.4b2/tests/test_server.py
--rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1937 2018-05-02 23:29:24.000000 aiocoap-0.4b2/tests/test_uri_handling.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.944424 aiocoap-0.4b3/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1174 2017-11-14 16:20:02.000000 aiocoap-0.4b3/LICENSE
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)       74 2017-11-14 16:20:02.000000 aiocoap-0.4b3/MANIFEST.in
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13393 2020-06-18 09:51:05.000000 aiocoap-0.4b3/NEWS
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      903 2020-06-18 09:54:06.944424 aiocoap-0.4b3/PKG-INFO
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6742 2020-06-11 14:32:08.000000 aiocoap-0.4b3/README.rst
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.916424 aiocoap-0.4b3/aiocoap/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1158 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/__init__.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.920424 aiocoap-0.4b3/aiocoap/cli/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      748 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    14550 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/client.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4047 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/common.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2106 2020-06-18 08:27:07.000000 aiocoap-0.4b3/aiocoap/cli/defaults.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8126 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/fileserver.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3977 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/proxy.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    20600 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/cli/rd.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11014 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/credentials.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6469 2020-06-18 08:27:07.000000 aiocoap-0.4b3/aiocoap/defaults.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6356 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/error.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11447 2020-03-24 10:34:36.000000 aiocoap-0.4b3/aiocoap/interfaces.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    24148 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/message.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    20340 2020-03-24 11:11:36.000000 aiocoap-0.4b3/aiocoap/messagemanager.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      897 2020-06-18 09:47:36.000000 aiocoap-0.4b3/aiocoap/meta.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.924424 aiocoap-0.4b3/aiocoap/numbers/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3414 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/numbers/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4690 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/numbers/codes.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4321 2020-02-10 11:49:02.000000 aiocoap-0.4b3/aiocoap/numbers/constants.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6688 2020-03-17 16:22:33.000000 aiocoap-0.4b3/aiocoap/numbers/optionnumbers.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      759 2017-11-14 16:20:02.000000 aiocoap-0.4b3/aiocoap/numbers/types.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8722 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/options.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6332 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/optiontypes.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    38630 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/oscore.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    48103 2020-06-18 09:12:35.000000 aiocoap-0.4b3/aiocoap/protocol.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.924424 aiocoap-0.4b3/aiocoap/proxy/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      475 2017-11-14 16:20:02.000000 aiocoap-0.4b3/aiocoap/proxy/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3006 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/proxy/client.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13287 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/proxy/server.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    16524 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/resource.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.924424 aiocoap-0.4b3/aiocoap/resourcedirectory/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      615 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/resourcedirectory/__init__.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.924424 aiocoap-0.4b3/aiocoap/resourcedirectory/client/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      537 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/resourcedirectory/client/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13839 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/resourcedirectory/client/register.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    12985 2020-06-11 14:18:20.000000 aiocoap-0.4b3/aiocoap/tokenmanager.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.928424 aiocoap-0.4b3/aiocoap/transports/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1061 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2190 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/generic_udp.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8828 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/oscore.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     9269 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/simple6.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6433 2020-06-18 09:14:19.000000 aiocoap-0.4b3/aiocoap/transports/simplesocketserver.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    17529 2020-06-18 08:43:08.000000 aiocoap-0.4b3/aiocoap/transports/tcp.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13330 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/tinydtls.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1254 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/transports/tls.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    16891 2020-06-18 08:30:50.000000 aiocoap-0.4b3/aiocoap/transports/udp6.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.932424 aiocoap-0.4b3/aiocoap/util/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3108 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/__init__.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.932424 aiocoap-0.4b3/aiocoap/util/asyncio/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      476 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/asyncio/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1232 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/asyncio/peekqueue.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1075 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/asyncio/pre35.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5592 2020-03-10 22:05:34.000000 aiocoap-0.4b3/aiocoap/util/asyncio/recvmsg.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4001 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/cli.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4856 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/linkformat.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1442 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/linkformat_pygments.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5142 2020-02-12 08:49:43.000000 aiocoap-0.4b3/aiocoap/util/prettyprint.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      692 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/secrets.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2383 2020-03-11 09:22:28.000000 aiocoap-0.4b3/aiocoap/util/socknumbers.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1063 2020-02-10 11:08:47.000000 aiocoap-0.4b3/aiocoap/util/uri.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.916424 aiocoap-0.4b3/aiocoap.egg-info/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      903 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/PKG-INFO
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2447 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/SOURCES.txt
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)        1 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/dependency_links.txt
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      245 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/entry_points.txt
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      380 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/requires.txt
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)       14 2020-06-18 09:54:06.000000 aiocoap-0.4b3/aiocoap.egg-info/top_level.txt
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1193 2020-02-10 11:08:47.000000 aiocoap-0.4b3/clientGET-observe.py
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1092 2020-06-18 08:14:06.000000 aiocoap-0.4b3/clientGET.py
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1318 2020-02-10 11:08:47.000000 aiocoap-0.4b3/clientPUT.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.932424 aiocoap-0.4b3/contrib/
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     1695 2020-02-10 11:08:47.000000 aiocoap-0.4b3/contrib/aiocoap-kivy-widget
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     3689 2020-02-10 11:08:47.000000 aiocoap-0.4b3/contrib/aiocoap-widgets
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     5916 2020-02-10 11:08:47.000000 aiocoap-0.4b3/contrib/rd-relay
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.940424 aiocoap-0.4b3/doc/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)       41 2017-11-14 16:20:02.000000 aiocoap-0.4b3/doc/LICENSE.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1491 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/README.doc
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5178 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/aiocoap_index.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2191 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/api.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6599 2020-06-18 09:47:45.000000 aiocoap-0.4b3/doc/conf.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1082 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/examples.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1450 2020-06-18 09:07:57.000000 aiocoap-0.4b3/doc/faq.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     9616 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/guidedtour.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      157 2020-06-18 08:34:54.000000 aiocoap-0.4b3/doc/index.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3243 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/installation.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     7263 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/logo-square.svg
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    26760 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/logo.svg
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      244 2017-11-14 16:20:02.000000 aiocoap-0.4b3/doc/news.rst
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      689 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/release-checklist
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2797 2020-02-10 11:08:47.000000 aiocoap-0.4b3/doc/tools.rst
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     3932 2020-06-18 08:26:52.000000 aiocoap-0.4b3/server.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)       38 2020-06-18 09:54:06.944424 aiocoap-0.4b3/setup.cfg
+-rwxr-xr-x   0 chrysn    (1000) chrysn    (1000)     4523 2020-06-18 09:47:26.000000 aiocoap-0.4b3/setup.py
+drwxr-xr-x   0 chrysn    (1000) chrysn    (1000)        0 2020-06-18 09:54:06.944424 aiocoap-0.4b3/tests/
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)      549 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/__init__.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2741 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/common.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    10320 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/fixtures.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4339 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_blockwise.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     7305 2020-06-11 16:24:43.000000 aiocoap-0.4b3/tests/test_client.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     6422 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_commandline.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     2368 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_credentials.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1153 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_doctest.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11113 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_encoding.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     5940 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_noncoap_client.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     7095 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_noncoap_tcp_client.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    13929 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_observe.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    11600 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_oscore.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     8396 2020-06-10 11:40:20.000000 aiocoap-0.4b3/tests/test_oscore_plugtest.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3262 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_proxy.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     3466 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_rd_examples.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     4452 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_reverseproxy.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)    12963 2020-06-11 14:18:20.000000 aiocoap-0.4b3/tests/test_server.py
+-rw-r--r--   0 chrysn    (1000) chrysn    (1000)     1937 2020-02-10 11:08:47.000000 aiocoap-0.4b3/tests/test_uri_handling.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiocoap-0.4b2/LICENSE` & `aiocoap-0.4b3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/NEWS` & `aiocoap-0.4b3/NEWS`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,47 @@
-Version next
-------------
+Version 0.4b3
+-------------
+
+Behavioral changes
+~~~~~~~~~~~~~~~~~~
+
+* Responses to NON requests are now sent as NON.
+
+Portability
+~~~~~~~~~~~
+
+* All uses of SO_REUSEPORT were changed to SO_REUSEADDR, as REUSEPORT is
+  considered dangerous by some and removed from newer Python versions.
+
+  On platoforms without support for that option, it is not set. Automatic
+  load-balancing by running parallel servers is not supported there.
+
+* The udp6 module is now usable on platforms without MSG_ERRQUEUE (ie. anything
+  but Linux). This comes with caveats, so it is still only enabled by default
+  on Linux.
+
+  The required constants are now shipped with aiocoap for macOS for the benefit
+  of Python versions less than 3.9.
+
+Minor fixes
+~~~~~~~~~~~
+
+* More effort is made to sync OSCORE persistence files to disk.
+* Memory leakage fixes on server and client side.
+* Option numbers for Echo and Request-Tag were updated according to the latest
+  draft version.
+
+Other
+~~~~~
+
+* FAQ section started in the documentation.
+* With `./setup.py test` being phased out, tests are now run via tox.
+
+Version 0.4b2
+-------------
 
 New features
 ~~~~~~~~~~~~
 
 * OSCORE: Implement Appendix B.1 recovery. This allows the aiocoap program to
   run OSCORE without writing sequence numbers and replay windows to disk all
   the time. Instead, they write pessimistic values to disk that are rarely
```

### Comparing `aiocoap-0.4b2/PKG-INFO` & `aiocoap-0.4b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocoap
-Version: 0.4b2
+Version: 0.4b3
 Summary: Python CoAP library
 Home-page: https://github.com/chrysn/aiocoap
 Author: Maciej Wasilak, Christian Amsüss
 Author-email: c.amsuess@energyharvesting.at
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: coap,asyncio,iot
```

### Comparing `aiocoap-0.4b2/README.rst` & `aiocoap-0.4b3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,15 @@
 and requires full POSIX network interfaces only available on Linux and possibly
 some BSDs. On Windows and macOS, more constrained server_ and client_
 transports with some caveats of their own are used; for more details, see the
 currently open `platform issues`_. Alternative main loops like uvloop_ or
 gbulb_ can be used without restriction.
 
 If your library depends on aiocoap, it should pick the required extras (as per
-installation_) and declare a dependency like ``aiocoap[linkheader,oscore] >=
-0.4a1``.
+installation_) and declare a dependency like ``aiocoap[linkheader,oscore] >= 0.4b2``.
 
 .. _Python: https://www.python.org/
 .. _PyPy3: http://pypy.org/
 .. _udp6: http://aiocoap.readthedocs.io/en/latest/module/aiocoap.transports.udp6.html
 .. _uvloop: https://uvloop.readthedocs.io/
 .. _gbulb: https://github.com/nathan-hoad/gbulb
 .. _`platform issues`: https://github.com/chrysn/aiocoap/issues?q=is%3Aissue+is%3Aopen+label%3A%22platform+support%22
@@ -101,25 +100,26 @@
 in the `github issue tracker`_. Pull requests are welcome there; if you start
 working on larger changes, please coordinate on the issue tracker.
 
 Documentation is built using sphinx_ with ``./setup.py build_sphinx``; hacks
 used there are described in ``./doc/README.doc``.
 
 Unit tests are implemented in the ``./tests/`` directory and easiest run using
-``./setup.py test``; complete test coverage is aimed for, but not yet complete
-(and might never be, as the error handling for pathological network partners is
-hard to trigger with a library designed not to misbehave). The tests are
-regularly run at the `CI suite at gitlab`_, from where `coverage reports`_ are
-available.
+tox_ (though still available through ``./setup.py test`` for the time being);
+complete test coverage is aimed for, but not yet complete (and might never be,
+as the error handling for pathological network partners is hard to trigger with
+a library designed not to misbehave). The tests are regularly run at the `CI
+suite at gitlab`_, from where `coverage reports`_ are available.
 
 .. _PEP8: http://legacy.python.org/dev/peps/pep-0008/
 .. _sphinx: http://sphinx-doc.org/
 .. _`github issue tracker`: https://github.com/chrysn/aiocoap/issues
-.. _`CI suite at gitlab`: https://gitlab.com/energyharvesting/aiocoap/commits/master
-.. _`coverage reports`: https://energyharvesting.gitlab.io/aiocoap/
+.. _`CI suite at gitlab`: https://gitlab.com/aiocoap/aiocoap/commits/master
+.. _`coverage reports`: https://aiocoap.gitlab.io/aiocoap/
+.. _tox: https://tox.readthedocs.io/
 
 Relevant URLs
 -------------
 
 * https://github.com/chrysn/aiocoap
 
   This is where the latest source code can be found, and bugs can be reported.
```

### Comparing `aiocoap-0.4b2/aiocoap/__init__.py` & `aiocoap-0.4b3/aiocoap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/__init__.py` & `aiocoap-0.4b3/aiocoap/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/client.py` & `aiocoap-0.4b3/aiocoap/cli/client.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/common.py` & `aiocoap-0.4b3/aiocoap/cli/common.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/fileserver.py` & `aiocoap-0.4b3/aiocoap/cli/fileserver.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/proxy.py` & `aiocoap-0.4b3/aiocoap/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/cli/rd.py` & `aiocoap-0.4b3/aiocoap/cli/rd.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/credentials.py` & `aiocoap-0.4b3/aiocoap/credentials.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/defaults.py` & `aiocoap-0.4b3/aiocoap/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 be used in the rest of the code for feature checking (just raise the
 ImportErrors) unless it's directly user-visible ("You configured OSCORE key
 material, but OSCORE needs the following unavailable modules") or in the test
 suite to decide which tests to skip.
 """
 
 import os
+import socket
 import sys
 import asyncio
 
-def get_default_clienttransports(*, loop=None):
+def get_default_clienttransports(*, loop=None, use_env=True):
     """Return a list of transports that should be connected when a client
     context is created.
 
     If an explicit ``AIOCOAP_CLIENT_TRANSPORT`` environment variable is set, it
     is read as a colon separated list of transport names.
 
     By default, a DTLS mechanism will be picked if the required modules are
     available, and a UDP transport will be selected depending on whether the
     full udp6 transport is known to work.
     """
 
-    if 'AIOCOAP_CLIENT_TRANSPORT' in os.environ:
+    if use_env and 'AIOCOAP_CLIENT_TRANSPORT' in os.environ:
         yield from os.environ['AIOCOAP_CLIENT_TRANSPORT'].split(':')
         return
 
     if not oscore_missing_modules():
         yield 'oscore'
 
     try:
@@ -62,42 +63,38 @@
         return
 
     # on android it seems that it's only the AI_V4MAPPED that causes trouble,
     # that should be managable in udp6 too.
     yield 'udp6'
     return
 
-def get_default_servertransports(*, loop=None):
+def get_default_servertransports(*, loop=None, use_env=True):
     """Return a list of transports that should be connected when a server
     context is created.
 
     If an explicit ``AIOCOAP_SERVER_TRANSPORT`` environment variable is set, it
     is read as a colon separated list of transport names.
 
     By default, a DTLS mechanism will be picked if the required modules are
     available, and a UDP transport will be selected depending on whether the
     full udp6 transport is known to work. Both a simple6 and a simplesocketserver
     will be selected when udp6 is not available, and the simple6 will be used
     for any outgoing requests, which the simplesocketserver could serve but is worse
     at.
     """
 
-    if 'AIOCOAP_SERVER_TRANSPORT' in os.environ:
+    if use_env and 'AIOCOAP_SERVER_TRANSPORT' in os.environ:
         yield from os.environ['AIOCOAP_SERVER_TRANSPORT'].split(':')
         return
 
     if not oscore_missing_modules():
         yield 'oscore'
 
     # no server support yet, but doesn't hurt either
-    try:
-        from DTLSSocket import dtls # noqa: F401
-    except ImportError:
-        pass
-    else:
+    if not dtls_missing_modules():
         yield 'tinydtls'
 
     yield 'tcpserver'
     yield 'tcpclient'
     yield 'tlsserver'
     yield 'tlsclient'
 
@@ -109,16 +106,40 @@
         return
 
     # on android it seems that it's only the AI_V4MAPPED that causes trouble,
     # that should be managable in udp6 too.
     yield 'udp6'
     return
 
+def has_reuse_port(*, use_env=True):
+    """Return true if the platform indicates support for SO_REUSEPORT.
+
+    Can be overridden by explicitly setting ``AIOCOAP_REUSE_PORT`` to 1 or
+    0."""
+
+    if use_env and os.environ.get('AIOCOAP_REUSE_PORT'):
+        return bool(int(os.environ['AIOCOAP_REUSE_PORT']))
+
+    return hasattr(socket, 'SO_REUSEPORT')
+
 # FIXME: If there were a way to check for the extras defined in setup.py, or to link these lists to what is descibed there, that'd be great.
 
+def dtls_missing_modules():
+    """Return a list of modules that are missing in order to use the DTLS
+    transport, or a false value if everything is present"""
+
+    missing = []
+
+    try:
+        from DTLSSocket import dtls # noqa: F401
+    except ImportError:
+        missing.append("DTLSSocket")
+
+    return missing
+
 def oscore_missing_modules():
     """Return a list of modules that are missing in order to use OSCORE, or a
     false value if everything is present"""
     missing = []
     try:
         import cbor # noqa: F401
     except ImportError:
@@ -131,15 +152,15 @@
         import cryptography # noqa: F401
     except ImportError:
         missing.append('cryptography')
     else:
         try:
             from cryptography.hazmat.primitives.ciphers.aead import AESCCM
             AESCCM(b"x" * 16, 8)
-        except cryptography.exceptions.UnsupportedAlgorithm:
+        except (cryptography.exceptions.UnsupportedAlgorithm, ImportError):
             missing.append('a version of OpenSSL that supports AES-CCM')
 
     return missing
 
 def linkheader_missing_modules():
     """Return a list of moudles that are missing in order to use link_header
     functionaity (eg. running a resource directory), of a false value if
```

### Comparing `aiocoap-0.4b2/aiocoap/error.py` & `aiocoap-0.4b3/aiocoap/error.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/interfaces.py` & `aiocoap-0.4b3/aiocoap/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,19 @@
     def request(self, request: "PlumbingRequest"):
         pass
 
 class RequestProvider(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def request(self, request_message):
         """Create and act on a a :class:`Request` object that will be handled
-        according to the provider's implementation."""
+        according to the provider's implementation.
+
+        Note that the request is not necessarily sent on the wire immediately;
+        it may (but, depend on the transport does not necessarily) rely on the
+        response to be waited for."""
 
 class Request(metaclass=abc.ABCMeta):
     """A CoAP request, initiated by sending a message. Typically, this is not
     instanciated directly, but generated by a :meth:`RequestProvider.request`
     method."""
 
     response = """A future that is present from the creation of the object and \
```

### Comparing `aiocoap-0.4b2/aiocoap/message.py` & `aiocoap-0.4b3/aiocoap/message.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/messagemanager.py` & `aiocoap-0.4b3/aiocoap/messagemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     rst = Message(mtype=RST, mid=message.mid, code=EMPTY, payload='')
                     rst.remote = message.remote.as_response_address()
                     self._send_initially(rst)
         else:
             self.log.warning("Received a message with code %s and type %s (those don't fit) from %s, ignoring it."%(message.code, message.mtype, message.remote))
 
     def dispatch_error(self, errno, remote):
-        self.log.debug("Incoming error %d from %r", errno, remote)
+        self.log.debug("Incoming error %s from %r", errno, remote)
 
         # cancel requests first, and then exchanges: cancelling the pending
         # exchange would trigger enqueued requests to be transmitted
         self.token_manager.dispatch_error(errno, remote)
 
         keys_for_removal = []
         for key, (monitor, cancellable_timeout) in self._active_exchanges.items():
```

### Comparing `aiocoap-0.4b2/aiocoap/meta.py` & `aiocoap-0.4b3/aiocoap/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # described in the accompanying LICENSE file.
 
 #: Make library version internally
 #:
 #: This is not supposed to be used in any decision-making process (use package
 #: dependencies for that) or workarounds, but used by command-line tools or the
 #: impl-info link to provide debugging information.
-version = "0.4b2"
+version = "0.4b3"
 
 #: URI used to describe the current version of the library
 #:
 #: This is used the same way as `version` but when a URI is required, for
 #: example as a default value for .well-known/core's rel=impl-info link.
 library_uri = "https://christian.amsuess.com/tools/aiocoap/#version-" + version
```

### Comparing `aiocoap-0.4b2/aiocoap/numbers/__init__.py` & `aiocoap-0.4b3/aiocoap/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/numbers/codes.py` & `aiocoap-0.4b3/aiocoap/numbers/codes.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/numbers/constants.py` & `aiocoap-0.4b3/aiocoap/numbers/constants.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/numbers/optionnumbers.py` & `aiocoap-0.4b3/aiocoap/numbers/optionnumbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     SIZE2 = 28
     PROXY_URI = 35
     PROXY_SCHEME = 39
     SIZE1 = 60
     NO_RESPONSE = 258
     OBJECT_SECURITY = 9
     # picked for draft-ietf-core-echo-request-tag-09
-    ECHO = 540
+    ECHO = 248
     REQUEST_TAG = 292
 
     def is_critical(self):
         return self & 0x01 == 0x01
 
     def is_elective(self):
         return not self.is_critical()
```

### Comparing `aiocoap-0.4b2/aiocoap/numbers/types.py` & `aiocoap-0.4b3/aiocoap/numbers/types.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/options.py` & `aiocoap-0.4b3/aiocoap/options.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/optiontypes.py` & `aiocoap-0.4b3/aiocoap/optiontypes.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/oscore.py` & `aiocoap-0.4b3/aiocoap/oscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,14 +961,16 @@
         if not self.replay_window_persisted:
             data['received'] = 'unknown'
         else:
             data['received'] = self.recipient_replay_window.persist()
 
         with os.fdopen(tmphand, 'w') as tmpfile:
             json.dump(data, tmpfile)
+            tmpfile.flush()
+            os.fsync(tmpfile.fileno())
 
         os.rename(tmpnam, os.path.join(self.basedir, 'sequence.json'))
 
     def _replay_window_changed(self):
         if self.replay_window_persisted:
             # Just remove the sequence numbers once from the file
             self.replay_window_persisted = False
```

### Comparing `aiocoap-0.4b2/aiocoap/protocol.py` & `aiocoap-0.4b3/aiocoap/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,19 @@
 
     @classmethod
     async def create_server_context(cls, site, bind=None, *, loggername="coap-server", loop=None, _ssl_context=None):
         """Create a context, bound to all addresses on the CoAP port (unless
         otherwise specified in the ``bind`` argument).
 
         This is the easiest way to get a context suitable both for sending
-        client and accepting server requests."""
+        client and accepting server requests.
+
+        The ``bind`` argument, if given, needs to be a 2-tuple of IP address
+        string and port number, where the port number can be None to use the default port.
+        """
 
         if loop is None:
             loop = asyncio.get_event_loop()
 
         self = cls(loop=loop, serversite=site, loggername=loggername)
 
         for transportname in defaults.get_default_servertransports(loop=loop):
@@ -590,18 +594,25 @@
         self.response = asyncio.Future()
 
         if plumbing_request.request.opt.observe == 0:
             self.observation = ClientObservation()
         else:
             self.observation = None
 
-        loop.create_task(self._run())
+        self._runner = loop.create_task(self._run())
 
         self.log = log
 
+        self.response.add_done_callback(self._response_cancellation_handler)
+
+    def _response_cancellation_handler(self, response):
+        if self.response.cancelled() and not self._runner.cancelled():
+            self._runner.cancel()
+            self._plumbing_request.stop_interest()
+
     @staticmethod
     def _add_response_properties(response, request):
         response.request = request
 
     async def _run(self):
         # FIXME: check that responses come from the same remmote as long as we're assuming unicast
```

### Comparing `aiocoap-0.4b2/aiocoap/proxy/client.py` & `aiocoap-0.4b3/aiocoap/proxy/client.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/proxy/server.py` & `aiocoap-0.4b3/aiocoap/proxy/server.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/resource.py` & `aiocoap-0.4b3/aiocoap/resource.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/resourcedirectory/__init__.py` & `aiocoap-0.4b3/aiocoap/resourcedirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/resourcedirectory/client/__init__.py` & `aiocoap-0.4b3/aiocoap/resourcedirectory/client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/resourcedirectory/client/register.py` & `aiocoap-0.4b3/aiocoap/resourcedirectory/client/register.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/tokenmanager.py` & `aiocoap-0.4b3/aiocoap/tokenmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from collections import namedtuple
 import functools
 import os
 import random
 
 from . import error
 from . import interfaces
+# To be used sparingly here: This deals with request / responses on the token
+# layer. But the layer below won't even know that messages are responses, so it
+# can't make the informed decisions we make here.
+from .numbers.types import NON
 
 class TokenManager(interfaces.RequestInterface, interfaces.TokenManager):
     def __init__(self, context):
         self.context = context
 
         self._token = random.randint(0, 65535)
         self.outgoing_requests = {}  #: Unfinished outgoing requests (identified by token and remote)
@@ -80,15 +84,15 @@
     #
 
     def dispatch_error(self, errno, remote):
         keys_for_removal = []
         for key, request in self.outgoing_requests.items():
             (token, request_remote) = key
             if request_remote == remote:
-                request.add_exception(OSError(errno, os.strerror(errno)))
+                request.add_exception(OSError(errno, "no details" if errno is None else os.strerror(errno)))
                 keys_for_removal.append(key)
         for k in keys_for_removal:
             self.outgoing_requests.pop(k)
 
         keys_for_removal = [
                 (_p, _r)
                 for (_p, _r)
@@ -124,20 +128,26 @@
             while True:
                 ev = await pr._events.get()
                 if ev.message is not None:
                     m = ev.message
                     # FIXME: should this code warn if token or remote are set?
                     m.token = request.token
                     m.remote = request.remote.as_response_address()
+
+                    if m.mtype is None and request.mtype is NON:
+                        # Default to sending NON to NON requests; rely on the
+                        # default (CON if stand-alone else ACK) otherwise.
+                        m.mtype = NON
                     self.token_interface.send_message(m)
                 else:
                     self.log.error("Requests shouldn't receive errors at the level of a TokenManager any more, but this did: %s", ev.exception)
                 if ev.is_last:
                     break
-            # no cleanup to do here: any piggybackable ack was already flushed
+            del self.incoming_requests[key]
+            # no further cleanup to do here: any piggybackable ack was already flushed
             # out by the first response, and if there was not even a
             # NoResponse, something went wrong above (and we can't tell easily
             # here).
         task = self.loop.create_task(run())
 
         self.incoming_requests[key] = (pr, task)
 
@@ -148,15 +158,18 @@
         if key not in self.outgoing_requests:
             # maybe it was a multicast...
             key = (response.token, None)
 
         try:
             request = self.outgoing_requests[key]
         except KeyError:
+            self.log.info("Response %r could not be matched to any request", response)
             return False
+        else:
+            self.log.debug("Response %r matched to request %r", response, request)
 
         # FIXME: there's a multicast aspect to that as well
         #
         # Is it necessary to look into .opt.observe here, wouldn't that better
         # be done by the higher-level code that knows about CoAP options?
         # Maybe, but at some point in TokenManager we *have* to look into the
         # options to see whether to expect a short- or long-running token.
```

### Comparing `aiocoap-0.4b2/aiocoap/transports/__init__.py` & `aiocoap-0.4b3/aiocoap/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/generic_udp.py` & `aiocoap-0.4b3/aiocoap/transports/generic_udp.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/oscore.py` & `aiocoap-0.4b3/aiocoap/transports/oscore.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/simple6.py` & `aiocoap-0.4b3/aiocoap/transports/simple6.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/simplesocketserver.py` & `aiocoap-0.4b3/aiocoap/transports/simplesocketserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,39 @@
 While it is in theory capable of sending requests too, it should not be used
 like that, because it won't receive ICMP errors (see below).
 
 Shortcomings
 ------------
 
 * This implementation does not receive ICMP errors. This violates the CoAP
-    standard and can lead to unnecessary network traffic, bad user experience
-    (when used for client requests) or even network attack amplification.
+  standard and can lead to unnecessary network traffic, bad user experience
+  (when used for client requests) or even network attack amplification.
+
+* The server can not be used with the "any-address" (``::``, ``0.0.0.0``).
+  If it were allowed to bind there, it would not receive any indication from the operating system
+  as to which of its own addresses a request was sent,
+  and could not send the response with the appropriate sender address.
+
+  (The :mod:`udp6<aiocoap.transports.udp6>` transport does not suffer that shortcoming,
+  simplesocketserver is typically only used when that is unavailable).
+
+  With simplesocketserver, you need to explicitly give the IP address of your server
+  in the ``bind`` argument of :meth:`aiocoap.protocol.Context.create_server_context`.
 
 * This transport is experimental and likely to change.
 """
 
 import asyncio
 from collections import namedtuple
 
 from ..numbers import COAP_PORT
 from .. import interfaces
 from .generic_udp import GenericMessageInterface
 from ..util import hostportjoin
+from .. import defaults
 
 class _Address(namedtuple('_Address', ['serversocket', 'address']), interfaces.EndpointAddress):
     # hashability and equality follow from being a namedtuple
     def __repr__(self):
         return '<%s via %s to %s>'%(type(self).__name__, self.serversocket, self.address)
 
     def send(self, data):
@@ -83,15 +95,15 @@
             raise ValueError("The transport can not be bound to any-address.")
 
         ready = asyncio.Future()
 
         transport, protocol = await loop.create_datagram_endpoint(
                 lambda: cls(ready.set_result, new_message_callback, new_error_callback, log),
                 local_addr=bind,
-                reuse_port=True,
+                reuse_port=defaults.has_reuse_port(),
                 )
 
         # Conveniently, we only bind to a single port (because we need to know
         # the return address, not because we insist we know the local
         # hostinfo), and can thus store the local hostinfo without distinction
         protocol.hostinfo_local = hostportjoin(bind[0], bind[1] if bind[1] != COAP_PORT else None)
```

### Comparing `aiocoap-0.4b2/aiocoap/transports/tcp.py` & `aiocoap-0.4b3/aiocoap/transports/tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import asyncio
 import socket
 
 from aiocoap import interfaces, optiontypes, error, util
 from aiocoap import COAP_PORT, Message
 from aiocoap.numbers.codes import CSM, PING, PONG, RELEASE, ABORT
+from aiocoap import defaults
 
 def _extract_message_size(data: bytes):
     """Read out the full length of a CoAP messsage represented by data.
 
     Returns None if data is too short to read the (full) length.
 
     The number returned is the number of bytes that has to be read into data to
@@ -375,15 +376,15 @@
         def new_connection():
             c = TcpConnection(self, log, loop)
             self._pool.add(c)
             return c
 
         try:
             server = await loop.create_server(new_connection, bind[0], bind[1],
-                    ssl=_server_context)
+                    ssl=_server_context, reuse_port=defaults.has_reuse_port())
         except socket.gaierror:
             raise error.ResolutionError("No local bindable address found for %s" % bind[0])
         self.server = server
 
         return self
 
     def _evict_from_pool(self, connection):
```

### Comparing `aiocoap-0.4b2/aiocoap/transports/tinydtls.py` & `aiocoap-0.4b3/aiocoap/transports/tinydtls.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/tls.py` & `aiocoap-0.4b3/aiocoap/transports/tls.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/transports/udp6.py` & `aiocoap-0.4b3/aiocoap/transports/udp6.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 
 This implementation strives to be correct and complete behavior while still
 only using a single socket; that is, to be usable for all kinds of multicast
 traffic, to support server and client behavior at the same time, and to work
 correctly even when multiple IPv6 and IPv4 (using V4MAPPED addresses)
 interfaces are present, and any of the interfaces has multiple addresses.
 
-This requires using a plethorea of standardized but not necessarily widely
-ported features: ``AI_V4MAPPED`` to support IPv4 without resorting to less
+This requires using some standardized but not necessarily widely ported
+features: ``AI_V4MAPPED`` to support IPv4 without resorting to less
 standardized mechanisms for later options, ``IPV6_RECVPKTINFO`` to determine
 incoming packages' destination addresses (was it multicast) and to return
-packages from the same address, ``IPV6_RECVERR`` to receive ICMP errors even on
-sockets that are not connected, ``IPV6_JOIN_GROUP`` for multicast membership
-management, and ``recvmsg`` and ``MSG_ERRQUEUE`` to obtain the data configured
-with the above options.
+packages from the same address, ``IPV6_JOIN_GROUP`` for multicast
+membership management and ``recvmsg`` to obtain data configured with the above
+options.
+
+To the author's knowledge, there is no standardized mechanism for receiving
+ICMP errors in such a setup. On Linux, ``IPV6_RECVERR`` and ``MSG_ERRQUEUE``
+are used to receive ICMP errors from the socket; on other platforms, a warning
+is emitted that ICMP errors are ignored. Using a :mod:`.simple6` for clients is
+recommended for those when working as a client only.
 
-There are, if at all, only little attempts made to fall back to a
+Exceeding for the above error handling, no attempts are made to fall back to a
 kind-of-correct or limited-functionality behavior if these options are
 unavailable, for the resulting code would be hard to maintain ("``ifdef``
 hell") or would cause odd bugs at users (eg. servers that stop working when an
 additional IPv6 address gets assigned). If the module does not work for you,
 and the options can not be added easily to your platform, consider using the
 :mod:`.simple6` module instead.
 """
@@ -38,14 +43,15 @@
 import ipaddress
 import struct
 import weakref
 from collections import namedtuple
 
 from ..message import Message
 from ..numbers import constants
+from .. import defaults
 from .. import error
 from .. import interfaces
 from ..numbers import COAP_PORT
 from ..util.asyncio.recvmsg import RecvmsgDatagramProtocol, create_recvmsg_datagram_endpoint
 from ..util import hostportjoin, hostportsplit
 from ..util import socknumbers
 
@@ -183,19 +189,25 @@
         # FIXME: either raise an error if this is 0, or send a message to self
         # to force the OS to decide on a port. Right now, this reports wrong
         # results while the first message has not been sent yet.
         return self.transport.get_extra_info('socket').getsockname()[1]
 
     @classmethod
     async def _create_transport_endpoint(cls, sock, ctx: interfaces.MessageManager, log, loop, multicast=False):
-        sock.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_RECVPKTINFO, 1)
-        sock.setsockopt(socket.IPPROTO_IPV6, socknumbers.IPV6_RECVERR, 1)
-        # i'm curious why this is required; didn't IPV6_V6ONLY=0 already make
-        # it clear that i don't care about the ip version as long as everything looks the same?
-        sock.setsockopt(socket.IPPROTO_IP, socknumbers.IP_RECVERR, 1)
+        try:
+            sock.setsockopt(socket.IPPROTO_IPV6, socknumbers.IPV6_RECVPKTINFO, 1)
+        except NameError:
+            raise RuntimeError("RFC3542 PKTINFO flags are unavailable, unable to create a udp6 transport.")
+        if socknumbers.HAS_RECVERR:
+            sock.setsockopt(socket.IPPROTO_IPV6, socknumbers.IPV6_RECVERR, 1)
+            # i'm curious why this is required; didn't IPV6_V6ONLY=0 already make
+            # it clear that i don't care about the ip version as long as everything looks the same?
+            sock.setsockopt(socket.IPPROTO_IP, socknumbers.IP_RECVERR, 1)
+        else:
+            log.warning("Transport udp6 set up on platform without RECVERR capability. ICMP errors will be ignored.")
 
         if multicast:
             # FIXME this all registers only for one interface, doesn't it?
             s = struct.pack('4s4si',
                     socket.inet_aton(constants.MCAST_IPV4_ALLCOAPNODES),
                     socket.inet_aton("0.0.0.0"), 0)
             try:
@@ -249,16 +261,18 @@
             raise error.ResolutionError("No local bindable address found for %s" % bind[0])
         assert bind, "getaddrinfo returned zero-length list rather than erring out"
         (*_, bind), *additional = bind
         if additional:
             log.warning("Multiple addresses to bind to, ")
 
         sock = socket.socket(family=socket.AF_INET6, type=socket.SOCK_DGRAM)
-        # FIXME: SO_REUSEPORT should be safer when available (no port hijacking), and the test suite should work with it just as well (even without). why doesn't it?
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        if defaults.has_reuse_port():
+            # I doubt that there is any platform that supports RECVPKTINFO but
+            # not REUSEPORT, but why take chances.
+            sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         sock.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
         sock.bind(bind)
 
         return (await cls._create_transport_endpoint(sock, ctx, log, loop, multicast=True))
 
     async def shutdown(self):
         self._shutting_down = asyncio.Future()
@@ -268,15 +282,15 @@
         await self._shutting_down
 
         del self._ctx
 
     def send(self, message):
         ancdata = []
         if message.remote.pktinfo is not None:
-            ancdata.append((socket.IPPROTO_IPV6, socket.IPV6_PKTINFO,
+            ancdata.append((socket.IPPROTO_IPV6, socknumbers.IPV6_PKTINFO,
                 message.remote.pktinfo))
         self.transport.sendmsg(message.encode(), ancdata, 0, message.remote.sockaddr)
 
     async def recognize_remote(self, remote):
         return isinstance(remote, UDP6EndpointAddress) and \
                 remote.interface == self
 
@@ -325,15 +339,15 @@
         self.ready.set_result(True)
         self.transport = transport
 
     def datagram_msg_received(self, data, ancdata, flags, address):
         """Implementation of the RecvmsgDatagramProtocol interface, called by the transport."""
         pktinfo = None
         for cmsg_level, cmsg_type, cmsg_data in ancdata:
-            if cmsg_level == socket.IPPROTO_IPV6 and cmsg_type == socket.IPV6_PKTINFO:
+            if cmsg_level == socket.IPPROTO_IPV6 and cmsg_type == socknumbers.IPV6_PKTINFO:
                 pktinfo = cmsg_data
             else:
                 self.log.info("Received unexpected ancillary data to recvmsg: level %d, type %d, data %r", cmsg_level, cmsg_type, cmsg_data)
         try:
             message = Message.decode(data, UDP6EndpointAddress(address, self, pktinfo=pktinfo))
         except error.UnparsableMessage:
             self.log.warning("Ignoring unparsable message from %s"%(address,))
```

### Comparing `aiocoap-0.4b2/aiocoap/util/__init__.py` & `aiocoap-0.4b3/aiocoap/util/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/asyncio/peekqueue.py` & `aiocoap-0.4b3/aiocoap/util/asyncio/peekqueue.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/asyncio/pre35.py` & `aiocoap-0.4b3/aiocoap/util/asyncio/pre35.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/asyncio/recvmsg.py` & `aiocoap-0.4b3/aiocoap/util/asyncio/recvmsg.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,27 +68,28 @@
         self._loop = None
 
     def __del__(self):
         if self.__sock is not None:
             self.close()
 
     def _read_ready(self):
-        try:
-            data, ancdata, flags, addr = self.__sock.recvmsg(self.max_size, 1024, socknumbers.MSG_ERRQUEUE)
-        except (BlockingIOError, InterruptedError):
-            pass
-        except OSError as exc:
-            if repr(exc) == "OSError('received malformed or improperly truncated ancillary data',)":
-                pass # workaround for https://bitbucket.org/pypy/pypy/issues/2649/recvmsg-with-empty-err-queue-raises-odd
+        if socknumbers.HAS_RECVERR:
+            try:
+                data, ancdata, flags, addr = self.__sock.recvmsg(self.max_size, 1024, socknumbers.MSG_ERRQUEUE)
+            except (BlockingIOError, InterruptedError):
+                pass
+            except OSError as exc:
+                if repr(exc) == "OSError('received malformed or improperly truncated ancillary data',)":
+                    pass # workaround for https://bitbucket.org/pypy/pypy/issues/2649/recvmsg-with-empty-err-queue-raises-odd
+                else:
+                    self._protocol.error_received(exc)
+            except Exception as exc:
+                self._fatal_error(exc, 'Fatal read error on datagram transport')
             else:
-                self._protocol.error_received(exc)
-        except Exception as exc:
-            self._fatal_error(exc, 'Fatal read error on datagram transport')
-        else:
-            self._protocol.datagram_errqueue_received(data, ancdata, flags, addr)
+                self._protocol.datagram_errqueue_received(data, ancdata, flags, addr)
 
         # copied and modified from _SelectorDatagramTransport
         try:
             data, ancdata, flags, addr = self.__sock.recvmsg(self.max_size, 1024) # TODO: find a way for the application to tell the trensport how much data is expected
         except (BlockingIOError, InterruptedError):
             pass
         except OSError as exc:
```

### Comparing `aiocoap-0.4b2/aiocoap/util/cli.py` & `aiocoap-0.4b3/aiocoap/util/cli.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/linkformat.py` & `aiocoap-0.4b3/aiocoap/util/linkformat.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/linkformat_pygments.py` & `aiocoap-0.4b3/aiocoap/util/linkformat_pygments.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/prettyprint.py` & `aiocoap-0.4b3/aiocoap/util/prettyprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,22 @@
             show_hex = "CBOR value is invalid"
         else:
             info("CBOR message shown in naïve Python decoding")
             # Formatting it via Python b/c that's reliably available (as
             # opposed to JSON which might not round-trip well). The repr for
             # tags might still not be parsable, but I think chances of good
             # highlighting are best this way
-            formatted = pprint.pformat(parsed)
+            #
+            # Not sorting dicts to give a more faithful representation of the
+            # original CBOR message
+            if sys.version_info >= (3, 8):
+                printer = pprint.PrettyPrinter(sort_dicts=False)
+            else:
+                printer = pprint.PrettyPrinter()
+            formatted = printer.pformat(parsed)
             return (infos, 'text/x-python3', formatted)
 
     elif subtype == 'json' or subtype.endswith('+json'):
         try:
             parsed = json.loads(message.payload.decode('utf8'))
         except ValueError:
             pass
```

### Comparing `aiocoap-0.4b2/aiocoap/util/secrets.py` & `aiocoap-0.4b3/aiocoap/util/secrets.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap/util/socknumbers.py` & `aiocoap-0.4b3/aiocoap/util/socknumbers.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,58 @@
 #
 # aiocoap is free software, this file is published under the MIT license as
 # described in the accompanying LICENSE file.
 
 """This module contains numeric constants that would be expected in the socket
 module, but are not exposed there.
 
-For some platforms (eg. python up to 3.5 on Linux), there is an IN module that
-exposes them; and they are gathered from there.
+This gathers both socket numbers that can be present in the socket module (eg.
+the PKTINFO constants) but are not in some versions (eg. on macOS before
+<https://bugs.python.org/issue35569> is fixed) and platform dependent constants
+that are not generally available at all (the ERR constants).
 
-As a fallback, the numbers are hardcoded. Any hints on where to get them from
-are appreciated; possible options are parsing C header files (at build time?)
-or interacting with shared libraries for obtaining the symbols. The right way
-would probably be including them in Python.
+Where available, the CPython-private IN module is used to obtain some platform
+specific constants.
+
+Any hints on where to get them from in a more reliable way are appreciated;
+possible options are parsing C header files (at build time?) or interacting
+with shared libraries for obtaining the symbols. The right way would probably
+be including them in Python in a "other constants defined on this platform for
+sockets" module or dictionary.
 """
 
+import sys
+
 try:
-    from IN import IPV6_RECVERR, IP_RECVERR, IPV6_PKTINFO
+    from socket import IPV6_PKTINFO, IPV6_RECVPKTINFO
+except NameError:
+    if sys.platform == 'linux':
+        # Not sure if here are any Linux builds at all where this is
+        # unavailable
+        IPV6_PKTINFO = 50
+        IPv6_RECVPKTINFO = 49
+    elif sys.platform == 'darwin':
+        # when __APPLE_USE_RFC_3542 is defined / as would be when
+        # https://bugs.python.org/issue35569 is fixed
+        IPV6_PKTINFO = 46
+        IPV6_RECVPKTINFO = 61
+    # Not attempting to make any guesses for other platforms; the udp6 module
+    # will fail to import where it needs the specifics
+
+try:
+    from IN import IPV6_RECVERR, IP_RECVERR
 except (ImportError, NameError):
-    IPV6_RECVERR = 25
-    IP_RECVERR = 11
-    IPV6_PKTINFO = 50
+    if sys.platform == 'linux':
+        IPV6_RECVERR = 25
+        IP_RECVERR = 11
 
 # for https://bitbucket.org/pypy/pypy/issues/2648/
 try:
     from socket import MSG_ERRQUEUE
 except (ImportError, NameError):
-    MSG_ERRQUEUE = 8192
+    if sys.platform == 'linux':
+        MSG_ERRQUEUE = 8192
+
+HAS_RECVERR = 'IP_RECVERR' in locals() and 'MSG_ERRQUEUE' in locals()
+"""Indicates whether the discovered constants indicate that the Linux
+`setsockopt(IPV6, RECVERR)` / `recvmsg(..., MSG_ERRQUEUE)` mechanism is
+available"""
```

### Comparing `aiocoap-0.4b2/aiocoap/util/uri.py` & `aiocoap-0.4b3/aiocoap/util/uri.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/aiocoap.egg-info/PKG-INFO` & `aiocoap-0.4b3/aiocoap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocoap
-Version: 0.4b2
+Version: 0.4b3
 Summary: Python CoAP library
 Home-page: https://github.com/chrysn/aiocoap
 Author: Maciej Wasilak, Christian Amsüss
 Author-email: c.amsuess@energyharvesting.at
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: coap,asyncio,iot
```

### Comparing `aiocoap-0.4b2/aiocoap.egg-info/SOURCES.txt` & `aiocoap-0.4b3/aiocoap.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 aiocoap.egg-info/dependency_links.txt
 aiocoap.egg-info/entry_points.txt
 aiocoap.egg-info/requires.txt
 aiocoap.egg-info/top_level.txt
 aiocoap/cli/__init__.py
 aiocoap/cli/client.py
 aiocoap/cli/common.py
+aiocoap/cli/defaults.py
 aiocoap/cli/fileserver.py
 aiocoap/cli/proxy.py
 aiocoap/cli/rd.py
 aiocoap/numbers/__init__.py
 aiocoap/numbers/codes.py
 aiocoap/numbers/constants.py
 aiocoap/numbers/optionnumbers.py
@@ -63,23 +64,22 @@
 aiocoap/util/uri.py
 aiocoap/util/asyncio/__init__.py
 aiocoap/util/asyncio/peekqueue.py
 aiocoap/util/asyncio/pre35.py
 aiocoap/util/asyncio/recvmsg.py
 contrib/aiocoap-kivy-widget
 contrib/aiocoap-widgets
-contrib/oscore-key-derivation~
 contrib/rd-relay
 doc/LICENSE.rst
 doc/README.doc
 doc/aiocoap_index.py
 doc/api.rst
 doc/conf.py
-doc/conf.py~
 doc/examples.rst
+doc/faq.rst
 doc/guidedtour.rst
 doc/index.rst
 doc/installation.rst
 doc/logo-square.svg
 doc/logo.svg
 doc/news.rst
 doc/release-checklist
```

### Comparing `aiocoap-0.4b2/clientGET-observe.py` & `aiocoap-0.4b3/clientGET-observe.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/clientGET.py` & `aiocoap-0.4b3/clientGET.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/clientPUT.py` & `aiocoap-0.4b3/clientPUT.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/contrib/aiocoap-kivy-widget` & `aiocoap-0.4b3/contrib/aiocoap-kivy-widget`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/contrib/aiocoap-widgets` & `aiocoap-0.4b3/contrib/aiocoap-widgets`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/contrib/rd-relay` & `aiocoap-0.4b3/contrib/rd-relay`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/README.doc` & `aiocoap-0.4b3/doc/README.doc`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/aiocoap_index.py` & `aiocoap-0.4b3/doc/aiocoap_index.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/api.rst` & `aiocoap-0.4b3/doc/api.rst`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/conf.py` & `aiocoap-0.4b3/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '0.4'
 # The full version, including alpha/beta/rc tags.
-release = '0.4b2'
+release = '0.4b3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `aiocoap-0.4b2/doc/examples.rst` & `aiocoap-0.4b3/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/guidedtour.rst` & `aiocoap-0.4b3/doc/guidedtour.rst`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/installation.rst` & `aiocoap-0.4b3/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/logo-square.svg` & `aiocoap-0.4b3/doc/logo-square.svg`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/logo.svg` & `aiocoap-0.4b3/doc/logo.svg`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/doc/tools.rst` & `aiocoap-0.4b3/doc/tools.rst`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/server.py` & `aiocoap-0.4b3/server.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/setup.py` & `aiocoap-0.4b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 (Internet of Things) devices."""
 
 from setuptools import setup, find_packages
 from distutils.core import Command
 import os
 
 name = "aiocoap"
-version = "0.4b2" # Don't forget meta.version and doc/conf.py
+version = "0.4b3" # Don't forget meta.version and doc/conf.py
 description = "Python CoAP library"
 longdescription = __doc__
 
 # When introducing something new, make sure to update doc/installation.rst
 extras_require = {
         'linkheader': ['LinkHeader'],
         'oscore': ['hkdf', 'cbor', 'cryptography (>= 2.0)', 'filelock'],
```

### Comparing `aiocoap-0.4b2/tests/__init__.py` & `aiocoap-0.4b3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/common.py` & `aiocoap-0.4b3/tests/common.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/fixtures.py` & `aiocoap-0.4b3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_blockwise.py` & `aiocoap-0.4b3/tests/test_blockwise.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_commandline.py` & `aiocoap-0.4b3/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_credentials.py` & `aiocoap-0.4b3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_doctest.py` & `aiocoap-0.4b3/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_encoding.py` & `aiocoap-0.4b3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_noncoap_client.py` & `aiocoap-0.4b3/tests/test_noncoap_client.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_noncoap_tcp_client.py` & `aiocoap-0.4b3/tests/test_noncoap_tcp_client.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_observe.py` & `aiocoap-0.4b3/tests/test_observe.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_oscore.py` & `aiocoap-0.4b3/tests/test_oscore.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_oscore_plugtest.py` & `aiocoap-0.4b3/tests/test_oscore_plugtest.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_proxy.py` & `aiocoap-0.4b3/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_rd_examples.py` & `aiocoap-0.4b3/tests/test_rd_examples.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_reverseproxy.py` & `aiocoap-0.4b3/tests/test_reverseproxy.py`

 * *Files identical despite different names*

### Comparing `aiocoap-0.4b2/tests/test_server.py` & `aiocoap-0.4b3/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,20 @@
             return aiocoap.Message(code=aiocoap.NOT_ACCEPTABLE)
 
         return aiocoap.Message(payload=response, content_format=request.opt.accept or 0)
 
 class SlowResource(aiocoap.resource.Resource):
     async def render_get(self, request):
         await asyncio.sleep(0.2)
-        return aiocoap.Message()
+        # Marking the response as confirmable overrides the default behavior of
+        # sending NON responses to NON requests.
+        #
+        # This is done to aid the test_freeoncancel test, and should revert to
+        # the default behavior once that has better control over the environment.
+        return aiocoap.Message(mtype=aiocoap.CON)
 
 class BigResource(aiocoap.resource.Resource):
     async def render_get(self, request):
         # 10kb
         payload = b"0123456789----------" * 512
         response = aiocoap.Message(payload=payload)
```

### Comparing `aiocoap-0.4b2/tests/test_uri_handling.py` & `aiocoap-0.4b3/tests/test_uri_handling.py`

 * *Files identical despite different names*

