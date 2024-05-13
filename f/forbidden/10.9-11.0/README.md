# Comparing `tmp/forbidden-10.9.tar.gz` & `tmp/forbidden-11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forbidden-10.9.tar", last modified: Sat May 11 10:15:23 2024, max compression
+gzip compressed data, was "forbidden-11.0.tar", last modified: Mon May 13 09:53:47 2024, max compression
```

## Comparing `forbidden-10.9.tar` & `forbidden-11.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:15:23.904621 forbidden-10.9/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 09:56:01.000000 forbidden-10.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-11 09:56:01.000000 forbidden-10.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15485 2024-05-11 10:15:23.904621 forbidden-10.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14779 2024-05-11 09:57:56.000000 forbidden-10.9/README.md
--rw-r--r--   0 root         (0) root         (0)      895 2024-05-11 10:10:42.000000 forbidden-10.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 10:15:23.904621 forbidden-10.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:15:23.900618 forbidden-10.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:15:23.900618 forbidden-10.9/src/forbidden/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:56:01.000000 forbidden-10.9/src/forbidden/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66238 2024-05-11 09:58:18.000000 forbidden-10.9/src/forbidden/forbidden.py
--rw-r--r--   0 root         (0) root         (0)    11174 2024-05-11 09:59:35.000000 forbidden-10.9/src/forbidden/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:15:23.904621 forbidden-10.9/src/forbidden.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15485 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-11 10:15:23.000000 forbidden-10.9/src/forbidden.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 10:15:23.904621 forbidden-10.9/src/stresser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:56:01.000000 forbidden-10.9/src/stresser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37259 2024-05-11 09:58:37.000000 forbidden-10.9/src/stresser/stresser.py
--rw-r--r--   0 root         (0) root         (0)    11174 2024-05-11 09:59:35.000000 forbidden-10.9/src/stresser/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/
+-rwxrwx---   0 root         (0) root         (0)     1090 2024-05-12 22:47:27.000000 forbidden-11.0/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      112 2024-05-12 22:47:28.000000 forbidden-11.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17214 2024-05-13 09:53:47.328743 forbidden-11.0/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    16508 2024-05-13 09:48:33.000000 forbidden-11.0/README.md
+-rwxrwx---   0 root         (0) root         (0)      895 2024-05-12 11:34:17.000000 forbidden-11.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:53:47.328743 forbidden-11.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/forbidden/
+-rwxrwx---   0 root         (0) root         (0)        0 2024-05-12 11:33:12.000000 forbidden-11.0/src/forbidden/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    72494 2024-05-13 09:39:28.000000 forbidden-11.0/src/forbidden/forbidden.py
+-rwxrwx---   0 root         (0) root         (0)    11174 2024-05-12 11:33:12.000000 forbidden-11.0/src/forbidden/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/forbidden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17214 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-13 09:53:47.000000 forbidden-11.0/src/forbidden.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:53:47.328743 forbidden-11.0/src/stresser/
+-rwxrwx---   0 root         (0) root         (0)        0 2024-05-12 11:33:12.000000 forbidden-11.0/src/stresser/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    43173 2024-05-13 09:39:20.000000 forbidden-11.0/src/stresser/stresser.py
+-rwxrwx---   0 root         (0) root         (0)    11174 2024-05-12 11:33:12.000000 forbidden-11.0/src/stresser/user_agents.txt
```

### Comparing `forbidden-10.9/PKG-INFO` & `forbidden-11.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: forbidden
-Version: 10.9
-Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
-Author: Ivan Sincek
-Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama>=0.4.6
-Requires-Dist: datetime>=5.2
-Requires-Dist: pycurl>=7.45.2
-Requires-Dist: pyjwt>=2.7.0
-Requires-Dist: regex>=2023.8.8
-Requires-Dist: requests>=2.31.0
-Requires-Dist: tabulate>=0.9.0
-Requires-Dist: termcolor>=1.1.0
-
 # Forbidden
 
 Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
 
 Script uses multithreading and is based on brute forcing, and as such, might have false positive results. Script has colored output.
 
 Results will be sorted by HTTP response status code ascending, HTTP response content length descending, and ID ascending.
@@ -66,34 +45,36 @@
 
 Made for educational purposes. I hope it will help!
 
 ---
 
 **Remarks:**
 
-* Python Requests seems to be up to 3x faster than PycURL, but PycURL is more customizable,
-* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
-* connection and read timeout is set to `60` seconds,
+* all HTTP request headers, values, URL path bypasses, etc. were validated through the official documentation or public infosec write-ups,
+* Python Requests is up to 3x faster than PycURL, but PycURL is more customizable,
+* only `2xx` and `3xx` status codes are included in results and shown in output,
 * `length` attribute in results includes only HTTP response body length,
 * testing `double headers` is locked to `Python Requests` because cURL does not support it,
 * testing `encodings` is locked to `cURL` because Python Requests does not support it,
+* connection and read timeout is set to `60` seconds,
+* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
 * some web proxies might normalize URLs (e.g. when testing `encodings`),
 * some web proxies might modify HTTP requests or drop them entirely,
 * some websites might require a valid or very specific `User-Agent` HTTP request header,
 * cross-site tracing (XST) is `no longer` considered to be a vulnerability.
 
 **High priority plans:**
 
 * use brute forcing to find allowed HTTP methods if HTTP OPTIONS method is not allowed,
 * test HTTP cookies, `User-Agent` HTTP request header, CRLF, and Log4j,
-* add more path bypasses.
+* ~add more path bypasses.~
 
 **Low priority plans:**
 
-* table output to make results more readable and take less screen space,
+* ~~table output to make results more readable,~~
 * add option to test custom HTTP header-value pairs for a list of domains/subdomains.
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
 	* [Install PycURL](#install-pycurl)
 	* [Standard Install](#standard-install)
@@ -155,15 +136,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-10.9-py3-none-any.whl
+python3 -m pip install dist/forbidden-11.0-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -330,29 +311,34 @@
 X-True-Client-IP
 X-True-IP
 X-Wap-Profile
 ```
 
 # URL Paths
 
-Inject at the beginning, end, and both, beginning and end of the URL path. All possible combinations.
+Inject at the beginning, end, and both, beginning and end of the URL path.
+
+You can use one payload set to test all positions simultaneously (sniper) or test using every possible combination of payload set (cluster bomb - default).
 
 ```fundamental
 /
 //
 %09
 %20
 %23
 %2e
+%a0
 *
 .
 ..
 ;
 .;
 ..;
+/;/
+;/../../
 ;foo=bar;
 ```
 
 Inject at the end of the URL path.
 
 ```fundamental
 #
@@ -398,40 +384,42 @@
     {
         "id": "860-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     },
     {
         "id": "861-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1:443"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v10.9 ( github.com/ivan-sincek/forbidden )
+Forbidden v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f POST ] [-v values.txt] [-p /home] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -442,15 +430,15 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 TESTS
     Tests to run
     Use comma-separated values
-    -t, --tests = base | methods | [method|scheme|port]-overrides | headers | paths | encodings | auths | redirects | parsers | all
+    -t, --tests = base | methods | (method|scheme|port)-overrides | headers | paths[-sniper] | encodings | auths | redirects | parsers | all
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
 VALUES
     File with additional HTTP request header values such as internal IPs, etc.
     Spacing will be stripped, empty lines ignored, and duplicates removed
     Tests: headers
@@ -461,14 +449,23 @@
     Default: /robots.txt | /index.html | /sitemap.xml | /README.txt
     -p, --path = /home | etc.
 EVIL
     Evil URL to test URL overrides
     Tests: headers | redirects
     Default: https://github.com
     -e, --evil = https://xyz.interact.sh | https://xyz.burpcollaborator.net | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override the test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override the test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -487,29 +484,33 @@
     -th, --threads = 20 | etc.
 SLEEP
     Sleep in milliseconds before sending an HTTP request
     Intended for a single-thread use
     -s, --sleep = 500 | etc.
 USER AGENT
     User agent to use
-    Default: Forbidden/10.9
+    Default: Forbidden/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Stresser v10.9 ( github.com/ivan-sincek/forbidden )
+Stresser v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -520,14 +521,23 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -541,19 +551,23 @@
     Number of total HTTP requests to send for each test case
     -r, --repeat = 1000 | etc.
 THREADS
     Number of parallel threads to run
     -th, --threads = 20 | etc.
 USER AGENT
     User agent to use
-    Default: Stresser/10.9
+    Default: Stresser/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DIRECTORY
     Output directory
     All valid and unique HTTP responses will be saved in this directory
     -dir, --directory = results | etc.
@@ -563,7 +577,11 @@
 ```
 
 ## Images
 
 <p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example.png" alt="Basic Example"></p>
 
 <p align="center">Figure 1 - Basic Example</p>
+
+<p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example_table.png" alt="Basic Example"></p>
+
+<p align="center">Figure 2 - Basic Example (Table Output)</p>
```

### Comparing `forbidden-10.9/README.md` & `forbidden-11.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: forbidden
+Version: 11.0
+Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: datetime>=5.2
+Requires-Dist: pycurl>=7.45.2
+Requires-Dist: pyjwt>=2.7.0
+Requires-Dist: regex>=2023.8.8
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tabulate>=0.9.0
+Requires-Dist: termcolor>=1.1.0
+
 # Forbidden
 
 Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
 
 Script uses multithreading and is based on brute forcing, and as such, might have false positive results. Script has colored output.
 
 Results will be sorted by HTTP response status code ascending, HTTP response content length descending, and ID ascending.
@@ -45,34 +66,36 @@
 
 Made for educational purposes. I hope it will help!
 
 ---
 
 **Remarks:**
 
-* Python Requests seems to be up to 3x faster than PycURL, but PycURL is more customizable,
-* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
-* connection and read timeout is set to `60` seconds,
+* all HTTP request headers, values, URL path bypasses, etc. were validated through the official documentation or public infosec write-ups,
+* Python Requests is up to 3x faster than PycURL, but PycURL is more customizable,
+* only `2xx` and `3xx` status codes are included in results and shown in output,
 * `length` attribute in results includes only HTTP response body length,
 * testing `double headers` is locked to `Python Requests` because cURL does not support it,
 * testing `encodings` is locked to `cURL` because Python Requests does not support it,
+* connection and read timeout is set to `60` seconds,
+* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
 * some web proxies might normalize URLs (e.g. when testing `encodings`),
 * some web proxies might modify HTTP requests or drop them entirely,
 * some websites might require a valid or very specific `User-Agent` HTTP request header,
 * cross-site tracing (XST) is `no longer` considered to be a vulnerability.
 
 **High priority plans:**
 
 * use brute forcing to find allowed HTTP methods if HTTP OPTIONS method is not allowed,
 * test HTTP cookies, `User-Agent` HTTP request header, CRLF, and Log4j,
-* add more path bypasses.
+* ~add more path bypasses.~
 
 **Low priority plans:**
 
-* table output to make results more readable and take less screen space,
+* ~~table output to make results more readable,~~
 * add option to test custom HTTP header-value pairs for a list of domains/subdomains.
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
 	* [Install PycURL](#install-pycurl)
 	* [Standard Install](#standard-install)
@@ -134,15 +157,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-10.9-py3-none-any.whl
+python3 -m pip install dist/forbidden-11.0-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -309,29 +332,34 @@
 X-True-Client-IP
 X-True-IP
 X-Wap-Profile
 ```
 
 # URL Paths
 
-Inject at the beginning, end, and both, beginning and end of the URL path. All possible combinations.
+Inject at the beginning, end, and both, beginning and end of the URL path.
+
+You can use one payload set to test all positions simultaneously (sniper) or test using every possible combination of payload set (cluster bomb - default).
 
 ```fundamental
 /
 //
 %09
 %20
 %23
 %2e
+%a0
 *
 .
 ..
 ;
 .;
 ..;
+/;/
+;/../../
 ;foo=bar;
 ```
 
 Inject at the end of the URL path.
 
 ```fundamental
 #
@@ -377,40 +405,42 @@
     {
         "id": "860-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     },
     {
         "id": "861-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1:443"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v10.9 ( github.com/ivan-sincek/forbidden )
+Forbidden v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f POST ] [-v values.txt] [-p /home] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -421,15 +451,15 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 TESTS
     Tests to run
     Use comma-separated values
-    -t, --tests = base | methods | [method|scheme|port]-overrides | headers | paths | encodings | auths | redirects | parsers | all
+    -t, --tests = base | methods | (method|scheme|port)-overrides | headers | paths[-sniper] | encodings | auths | redirects | parsers | all
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
 VALUES
     File with additional HTTP request header values such as internal IPs, etc.
     Spacing will be stripped, empty lines ignored, and duplicates removed
     Tests: headers
@@ -440,14 +470,23 @@
     Default: /robots.txt | /index.html | /sitemap.xml | /README.txt
     -p, --path = /home | etc.
 EVIL
     Evil URL to test URL overrides
     Tests: headers | redirects
     Default: https://github.com
     -e, --evil = https://xyz.interact.sh | https://xyz.burpcollaborator.net | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override the test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override the test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -466,29 +505,33 @@
     -th, --threads = 20 | etc.
 SLEEP
     Sleep in milliseconds before sending an HTTP request
     Intended for a single-thread use
     -s, --sleep = 500 | etc.
 USER AGENT
     User agent to use
-    Default: Forbidden/10.9
+    Default: Forbidden/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Stresser v10.9 ( github.com/ivan-sincek/forbidden )
+Stresser v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -499,14 +542,23 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -520,19 +572,23 @@
     Number of total HTTP requests to send for each test case
     -r, --repeat = 1000 | etc.
 THREADS
     Number of parallel threads to run
     -th, --threads = 20 | etc.
 USER AGENT
     User agent to use
-    Default: Stresser/10.9
+    Default: Stresser/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DIRECTORY
     Output directory
     All valid and unique HTTP responses will be saved in this directory
     -dir, --directory = results | etc.
@@ -542,7 +598,11 @@
 ```
 
 ## Images
 
 <p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example.png" alt="Basic Example"></p>
 
 <p align="center">Figure 1 - Basic Example</p>
+
+<p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example_table.png" alt="Basic Example"></p>
+
+<p align="center">Figure 2 - Basic Example (Table Output)</p>
```

### Comparing `forbidden-10.9/pyproject.toml` & `forbidden-11.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "forbidden"
-version = "10.9"
+version = "11.0"
 authors = [{ name = "Ivan Sincek" }]
 description = "Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `forbidden-10.9/src/forbidden/forbidden.py` & `forbidden-11.0/src/forbidden/forbidden.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,56 @@
 		self.__end = datetime.datetime.now()
 		print(("Script has finished in {0}").format(self.__end - self.__start))
 
 stopwatch = Stopwatch()
 
 # ----------------------------------------
 
-default_quotes = "'"
+default_quotes = "'" # NOTE: Default quotes in the JSON 'command' attribute.
 
 def escape_quotes(value):
 	return str(value).replace(default_quotes, ("\\{0}").format(default_quotes))
 
 def set_param(value, param = ""):
 	value = default_quotes + escape_quotes(value) + default_quotes
 	if param:
 		value = ("{0} {1}").format(param, value)
 	return value
 
 # ----------------------------------------
 
+def get_header_key_value(header):
+	key = ""; value = ""
+	if re.search(r"^.+\:.+$", header):
+		key, value = header.split(":", 1)
+	elif re.search(r"^[^\;]+\;$", header):
+		key, value = header.split(";", 1)
+	return key.strip(), value.strip()
+
+def format_header_key_value(key, value):
+	return ("{0}: {1}").format(key, value) if value else ("{0};").format(key)
+
+def get_cookie_key_value(cookie):
+	key = ""; value = ""
+	if re.search(r"^[^\=\;]+\=[^\=\;]+$|^[^\=\;]+\=$", cookie):
+		key, value = cookie.split("=", 1)
+	return key.strip(), value.strip()
+
+def format_cookie_key_value(key, value):
+	return ("{0}={1}").format(key, value)
+
+def array_to_dict(array, separator):
+	tmp = {}
+	for entry in array:
+		key, value = entry.split(separator)
+		tmp[key] = value
+	return tmp
+
+# ----------------------------------------
+
 def strip_url_scheme(url):
 	return url.split("://", 1)[-1]
 
 def strip_url_schemes(urls):
 	tmp = []
 	for url in urls:
 		tmp.append(strip_url_scheme(url))
@@ -284,15 +313,17 @@
 	if confirm.lower() == "yes":
 		try:
 			open(out, "w").write(data)
 			print(("Results have been saved to '{0}'").format(out))
 		except FileNotFoundError:
 			print(("Cannot save results to '{0}'").format(out))
 
-default_user_agent = "Forbidden/10.9"
+# ----------------------------------------
+
+default_user_agent = "Forbidden/11.0"
 
 def get_all_user_agents():
 	tmp = []
 	file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 	if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 		with open(file, "r", encoding = default_encoding) as stream:
 			for line in stream:
@@ -303,35 +334,41 @@
 
 def get_random_user_agent():
 	tmp = get_all_user_agents()
 	return tmp[random.randint(0, len(tmp) - 1)]
 
 # ----------------------------------------
 
+ERROR   =  0
+IGNORED = -1
+
 class Forbidden:
 
-	def __init__(self, url, ignore_qsf, ignore_curl, tests, force, values, paths, evil, ignore, content_lengths, request_timeout, threads, sleep, user_agents, proxy, debug):
+	def __init__(self, url, ignore_qsf, ignore_curl, tests, force, values, paths, evil, headers, cookies, ignore, content_lengths, request_timeout, threads, sleep, user_agents, proxy, show_table, debug):
 		# --------------------------------
 		# NOTE: User-controlled input.
 		self.__url             = self.__parse_url(url, ignore_qsf)
 		self.__tests           = tests
 		self.__force           = force
 		self.__values          = values
 		self.__accessible      = append_paths(self.__url["scheme_domain"], paths)
 		self.__evil            = self.__parse_url(evil, ignore_qsf)
+		self.__headers         = headers
+		self.__cookies         = cookies
 		self.__ignore          = ignore
 		self.__content_lengths = content_lengths
 		self.__threads         = threads
 		self.__sleep           = sleep
 		self.__user_agents     = user_agents
 		self.__user_agents_len = len(self.__user_agents)
 		self.__proxy           = proxy
+		self.__show_table      = show_table
 		self.__debug           = debug
 		# --------------------------------
-		# NOTE: Python cURL configuration.
+		# NOTE: PycURL configuration.
 		self.__curl            = not ignore_curl
 		self.__verify          = False # NOTE: Ignore SSL/TLS verification.
 		self.__allow_redirects = True
 		self.__max_redirects   = 10
 		self.__connect_timeout = request_timeout
 		self.__read_timeout    = request_timeout
 		self.__encoding        = "UTF-8" # NOTE: ISO-8859-1 works better than UTF-8 when accessing files.
@@ -489,23 +526,23 @@
 		if not self.__error and self.__check_tests(["headers", "auths", "redirects", "parsers", "all"]):
 			print_time("Fetching the IP of evil URL...")
 			self.__evil = self.__parse_ip(copy.deepcopy(self.__evil))
 			if not self.__evil["ip_no_port"]:
 				self.__print_error("Cannot fetch the IP of evil URL, script will exit shortly...")
 		# --------------------------------
 
-	# NOTE: Select only the first valid accessible URL.
+	# NOTE: Proceed with the first valid accessible URL.
 	def __validate_accessible_urls(self):
 		if self.__check_tests(["headers", "all"]):
 			print_time(("Validating the accessible URLs using HTTP {0} method...").format(self.__default_method))
 			for url in copy.deepcopy(self.__accessible):
 				self.__accessible = ""
 				record = self.__fetch(url = url, method = self.__default_method)
 				if record["code"] >= 200 and record["code"] < 400:
-					print_green(("First valid accessible URL: {0}").format(record["url"]))
+					print_green(("Valid accessible URL found: {0}").format(record["url"]))
 					self.__accessible = record["url"]
 					if "path" in self.__content_lengths:
 						print_green(("Ignoring the accessible URL response content length: {0}").format(record["length"]))
 						self.__content_lengths.pop(self.__content_lengths.index("path"))
 						self.__add_content_lengths(record["length"])
 					break
 			if not self.__accessible:
@@ -540,88 +577,123 @@
 				print_cyan("Cannot fetch allowed HTTP methods, moving on...")
 				self.__allowed_methods = self.__get_methods()
 				# TO DO: Brute-force allowed HTTP methods.
 			else:
 				print_green(("Allowed HTTP methods: [{0}]").format((", ").join(self.__allowed_methods)))
 		# --------------------------------
 
-	def __fetch(self, url, method = None, headers = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
-		record = self.__record("SYSTEM-0", url, method, headers, body, user_agent, proxy, curl)
+	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
+		record = self.__record("SYSTEM-0", url, method, headers, cookies, body, user_agent, proxy, curl)
 		return self.__send_curl(record, passthrough) if record["curl"] else self.__send_request(record, passthrough)
 
-	def __records(self, identifier, urls, methods = None, headers = None, body = None, user_agent = None, proxy = None, curl = None):
+	def __records(self, identifier, urls, methods = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None):
 		if not isinstance(urls, list):
 			urls = [urls]
 		if not isinstance(methods, list):
 			methods = [methods]
 		if headers:
 			for url in urls:
 				for method in methods:
 					for header in headers:
 						if not isinstance(header, list):
-							# NOTE: Python cURL accepts only string arrays as HTTP request headers.
+							# NOTE: PycURL accepts only string arrays as HTTP request headers.
 							header = [header]
-						self.__collection.append(self.__record(identifier, url, method, header, body, user_agent, proxy, curl))
+						self.__collection.append(self.__record(identifier, url, method, header, cookies, body, user_agent, proxy, curl))
 		else:
 			for url in urls:
 				for method in methods:
-					self.__collection.append(self.__record(identifier, url, method, [], body, user_agent, proxy, curl))
+					self.__collection.append(self.__record(identifier, url, method, [], cookies, body, user_agent, proxy, curl))
 
-	def __record(self, identifier, url, method, headers, body, user_agent, proxy, curl):
+	def __record(self, identifier, url, method, headers, cookies, body, user_agent, proxy, curl):
 		self.__identifier += 1
 		identifier = ("{0}-{1}").format(self.__identifier, identifier)
 		if not method:
 			method = self.__force if self.__force else self.__default_method
+		headers = self.__inspect_headers(headers)
+		cookies = self.__inspect_cookies(cookies)
 		if not user_agent:
 			user_agent = self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
 		if not proxy:
 			proxy = self.__proxy
-		if not curl:
+		if not curl and curl is not False:
 			curl = self.__curl
 		record = {
 			"raw"             : self.__identifier,
 			"id"              : identifier,
 			"url"             : url,
 			"method"          : method,
 			"headers"         : headers,
+			"cookies"         : cookies,
 			"body"            : body,
 			"user_agent"      : user_agent,
 			"proxy"           : proxy,
 			"command"         : None,
-			"code"            : 0,
+			"code"            : ERROR,
 			"length"          : 0,
 			"response"        : None,
 			"response_headers": None,
 			"curl"            : curl
 		}
 		record["command"] = self.__build_command(record)
 		return record
 
+	def __inspect_headers(self, headers = None):
+		tmp = []
+		exists = set()
+		if headers:
+			for header in headers:
+				key, value = get_header_key_value(header)
+				if key:
+					exists.add(key.lower())
+					tmp.append(format_header_key_value(key, value))
+		for header in self.__headers:
+			key, value = get_header_key_value(header)
+			if key and key.lower() not in exists: # NOTE: Extra HTTP request headers cannot override test HTTP request headers.
+				tmp.append(format_header_key_value(key, value))
+		return tmp
+
+	def __inspect_cookies(self, cookies = None):
+		tmp = []
+		exists = set()
+		if cookies:
+			for cookie in cookies:
+				key, value = get_cookie_key_value(cookie)
+				if key:
+					exists.add(key.lower())
+					tmp.append(format_cookie_key_value(key, value))
+		for cookie in self.__cookies:
+			key, value = get_cookie_key_value(cookie)
+			if key and key.lower() not in exists: # NOTE: Extra HTTP cookies cannot override test HTTP cookies.
+				tmp.append(format_cookie_key_value(key, value))
+		return tmp
+
 	def __build_command(self, record):
 		tmp = ["curl", ("--connect-timeout {0}").format(self.__connect_timeout), ("-m {0}").format(self.__read_timeout), "-iskL", ("--max-redirs {0}").format(self.__max_redirects), "--path-as-is"]
 		if record["body"]:
 			tmp.append(set_param(record["body"], "-d"))
 		if record["proxy"]:
 			tmp.append(set_param(record["proxy"], "-x"))
 		if record["user_agent"]:
 			tmp.append(set_param(record["user_agent"], "-A"))
 		if record["headers"]:
 			for header in record["headers"]:
 				tmp.append(set_param(header, "-H"))
+		if record["cookies"]:
+			tmp.append(set_param(("; ").join(record["cookies"]), "-b"))
 		tmp.append(set_param(record["method"], "-X"))
 		tmp.append(set_param(record["url"]))
 		tmp = (" ").join(tmp)
 		return tmp
 
 	# NOTE: Remove duplicate test records.
 	def __filter_collection(self):
 		tmp = []
 		exists = set()
 		for record in self.__collection:
-			command = re.sub((" -A \\{0}.+?\\{0}").format(default_quotes), "", record["command"])
+			command = re.sub((" -A \\{0}.+?\\{0} ").format(default_quotes), " ", record["command"])
 			if command not in exists and not exists.add(command):
 				tmp.append(record)
 		self.__collection = tmp
 
 	def __run_tests(self):
 		results = []
 		print_time(("Running tests with {0} engine...").format("PycURL" if self.__curl else "Python Requests"))
@@ -680,28 +752,30 @@
 			curl.setopt(pycurl.CUSTOMREQUEST, record["method"])
 			if record["method"] in ["HEAD"]:
 				curl.setopt(pycurl.NOBODY, True)
 			if record["user_agent"]:
 				curl.setopt(pycurl.USERAGENT, self.__encode(record["user_agent"]))
 			if record["headers"]:
 				curl.setopt(pycurl.HTTPHEADER, self.__encode(record["headers"])) # Will override 'User-Agent' HTTP request header.
+			if record["cookies"]:
+				curl.setopt(pycurl.COOKIE, ("; ").join(record["cookies"]))
 			if record["body"]:
 				curl.setopt(pycurl.POSTFIELDS, record["body"])
 			if record["proxy"]:
 				curl.setopt(pycurl.PROXY, record["proxy"])
 			# ----------------------------
 			curl.perform()
 			# ----------------------------
 			record["code"] = int(curl.getinfo(pycurl.RESPONSE_CODE))
 			record["length"] = int(curl.getinfo(pycurl.SIZE_DOWNLOAD))
 			if passthrough:
 				record["response_headers"] = self.__decode(headers.getvalue())
 				# record["response"] = self.__decode(response.getvalue())
 			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(response.getvalue()), self.__regex_flags)):
-				record["code"] = -1
+				record["code"] = IGNORED
 			# ----------------------------
 		except pycurl.error as ex:
 			# ----------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -735,14 +809,16 @@
 				record["method"],
 				record["url"]
 			)
 			if record["user_agent"]:
 				request.headers["User-Agent"] = self.__encode(record["user_agent"])
 			if record["headers"]:
 				self.__set_double_headers(request, record["headers"]) # Will override 'User-Agent' HTTP request header.
+			if record["cookies"]:
+				session.cookies.update(array_to_dict(record["cookies"], "="))
 			if record["body"]:
 				request.data = record["body"]
 			if record["proxy"]:
 				session.proxies["https"] = session.proxies["http"] = record["proxy"]
 			# ----------------------------
 			prepared = session.prepare_request(request)
 			prepared.url = record["url"]
@@ -756,15 +832,15 @@
 			# ----------------------------
 			record["code"] = int(response.status_code)
 			record["length"] = len(response.content)
 			if passthrough:
 				record["response_headers"] = dict(response.headers)
 				# record["response"] = self.__decode(response.content)
 			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(response.content), self.__regex_flags)):
-				record["code"] = -1
+				record["code"] = IGNORED
 			# ----------------------------
 		except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException) as ex:
 			# ----------------------------
 			self.__print_debug(ex, ("{0}: {1}").format(record["id"], record["command"]))
 			# ----------------------------
 		finally:
 			# ----------------------------
@@ -775,51 +851,22 @@
 				session.close()
 			# ----------------------------
 		return record
 
 	def __set_double_headers(self, request, headers):
 		exists = set()
 		for header in headers:
-			array = header.split(":", 1)
-			key = array[0].rstrip(";")
-			value = self.__encode(array[1].strip() if len(array) > 1 else "")
-			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = value
+			key, value = get_header_key_value(header)
+			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value) # NOTE: Allows double headers.
 
 	def __validate_results(self):
-		tmp = []
-		# --------------------------------
 		print_time("Validating results...")
-		table = Table(self.__collection) # unfiltered
-		# --------------------------------
-		self.__collection = pop(sorted([record for record in self.__collection if record["code"] > 0], key = lambda x: (x["code"], -x["length"], x["raw"])), ["raw", "proxy", "response_headers", "response", "curl"])
-		# --------------------------------
-		for record in self.__collection:
-			if record["code"] >= 500:
-				continue
-				print_cyan(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 400:
-				continue
-				print_red(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 300:
-				# continue
-				print_yellow(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 200:
-				# continue
-				print_green(jdump(record))
-				tmp.append(record)
-			elif record["code"] > 0:
-				continue
-				print_white(jdump(record))
-				tmp.append(record)
-		# --------------------------------
-		self.__collection = tmp
-		table.show()
+		output = Output(self.__collection)
+		self.__collection = output.results_table() if self.__show_table else output.results_json()
+		output.stats_table()
 
 	def __check_tests(self, array):
 		return any(test in array for test in self.__tests)
 
 	def __prepare_collection(self):
 		print_time("Preparing test records...")
 		# --------------------------------
@@ -957,15 +1004,21 @@
 				curl       = False
 			)
 		# --------------------------------
 		if self.__check_tests(["paths", "all"]):
 			# NOTE: Test URL path bypasses.
 			self.__records(
 				identifier = "PATHS-1",
-				urls       = self.__get_path_bypass_urls()
+				urls       = self.__get_path_bypass_urls(sniper = False)
+			)
+		elif self.__check_tests(["paths-sniper"]):
+			# NOTE: Test URL path bypasses.
+			self.__records(
+				identifier = "PATHS-1",
+				urls       = self.__get_path_bypass_urls(sniper = True)
 			)
 		# --------------------------------
 		if self.__check_tests(["encodings", "all"]):
 			# NOTE: Test domain name and URL path transformations and encodings.
 			self.__records(
 				identifier = "ENCODINGS-1",
 				urls       = self.__get_encoded_urls(),
@@ -1021,15 +1074,15 @@
 			"ARBITRARY",
 			"BASELINE-CONTROL",
 			"BIND",
 			"CHECKIN",
 			"CHECKOUT",
 			"CONNECT",
 			"COPY",
-			# "DELETE", # NOTE: This HTTP method is dangerous!
+			# "DELETE", # NOTE: Enabling this HTTP method is dangerous!
 			"GET",
 			"HEAD",
 			"INDEX",
 			"LABEL",
 			"LINK",
 			"LOCK",
 			"MERGE",
@@ -1237,14 +1290,17 @@
 		]
 		for header in headers:
 			for value in values:
 				tmp.append(("{0}: [{1}]").format(header, value))
 		# --------------------------------
 		return unique(tmp)
 
+	def __get_all_headers(self, values):
+		return unique(self.__get_url_headers(values) + self.__get_ip_headers(values))
+
 	def __get_special_headers(self):
 		tmp = []
 		# --------------------------------
 		headers = [
 			"From"
 		]
 		for header in headers:
@@ -1263,28 +1319,25 @@
 		]
 		for header in headers:
 			for value in ["XMLHttpRequest"]:
 				tmp.append(("{0}: {0}").format(header, value))
 		# --------------------------------
 		return unique(tmp)
 
-	def __get_all_headers(self, values):
-		return unique(self.__get_url_headers(values) + self.__get_ip_headers(values))
-
-	def __get_localhost_urls(self):
+	def __get_localhost_values(self):
 		return get_all_domains(self.__url["scheme"], ["localhost", "127.0.0.1", unicode_encode("127.0.0.1"), "127.000.000.001"], self.__url["port"])
 
-	def __get_random_urls(self):
+	def __get_random_values(self):
 		return get_all_domains(self.__url["scheme"], ["192.168.1.1", "172.16.1.1", "173.245.48.1", "10.1.1.1", "169.254.169.254"], self.__url["port"])
 
 	def __get_all_values(self, scheme = True, ip = False):
 		tmp = []
 		domain_extended = "ip_extended" if ip else "domain_extended"
 		localhost = "127.0.0.1" if ip else "localhost"
-		temp = strip_url_schemes(self.__get_localhost_urls() + self.__get_random_urls() + self.__url[domain_extended])
+		temp = strip_url_schemes(self.__get_localhost_values() + self.__get_random_values() + self.__url[domain_extended])
 		if scheme:
 			tmp.extend([("{0}://{1}").format(self.__url["scheme"], entry + self.__url["path_full"]) for entry in temp])
 		else:
 			tmp += temp
 		temp = strip_url_schemes(self.__evil[domain_extended])
 		if scheme:
 			tmp.extend([("{0}://{1}").format(self.__evil["scheme"], entry + self.__url["path_full"]) for entry in temp])
@@ -1306,27 +1359,29 @@
 				if exist not in exists and not exists.add(exist):
 					tmp.append([
 						("Host: {0}").format(initial),
 						("Host: {0}").format(override)
 					])
 		return tmp
 
-	def __get_path_bypass_urls(self):
+	def __get_path_bypass_urls(self, sniper = False):
 		path_bypasses = []
 		# --------------------------------
 		path = self.__url["path"].strip(path_const)
 		# --------------------------------
 		# NOTE: Inject at the beginning, end, and both, beginning and end of the URL path.
-		# NOTE: All possible combinations.
+		# NOTE: Use one payload set to test all positions simultaneously (sniper) or test using every possible combination of payload set (cluster bomb - default).
 		injections = []
-		for i in ["", "%09", "%20", "%23", "%2e", "*", ".", "..", ";", ".;", "..;", ";foo=bar;"]:
+		for i in ["", "%09", "%20", "%23", "%2e", "%a0", "*", ".", "..", ";", ".;", "..;", "/;/", ";/../../", ";foo=bar;"]:
 			injections.extend([path_const + i + path_const, i + path_const, path_const + i, i])
-		for i in injections:
-			path_bypasses.extend([path + i, i + path])
-			if path:
+		if sniper:
+			for i in injections:
+				path_bypasses.extend([path + i, i + path, i + path + i])
+		else:
+			for i in injections:
 				for j in injections:
 					path_bypasses.extend([i + path + j])
 		# --------------------------------
 		# NOTE: Inject at the end of the URL path.
 		injections = []
 		for i in ["#", "*", ".", "?", "~"]:
 			injections.extend([i, i + i, ("{0}random").format(i)])
@@ -1425,54 +1480,106 @@
 					tmp.append(initial + injection + override)
 		if scheme:
 			tmp = [("{0}://{1}").format(self.__evil["scheme"], entry + self.__url["path_full"]) for entry in tmp]
 		return unique(tmp)
 
 # ----------------------------------------
 
-class Table:
+class Output:
 
 	def __init__(self, collection):
-		self.__table = self.__init_table(collection)
+		self.__collection = pop(sorted([record for record in collection if record["code"] >= 100 and record["code"] < 600], key = lambda x: (x["code"], -x["length"], x["raw"])), ["raw", "proxy", "response_headers", "response", "curl"]) # filtered
+		self.__stats      = self.__count(collection) # unfiltered
 
-	def __init_table(self, collection):
-		table = {}
-		for record in collection:
-			if record["code"] not in table:
-				table[record["code"]] = 0
-			table[record["code"]] += 1
-		return dict(sorted(table.items()))
-
-	def __row(self, code, count, color):
-		return [
-			("{0}{1}{2}").format(color, code, colorama.Style.RESET_ALL),
-			("{0}{1}{2}").format(color, count, colorama.Style.RESET_ALL)
-		]
+	def __color(self, value, color):
+		return ("{0}{1}{2}").format(color, value, colorama.Style.RESET_ALL)
 
-	def show(self):
+	def __results_row(self, record, color):
+		return [self.__color(record[key], color) for key in ["id", "code", "length", "command"]]
+
+	def results_table(self):
+		tmp = []; table = []
+		for record in self.__collection:
+			if record["code"] < 100 or record["code"] >= 600:
+				continue
+			elif record["code"] >= 500:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.CYAN))
+			elif record["code"] >= 400:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.RED))
+			elif record["code"] >= 300:
+				# continue
+				table.append(self.__results_row(record, colorama.Fore.YELLOW))
+			elif record["code"] >= 200:
+				# continue
+				table.append(self.__results_row(record, colorama.Fore.GREEN))
+			elif record["code"] >= 100:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.WHITE))
+			tmp.append(record)
+		if table:
+			print(tabulate.tabulate(table, tablefmt = "plain", colalign = ("right", "right", "right", "left")))
+		return tmp
+
+	def results_json(self): # NOTE: To see more or less results, comment in or out 'continue' line.
 		tmp = []
-		for code, count in self.__table.items():
-			if code >= 500:
-				tmp.append(self.__row(code, count, colorama.Fore.CYAN))
+		for record in self.__collection:
+			if record["code"] < 100 or record["code"] >= 600:
+				continue
+			elif record["code"] >= 500:
+				continue
+				print_cyan(jdump(record))
+			elif record["code"] >= 400:
+				continue
+				print_red(jdump(record))
+			elif record["code"] >= 300:
+				# continue
+				print_yellow(jdump(record))
+			elif record["code"] >= 200:
+				# continue
+				print_green(jdump(record))
+			elif record["code"] >= 100:
+				continue
+				print_white(jdump(record))
+			tmp.append(record)
+		return tmp
+
+	def __count(self, collection):
+		tmp = {}
+		for record in collection:
+			if record["code"] not in tmp:
+				tmp[record["code"]] = 0
+			tmp[record["code"]] += 1
+		return dict(sorted(tmp.items()))
+
+	def __stats_row(self, code, count, color):
+		return [self.__color(entry, color) for entry in [code, count]]
+
+	def stats_table(self):
+		table = []; table_special = []
+		for code, count in self.__stats.items():
+			if code == ERROR:
+				table_special.append(self.__stats_row("Errors", count, colorama.Fore.WHITE))
+			elif code == IGNORED:
+				table_special.append(self.__stats_row("Ignored", count, colorama.Fore.WHITE))
+			elif code < 100 or code >= 600:
+				continue
+			elif code >= 500:
+				table.append(self.__stats_row(code, count, colorama.Fore.CYAN))
 			elif code >= 400:
-				tmp.append(self.__row(code, count, colorama.Fore.RED))
+				table.append(self.__stats_row(code, count, colorama.Fore.RED))
 			elif code >= 300:
-				tmp.append(self.__row(code, count, colorama.Fore.YELLOW))
+				table.append(self.__stats_row(code, count, colorama.Fore.YELLOW))
 			elif code >= 200:
-				tmp.append(self.__row(code, count, colorama.Fore.GREEN))
-			elif code > 0:
-				tmp.append(self.__row(code, count, colorama.Fore.WHITE))
-			elif code == 0:
-				tmp.append(self.__row("Errors", count, colorama.Fore.WHITE))
-			elif code == -1:
-				tmp.append(self.__row("Ignored", count, colorama.Fore.WHITE))
-			elif code == -2:
-				tmp.append(self.__row("Duplicates", count, colorama.Fore.WHITE))
-		if tmp:
-			print(tabulate.tabulate(tmp, ["Code", "Count"], tablefmt = "outline", colalign = ("left", "left")))
+				table.append(self.__stats_row(code, count, colorama.Fore.GREEN))
+			elif code >= 100:
+				table.append(self.__stats_row(code, count, colorama.Fore.WHITE))
+		if table or table_special:
+			print(tabulate.tabulate(table + table_special, ["Status Code", "Count"], tablefmt = "outline", colalign = ("left", "right")))
 
 # ----------------------------------------
 
 class Progress:
 
 	def __init__(self, total, print_lock):
 		self.__total      = total
@@ -1483,17 +1590,17 @@
 		with self.__print_lock:
 			print(("Progress: {0}/{1} | {2:.2f}%").format(self.__count, self.__total, (self.__count / self.__total) * 100), end = "\n" if self.__count == self.__total else "\r")
 			self.__count += 1
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
-	
+
 	def print_help(self):
-		print("Forbidden v10.9 ( github.com/ivan-sincek/forbidden )")
+		print("Forbidden v11.0 ( github.com/ivan-sincek/forbidden )")
 		print("")
 		print("Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path ] [-o out         ]")
 		print("Example: forbidden -u https://example.com/admin -t all   [-f POST ] [-v values.txt] [-p /home] [-o results.json]")
 		print("")
 		print("DESCRIPTION")
 		print("    Bypass 4xx HTTP response status codes and more")
 		print("URL")
@@ -1504,15 +1611,15 @@
 		print("    -iqsf, --ignore-query-string-and-fragment")
 		print("IGNORE CURL")
 		print("    Use Python Requests instead of PycURL where applicable")
 		print("    -ic, --ignore-curl")
 		print("TESTS")
 		print("    Tests to run")
 		print("    Use comma-separated values")
-		print("    -t, --tests = base | methods | [method|scheme|port]-overrides | headers | paths | encodings | auths | redirects | parsers | all")
+		print("    -t, --tests = base | methods | (method|scheme|port)-overrides | headers | paths[-sniper] | encodings | auths | redirects | parsers | all")
 		print("FORCE")
 		print("    Force an HTTP method for all non-specific test cases")
 		print("    -f, --force = GET | POST | CUSTOM | etc.")
 		print("VALUES")
 		print("    File with additional HTTP request header values such as internal IPs, etc.")
 		print("    Spacing will be stripped, empty lines ignored, and duplicates removed")
 		print("    Tests: headers")
@@ -1523,14 +1630,23 @@
 		print("    Default: /robots.txt | /index.html | /sitemap.xml | /README.txt")
 		print("    -p, --path = /home | etc.")
 		print("EVIL")
 		print("    Evil URL to test URL overrides")
 		print("    Tests: headers | redirects")
 		print("    Default: https://github.com")
 		print("    -e, --evil = https://xyz.interact.sh | https://xyz.burpcollaborator.net | etc.")
+		print("HEADER")
+		print("    Specify any number of extra HTTP request headers")
+		print("    Extra HTTP request headers will not override the test HTTP request headers")
+		print("    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.")
+		print("    -H, --header = \"Authorization: Bearer ey...\" | Content-Type; | etc.")
+		print("COOKIE")
+		print("    Specify any number of extra HTTP cookies")
+		print("    Extra HTTP cookies will not override the test HTTTP cookies")
+		print("    -b, --cookie = PHPSESSIONID=3301 | etc.")
 		print("IGNORE")
 		print("    Filter out 200 OK false positive results with RegEx")
 		print("    Spacing will be stripped")
 		print("    -i, --ignore = Inaccessible | \"Access Denied\" | etc.")
 		print("CONTENT LENGTHS")
 		print("    Filter out 200 OK false positive results by HTTP response content lengths")
 		print("    Specify 'base' to ignore content length of the base HTTP response")
@@ -1554,24 +1670,28 @@
 		print("USER AGENT")
 		print("    User agent to use")
 		print(("    Default: {0}").format(default_user_agent))
 		print("    -a, --user-agent = curl/3.30.1 | random[-all] | etc.")
 		print("PROXY")
 		print("    Web proxy to use")
 		print("    -x, --proxy = http://127.0.0.1:8080 | etc.")
+		print("SHOW TABLE")
+		print("    Display the results in a table instead of JSON")
+		print("    Intended for a wide screen use")
+		print("    -st, --show-table")
 		print("OUT")
 		print("    Output file")
 		print("    -o, --out = results.json | etc.")
 		print("DEBUG")
 		print("    Debug output")
 		print("    -dbg, --debug")
 
 	def error(self, message):
 		if len(sys.argv) > 1:
-			print("Missing a mandatory option (-u, -t) and/or optional (-iqsf, -ic, -f, -v, -p, -e, -i, -l, -rt, -th, -s, -a, -x, -o, -dbg)")
+			print("Missing a mandatory option (-u, -t) and/or optional (-iqsf, -ic, -f, -v, -p, -e, -H, -b, -i, -l, -rt, -th, -s, -a, -x, -o, -dbg)")
 			print("Use -h or --help for more info")
 		else:
 			self.print_help()
 		exit()
 
 class Validate:
 
@@ -1582,31 +1702,36 @@
 		self.__parser.add_argument("-iqsf", "--ignore-query-string-and-fragment", required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-ic"  , "--ignore-curl"                     , required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-t"   , "--tests"                           , required = True , type   = str.lower   , default = ""   )
 		self.__parser.add_argument("-f"   , "--force"                           , required = False, type   = str.upper   , default = ""   )
 		self.__parser.add_argument("-v"   , "--values"                          , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-p"   , "--path"                            , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-e"   , "--evil"                            , required = False, type   = str         , default = ""   )
+		self.__parser.add_argument("-H"   , "--header"                          , required = False, action = "append"    , nargs   = "+"  )
+		self.__parser.add_argument("-b"   , "--cookie"                          , required = False, action = "append"    , nargs   = "+"  )
 		self.__parser.add_argument("-i"   , "--ignore"                          , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-l"   , "--content-lengths"                 , required = False, type   = str.lower   , default = ""   )
 		self.__parser.add_argument("-rt"  , "--request-timeout"                 , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-th"  , "--threads"                         , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-s"   , "--sleep"                           , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-a"   , "--user-agent"                      , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-x"   , "--proxy"                           , required = False, type   = str         , default = ""   )
+		self.__parser.add_argument("-st"  , "--show-table"                      , required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-o"   , "--out"                             , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-dbg" , "--debug"                           , required = False, action = "store_true", default = False)
 
 	def run(self):
 		self.__args                 = self.__parser.parse_args()
 		self.__args.url             = self.__parse_url(self.__args.url, "url")                  # required
 		self.__args.tests           = self.__parse_tests(self.__args.tests)                     # required
 		self.__args.values          = self.__parse_values(self.__args.values)                   if self.__args.values          else []
 		self.__args.path            = self.__parse_path(self.__args.path)                       if self.__args.path            else ["/robots.txt", "/index.html", "/sitemap.xml", "/README.txt"]
 		self.__args.evil            = self.__parse_url(self.__args.evil, "evil")                if self.__args.evil            else "https://github.com"
+		self.__args.header          = self.__parse_header(self.__args.header)                   if self.__args.header          else []
+		self.__args.cookie          = self.__parse_cookie(self.__args.cookie)                   if self.__args.cookie          else []
 		self.__args.ignore          = self.__parse_ignore(self.__args.ignore)                   if self.__args.ignore          else ""
 		self.__args.content_lengths = self.__parse_content_lengths(self.__args.content_lengths) if self.__args.content_lengths else []
 		self.__args.request_timeout = self.__parse_request_timeout(self.__args.request_timeout) if self.__args.request_timeout else 60
 		self.__args.threads         = self.__parse_threads(self.__args.threads)                 if self.__args.threads         else 5
 		self.__args.sleep           = self.__parse_sleep(self.__args.sleep)                     if self.__args.sleep           else 0
 		self.__args.user_agent      = self.__parse_user_agent(self.__args.user_agent)           if self.__args.user_agent      else [default_user_agent]
 		self.__args.proxy           = self.__parse_url(self.__args.proxy, "proxy")              if self.__args.proxy           else ""
@@ -1666,16 +1791,16 @@
 
 	def __parse_tests(self, value):
 		tmp = []
 		for entry in value.lower().split(","):
 			entry = entry.strip()
 			if not entry:
 				continue
-			elif entry not in ["base", "methods", "method-overrides", "scheme-overrides", "port-overrides", "headers", "paths", "encodings", "auths", "redirects", "parsers", "all"]:
-				self.__error("Supported tests are 'base', 'methods', '[method|scheme|port]-overrides', 'headers', 'paths', 'encodings', 'auths', 'redirects', 'parsers', or 'all'")
+			elif entry not in ["base", "methods", "method-overrides", "scheme-overrides", "port-overrides", "headers", "paths", "paths-sniper", "encodings", "auths", "redirects", "parsers", "all"]:
+				self.__error("Supported tests are 'base', 'methods', '(method|scheme|port)-overrides', 'headers', 'paths[-sniper]', 'encodings', 'auths', 'redirects', 'parsers', or 'all'")
 				break
 			elif entry == "all":
 				tmp = [entry]
 				break
 			else:
 				tmp.append(entry)
 		return unique(tmp)
@@ -1693,19 +1818,41 @@
 			if not tmp:
 				self.__error("No additional values were found")
 		return tmp
 
 	def __parse_path(self, value):
 		return [prepend_slash(replace_multiple_slashes(value))]
 
+	def __parse_header(self, headers):
+		tmp = []
+		for header in headers:
+			header = header[0]
+			key, value = get_header_key_value(header)
+			if not key:
+				self.__error(("Invalid header: {0}").format(header))
+				continue
+			tmp.append(format_header_key_value(key, value))
+		return tmp
+
+	def __parse_cookie(self, cookies):
+		tmp = []
+		for cookie in cookies:
+			cookie = cookie[0]
+			key, value = get_cookie_key_value(cookie)
+			if not key:
+				self.__error(("Invalid cookie: {0}").format(cookie))
+				continue
+			tmp.append(format_cookie_key_value(key, value))
+		return tmp
+
 	def __parse_ignore(self, value):
 		try:
 			re.compile(value)
 		except re.error:
-			self.__error("Invalid RegEx")
+			self.__error(("Invalid RegEx: {0}").format(value))
 		return value
 
 	def __parse_content_lengths(self, value):
 		tmp = []
 		for entry in value.lower().split(","):
 			entry = entry.strip()
 			if not entry:
@@ -1758,15 +1905,15 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("###########################################################################")
 		print("#                                                                         #")
-		print("#                             Forbidden v10.9                             #")
+		print("#                             Forbidden v11.0                             #")
 		print("#                                  by Ivan Sincek                         #")
 		print("#                                                                         #")
 		print("# Bypass 4xx HTTP response status codes and more.                         #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                  #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
 		print("#                                                                         #")
 		print("###########################################################################")
@@ -1776,21 +1923,24 @@
 			validate.get_arg("ignore_query_string_and_fragment"),
 			validate.get_arg("ignore_curl"),
 			validate.get_arg("tests"),
 			validate.get_arg("force"),
 			validate.get_arg("values"),
 			validate.get_arg("path"),
 			validate.get_arg("evil"),
+			validate.get_arg("header"),
+			validate.get_arg("cookie"),
 			validate.get_arg("ignore"),
 			validate.get_arg("content_lengths"),
 			validate.get_arg("request_timeout"),
 			validate.get_arg("threads"),
 			validate.get_arg("sleep"),
 			validate.get_arg("user_agent"),
 			validate.get_arg("proxy"),
+			validate.get_arg("show_table"),
 			validate.get_arg("debug")
 		)
 		forbidden.run()
 		results = forbidden.get_results()
 		if results and out:
 			write_file(jdump(results), out)
 		stopwatch.stop()
```

### Comparing `forbidden-10.9/src/forbidden/user_agents.txt` & `forbidden-11.0/src/forbidden/user_agents.txt`

 * *Files identical despite different names*

### Comparing `forbidden-10.9/src/forbidden.egg-info/PKG-INFO` & `forbidden-11.0/src/forbidden.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 10.9
+Version: 11.0
 Summary: Bypass 4xx HTTP response status codes and more. Based on PycURL and Python Requests.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -66,34 +66,36 @@
 
 Made for educational purposes. I hope it will help!
 
 ---
 
 **Remarks:**
 
-* Python Requests seems to be up to 3x faster than PycURL, but PycURL is more customizable,
-* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
-* connection and read timeout is set to `60` seconds,
+* all HTTP request headers, values, URL path bypasses, etc. were validated through the official documentation or public infosec write-ups,
+* Python Requests is up to 3x faster than PycURL, but PycURL is more customizable,
+* only `2xx` and `3xx` status codes are included in results and shown in output,
 * `length` attribute in results includes only HTTP response body length,
 * testing `double headers` is locked to `Python Requests` because cURL does not support it,
 * testing `encodings` is locked to `cURL` because Python Requests does not support it,
+* connection and read timeout is set to `60` seconds,
+* beware of `rate limiting` and other similar anti-bot protections, take some time before you run the script again on the same domain,
 * some web proxies might normalize URLs (e.g. when testing `encodings`),
 * some web proxies might modify HTTP requests or drop them entirely,
 * some websites might require a valid or very specific `User-Agent` HTTP request header,
 * cross-site tracing (XST) is `no longer` considered to be a vulnerability.
 
 **High priority plans:**
 
 * use brute forcing to find allowed HTTP methods if HTTP OPTIONS method is not allowed,
 * test HTTP cookies, `User-Agent` HTTP request header, CRLF, and Log4j,
-* add more path bypasses.
+* ~add more path bypasses.~
 
 **Low priority plans:**
 
-* table output to make results more readable and take less screen space,
+* ~~table output to make results more readable,~~
 * add option to test custom HTTP header-value pairs for a list of domains/subdomains.
 
 ## Table of Contents
 
 * [How to Install](#how-to-install)
 	* [Install PycURL](#install-pycurl)
 	* [Standard Install](#standard-install)
@@ -155,15 +157,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-10.9-py3-none-any.whl
+python3 -m pip install dist/forbidden-11.0-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -330,29 +332,34 @@
 X-True-Client-IP
 X-True-IP
 X-Wap-Profile
 ```
 
 # URL Paths
 
-Inject at the beginning, end, and both, beginning and end of the URL path. All possible combinations.
+Inject at the beginning, end, and both, beginning and end of the URL path.
+
+You can use one payload set to test all positions simultaneously (sniper) or test using every possible combination of payload set (cluster bomb - default).
 
 ```fundamental
 /
 //
 %09
 %20
 %23
 %2e
+%a0
 *
 .
 ..
 ;
 .;
 ..;
+/;/
+;/../../
 ;foo=bar;
 ```
 
 Inject at the end of the URL path.
 
 ```fundamental
 #
@@ -398,40 +405,42 @@
     {
         "id": "860-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     },
     {
         "id": "861-HEADERS-3",
         "url": "https://example.com:443/admin",
         "method": "GET",
         "headers": [
             "Host: 127.0.0.1:443"
         ],
+        "cookies": [],
         "body": null,
-        "user_agent": "Forbidden/10.9",
-        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/10.9' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
+        "user_agent": "Forbidden/11.0",
+        "command": "curl --connect-timeout 60 -m 60 -iskL --max-redirs 10 --path-as-is -A 'Forbidden/11.0' -H 'Host: 127.0.0.1:443' -X 'GET' 'https://example.com:443/admin'",
         "code": 200,
         "length": 255408
     }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v10.9 ( github.com/ivan-sincek/forbidden )
+Forbidden v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f POST ] [-v values.txt] [-p /home] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -442,15 +451,15 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 TESTS
     Tests to run
     Use comma-separated values
-    -t, --tests = base | methods | [method|scheme|port]-overrides | headers | paths | encodings | auths | redirects | parsers | all
+    -t, --tests = base | methods | (method|scheme|port)-overrides | headers | paths[-sniper] | encodings | auths | redirects | parsers | all
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
 VALUES
     File with additional HTTP request header values such as internal IPs, etc.
     Spacing will be stripped, empty lines ignored, and duplicates removed
     Tests: headers
@@ -461,14 +470,23 @@
     Default: /robots.txt | /index.html | /sitemap.xml | /README.txt
     -p, --path = /home | etc.
 EVIL
     Evil URL to test URL overrides
     Tests: headers | redirects
     Default: https://github.com
     -e, --evil = https://xyz.interact.sh | https://xyz.burpcollaborator.net | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override the test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override the test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -487,29 +505,33 @@
     -th, --threads = 20 | etc.
 SLEEP
     Sleep in milliseconds before sending an HTTP request
     Intended for a single-thread use
     -s, --sleep = 500 | etc.
 USER AGENT
     User agent to use
-    Default: Forbidden/10.9
+    Default: Forbidden/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DEBUG
     Debug output
     -dbg, --debug
 ```
 
 ```fundamental
-Stresser v10.9 ( github.com/ivan-sincek/forbidden )
+Stresser v11.0 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -520,14 +542,23 @@
     -iqsf, --ignore-query-string-and-fragment
 IGNORE CURL
     Use Python Requests instead of PycURL where applicable
     -ic, --ignore-curl
 FORCE
     Force an HTTP method for all non-specific test cases
     -f, --force = GET | POST | CUSTOM | etc.
+HEADER
+    Specify any number of extra HTTP request headers
+    Extra HTTP request headers will not override test HTTP request headers
+    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.
+    -H, --header = "Authorization: Bearer ey..." | Content-Type; | etc.
+COOKIE
+    Specify any number of extra HTTP cookies
+    Extra HTTP cookies will not override test HTTTP cookies
+    -b, --cookie = PHPSESSIONID=3301 | etc.
 IGNORE
     Filter out 200 OK false positive results with RegEx
     Spacing will be stripped
     -i, --ignore = Inaccessible | "Access Denied" | etc.
 CONTENT LENGTHS
     Filter out 200 OK false positive results by HTTP response content lengths
     Specify 'base' to ignore content length of the base HTTP response
@@ -541,19 +572,23 @@
     Number of total HTTP requests to send for each test case
     -r, --repeat = 1000 | etc.
 THREADS
     Number of parallel threads to run
     -th, --threads = 20 | etc.
 USER AGENT
     User agent to use
-    Default: Stresser/10.9
+    Default: Stresser/11.0
     -a, --user-agent = curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x, --proxy = http://127.0.0.1:8080 | etc.
+SHOW TABLE
+    Display the results in a table instead of JSON
+    Intended for a wide screen use
+    -st, --show-table
 OUT
     Output file
     -o, --out = results.json | etc.
 DIRECTORY
     Output directory
     All valid and unique HTTP responses will be saved in this directory
     -dir, --directory = results | etc.
@@ -563,7 +598,11 @@
 ```
 
 ## Images
 
 <p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example.png" alt="Basic Example"></p>
 
 <p align="center">Figure 1 - Basic Example</p>
+
+<p align="center"><img src="https://github.com/ivan-sincek/forbidden/blob/main/img/basic_example_table.png" alt="Basic Example"></p>
+
+<p align="center">Figure 2 - Basic Example (Table Output)</p>
```

### Comparing `forbidden-10.9/src/stresser/stresser.py` & `forbidden-11.0/src/stresser/stresser.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,56 @@
 		self.__end = datetime.datetime.now()
 		print(("Script has finished in {0}").format(self.__end - self.__start))
 
 stopwatch = Stopwatch()
 
 # ----------------------------------------
 
-default_quotes = "'"
+default_quotes = "'" # NOTE: Default quotes in the JSON 'command' attribute.
 
 def escape_quotes(value):
 	return str(value).replace(default_quotes, ("\\{0}").format(default_quotes))
 
 def set_param(value, param = ""):
 	value = default_quotes + escape_quotes(value) + default_quotes
 	if param:
 		value = ("{0} {1}").format(param, value)
 	return value
 
 # ----------------------------------------
 
+def get_header_key_value(header):
+	key = ""; value = ""
+	if re.search(r"^.+\:.+$", header):
+		key, value = header.split(":", 1)
+	elif re.search(r"^[^\;]+\;$", header):
+		key, value = header.split(";", 1)
+	return key.strip(), value.strip()
+
+def format_header_key_value(key, value):
+	return ("{0}: {1}").format(key, value) if value else ("{0};").format(key)
+
+def get_cookie_key_value(cookie):
+	key = ""; value = ""
+	if re.search(r"^[^\=\;]+\=[^\=\;]+$|^[^\=\;]+\=$", cookie):
+		key, value = cookie.split("=", 1)
+	return key.strip(), value.strip()
+
+def format_cookie_key_value(key, value):
+	return ("{0}={1}").format(key, value)
+
+def array_to_dict(array, separator):
+	tmp = {}
+	for entry in array:
+		key, value = entry.split(separator)
+		tmp[key] = value
+	return tmp
+
+# ----------------------------------------
+
 def get_base_https_url(scheme, dnp, port, full_path):
 	return ("https://{0}:{1}{2}").format(dnp, port if scheme == "https" else 443, full_path)
 
 def get_base_http_url(scheme, dnp, port, full_path):
 	return ("http://{0}:{1}{2}").format(dnp, port if scheme == "http" else 80, full_path)
 
 def get_all_domains(scheme, dnps, port): # NOTE: Extends domain names and IPs.
@@ -151,15 +180,17 @@
 	if confirm.lower() == "yes":
 		try:
 			open(out, "w").write(data)
 			print(("Results have been saved to '{0}'").format(out))
 		except FileNotFoundError:
 			print(("Cannot save results to '{0}'").format(out))
 
-default_user_agent = "Stresser/10.9"
+# ----------------------------------------
+
+default_user_agent = "Stresser/11.0"
 
 def get_all_user_agents():
 	tmp = []
 	file = os.path.join(os.path.abspath(os.path.split(__file__)[0]), "user_agents.txt")
 	if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
 		with open(file, "r", encoding = default_encoding) as stream:
 			for line in stream:
@@ -170,32 +201,39 @@
 
 def get_random_user_agent():
 	tmp = get_all_user_agents()
 	return tmp[random.randint(0, len(tmp) - 1)]
 
 # ----------------------------------------
 
+ERROR     =  0
+IGNORED   = -1
+DUPLICATE = -2
+
 class Stresser:
 
-	def __init__(self, url, ignore_qsf, ignore_curl, force, ignore, content_lengths, request_timeout, repeat, threads, user_agents, proxy, directory, debug):
+	def __init__(self, url, ignore_qsf, ignore_curl, force, headers, cookies, ignore, content_lengths, request_timeout, repeat, threads, user_agents, proxy, directory, show_table, debug):
 		# --------------------------------
 		# NOTE: User-controlled input.
 		self.__url             = self.__parse_url(url, bool(ignore_qsf))
 		self.__force           = force
+		self.__headers         = headers
+		self.__cookies         = cookies
 		self.__ignore          = ignore
 		self.__content_lengths = content_lengths
 		self.__repeat          = repeat
 		self.__threads         = threads
 		self.__user_agents     = user_agents
 		self.__user_agents_len = len(self.__user_agents)
 		self.__proxy           = proxy
+		self.__show_table      = show_table
 		self.__directory       = directory
 		self.__debug           = debug
 		# --------------------------------
-		# NOTE: Python cURL configuration.
+		# NOTE: PycURL configuration.
 		self.__curl            = not ignore_curl
 		self.__verify          = False # NOTE: Ignore SSL/TLS verification.
 		self.__allow_redirects = True
 		self.__max_redirects   = 10
 		self.__connect_timeout = request_timeout
 		self.__read_timeout    = request_timeout
 		self.__encoding        = "UTF-8" # NOTE: ISO-8859-1 works better than UTF-8 when accessing files.
@@ -371,81 +409,116 @@
 				print_cyan(("Cannot fetch allowed HTTP methods, defaulting to HTTP {0} method for all non-specific test cases...").format(self.__default_method))
 				self.__allowed_methods = [self.__default_method]
 				# TO DO: Brute-force allowed HTTP methods.
 			else:
 				print_green(("Allowed HTTP methods: [{0}]").format((", ").join(self.__allowed_methods)))
 		# --------------------------------
 
-	def __fetch(self, url, method = None, headers = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
-		record = self.__record("SYSTEM-0", url, method, headers, body, user_agent, proxy, curl)
+	def __fetch(self, url, method = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, passthrough = True):
+		record = self.__record("SYSTEM-0", url, method, headers, cookies, body, user_agent, proxy, curl)
 		return self.__send_curl(record, passthrough) if record["curl"] else self.__send_request(record, passthrough)
 
-	def __records(self, identifier, urls, methods = None, headers = None, body = None, user_agent = None, proxy = None, curl = None, repeat = None):
+	def __records(self, identifier, urls, methods = None, headers = None, cookies = None, body = None, user_agent = None, proxy = None, curl = None, repeat = None):
 		if not isinstance(urls, list):
 			urls = [urls]
 		if not isinstance(methods, list):
 			methods = [methods]
 		if not repeat:
 			repeat = self.__repeat
 		if headers:
 			for url in urls:
 				for method in methods:
 					for header in headers:
 						if not isinstance(header, list):
-							# NOTE: Python cURL accepts only string arrays as HTTP request headers.
+							# NOTE: PycURL accepts only string arrays as HTTP request headers.
 							header = [header]
 						for i in range(repeat):
-							self.__collection.append(self.__record(identifier, url, method, header, body, user_agent, proxy, curl))
+							self.__collection.append(self.__record(identifier, url, method, header, cookies, body, user_agent, proxy, curl))
 		else:
 			for url in urls:
 				for method in methods:
 					for i in range(repeat):
-						self.__collection.append(self.__record(identifier, url, method, [], body, user_agent, proxy, curl))
+						self.__collection.append(self.__record(identifier, url, method, [], cookies, body, user_agent, proxy, curl))
 
-	def __record(self, identifier, url, method, headers, body, user_agent, proxy, curl):
+	def __record(self, identifier, url, method, headers, cookies, body, user_agent, proxy, curl):
 		self.__identifier += 1
 		# identifier = ("{0}-{1}").format(self.__identifier, identifier)
 		if not method:
 			method = self.__force if self.__force else self.__default_method
+		headers = self.__inspect_headers(headers)
+		cookies = self.__inspect_cookies(cookies)
 		if not user_agent:
 			user_agent = self.__user_agents[random.randint(0, self.__user_agents_len - 1)] if self.__user_agents_len > 1 else self.__user_agents[0]
 		if not proxy:
 			proxy = self.__proxy
-		if not curl:
+		if not curl and curl is not False:
 			curl = self.__curl
 		record = {
 			"raw"             : self.__identifier,
 			"id"              : identifier,
 			"url"             : url,
 			"method"          : method,
 			"headers"         : headers,
+			"cookies"         : cookies,
 			"body"            : body,
 			"user_agent"      : user_agent,
 			"proxy"           : proxy,
 			"command"         : None,
-			"code"            : 0,
+			"code"            : ERROR,
 			"length"          : 0,
 			"response"        : None,
 			"response_headers": None,
 			"curl"            : curl
 		}
 		record["command"] = self.__build_command(record)
 		return record
 
+	def __inspect_headers(self, headers = None):
+		tmp = []
+		exists = set()
+		if headers:
+			for header in headers:
+				key, value = get_header_key_value(header)
+				if key:
+					exists.add(key.lower())
+					tmp.append(format_header_key_value(key, value))
+		for header in self.__headers:
+			key, value = get_header_key_value(header)
+			if key and key.lower() not in exists: # NOTE: Extra HTTP request headers cannot override test HTTP request headers.
+				tmp.append(format_header_key_value(key, value))
+		return tmp
+
+	def __inspect_cookies(self, cookies = None):
+		tmp = []
+		exists = set()
+		if cookies:
+			for cookie in cookies:
+				key, value = get_cookie_key_value(cookie)
+				if key:
+					exists.add(key.lower())
+					tmp.append(format_cookie_key_value(key, value))
+		for cookie in self.__cookies:
+			key, value = get_cookie_key_value(cookie)
+			if key and key.lower() not in exists: # NOTE: Extra HTTP cookies cannot override test HTTP cookies.
+				tmp.append(format_cookie_key_value(key, value))
+		return tmp
+
 	def __build_command(self, record):
 		tmp = ["curl", ("--connect-timeout {0}").format(self.__connect_timeout), ("-m {0}").format(self.__read_timeout), "-iskL", ("--max-redirs {0}").format(self.__max_redirects), "--path-as-is"]
 		if record["body"]:
 			tmp.append(set_param(record["body"], "-d"))
 		if record["proxy"]:
 			tmp.append(set_param(record["proxy"], "-x"))
 		if record["user_agent"]:
 			tmp.append(set_param(record["user_agent"], "-A"))
 		if record["headers"]:
 			for header in record["headers"]:
 				tmp.append(set_param(header, "-H"))
+		if record["cookies"]:
+			tmp.append(set_param(("; ").join(record["cookies"]), "-b"))
 		tmp.append(set_param(record["method"], "-X"))
 		tmp.append(set_param(record["url"]))
 		tmp = (" ").join(tmp)
 		return tmp
 
 	def __run_tests(self):
 		results = []
@@ -503,14 +576,16 @@
 			curl.setopt(pycurl.CUSTOMREQUEST, record["method"])
 			if record["method"] in ["HEAD"]:
 				curl.setopt(pycurl.NOBODY, True)
 			if record["user_agent"]:
 				curl.setopt(pycurl.USERAGENT, self.__encode(record["user_agent"]))
 			if record["headers"]:
 				curl.setopt(pycurl.HTTPHEADER, self.__encode(record["headers"])) # Will override 'User-Agent' HTTP request header.
+			if record["cookies"]:
+				curl.setopt(pycurl.COOKIE, ("; ").join(record["cookies"]))
 			if record["body"]:
 				curl.setopt(pycurl.POSTFIELDS, record["body"])
 			if record["proxy"]:
 				curl.setopt(pycurl.PROXY, record["proxy"])
 			# ----------------------------
 			curl.perform()
 			# ----------------------------
@@ -518,15 +593,15 @@
 			record["length"] = int(curl.getinfo(pycurl.SIZE_DOWNLOAD))
 			record["id"] = ("{0}-{1}-{2}").format(record["code"], record["length"], record["id"])
 			content = response.getvalue()
 			if passthrough:
 				record["response_headers"] = self.__decode(headers.getvalue())
 				# record["response"] = self.__decode(content)
 			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(content), self.__regex_flags)):
-				record["code"] = -1
+				record["code"] = IGNORED
 			# NOTE: Additional validation to prevent congestion from writing large and usless data to files.
 			elif record["code"] >= 200 and record["code"] < 400:
 				file = os.path.join(self.__directory, ("{0}.txt").format(record["id"]))
 				if not os.path.exists(file):
 					open(file, "wb").write(content)
 			# ----------------------------
 		except (pycurl.error, FileNotFoundError) as ex:
@@ -563,14 +638,16 @@
 				record["method"],
 				record["url"]
 			)
 			if record["user_agent"]:
 				request.headers["User-Agent"] = self.__encode(record["user_agent"])
 			if record["headers"]:
 				self.__set_double_headers(request, record["headers"]) # Will override 'User-Agent' HTTP request header.
+			if record["cookies"]:
+				session.cookies.update(array_to_dict(record["cookies"], "="))
 			if record["body"]:
 				request.data = record["body"]
 			if record["proxy"]:
 				session.proxies["https"] = session.proxies["http"] = record["proxy"]
 			# ----------------------------
 			prepared = session.prepare_request(request)
 			prepared.url = record["url"]
@@ -586,15 +663,15 @@
 			record["length"] = len(response.content)
 			record["id"] = ("{0}-{1}-{2}").format(record["code"], record["length"], record["id"])
 			content = response.content
 			if passthrough:
 				record["response_headers"] = dict(response.headers)
 				# record["response"] = self.__decode(content)
 			elif record["length"] in self.__content_lengths or (self.__ignore and re.search(self.__ignore, self.__decode(content), self.__regex_flags)):
-				record["code"] = -1
+				record["code"] = IGNORED
 			# NOTE: Additional validation to prevent congestion from writing large and usless data to files.
 			elif record["code"] >= 200 and record["code"] < 400:
 				file = os.path.join(self.__directory, ("{0}.txt").format(record["id"]))
 				if not os.path.exists(file):
 					open(file, "wb").write(content)
 			# ----------------------------
 		except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException, FileNotFoundError) as ex:
@@ -610,111 +687,136 @@
 				session.close()
 			# ----------------------------
 		return record
 
 	def __set_double_headers(self, request, headers):
 		exists = set()
 		for header in headers:
-			array = header.split(":", 1)
-			key = array[0].rstrip(";")
-			value = self.__encode(array[1].strip() if len(array) > 1 else "")
-			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = value
+			key, value = get_header_key_value(header)
+			request.headers[key if key not in exists and not exists.add(key) else uniquestr(key)] = self.__encode(value) # NOTE: Allows double headers.
 
 	def __validate_results(self):
-		tmp = []
-		# --------------------------------
 		print_time("Validating results...")
 		self.__mark_duplicates()
-		table = Table(self.__collection) # unfiltered
-		# --------------------------------
-		self.__collection = pop(sorted([record for record in self.__collection if record["code"] > 0], key = lambda x: (x["code"], -x["length"], x["raw"])), ["raw", "proxy", "response_headers", "response", "curl"])
-		# --------------------------------
-		for record in self.__collection:
-			if record["code"] >= 500:
-				continue
-				print_cyan(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 400:
-				continue
-				print_red(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 300:
-				# continue
-				print_yellow(jdump(record))
-				tmp.append(record)
-			elif record["code"] >= 200:
-				# continue
-				print_green(jdump(record))
-				tmp.append(record)
-			elif record["code"] > 0:
-				continue
-				print_white(jdump(record))
-				tmp.append(record)
-		# --------------------------------
-		self.__collection = tmp
-		table.show()
+		output = Output(self.__collection)
+		self.__collection = output.results_table() if self.__show_table else output.results_json()
+		output.stats_table()
 
 	def __mark_duplicates(self):
 		exists = set()
 		for record in self.__collection:
 			if record["id"] not in exists and not exists.add(record["id"]):
 				continue
-			record["code"] = -2
+			record["code"] = DUPLICATE
 
 	def __prepare_collection(self):
 		print_time("Preparing test records...")
 		# --------------------------------
 		# NOTE: Stress testing.
 		self.__records(
 			identifier = "STRESS-1",
 			urls       = self.__url["urls"]["base"]
 		)
 
 # ----------------------------------------
 
-class Table:
+class Output:
 
 	def __init__(self, collection):
-		self.__table = self.__init_table(collection)
+		self.__collection = pop(sorted([record for record in collection if record["code"] >= 100 and record["code"] < 600], key = lambda x: (x["code"], -x["length"], x["raw"])), ["raw", "proxy", "response_headers", "response", "curl"]) # filtered
+		self.__stats      = self.__count(collection) # unfiltered
 
-	def __init_table(self, collection):
-		table = {}
-		for record in collection:
-			if record["code"] not in table:
-				table[record["code"]] = 0
-			table[record["code"]] += 1
-		return dict(sorted(table.items()))
-
-	def __row(self, code, count, color):
-		return [
-			("{0}{1}{2}").format(color, code, colorama.Style.RESET_ALL),
-			("{0}{1}{2}").format(color, count, colorama.Style.RESET_ALL)
-		]
+	def __color(self, value, color):
+		return ("{0}{1}{2}").format(color, value, colorama.Style.RESET_ALL)
 
-	def show(self):
+	def __results_row(self, record, color):
+		return [self.__color(record[key], color) for key in ["id", "code", "length", "command"]]
+
+	def results_table(self):
+		tmp = []; table = []
+		for record in self.__collection:
+			if record["code"] < 100 or record["code"] >= 600:
+				continue
+			elif record["code"] >= 500:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.CYAN))
+			elif record["code"] >= 400:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.RED))
+			elif record["code"] >= 300:
+				# continue
+				table.append(self.__results_row(record, colorama.Fore.YELLOW))
+			elif record["code"] >= 200:
+				# continue
+				table.append(self.__results_row(record, colorama.Fore.GREEN))
+			elif record["code"] >= 100:
+				continue
+				table.append(self.__results_row(record, colorama.Fore.WHITE))
+			tmp.append(record)
+		if table:
+			print(tabulate.tabulate(table, tablefmt = "plain", colalign = ("right", "right", "right", "left")))
+		return tmp
+
+	def results_json(self): # NOTE: To see more or less results, comment in or out 'continue' line.
 		tmp = []
-		for code, count in self.__table.items():
-			if code >= 500:
-				tmp.append(self.__row(code, count, colorama.Fore.CYAN))
+		for record in self.__collection:
+			if record["code"] < 100 or record["code"] >= 600:
+				continue
+			elif record["code"] >= 500:
+				continue
+				print_cyan(jdump(record))
+			elif record["code"] >= 400:
+				continue
+				print_red(jdump(record))
+			elif record["code"] >= 300:
+				# continue
+				print_yellow(jdump(record))
+			elif record["code"] >= 200:
+				# continue
+				print_green(jdump(record))
+			elif record["code"] >= 100:
+				continue
+				print_white(jdump(record))
+			tmp.append(record)
+		return tmp
+
+	def __count(self, collection):
+		tmp = {}
+		for record in collection:
+			if record["code"] not in tmp:
+				tmp[record["code"]] = 0
+			tmp[record["code"]] += 1
+		return dict(sorted(tmp.items()))
+
+	def __stats_row(self, code, count, color):
+		return [self.__color(entry, color) for entry in [code, count]]
+
+	def stats_table(self):
+		table = []; table_special = []
+		for code, count in self.__stats.items():
+			if code == ERROR:
+				table_special.append(self.__stats_row("Errors", count, colorama.Fore.WHITE))
+			elif code == IGNORED:
+				table_special.append(self.__stats_row("Ignored", count, colorama.Fore.WHITE))
+			elif code == DUPLICATE:
+				table_special.append(self.__stats_row("Duplicates", count, colorama.Fore.WHITE))
+			elif code < 100 or code >= 600:
+				continue
+			elif code >= 500:
+				table.append(self.__stats_row(code, count, colorama.Fore.CYAN))
 			elif code >= 400:
-				tmp.append(self.__row(code, count, colorama.Fore.RED))
+				table.append(self.__stats_row(code, count, colorama.Fore.RED))
 			elif code >= 300:
-				tmp.append(self.__row(code, count, colorama.Fore.YELLOW))
+				table.append(self.__stats_row(code, count, colorama.Fore.YELLOW))
 			elif code >= 200:
-				tmp.append(self.__row(code, count, colorama.Fore.GREEN))
-			elif code > 0:
-				tmp.append(self.__row(code, count, colorama.Fore.WHITE))
-			elif code == 0:
-				tmp.append(self.__row("Errors", count, colorama.Fore.WHITE))
-			elif code == -1:
-				tmp.append(self.__row("Ignored", count, colorama.Fore.WHITE))
-			elif code == -2:
-				tmp.append(self.__row("Duplicates", count, colorama.Fore.WHITE))
-		if tmp:
-			print(tabulate.tabulate(tmp, ["Code", "Count"], tablefmt = "outline", colalign = ("left", "left")))
+				table.append(self.__stats_row(code, count, colorama.Fore.GREEN))
+			elif code >= 100:
+				table.append(self.__stats_row(code, count, colorama.Fore.WHITE))
+		if table or table_special:
+			print(tabulate.tabulate(table + table_special, ["Status Code", "Count"], tablefmt = "outline", colalign = ("left", "right")))
 
 # ----------------------------------------
 
 class Progress:
 
 	def __init__(self, total, print_lock):
 		self.__total      = total
@@ -725,17 +827,17 @@
 		with self.__print_lock:
 			print(("Progress: {0}/{1} | {2:.2f}%").format(self.__count, self.__total, (self.__count / self.__total) * 100), end = "\n" if self.__count == self.__total else "\r")
 			self.__count += 1
 
 # ----------------------------------------
 
 class MyArgParser(argparse.ArgumentParser):
-	
+
 	def print_help(self):
-		print("Stresser v10.9 ( github.com/ivan-sincek/forbidden )")
+		print("Stresser v11.0 ( github.com/ivan-sincek/forbidden )")
 		print("")
 		print("Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]")
 		print("Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]")
 		print("")
 		print("DESCRIPTION")
 		print("    Bypass 4xx HTTP response status codes with stress testing")
 		print("URL")
@@ -746,14 +848,23 @@
 		print("    -iqsf, --ignore-query-string-and-fragment")
 		print("IGNORE CURL")
 		print("    Use Python Requests instead of PycURL where applicable")
 		print("    -ic, --ignore-curl")
 		print("FORCE")
 		print("    Force an HTTP method for all non-specific test cases")
 		print("    -f, --force = GET | POST | CUSTOM | etc.")
+		print("HEADER")
+		print("    Specify any number of extra HTTP request headers")
+		print("    Extra HTTP request headers will not override test HTTP request headers")
+		print("    Semi-colon in e.g. 'Content-Type;' will expand to an empty HTTP request header.")
+		print("    -H, --header = \"Authorization: Bearer ey...\" | Content-Type; | etc.")
+		print("COOKIE")
+		print("    Specify any number of extra HTTP cookies")
+		print("    Extra HTTP cookies will not override test HTTTP cookies")
+		print("    -b, --cookie = PHPSESSIONID=3301 | etc.")
 		print("IGNORE")
 		print("    Filter out 200 OK false positive results with RegEx")
 		print("    Spacing will be stripped")
 		print("    -i, --ignore = Inaccessible | \"Access Denied\" | etc.")
 		print("CONTENT LENGTHS")
 		print("    Filter out 200 OK false positive results by HTTP response content lengths")
 		print("    Specify 'base' to ignore content length of the base HTTP response")
@@ -772,56 +883,65 @@
 		print("USER AGENT")
 		print("    User agent to use")
 		print(("    Default: {0}").format(default_user_agent))
 		print("    -a, --user-agent = curl/3.30.1 | random[-all] | etc.")
 		print("PROXY")
 		print("    Web proxy to use")
 		print("    -x, --proxy = http://127.0.0.1:8080 | etc.")
+		print("SHOW TABLE")
+		print("    Display the results in a table instead of JSON")
+		print("    Intended for a wide screen use")
+		print("    -st, --show-table")
 		print("OUT")
 		print("    Output file")
 		print("    -o, --out = results.json | etc.")
 		print("DIRECTORY")
 		print("    Output directory")
 		print("    All valid and unique HTTP responses will be saved in this directory")
 		print("    -dir, --directory = results | etc.")
 		print("DEBUG")
 		print("    Debug output")
 		print("    -dbg, --debug")
 
 	def error(self, message):
 		if len(sys.argv) > 1:
-			print("Missing a mandatory option (-u, -dir, -r, -th) and/or optional (-iqsf, -ic, -f, -i, -l, -rt, -a, -x, -o, -dbg)")
+			print("Missing a mandatory option (-u, -dir, -r, -th) and/or optional (-iqsf, -ic, -f, -H, -b, -i, -l, -rt, -a, -x, -o, -dbg)")
 			print("Use -h or --help for more info")
 		else:
 			self.print_help()
 		exit()
 
 class Validate:
 
 	def __init__(self):
 		self.__proceed = True
 		self.__parser  = MyArgParser()
 		self.__parser.add_argument("-u"   , "--url"                             , required = True , type   = str         , default = ""   )
 		self.__parser.add_argument("-iqsf", "--ignore-query-string-and-fragment", required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-ic"  , "--ignore-curl"                     , required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-f"   , "--force"                           , required = False, type   = str.upper   , default = ""   )
+		self.__parser.add_argument("-H"   , "--header"                          , required = False, action = "append"    , nargs   = "+"  )
+		self.__parser.add_argument("-b"   , "--cookie"                          , required = False, action = "append"    , nargs   = "+"  )
 		self.__parser.add_argument("-i"   , "--ignore"                          , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-l"   , "--content-lengths"                 , required = False, type   = str.lower   , default = ""   )
 		self.__parser.add_argument("-rt"  , "--request-timeout"                 , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-r"   , "--repeat"                          , required = True , type   = str         , default = ""   )
 		self.__parser.add_argument("-th"  , "--threads"                         , required = True , type   = str         , default = ""   )
 		self.__parser.add_argument("-a"   , "--user-agent"                      , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-x"   , "--proxy"                           , required = False, type   = str         , default = ""   )
+		self.__parser.add_argument("-st"  , "--show-table"                      , required = False, action = "store_true", default = False)
 		self.__parser.add_argument("-o"   , "--out"                             , required = False, type   = str         , default = ""   )
 		self.__parser.add_argument("-dir" , "--directory"                       , required = True , type   = str         , default = ""   )
 		self.__parser.add_argument("-dbg" , "--debug"                           , required = False, action = "store_true", default = False)
 
 	def run(self):
 		self.__args                 = self.__parser.parse_args()
 		self.__args.url             = self.__parse_url(self.__args.url, "url")                  # required
+		self.__args.header          = self.__parse_header(self.__args.header)                   if self.__args.header          else []
+		self.__args.cookie          = self.__parse_cookie(self.__args.cookie)                   if self.__args.cookie          else []
 		self.__args.ignore          = self.__parse_ignore(self.__args.ignore)                   if self.__args.ignore          else ""
 		self.__args.content_lengths = self.__parse_content_lengths(self.__args.content_lengths) if self.__args.content_lengths else []
 		self.__args.request_timeout = self.__parse_request_timeout(self.__args.request_timeout) if self.__args.request_timeout else 60
 		self.__args.repeat          = self.__parse_repeat(self.__args.repeat)                   # required
 		self.__args.threads         = self.__parse_threads(self.__args.threads)                 # required
 		self.__args.user_agent      = self.__parse_user_agent(self.__args.user_agent)           if self.__args.user_agent      else [default_user_agent]
 		self.__args.proxy           = self.__parse_url(self.__args.proxy, "proxy")              if self.__args.proxy           else ""
@@ -867,19 +987,41 @@
 			self.__error(data[key]["scheme_error"][1])
 		elif not tmp.netloc:
 			self.__error(data[key]["domain_error"])
 		elif tmp.port and (tmp.port < 1 or tmp.port > 65535):
 			self.__error(data[key]["port_error"])
 		return value
 
+	def __parse_header(self, headers):
+		tmp = []
+		for header in headers:
+			header = header[0]
+			key, value = get_header_key_value(header)
+			if not key:
+				self.__error(("Invalid header: {0}").format(header))
+				continue
+			tmp.append(format_header_key_value(key, value))
+		return tmp
+
+	def __parse_cookie(self, cookies):
+		tmp = []
+		for cookie in cookies:
+			cookie = cookie[0]
+			key, value = get_cookie_key_value(cookie)
+			if not key:
+				self.__error(("Invalid cookie: {0}").format(cookie))
+				continue
+			tmp.append(format_cookie_key_value(key, value))
+		return tmp
+
 	def __parse_ignore(self, value):
 		try:
 			re.compile(value)
 		except re.error:
-			self.__error("Invalid RegEx")
+			self.__error(("Invalid RegEx: {0}").format(value))
 		return value
 
 	def __parse_content_lengths(self, value):
 		tmp = []
 		for entry in value.lower().split(","):
 			entry = entry.strip()
 			if not entry:
@@ -937,36 +1079,39 @@
 # ----------------------------------------
 
 def main():
 	validate = Validate()
 	if validate.run():
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                             Stresser v10.9                             #")
+		print("#                             Stresser v11.0                             #")
 		print("#                                 by Ivan Sincek                         #")
 		print("#                                                                        #")
 		print("# Bypass 4xx HTTP response status codes  with stress testing.            #")
 		print("# GitHub repository at github.com/ivan-sincek/forbidden.                 #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
 		out = validate.get_arg("out")
 		stresser = Stresser(
 			validate.get_arg("url"),
 			validate.get_arg("ignore_query_string_and_fragment"),
 			validate.get_arg("ignore_curl"),
 			validate.get_arg("force"),
+			validate.get_arg("header"),
+			validate.get_arg("cookie"),
 			validate.get_arg("ignore"),
 			validate.get_arg("content_lengths"),
 			validate.get_arg("request_timeout"),
 			validate.get_arg("repeat"),
 			validate.get_arg("threads"),
 			validate.get_arg("user_agent"),
 			validate.get_arg("proxy"),
 			validate.get_arg("directory"),
+			validate.get_arg("show_table"),
 			validate.get_arg("debug")
 		)
 		stresser.run()
 		results = stresser.get_results()
 		if results and out:
 			write_file(jdump(results), out)
 		stopwatch.stop()
```

### Comparing `forbidden-10.9/src/stresser/user_agents.txt` & `forbidden-11.0/src/stresser/user_agents.txt`

 * *Files identical despite different names*

