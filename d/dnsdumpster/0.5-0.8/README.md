# Comparing `tmp/dnsdumpster-0.5.tar.gz` & `tmp/dnsdumpster-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dnsdumpster-0.5.tar", last modified: Fri Feb 16 19:07:04 2018, max compression
+gzip compressed data, was "dist/dnsdumpster-0.8.tar", last modified: Thu Feb 25 21:25:50 2021, max compression
```

## Comparing `dnsdumpster-0.5.tar` & `dnsdumpster-0.8.tar`

### file list

```diff
@@ -1,9 +1,16 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2018-02-16 19:07:04.000000 dnsdumpster-0.5/
--rw-r--r--   0 paul       (501) staff       (20)      355 2018-02-16 19:07:04.000000 dnsdumpster-0.5/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      504 2018-02-16 19:06:42.000000 dnsdumpster-0.5/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2018-02-16 19:07:04.000000 dnsdumpster-0.5/dnsdumpster/
--rw-r--r--   0 paul       (501) staff       (20)        0 2017-02-28 17:45:39.000000 dnsdumpster-0.5/dnsdumpster/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1534 2017-10-24 19:30:04.000000 dnsdumpster-0.5/dnsdumpster/API_example.py
--rw-r--r--   0 paul       (501) staff       (20)     4256 2018-02-16 19:05:18.000000 dnsdumpster-0.5/dnsdumpster/DNSDumpsterAPI.py
--rw-r--r--   0 paul       (501) staff       (20)      204 2017-10-25 18:52:04.000000 dnsdumpster-0.5/dnsdumpster/test_api.py
--rw-r--r--   0 paul       (501) staff       (20)       40 2017-02-28 17:33:41.000000 dnsdumpster-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2021-02-25 21:25:50.000000 dnsdumpster-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    25618 2021-02-25 21:25:49.000000 dnsdumpster-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster/
+-rw-r--r--   0 runner    (1001) docker     (116)     1534 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/API_example.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4334 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/DNSDumpsterAPI.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      204 2021-02-25 21:25:49.000000 dnsdumpster-0.8/dnsdumpster/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2021-02-25 21:25:50.000000 dnsdumpster-0.8/dnsdumpster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       79 2021-02-25 21:25:50.000000 dnsdumpster-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      501 2021-02-25 21:25:49.000000 dnsdumpster-0.8/setup.py
```

### Comparing `dnsdumpster-0.5/dnsdumpster/API_example.py` & `dnsdumpster-0.8/dnsdumpster/API_example.py`

 * *Files identical despite different names*

### Comparing `dnsdumpster-0.5/dnsdumpster/DNSDumpsterAPI.py` & `dnsdumpster-0.8/dnsdumpster/DNSDumpsterAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         res = []
         trs = table.findAll('tr')
         for tr in trs:
             tds = tr.findAll('td')
             pattern_ip = r'([0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3})'
             try:
                 ip = re.findall(pattern_ip, tds[1].text)[0]
-                domain = str(tds[0]).split('<br/>')[0].split('>')[1]
+                domain = str(tds[0]).split('<br/>')[0].split('>')[1].split('<')[0]
                 header = ' '.join(tds[0].text.replace('\n', '').split(' ')[1:])
                 reverse_dns = tds[1].find('span', attrs={}).text
 
                 additional_info = tds[2].text
                 country = tds[2].find('span', attrs={}).text
                 autonomous_system = additional_info.split(' ')[0]
                 provider = ' '.join(additional_info.split(' ')[1:])
@@ -81,15 +81,15 @@
             print(
                 "Unexpected status code from {url}: {code}".format(
                     url=dnsdumpster_url, code=req.status_code),
                 file=sys.stderr,
             )
             return []
 
-        if 'error' in req.content.decode('utf-8'):
+        if 'There was an error getting results' in req.content.decode('utf-8'):
             print("There was an error getting results", file=sys.stderr)
             return []
 
         soup = BeautifulSoup(req.content, 'html.parser')
         tables = soup.findAll('table')
 
         res = {}
@@ -108,16 +108,17 @@
             image_data = None
         finally:
             res['image_data'] = image_data
 
         # XLS hosts.
         # eg. tsebo.com-201606131255.xlsx
         try:
-            pattern = r'https://dnsdumpster.com/static/xls/' + domain + '-[0-9]{12}\.xlsx'
+            pattern = r'/static/xls/' + domain + '-[0-9]{12}\.xlsx'
             xls_url = re.findall(pattern, req.content.decode('utf-8'))[0]
+            xls_url = 'https://dnsdumpster.com' + xls_url
             xls_data = base64.b64encode(self.session.get(xls_url).content)
         except Exception as err:
             print(err)
             xls_data = None
         finally:
             res['xls_data'] = xls_data
```

