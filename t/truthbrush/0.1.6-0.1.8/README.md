# Comparing `tmp/truthbrush-0.1.6.tar.gz` & `tmp/truthbrush-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truthbrush-0.1.6.tar", max compression
+gzip compressed data, was "truthbrush-0.1.8.tar", max compression
```

## Comparing `truthbrush-0.1.6.tar` & `truthbrush-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-10-18 17:17:37.547285 truthbrush-0.1.6/LICENSE
--rw-r--r--   0        0        0     3166 2023-10-18 17:17:37.547285 truthbrush-0.1.6/README.md
--rw-r--r--   0        0        0      584 2023-10-18 17:17:37.551285 truthbrush-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       31 2023-10-18 17:17:37.551285 truthbrush-0.1.6/truthbrush/__init__.py
--rw-r--r--   0        0        0    12550 2023-10-18 17:17:37.551285 truthbrush-0.1.6/truthbrush/api.py
--rw-r--r--   0        0        0     3342 2023-10-18 17:17:37.551285 truthbrush-0.1.6/truthbrush/cli.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 truthbrush-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 18:02:28.662067 truthbrush-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3838 2024-05-13 18:02:28.662067 truthbrush-0.1.8/README.md
+-rw-r--r--   0        0        0      582 2024-05-13 18:02:28.662067 truthbrush-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-13 18:02:28.662067 truthbrush-0.1.8/truthbrush/__init__.py
+-rw-r--r--   0        0        0    14410 2024-05-13 18:02:28.662067 truthbrush-0.1.8/truthbrush/api.py
+-rw-r--r--   0        0        0     4101 2024-05-13 18:02:28.662067 truthbrush-0.1.8/truthbrush/cli.py
+-rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 truthbrush-0.1.8/PKG-INFO
```

### Comparing `truthbrush-0.1.6/LICENSE` & `truthbrush-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `truthbrush-0.1.6/README.md` & `truthbrush-0.1.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # truthbrush
 Truthbrush is an API client for Truth Social. Truthbrush is built and maintained by the [Stanford Internet Observatory](https://io.stanford.edu).
 
 Currently, this tool can:
 
-* Search for users, statuses, or hashtags
+* Search for users, statuses, groups, or hashtags
 * Pull a user's statuses
 * Pull the list of "People to Follow" or suggested users
 * Pull "trending" hashtags
 * Pull "trending" Truth posts
 * Pull ads
 * Pull a user's metadata
+* Pull "trending" groups 
+* Pull list of suggested groups 
+* Pull "trending" group hashtags
 
 Truthbrush is designed for academic research, open source intelligence gathering, and data archival. It pulls all of the data from the publicly accessible API.
 
 ## Installation
 
 Truthbrush is not yet available on PyPI. To install it, run `pip install git+https://github.com/stanfordio/truthbrush.git`, or clone the repository and run `pip3 install .`. Provided your `pip` is setup correctly, this will make `truthbrush` available both as a command and as a Python package. **Note that Truthbrush requires Python 3.9 or higher.**
 
@@ -31,27 +34,31 @@
 Usage: truthbrush [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help     Show this message and exit.
 
 
 Commands:
-  search       Search for users, statuses or hashtags.
-  statuses     Pull a user's statuses.
-  suggestions  Pull the list of suggested users.
-  tags         Pull trendy tags.
-  trends       Pull trendy Truths.
-  ads          Pull ads.
-  user         Pull a user's metadata.
+  search             Search for users, statuses, groups, or hashtags.
+  statuses           Pull a user's statuses.
+  suggestions        Pull the list of suggested users.
+  tags               Pull trendy tags.
+  trends             Pull trendy Truths.
+  ads                Pull ads.
+  user               Pull a user's metadata.
+  likes              Pull the list of users who liked a post
+  group-tags         Pull trending group tags. 
+  group-trends       Pull trending groups.
+  group-suggestions  Pull list of suggested groups.
 ``````
 
-**Search for users, statuses, or hashtags**
+**Search for users, statuses, groups, or hashtags**
 
 ```bash
-truthbrush search --searchtype [accounts|statuses|hashtags] QUERY
+truthbrush search --searchtype [accounts|statuses|hashtags|groups] QUERY
 ```
 
 **Pull all statuses (posts) from a user**
 
 ```bash
 truthbrush statuses HANDLE
 ```
@@ -74,14 +81,38 @@
 
 **Pull all of a user's metadata**
 
 ```bash
 truthbrush user HANDLE
 ```
 
+**Pull the list of users who liked a post**
+
+```bash
+truthbrush likes POST TOP_NUM
+```
+
+**Pull trending group tags**
+
+```bash
+truthbrush group-tags
+```
+
+**Pull trending groups**
+
+```bash 
+truthbrush group-trends      
+``` 
+
+**Pull list of suggested groups**
+
+```bash 
+truthbrush group-suggestions
+```
+
 ## Contributing
 
 Contributions are encouraged! For small bug fixes and minor improvements, feel free to just open a PR. For larger changes, please open an issue first so that other contributors can discuss your plan, avoid duplicated work, and ensure it aligns with the goals of the project. Be sure to also follow the [code of conduct](CODE_OF_CONDUCT.md). Thanks!
 
 Development setup (ensure you have [Poetry](https://python-poetry.org/) installed):
 
 ```sh
```

### Comparing `truthbrush-0.1.6/pyproject.toml` & `truthbrush-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "truthbrush"
-version = "0.1.6"
+version = "0.1.8"
 description = "API client for Truth Social"
 authors = ["R. Miles McCain <github@sendmiles.email>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 truthbrush = "truthbrush.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-click = "^8.0.4"
-loguru = "^0.6.0"
-python-dotenv = "^0.19.2"
-python-dateutil = "^2.8.2"
-curl_cffi = "^0.5.2"
+click = "^8.1.0"
+loguru = "^0.7.0"
+python-dotenv = "^1.0.1"
+python-dateutil = "2.9.0"
+curl_cffi = "^0.6.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
+black = "^24.3.0"
 pytest = "^7.0.1"
 pylint = "^2.12.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `truthbrush-0.1.6/truthbrush/api.py` & `truthbrush-0.1.8/truthbrush/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if os.getenv("DEBUG") and os.getenv("DEBUG").lower() != "false"
         else logging.INFO
     )
 )
 
 BASE_URL = "https://truthsocial.com"
 API_BASE_URL = "https://truthsocial.com/api"
-USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36"
+USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
 
 # Oauth client credentials, from https://truthsocial.com/packs/js/application-d77ef3e9148ad1d0624c.js
 CLIENT_ID = "9X1Fdd-pxNsAgEDNi_SfhJWi8T-vLuV2WVzKIbkTCw4"
 CLIENT_SECRET = "ozF8jzI4968oTKFkEnsBC-UbLPCdrSv0MkXGQu2o_-M"
 
 proxies = {"http": os.getenv("http_proxy"), "https": os.getenv("https_proxy")}
 
@@ -56,14 +56,15 @@
         """Runs before any login-walled function to check for login credentials and generates an auth ID token"""
         if self.auth_id is None:
             if self.__username is None:
                 raise LoginErrorException("Username is missing.")
             if self.__password is None:
                 raise LoginErrorException("Password is missing.")
             self.auth_id = self.get_auth_id(self.__username, self.__password)
+            logger.warning(f"Using token {self.auth_id}")
 
     def _make_session(self):
         s = requests.Session()
         return s
 
     def _check_ratelimit(self, resp):
         if resp.headers.get("x-ratelimit-limit") is not None:
@@ -81,45 +82,54 @@
             now = datetime.utcnow().replace(tzinfo=timezone.utc)
             time_to_sleep = (
                 self.ratelimit_reset.replace(tzinfo=timezone.utc) - now
             ).total_seconds()
             logger.warning(
                 f"Approaching rate limit; sleeping for {time_to_sleep} seconds..."
             )
-            sleep(time_to_sleep)
+            if time_to_sleep > 0:
+                sleep(time_to_sleep)
+            else:
+                sleep(10)
 
     def _get(self, url: str, params: dict = None) -> Any:
         resp = self._make_session().get(
             API_BASE_URL + url,
             params=params,
             proxies=proxies,
-            impersonate="chrome110",
+            impersonate="chrome120",
             headers={
                 "Authorization": "Bearer " + self.auth_id,
                 "User-Agent": USER_AGENT,
             },
         )
 
         # Will also sleep
         self._check_ratelimit(resp)
 
-        return resp.json()
+        try:
+            r = resp.json()
+        except json.JSONDecodeError:
+            logger.error(f"Failed to decode JSON: {resp.text}")
+            r = None
+
+        return r
 
     def _get_paginated(self, url: str, params: dict = None, resume: str = None) -> Any:
         next_link = API_BASE_URL + url
 
         if resume is not None:
             next_link += f"?max_id={resume}"
 
         while next_link is not None:
             resp = self._make_session().get(
                 next_link,
                 params=params,
                 proxies=proxies,
-                impersonate="chrome110",
+                impersonate="chrome120",
                 headers={
                     "Authorization": "Bearer " + self.auth_id,
                     "User-Agent": USER_AGENT,
                 },
             )
             link_header = resp.headers.get("Link", "")
             next_link = None
@@ -130,14 +140,31 @@
                     break
             logger.info(f"Next: {next_link}, resp: {resp}, headers: {resp.headers}")
             yield resp.json()
 
             # Will also sleep
             self._check_ratelimit(resp)
 
+    def userLikes(self, post: str, top_num: int = 40) -> bool | Any:
+        """Return the top_num most recent users who liked the post."""
+        self.__check_login()
+        top_num = int(top_num)
+        if top_num < 1:
+            return
+        post = post.split("/")[-1]
+        n_output = 0
+        for followers_batch in self._get_paginated(
+            f"/v1/statuses/{post}/favourited_by", resume=None, params=dict(limit=80)
+        ):
+            for f in followers_batch:
+                yield f
+                n_output += 1
+                if n_output >= top_num:
+                    return
+
     def lookup(self, user_handle: str = None) -> Optional[dict]:
         """Lookup a user's information."""
 
         self.__check_login()
         assert user_handle is not None
         return self._get("/v1/accounts/lookup", params=dict(acct=user_handle))
 
@@ -182,36 +209,56 @@
                         offset=offset,
                         min_id=min_id,
                         max_id=max_id,
                     ),
                 )
 
             offset += 40
-            if not resp[searchtype]:
+            # added new not sure if helpful 
+            if not resp or all(value == [] for value in resp.values()):
                 break
 
             yield resp
 
-    def trending(self):
-        """Return trending truths."""
+    def trending(self, limit=10):
+        """Return trending truths.
+        Optional arg limit<20 specifies number to return."""
 
         self.__check_login()
-        return self._get("/v1/truth/trending/truths")
+        return self._get(f"/v1/truth/trending/truths?limit={limit}")
 
     def tags(self):
         """Return trending tags."""
 
         self.__check_login()
         return self._get("/v1/trends")
 
     def suggested(self, maximum: int = 50) -> dict:
         """Return a list of suggested users to follow."""
         self.__check_login()
         return self._get(f"/v2/suggestions?limit={maximum}")
 
+    def trending_groups(self, limit=10):
+        """Return trending group truths.
+        Optional arg limit<20 specifies number to return."""
+
+        self.__check_login()
+        return self._get(f"/v1/truth/trends/groups?limit={limit}")
+
+    def group_tags(self):
+        """Return trending group tags."""
+
+        self.__check_login()
+        return self._get("/v1/groups/tags")
+
+    def suggested_groups(self, maximum: int = 50) -> dict:
+        """Return a list of suggested groups to follow."""
+        self.__check_login()
+        return self._get(f"/v1/truth/suggestions/groups?limit={maximum}")
+
     def ads(self, device: str = "desktop") -> dict:
         """Return a list of ads from Rumble's Ad Platform via Truth Social API."""
 
         return self._get(f"/v3/truth/ads?device={device}")
 
     def user_followers(
         self,
@@ -256,14 +303,15 @@
     def pull_statuses(
         self,
         username: str,
         replies=False,
         verbose=False,
         created_after: datetime = None,
         since_id=None,
+        pinned=False,
     ) -> List[dict]:
         """Pull the given user's statuses.
 
         Params:
             created_after : timezone aware datetime object
             since_id : number or string
 
@@ -274,15 +322,17 @@
         params = {}
         user_id = self.lookup(username)["id"]
         page_counter = 0
         keep_going = True
         while keep_going:
             try:
                 url = f"/v1/accounts/{user_id}/statuses"
-                if not replies:
+                if pinned:
+                    url += "?pinned=true&with_muted=true"
+                elif not replies:
                     url += "?exclude_replies=true"
                 if verbose:
                     logger.debug("--------------------------")
                     logger.debug(f"{url} {params}")
                 result = self._get(url, params=params)
                 page_counter += 1
             except json.JSONDecodeError as e:
@@ -310,14 +360,17 @@
             params["max_id"] = posts[-1][
                 "id"
             ]  # when pulling the next page, get posts before this (the oldest)
 
             if verbose:
                 logger.debug(f"PAGE: {page_counter}")
 
+            if pinned:  # assume single page
+                keep_going = False
+
             for post in posts:
                 post["_pulled"] = datetime.now().isoformat()
 
                 # only keep posts created after the specified date
                 # exclude posts created before the specified date
                 # since the page is listed in reverse chronology, we don't need any remaining posts on this page either
                 post_at = date_parse.parse(post["created_at"]).replace(
@@ -349,15 +402,15 @@
             }
 
             sess_req = requests.request(
                 "POST",
                 url,
                 json=payload,
                 proxies=proxies,
-                impersonate="chrome110",
+                impersonate="chrome120",
                 headers={
                     "User-Agent": USER_AGENT,
                 },
             )
             sess_req.raise_for_status()
         except requests.RequestsError as e:
             logger.error(f"Failed login request: {str(e)}")
```

### Comparing `truthbrush-0.1.6/truthbrush/cli.py` & `truthbrush-0.1.8/truthbrush/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,36 +25,53 @@
 
 @cli.command()
 def tags():
     """Pull trendy tags."""
 
     print(json.dumps(api.tags()))
 
+@cli.command()
+def grouptags():
+    """Pull group tags."""
+
+    print(json.dumps(api.group_tags()))
+
+@cli.command()
+def grouptrends():
+    """Pull group trends."""
+
+    print(json.dumps(api.trending_groups()))
+
+@cli.command()
+def groupsuggest():
+    """Pull group suggestions."""
+
+    print(json.dumps(api.suggested_groups()))
 
 @cli.command()
 @click.argument("handle")
 def user(handle: str):
     """Pull a user's metadata."""
 
     print(json.dumps(api.lookup(handle)))
 
 
 @cli.command()
 @click.argument("query")
 @click.option(
     "--searchtype",
-    help="Type of search query (accounts, statuses, or hashtags)",
-    type=click.Choice(["accounts", "statuses", "hashtags"]),
+    help="Type of search query (accounts, statuses, groups, or hashtags)",
+    type=click.Choice(["accounts", "statuses", "hashtags", "groups"]),
 )
 @click.option(
     "--limit", default=40, help="Limit the number of items returned", type=int
 )
 @click.option("--resolve", help="Resolve", type=bool)
 def search(searchtype: str, query: str, limit: int, resolve: bool):
-    """Search for users, statuses or hashtags."""
+    """Search for users, statuses, groups, or hashtags."""
 
     for page in api.search(searchtype, query, limit, resolve):
         print(json.dumps(page[searchtype]))
 
 
 @cli.command()
 def suggestions():
@@ -111,18 +128,35 @@
 )
 @click.option(
     "--created-after",
     default=None,
     help="Only pull posts created on or after the specified datetime, e.g. 2021-10-02 or 2011-11-04T00:05:23+04:00 (defaults to none). If a timezone is not specified, UTC is assumed.",
     type=datetime.datetime.fromisoformat,
 )
-def statuses(username: str, replies: bool = False, created_after: date = None):
+@click.option(
+    "--pinned/--all", default=False, help="Only pull pinned posts (defaults to all)"
+)
+def statuses(
+    username: str,
+    replies: bool = False,
+    created_after: date = None,
+    pinned: bool = False,
+):
     """Pull a user's statuses"""
 
     # Assume UTC if no timezone is specified
     if created_after and created_after.tzinfo is None:
         created_after = created_after.replace(tzinfo=datetime.timezone.utc)
 
     for page in api.pull_statuses(
-        username, created_after=created_after, replies=replies
+        username, created_after=created_after, replies=replies, pinned=pinned
     ):
         print(json.dumps(page))
+
+
+@cli.command()
+@click.argument("post")
+@click.argument("top_num")
+def likes(post: str, top_num: int):
+    """Pull the top_num most recent users who liked the post."""
+    for page in api.userLikes(post, top_num):
+        print(json.dumps(page))
```

### Comparing `truthbrush-0.1.6/PKG-INFO` & `truthbrush-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: truthbrush
-Version: 0.1.6
+Version: 0.1.8
 Summary: API client for Truth Social
 License: Apache 2.0
 Author: R. Miles McCain
 Author-email: github@sendmiles.email
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: curl_cffi (>=0.5.2,<0.6.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.0,<9.0.0)
+Requires-Dist: curl_cffi (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: python-dateutil (==2.9.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # truthbrush
 Truthbrush is an API client for Truth Social. Truthbrush is built and maintained by the [Stanford Internet Observatory](https://io.stanford.edu).
 
 Currently, this tool can:
 
-* Search for users, statuses, or hashtags
+* Search for users, statuses, groups, or hashtags
 * Pull a user's statuses
 * Pull the list of "People to Follow" or suggested users
 * Pull "trending" hashtags
 * Pull "trending" Truth posts
 * Pull ads
 * Pull a user's metadata
+* Pull "trending" groups 
+* Pull list of suggested groups 
+* Pull "trending" group hashtags
 
 Truthbrush is designed for academic research, open source intelligence gathering, and data archival. It pulls all of the data from the publicly accessible API.
 
 ## Installation
 
 Truthbrush is not yet available on PyPI. To install it, run `pip install git+https://github.com/stanfordio/truthbrush.git`, or clone the repository and run `pip3 install .`. Provided your `pip` is setup correctly, this will make `truthbrush` available both as a command and as a Python package. **Note that Truthbrush requires Python 3.9 or higher.**
 
@@ -51,27 +55,31 @@
 Usage: truthbrush [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help     Show this message and exit.
 
 
 Commands:
-  search       Search for users, statuses or hashtags.
-  statuses     Pull a user's statuses.
-  suggestions  Pull the list of suggested users.
-  tags         Pull trendy tags.
-  trends       Pull trendy Truths.
-  ads          Pull ads.
-  user         Pull a user's metadata.
+  search             Search for users, statuses, groups, or hashtags.
+  statuses           Pull a user's statuses.
+  suggestions        Pull the list of suggested users.
+  tags               Pull trendy tags.
+  trends             Pull trendy Truths.
+  ads                Pull ads.
+  user               Pull a user's metadata.
+  likes              Pull the list of users who liked a post
+  group-tags         Pull trending group tags. 
+  group-trends       Pull trending groups.
+  group-suggestions  Pull list of suggested groups.
 ``````
 
-**Search for users, statuses, or hashtags**
+**Search for users, statuses, groups, or hashtags**
 
 ```bash
-truthbrush search --searchtype [accounts|statuses|hashtags] QUERY
+truthbrush search --searchtype [accounts|statuses|hashtags|groups] QUERY
 ```
 
 **Pull all statuses (posts) from a user**
 
 ```bash
 truthbrush statuses HANDLE
 ```
@@ -94,14 +102,38 @@
 
 **Pull all of a user's metadata**
 
 ```bash
 truthbrush user HANDLE
 ```
 
+**Pull the list of users who liked a post**
+
+```bash
+truthbrush likes POST TOP_NUM
+```
+
+**Pull trending group tags**
+
+```bash
+truthbrush group-tags
+```
+
+**Pull trending groups**
+
+```bash 
+truthbrush group-trends      
+``` 
+
+**Pull list of suggested groups**
+
+```bash 
+truthbrush group-suggestions
+```
+
 ## Contributing
 
 Contributions are encouraged! For small bug fixes and minor improvements, feel free to just open a PR. For larger changes, please open an issue first so that other contributors can discuss your plan, avoid duplicated work, and ensure it aligns with the goals of the project. Be sure to also follow the [code of conduct](CODE_OF_CONDUCT.md). Thanks!
 
 Development setup (ensure you have [Poetry](https://python-poetry.org/) installed):
 
 ```sh
```

