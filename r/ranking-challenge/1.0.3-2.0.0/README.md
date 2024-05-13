# Comparing `tmp/ranking_challenge-1.0.3.tar.gz` & `tmp/ranking_challenge-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ranking_challenge-1.0.3.tar", last modified: Tue May  7 16:55:00 2024, max compression
+gzip compressed data, was "ranking_challenge-2.0.0.tar", last modified: Mon May 13 21:13:56 2024, max compression
```

## Comparing `ranking_challenge-1.0.3.tar` & `ranking_challenge-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-07 16:55:00.741468 ranking_challenge-1.0.3/
--rw-r--r--   0 raindrift   (501) staff       (20)     1137 2024-05-07 08:57:49.000000 ranking_challenge-1.0.3/LICENSE
--rw-r--r--   0 raindrift   (501) staff       (20)     4978 2024-05-07 16:55:00.741273 ranking_challenge-1.0.3/PKG-INFO
--rw-r--r--   0 raindrift   (501) staff       (20)     2503 2024-05-07 08:38:28.000000 ranking_challenge-1.0.3/README.md
--rw-r--r--   0 raindrift   (501) staff       (20)     1221 2024-05-07 16:54:39.000000 ranking_challenge-1.0.3/pyproject.toml
--rw-r--r--   0 raindrift   (501) staff       (20)       38 2024-05-07 16:55:00.741509 ranking_challenge-1.0.3/setup.cfg
-drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-07 16:55:00.738553 ranking_challenge-1.0.3/src/
--rw-r--r--   0 raindrift   (501) staff       (20)        0 2024-05-07 16:51:45.000000 ranking_challenge-1.0.3/src/__init__.py
-drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-07 16:55:00.739796 ranking_challenge-1.0.3/src/ranking_challenge/
--rw-r--r--   0 raindrift   (501) staff       (20)        0 2024-05-07 08:39:40.000000 ranking_challenge-1.0.3/src/ranking_challenge/__init__.py
--rw-r--r--   0 raindrift   (501) staff       (20)     3743 2024-05-07 16:54:05.000000 ranking_challenge-1.0.3/src/ranking_challenge/fake.py
--rw-r--r--   0 raindrift   (501) staff       (20)     1186 2024-05-07 16:21:10.000000 ranking_challenge-1.0.3/src/ranking_challenge/fake_test.py
--rw-r--r--   0 raindrift   (501) staff       (20)     4491 2024-05-07 08:39:40.000000 ranking_challenge-1.0.3/src/ranking_challenge/request.py
--rw-r--r--   0 raindrift   (501) staff       (20)      775 2024-05-07 08:39:40.000000 ranking_challenge-1.0.3/src/ranking_challenge/response.py
--rw-r--r--   0 raindrift   (501) staff       (20)     4335 2024-05-07 08:39:40.000000 ranking_challenge-1.0.3/src/ranking_challenge/survey.py
-drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-07 16:55:00.740889 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/
--rw-r--r--   0 raindrift   (501) staff       (20)     4978 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/PKG-INFO
--rw-r--r--   0 raindrift   (501) staff       (20)      518 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 raindrift   (501) staff       (20)        1 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 raindrift   (501) staff       (20)       56 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/entry_points.txt
--rw-r--r--   0 raindrift   (501) staff       (20)       58 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/requires.txt
--rw-r--r--   0 raindrift   (501) staff       (20)       27 2024-05-07 16:55:00.000000 ranking_challenge-1.0.3/src/ranking_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-13 21:13:56.348060 ranking_challenge-2.0.0/
+-rw-r--r--   0 raindrift   (501) staff       (20)     1137 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/LICENSE
+-rw-r--r--   0 raindrift   (501) staff       (20)     4978 2024-05-13 21:13:56.347852 ranking_challenge-2.0.0/PKG-INFO
+-rw-r--r--   0 raindrift   (501) staff       (20)     2503 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/README.md
+-rw-r--r--   0 raindrift   (501) staff       (20)     1221 2024-05-13 20:39:21.000000 ranking_challenge-2.0.0/pyproject.toml
+-rw-r--r--   0 raindrift   (501) staff       (20)       38 2024-05-13 21:13:56.348097 ranking_challenge-2.0.0/setup.cfg
+drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-13 21:13:56.345272 ranking_challenge-2.0.0/src/
+-rw-r--r--   0 raindrift   (501) staff       (20)        0 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/src/__init__.py
+drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-13 21:13:56.346558 ranking_challenge-2.0.0/src/ranking_challenge/
+-rw-r--r--   0 raindrift   (501) staff       (20)        0 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/src/ranking_challenge/__init__.py
+-rw-r--r--   0 raindrift   (501) staff       (20)     4071 2024-05-13 21:08:53.000000 ranking_challenge-2.0.0/src/ranking_challenge/fake.py
+-rw-r--r--   0 raindrift   (501) staff       (20)     1186 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/src/ranking_challenge/fake_test.py
+-rw-r--r--   0 raindrift   (501) staff       (20)     4886 2024-05-13 21:10:41.000000 ranking_challenge-2.0.0/src/ranking_challenge/request.py
+-rw-r--r--   0 raindrift   (501) staff       (20)      775 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/src/ranking_challenge/response.py
+-rw-r--r--   0 raindrift   (501) staff       (20)     4335 2024-05-07 21:49:31.000000 ranking_challenge-2.0.0/src/ranking_challenge/survey.py
+drwxr-xr-x   0 raindrift   (501) staff       (20)        0 2024-05-13 21:13:56.347418 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/
+-rw-r--r--   0 raindrift   (501) staff       (20)     4978 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 raindrift   (501) staff       (20)      518 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 raindrift   (501) staff       (20)        1 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 raindrift   (501) staff       (20)       56 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/entry_points.txt
+-rw-r--r--   0 raindrift   (501) staff       (20)       58 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/requires.txt
+-rw-r--r--   0 raindrift   (501) staff       (20)       27 2024-05-13 21:13:56.000000 ranking_challenge-2.0.0/src/ranking_challenge.egg-info/top_level.txt
```

### Comparing `ranking_challenge-1.0.3/LICENSE` & `ranking_challenge-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ranking_challenge-1.0.3/PKG-INFO` & `ranking_challenge-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranking_challenge
-Version: 1.0.3
+Version: 2.0.0
 Summary: The Prosocial Ranking Challenge
 Author-email: Ian Baker <ian@sonic.net>
 License: Prosocial Ranking Challenge
         
         The MIT License (MIT)
         
         Copyright (c) 2024 Center for Human-Compatible AI and others
```

### Comparing `ranking_challenge-1.0.3/README.md` & `ranking_challenge-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ranking_challenge-1.0.3/pyproject.toml` & `ranking_challenge-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ranking_challenge"
-version = "1.0.3"
+version = "2.0.0"
 description = "The Prosocial Ranking Challenge"
 readme = "README.md"
 authors = [{ name = "Ian Baker", email = "ian@sonic.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Framework :: Pydantic :: 2",
```

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge/fake.py` & `ranking_challenge-2.0.0/src/ranking_challenge/fake.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 fake = Faker(locale="la")  # remove locale to get rid of the fake latin
 
 from ranking_challenge.request import ContentItem, RankingRequest, Session
 from ranking_challenge.response import RankingResponse
 from ranking_challenge.survey import SurveyResponse
 
 
+URI_PATHS = {
+    "reddit": ["", "r/aww", "r/politics", "r/programming", "r/technology"],
+    "twitter": ["", "jack", "TiredActor", "horse_ebooks"],
+    "facebook": ["", "photo", "groups"],
+}
+
 def fake_request(n_posts=1, n_comments=0, platform="reddit"):
     posts = [fake_item(platform=platform, type="post") for _ in range(n_posts)]
     comments = []
     for post in posts:
         last_comment_id = None
         for _ in range(n_comments):
             comments.append(
@@ -27,14 +33,16 @@
                 )
             )
             last_comment_id = comments[-1].id
 
     return RankingRequest(
         session=Session(
             user_id=str(uuid4()),
+            session_id=str(uuid4()),
+            url=f"https://{platform}.com/{fake.random_element(URI_PATHS[platform])}",
             user_name_hash=hashlib.sha256(fake.name().encode()).hexdigest(),
             cohort="AB",
             platform=platform,
             current_time=time.time(),
         ),
         survey=SurveyResponse(
             party_id="democrat",
@@ -107,20 +115,22 @@
 
 def fake_new_item():
     return {
         "id": str(uuid4()),
         "url": fake.url(),
     }
 
+
 # if run from command line
 def main():
     request = fake_request(n_posts=1, n_comments=2)
     print("Request:")
     print(request.model_dump_json(indent=2))
 
     # use ids from request
     response = fake_response([item.id for item in request.items], 2)
     print("\nResponse:")
     print(response.model_dump_json(indent=2))
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge/fake_test.py` & `ranking_challenge-2.0.0/src/ranking_challenge/fake_test.py`

 * *Files identical despite different names*

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge/request.py` & `ranking_challenge-2.0.0/src/ranking_challenge/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,27 +83,32 @@
     engagements: Union[TwitterEngagements, RedditEngagements, FacebookEngagements] = (
         Field(description="Engagement counts for the content item.")
     )
 
 
 class Session(BaseModel):
     """Data that is scoped to the user's browsing session (generally a single page view)"""
-
+    session_id: str = Field(
+        description="A unique ID for this page view, updated on navigation events. Use this to determine if two requests came from the same page."
+    )
     user_id: str = Field(
         description="A unique id for this study participant. Will remain fixed for the duration of the experiment."
     )
     user_name_hash: str = Field(
         description="A (salted) hash of the user's username. We'll do our best to make it match the `item.author_name_hash` on posts authored by the current user."
     )
     cohort: str = Field(
         description="The cohort to which the user has been assigned. You can safely ignore this. It is used by the PRC request router."
     )
     platform: Literal["twitter", "reddit", "facebook"] = Field(
         description="The platform on which the user is viewing content."
     )
+    url: HttpUrl = Field(
+        description="The URL of the page that the user is viewing, minus the query string portion. This can help you to determine which part of the application the user is in."
+    )
     current_time: datetime = Field(
         description="The current time according to the user's browser, in UTC, in `YYYY-MM-DD hh:mm:ss` format."
     )
 
 
 class RankingRequest(BaseModel):
     """A complete ranking request"""
```

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge/response.py` & `ranking_challenge-2.0.0/src/ranking_challenge/response.py`

 * *Files identical despite different names*

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge/survey.py` & `ranking_challenge-2.0.0/src/ranking_challenge/survey.py`

 * *Files identical despite different names*

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge.egg-info/PKG-INFO` & `ranking_challenge-2.0.0/src/ranking_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranking_challenge
-Version: 1.0.3
+Version: 2.0.0
 Summary: The Prosocial Ranking Challenge
 Author-email: Ian Baker <ian@sonic.net>
 License: Prosocial Ranking Challenge
         
         The MIT License (MIT)
         
         Copyright (c) 2024 Center for Human-Compatible AI and others
```

### Comparing `ranking_challenge-1.0.3/src/ranking_challenge.egg-info/SOURCES.txt` & `ranking_challenge-2.0.0/src/ranking_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

