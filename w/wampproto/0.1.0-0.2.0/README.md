# Comparing `tmp/wampproto-0.1.0.tar.gz` & `tmp/wampproto-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wampproto-0.1.0.tar", last modified: Sat May  4 20:43:42 2024, max compression
+gzip compressed data, was "wampproto-0.2.0.tar", last modified: Mon May 13 12:56:20 2024, max compression
```

## Comparing `wampproto-0.1.0.tar` & `wampproto-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.532258 wampproto-0.1.0/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1102 2024-05-03 22:17:40.000000 wampproto-0.1.0/LICENSE
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2205 2024-05-04 20:43:42.532258 wampproto-0.1.0/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       69 2024-03-20 22:36:12.000000 wampproto-0.1.0/README.md
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      869 2024-05-04 20:31:55.000000 wampproto-0.1.0/pyproject.toml
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       38 2024-05-04 20:43:42.532258 wampproto-0.1.0/setup.cfg
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.524258 wampproto-0.1.0/tests/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-04-26 20:50:48.000000 wampproto-0.1.0/tests/test_session.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.524258 wampproto-0.1.0/wampproto/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       69 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     6939 2024-03-25 22:49:58.000000 wampproto-0.1.0/wampproto/acceptor.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.528258 wampproto-0.1.0/wampproto/auth/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1105 2024-03-25 20:18:27.000000 wampproto-0.1.0/wampproto/auth/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      384 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/auth/anonymous.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2537 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/auth/auth.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1616 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/auth/cryptosign.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      437 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/auth/ticket.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1551 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/auth/wampcra.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     3490 2024-05-03 22:17:40.000000 wampproto-0.1.0/wampproto/broker.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     4806 2024-05-04 20:12:12.000000 wampproto-0.1.0/wampproto/dealer.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      327 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/idgen.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2723 2024-03-25 22:49:58.000000 wampproto-0.1.0/wampproto/joiner.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.532258 wampproto-0.1.0/wampproto/messages/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1514 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      725 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/abort.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      958 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/authenticate.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1776 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/call.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      940 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/challenge.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1978 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/error.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1628 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/event.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1167 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/exceptions.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      743 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/goodbye.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     3286 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/hello.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1946 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/invocation.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      244 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/message.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1522 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/publish.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      868 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/published.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      927 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/register.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/registered.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1682 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/result.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      932 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/subscribe.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/subscribed.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/unregister.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/unregistered.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      859 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/unsubscribe.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/unsubscribed.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2750 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/util.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     3136 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/welcome.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1671 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/messages/yield_.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.532258 wampproto-0.1.0/wampproto/serializers/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      326 2024-03-25 22:49:58.000000 wampproto-0.1.0/wampproto/serializers/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      411 2024-03-25 20:18:27.000000 wampproto-0.1.0/wampproto/serializers/cbor.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      534 2024-03-31 00:09:12.000000 wampproto-0.1.0/wampproto/serializers/json.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      420 2024-03-25 20:18:27.000000 wampproto-0.1.0/wampproto/serializers/msgpack.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2638 2024-05-03 22:17:40.000000 wampproto-0.1.0/wampproto/serializers/serializer.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     6723 2024-05-03 22:17:40.000000 wampproto-0.1.0/wampproto/session.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1061 2024-04-26 20:50:48.000000 wampproto-0.1.0/wampproto/types.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-04 20:43:42.532258 wampproto-0.1.0/wampproto.egg-info/
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2205 2024-05-04 20:43:42.000000 wampproto-0.1.0/wampproto.egg-info/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1508 2024-05-04 20:43:42.000000 wampproto-0.1.0/wampproto.egg-info/SOURCES.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-04 20:43:42.000000 wampproto-0.1.0/wampproto.egg-info/dependency_links.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       50 2024-05-04 20:43:42.000000 wampproto-0.1.0/wampproto.egg-info/requires.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       10 2024-05-04 20:43:42.000000 wampproto-0.1.0/wampproto.egg-info/top_level.txt
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-10 20:22:04.000000 wampproto-0.2.0/LICENSE
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-13 12:56:20.062290 wampproto-0.2.0/PKG-INFO
+-rw-r--r--   0 om26er    (1000) om26er    (1000)       73 2024-05-13 12:47:17.000000 wampproto-0.2.0/README.md
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2405 2024-05-13 12:49:31.000000 wampproto-0.2.0/pyproject.toml
+-rw-r--r--   0 om26er    (1000) om26er    (1000)       38 2024-05-13 12:56:20.062290 wampproto-0.2.0/setup.cfg
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/tests/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-08 19:53:09.000000 wampproto-0.2.0/tests/test_session.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/wampproto/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       69 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     6939 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/acceptor.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.058290 wampproto-0.2.0/wampproto/auth/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1105 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      384 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/anonymous.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2537 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/auth.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1616 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/cryptosign.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      437 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/ticket.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1551 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/auth/wampcra.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     4140 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/broker.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     5216 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/dealer.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      327 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/idgen.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2723 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/joiner.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto/messages/
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     1641 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      725 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/abort.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      958 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/authenticate.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1776 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/call.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)      923 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/cancel.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      940 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/challenge.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1978 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/error.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1628 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/event.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1167 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/exceptions.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      743 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/goodbye.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     3286 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/hello.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)      958 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/interrupt.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1946 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/invocation.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      244 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/message.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1522 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/publish.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)      868 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/messages/published.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      927 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/register.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/registered.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1682 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/result.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      932 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/subscribe.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/subscribed.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      850 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unregister.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unregistered.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      859 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unsubscribe.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      654 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/unsubscribed.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2750 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/util.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     3136 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/welcome.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1671 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/messages/yield_.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto/serializers/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      326 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      411 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/cbor.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      534 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/json.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      420 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/serializers/msgpack.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2814 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/serializers/serializer.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     6723 2024-05-08 19:53:09.000000 wampproto-0.2.0/wampproto/session.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     1210 2024-05-13 12:47:17.000000 wampproto-0.2.0/wampproto/types.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 12:56:20.062290 wampproto-0.2.0/wampproto.egg-info/
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2320 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1569 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/SOURCES.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/dependency_links.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       73 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/requires.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       10 2024-05-13 12:56:20.000000 wampproto-0.2.0/wampproto.egg-info/top_level.txt
```

### Comparing `wampproto-0.1.0/LICENSE` & `wampproto-0.2.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
-Copyright (c) 2024 XConnIO
 Copyright (c) 2024 Simple Things Inc.
+Copyright (c) 2024 XConnIO Ltd.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `wampproto-0.1.0/PKG-INFO` & `wampproto-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wampproto
-Version: 0.1.0
+Version: 0.2.0
 Summary: https://github.com/xconnio/wampproto.py
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
-        Copyright (c) 2024 XConnIO
         Copyright (c) 2024 Simple Things Inc.
+        Copyright (c) 2024 XConnIO Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -39,10 +39,13 @@
 Requires-Dist: cbor2
 Requires-Dist: msgpack
 Requires-Dist: pynacl
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruff; extra == "test"
+Provides-Extra: publish
+Requires-Dist: twine; extra == "publish"
+Requires-Dist: build; extra == "publish"
 
-# wampproto.py
+# wampproto-python
 Sans-IO implementation of the WAMP protocol in Python
```

### Comparing `wampproto-0.1.0/tests/test_session.py` & `wampproto-0.2.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/acceptor.py` & `wampproto-0.2.0/wampproto/acceptor.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/auth/__init__.py` & `wampproto-0.2.0/wampproto/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/auth/auth.py` & `wampproto-0.2.0/wampproto/auth/auth.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/auth/cryptosign.py` & `wampproto-0.2.0/wampproto/auth/cryptosign.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/auth/wampcra.py` & `wampproto-0.2.0/wampproto/auth/wampcra.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/broker.py` & `wampproto-0.2.0/wampproto/broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,97 @@
-from typing import Optional
+from dataclasses import dataclass
 
 from wampproto import messages, types, idgen
 
 
+@dataclass
+class Subscription:
+    id: int
+    topic: str
+    subscribers: dict[int, int]
+
+
 class Broker:
     def __init__(self):
         super().__init__()
-        self.subscriptions_by_topic: dict[str, dict[int, int]] = {}
-        self.subscriptions_by_session: dict[int, dict[int, str]] = {}
+        self.subscriptions_by_topic: dict[str, Subscription] = {}
+        self.subscriptions_by_session: dict[int, dict[int, Subscription]] = {}
         self.id_gen = idgen.SessionScopeIDGenerator()
 
     def add_session(self, sid: int):
         if sid in self.subscriptions_by_session:
             raise ValueError("cannot add session twice")
 
         self.subscriptions_by_session[sid] = {}
 
     def remove_session(self, sid: int):
         if sid not in self.subscriptions_by_session:
             raise ValueError("cannot remove non-existing session")
 
-        subscription = self.subscriptions_by_session.pop(sid)
-        for k, v in subscription.items():
-            del self.subscriptions_by_topic[v][k]
-            if len(self.subscriptions_by_topic[v]) == 0:
-                del self.subscriptions_by_topic[v]
+        subscriptions = self.subscriptions_by_session.pop(sid)
+        for subscription_id, sub in subscriptions.items():
+            subscription = self.subscriptions_by_topic[sub.topic]
+            if sid in subscription.subscribers:
+                del subscription.subscribers[sid]
+
+            if len(subscription.subscribers) == 0:
+                del self.subscriptions_by_topic[subscription.topic]
 
     def has_subscription(self, topic: str):
-        return len(self.subscriptions_by_topic[topic]) != 0
+        return topic in self.subscriptions_by_topic
 
-    def receive_message(self, session_id: int, message: messages.Message) -> Optional[list[types.MessageWithRecipient]]:
+    def receive_message(self, session_id: int, message: messages.Message) -> types.MessageWithRecipient:
         if isinstance(message, messages.Subscribe):
             if session_id not in self.subscriptions_by_session:
                 raise ValueError(f"cannot subscribe, session {session_id} doesn't exist")
 
-            subscription_id = self.id_gen.next()
-            self.subscriptions_by_session[session_id][subscription_id] = message.topic
-            if message.topic not in self.subscriptions_by_topic:
-                self.subscriptions_by_topic[message.topic] = {}
+            subscription = self.subscriptions_by_topic.get(message.topic)
+            if subscription is None:
+                subscription = Subscription(self.id_gen.next(), message.topic, {session_id: session_id})
+                self.subscriptions_by_topic[message.topic] = subscription
+            else:
+                subscription.subscribers[session_id] = session_id
 
-            self.subscriptions_by_topic[message.topic][subscription_id] = session_id
+            self.subscriptions_by_session[session_id][subscription.id] = subscription
 
-            subscribed = messages.Subscribed(message.request_id, subscription_id)
-            return [types.MessageWithRecipient(subscribed, session_id)]
+            subscribed = messages.Subscribed(message.request_id, subscription.id)
+            return types.MessageWithRecipient(subscribed, session_id)
         elif isinstance(message, messages.UnSubscribe):
             if session_id not in self.subscriptions_by_session:
                 raise ValueError(f"cannot unsubscribe, session {session_id} doesn't exist")
 
             subscriptions = self.subscriptions_by_session[session_id]
-            topic = subscriptions.get(message.subscription_id)
-            if topic is None:
+            subscription = subscriptions.get(message.subscription_id)
+            if subscription is None:
                 raise ValueError(f"cannot unsubscribe, subscription {message.subscription_id} doesn't exist")
 
+            del subscription.subscribers[session_id]
+            if len(subscription.subscribers) == 0:
+                del self.subscriptions_by_topic[subscription.topic]
+
             del self.subscriptions_by_session[session_id][message.subscription_id]
-            del self.subscriptions_by_topic[topic][message.subscription_id]
 
             unsubscribed = messages.UnSubscribed(message.request_id)
-            return [types.MessageWithRecipient(unsubscribed, session_id)]
-        elif isinstance(message, messages.Publish):
-            if session_id not in self.subscriptions_by_session:
-                raise ValueError(f"cannot publish, session {session_id} doesn't exist")
-
-            subscriptions = self.subscriptions_by_topic.get(message.uri, [])
-            if len(subscriptions) == 0:
-                return None
-
-            publication_id = self.id_gen.next()
-            result: list[types.MessageWithRecipient] = []
-            for subscription_id, recipient_id in subscriptions.items():
-                event = messages.Event(subscription_id, publication_id, message.args, message.kwargs)
-                result.append(types.MessageWithRecipient(event, recipient_id))
-
-            return result
+            return types.MessageWithRecipient(unsubscribed, session_id)
         else:
             raise ValueError("message type not supported")
+
+    def receive_publish(self, session_id: int, message: messages.Publish) -> types.Publication:
+        if session_id not in self.subscriptions_by_session:
+            raise ValueError(f"cannot publish, session {session_id} doesn't exist")
+
+        result = types.Publication(recipients=[])
+        publication_id = self.id_gen.next()
+
+        subscription = self.subscriptions_by_topic.get(message.uri)
+        if subscription is not None:
+            event = messages.Event(subscription.id, publication_id, message.args, message.kwargs)
+            result.event = event
+            for subscriber_id in subscription.subscribers.keys():
+                result.recipients.append(subscriber_id)
+
+        ack = message.options.get("acknowledge", False)
+        if ack:
+            published = messages.Published(message.request_id, publication_id)
+            result.ack = types.MessageWithRecipient(published, session_id)
+
+        return result
```

### Comparing `wampproto-0.1.0/wampproto/dealer.py` & `wampproto-0.2.0/wampproto/dealer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,26 @@
 @dataclass
 class PendingInvocation:
     request_id: int
     caller_id: int
     callee_id: int
 
 
+@dataclass
+class Registration:
+    id: int
+    procedure: str
+    registrants: dict[int, int]
+    invocation_policy: str | None = None
+
+
 class Dealer:
     def __init__(self):
-        self.registrations_by_procedure: dict[str, dict[int, int]] = {}
-        self.registrations_by_session: dict[int, dict[int, str]] = {}
+        self.registrations_by_procedure: dict[str, Registration] = {}
+        self.registrations_by_session: dict[int, dict[int, Registration]] = {}
         self.pending_calls: dict[int, PendingInvocation] = {}
 
         self.id_gen = idgen.SessionScopeIDGenerator()
 
     def add_session(self, sid: int):
         if sid in self.registrations_by_session:
             raise ValueError("cannot add session twice")
@@ -25,41 +33,42 @@
         self.registrations_by_session[sid] = {}
 
     def remove_session(self, sid: int):
         if sid not in self.registrations_by_session:
             raise ValueError("cannot remove non-existing session")
 
         registrations = self.registrations_by_session.pop(sid)
-        for k, v in registrations.items():
-            del self.registrations_by_procedure[v][k]
-            if len(self.registrations_by_procedure[v]) == 0:
-                del self.registrations_by_procedure[v]
+        for registration_id, registration in registrations.items():
+            registration = self.registrations_by_procedure[registration.procedure]
+            if sid in registration.registrants:
+                del registration.registrants[sid]
 
-    def has_registration(self, procedure: str):
-        return len(self.registrations_by_procedure[procedure]) != 0
+            if len(registration.registrants) == 0:
+                del self.registrations_by_procedure[registration.procedure]
+
+    def has_registration(self, procedure: str) -> bool:
+        return procedure in self.registrations_by_procedure
 
     def receive_message(self, session_id: int, message: messages.Message) -> types.MessageWithRecipient:
         if isinstance(message, messages.Call):
-            registrations = self.registrations_by_procedure.get(message.uri)
-            if registrations is None or len(registrations) == 0:
+            registration = self.registrations_by_procedure.get(message.uri)
+            if registration is None:
                 err = messages.Error(message.TYPE, message.request_id, "wamp.error.no_such_procedure")
                 return types.MessageWithRecipient(err, session_id)
 
             callee_id: int = 0
-            registration: int = 0
-            for reg_id, session in registrations.items():
-                registration = reg_id
+            for session in registration.registrants.keys():
                 callee_id = session
                 break
 
             request_id = self.id_gen.next()
             self.pending_calls[request_id] = PendingInvocation(message.request_id, session_id, callee_id)
             invocation = messages.Invocation(
                 request_id=request_id,
-                registration_id=registration,
+                registration_id=registration.id,
                 args=message.args,
                 kwargs=message.kwargs,
             )
 
             return types.MessageWithRecipient(invocation, callee_id)
         elif isinstance(message, messages.Yield):
             try:
@@ -72,37 +81,42 @@
 
             result = messages.Result(request_id=invocation.request_id, args=message.args, kwargs=message.kwargs)
             return types.MessageWithRecipient(result, invocation.caller_id)
         elif isinstance(message, messages.Register):
             if session_id not in self.registrations_by_session:
                 raise ValueError(f"cannot register, session {session_id} doesn't exist")
 
-            if message.uri in self.registrations_by_procedure:
+            registration = self.registrations_by_procedure.get(message.uri)
+            if registration is None:
+                registration = Registration(self.id_gen.next(), message.uri, {session_id: session_id})
+                self.registrations_by_procedure[message.uri] = registration
+                self.registrations_by_session[session_id][registration.id] = registration
+            else:
+                # TODO: implement shared registrations.
                 registered = messages.Error(
                     messages.Register.TYPE, message.request_id, "wamp.error.procedure_already_exists"
                 )
                 return types.MessageWithRecipient(registered, session_id)
 
-            registration_id = self.id_gen.next()
-            self.registrations_by_session[session_id][registration_id] = message.uri
-            if message.uri not in self.registrations_by_procedure:
-                self.registrations_by_procedure[message.uri] = {}
-
-            self.registrations_by_procedure[message.uri][registration_id] = session_id
-
-            registered = messages.Registered(message.request_id, registration_id)
+            registered = messages.Registered(message.request_id, registration.id)
             return types.MessageWithRecipient(registered, session_id)
         elif isinstance(message, messages.UnRegister):
-            if session_id not in self.registrations_by_session:
+            registrations = self.registrations_by_session.get(session_id)
+            if registrations is None:
                 raise ValueError(f"cannot unregister, session {session_id} doesn't exist")
 
-            registrations = self.registrations_by_session[session_id]
-            procedure = registrations.get(message.registration_id)
-            del self.registrations_by_session[session_id][message.registration_id]
-            del self.registrations_by_procedure[procedure][message.registration_id]
-            if len(self.registrations_by_procedure[procedure]) == 0:
-                del self.registrations_by_procedure[procedure]
+            registration = registrations.get(message.registration_id)
+            try:
+                registration.registrants.pop(session_id)
+            except KeyError:
+                raise ValueError(f"cannot unregister, session {session_id} haven't registered for {registration.id}")
+
+            if len(registration.registrants) == 0:
+                del registrations[message.registration_id]
+                del self.registrations_by_procedure[registration.procedure]
+
+            self.registrations_by_session[session_id] = registrations
 
             unregistered = messages.UnRegistered(message.request_id)
             return types.MessageWithRecipient(unregistered, session_id)
         else:
             raise ValueError("message type not supported")
```

### Comparing `wampproto-0.1.0/wampproto/joiner.py` & `wampproto-0.2.0/wampproto/joiner.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/__init__.py` & `wampproto-0.2.0/wampproto/messages/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from wampproto.messages.published import Published
 from wampproto.messages.event import Event
 from wampproto.messages.subscribe import Subscribe
 from wampproto.messages.subscribed import Subscribed
 from wampproto.messages.unsubscribe import UnSubscribe
 from wampproto.messages.unsubscribed import UnSubscribed
 from wampproto.messages.error import Error
+from wampproto.messages.cancel import Cancel
+from wampproto.messages.interrupt import Interrupt
 
 __all__ = (
     "Message",
     "Hello",
     "Welcome",
     "Abort",
     "Challenge",
@@ -42,8 +44,10 @@
     "Published",
     "Event",
     "Subscribe",
     "Subscribed",
     "UnSubscribe",
     "UnSubscribed",
     "Error",
+    "Cancel",
+    "Interrupt",
 )
```

### Comparing `wampproto-0.1.0/wampproto/messages/abort.py` & `wampproto-0.2.0/wampproto/messages/abort.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/authenticate.py` & `wampproto-0.2.0/wampproto/messages/authenticate.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/call.py` & `wampproto-0.2.0/wampproto/messages/call.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/challenge.py` & `wampproto-0.2.0/wampproto/messages/challenge.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/error.py` & `wampproto-0.2.0/wampproto/messages/error.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/event.py` & `wampproto-0.2.0/wampproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/exceptions.py` & `wampproto-0.2.0/wampproto/messages/exceptions.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/goodbye.py` & `wampproto-0.2.0/wampproto/messages/goodbye.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/hello.py` & `wampproto-0.2.0/wampproto/messages/hello.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/invocation.py` & `wampproto-0.2.0/wampproto/messages/invocation.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/publish.py` & `wampproto-0.2.0/wampproto/messages/publish.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/published.py` & `wampproto-0.2.0/wampproto/messages/published.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
         request_id = util.validate_session_id_or_raise(msg[1], Published.TEXT, "request ID")
         publication_id = util.validate_session_id_or_raise(msg[2], Published.TEXT, "publication ID")
 
         return Published(request_id, publication_id)
 
     def marshal(self) -> list[Any]:
-        return [Published.TEXT, self.request_id, self.publication_id]
+        return [Published.TYPE, self.request_id, self.publication_id]
```

### Comparing `wampproto-0.1.0/wampproto/messages/register.py` & `wampproto-0.2.0/wampproto/messages/register.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/registered.py` & `wampproto-0.2.0/wampproto/messages/registered.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/result.py` & `wampproto-0.2.0/wampproto/messages/result.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/subscribe.py` & `wampproto-0.2.0/wampproto/messages/subscribe.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/subscribed.py` & `wampproto-0.2.0/wampproto/messages/subscribed.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/unregister.py` & `wampproto-0.2.0/wampproto/messages/unregister.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/unregistered.py` & `wampproto-0.2.0/wampproto/messages/unregistered.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/unsubscribe.py` & `wampproto-0.2.0/wampproto/messages/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/unsubscribed.py` & `wampproto-0.2.0/wampproto/messages/unsubscribed.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/util.py` & `wampproto-0.2.0/wampproto/messages/util.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/welcome.py` & `wampproto-0.2.0/wampproto/messages/welcome.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/messages/yield_.py` & `wampproto-0.2.0/wampproto/messages/yield_.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/serializers/json.py` & `wampproto-0.2.0/wampproto/serializers/json.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/serializers/serializer.py` & `wampproto-0.2.0/wampproto/serializers/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,13 @@
             return messages.Publish.parse(message)
         case messages.Published.TYPE:
             return messages.Published.parse(message)
         case messages.Event.TYPE:
             return messages.Event.parse(message)
         case messages.Error.TYPE:
             return messages.Error.parse(message)
+        case messages.Cancel.TYPE:
+            return messages.Cancel.parse(message)
+        case messages.Interrupt.TYPE:
+            return messages.Interrupt.parse(message)
         case _:
             raise ValueError("unknown message type")
```

### Comparing `wampproto-0.1.0/wampproto/session.py` & `wampproto-0.2.0/wampproto/session.py`

 * *Files identical despite different names*

### Comparing `wampproto-0.1.0/wampproto/types.py` & `wampproto-0.2.0/wampproto/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -38,7 +38,14 @@
         )
 
 
 @dataclass
 class MessageWithRecipient:
     message: messages.Message
     recipient: int
+
+
+@dataclass
+class Publication:
+    event: messages.Event | None = None
+    recipients: list[int] = None
+    ack: MessageWithRecipient | None = None
```

### Comparing `wampproto-0.1.0/wampproto.egg-info/PKG-INFO` & `wampproto-0.2.0/wampproto.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wampproto
-Version: 0.1.0
+Version: 0.2.0
 Summary: https://github.com/xconnio/wampproto.py
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
-        Copyright (c) 2024 XConnIO
         Copyright (c) 2024 Simple Things Inc.
+        Copyright (c) 2024 XConnIO Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -39,10 +39,13 @@
 Requires-Dist: cbor2
 Requires-Dist: msgpack
 Requires-Dist: pynacl
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruff; extra == "test"
+Provides-Extra: publish
+Requires-Dist: twine; extra == "publish"
+Requires-Dist: build; extra == "publish"
 
-# wampproto.py
+# wampproto-python
 Sans-IO implementation of the WAMP protocol in Python
```

### Comparing `wampproto-0.1.0/wampproto.egg-info/SOURCES.txt` & `wampproto-0.2.0/wampproto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 wampproto/auth/cryptosign.py
 wampproto/auth/ticket.py
 wampproto/auth/wampcra.py
 wampproto/messages/__init__.py
 wampproto/messages/abort.py
 wampproto/messages/authenticate.py
 wampproto/messages/call.py
+wampproto/messages/cancel.py
 wampproto/messages/challenge.py
 wampproto/messages/error.py
 wampproto/messages/event.py
 wampproto/messages/exceptions.py
 wampproto/messages/goodbye.py
 wampproto/messages/hello.py
+wampproto/messages/interrupt.py
 wampproto/messages/invocation.py
 wampproto/messages/message.py
 wampproto/messages/publish.py
 wampproto/messages/published.py
 wampproto/messages/register.py
 wampproto/messages/registered.py
 wampproto/messages/result.py
```

