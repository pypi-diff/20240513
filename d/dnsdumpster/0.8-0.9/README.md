# Comparing `tmp/dnsdumpster-0.8.tar.gz` & `tmp/dnsdumpster-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dnsdumpster-0.8.tar", last modified: Thu Feb 25 21:25:50 2021, max compression
+gzip compressed data, was "dist/dnsdumpster-0.9.tar", last modified: Mon May 13 21:10:40 2024, max compression
```

## Comparing `dnsdumpster-0.8.tar` & `dnsdumpster-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      355 2021-02-25 21:25:50.000000 dnsdumpster-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    25618 2021-02-25 21:25:49.000000 dnsdumpster-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster/
--rw-r--r--   0 runner    (1001) docker     (116)     1534 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/API_example.py
--rw-r--r--   0 runner    (1001) docker     (116)     4334 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/DNSDumpsterAPI.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      204 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      355 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      307 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-02-25 21:25:50.000000 dnsdumpster-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      501 2021-02-25 21:25:49.000000 dnsdumpster-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:10:40.000000 dnsdumpster-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 21:10:40.000000 dnsdumpster-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-13 21:10:37.000000 dnsdumpster-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:10:40.000000 dnsdumpster-0.9/dnsdumpster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 21:10:37.000000 dnsdumpster-0.9/dnsdumpster/API_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-13 21:10:37.000000 dnsdumpster-0.9/dnsdumpster/DNSDumpsterAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:10:37.000000 dnsdumpster-0.9/dnsdumpster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 21:10:37.000000 dnsdumpster-0.9/dnsdumpster/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:10:40.000000 dnsdumpster-0.9/dnsdumpster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 21:10:39.000000 dnsdumpster-0.9/dnsdumpster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 21:10:40.000000 dnsdumpster-0.9/dnsdumpster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:10:39.000000 dnsdumpster-0.9/dnsdumpster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 21:10:39.000000 dnsdumpster-0.9/dnsdumpster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 21:10:39.000000 dnsdumpster-0.9/dnsdumpster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 21:10:40.000000 dnsdumpster-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 21:10:37.000000 dnsdumpster-0.9/setup.py
```

### Comparing `dnsdumpster-0.8/README.md` & `dnsdumpster-0.9/README.md`

 * *Files identical despite different names*

### Comparing `dnsdumpster-0.8/dnsdumpster/API_example.py` & `dnsdumpster-0.9/dnsdumpster/API_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 image_retrieved = res['image_data'] is not None
 print("\n\n\nRetrieved Network mapping image? {} (accessible in 'image_data')".format(image_retrieved))
 print(repr(base64.b64decode(res['image_data'])[:20]) + '...') # to save it somewhere else.
 
 xls_retrieved = res['xls_data'] is not None
 print("\n\n\nRetrieved XLS hosts? {} (accessible in 'xls_data')".format(xls_retrieved))
 print(repr(base64.b64decode(res['xls_data'])[:20]) + '...') # to save it somewhere else.
-# open('tsebo.com.xlsx','wb').write(res['xls_data'].decode('base64')) # example of saving xlsx
+# open('tsebo.com.xlsx','wb').write(base64.b64decode(res['xls_data'])) # example of saving xlsx
```

### Comparing `dnsdumpster-0.8/dnsdumpster/DNSDumpsterAPI.py` & `dnsdumpster-0.9/dnsdumpster/DNSDumpsterAPI.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
         req = self.session.get(dnsdumpster_url)
         soup = BeautifulSoup(req.content, 'html.parser')
         csrf_middleware = soup.findAll('input', attrs={'name': 'csrfmiddlewaretoken'})[0]['value']
         self.display_message('Retrieved token: %s' % csrf_middleware)
 
         cookies = {'csrftoken': csrf_middleware}
-        headers = {'Referer': dnsdumpster_url}
-        data = {'csrfmiddlewaretoken': csrf_middleware, 'targetip': domain}
+        headers = {'Referer': dnsdumpster_url, 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.107 Safari/537.36'}
+        data = {'csrfmiddlewaretoken': csrf_middleware, 'targetip': domain, 'user': 'free'}
         req = self.session.post(dnsdumpster_url, cookies=cookies, data=data, headers=headers)
 
         if req.status_code != 200:
             print(
                 "Unexpected status code from {url}: {code}".format(
                     url=dnsdumpster_url, code=req.status_code),
                 file=sys.stderr,
```

