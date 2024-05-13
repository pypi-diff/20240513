# Comparing `tmp/moveread_dfy-0.1.0.tar.gz` & `tmp/moveread_dfy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_dfy-0.1.0.tar", last modified: Sun May 12 09:38:19 2024, max compression
+gzip compressed data, was "moveread_dfy-0.1.2.tar", last modified: Mon May 13 14:43:47 2024, max compression
```

## Comparing `moveread_dfy-0.1.0.tar` & `moveread_dfy-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1025 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      987 2024-05-12 09:06:02.000000 moveread_dfy-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.025338 moveread_dfy-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.015182 moveread_dfy-0.1.0/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.025338 moveread_dfy-0.1.0/src/moveread/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.0/src/moveread/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.0/src/moveread/dfy/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.025338 moveread_dfy-0.1.0/src/moveread/dfy/doer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.0/src/moveread/dfy/doer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.0/src/moveread/dfy/doer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1396 2024-05-07 17:01:43.000000 moveread_dfy-0.1.0/src/moveread/dfy/doer/_puller.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1199 2024-05-07 18:43:43.000000 moveread_dfy-0.1.0/src/moveread/dfy/doer/_pusher.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      878 2024-05-07 15:45:40.000000 moveread_dfy-0.1.0/src/moveread/dfy/doer/_run_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.025338 moveread_dfy-0.1.0/src/moveread/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.0/src/moveread/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1866 2024-05-07 17:56:09.000000 moveread_dfy-0.1.0/src/moveread/dfy/integrations/core.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/src/moveread/dfy/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.0/src/moveread/dfy/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1489 2024-05-12 09:12:40.000000 moveread_dfy-0.1.0/src/moveread/dfy/scripts/api_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      472 2024-05-08 07:12:54.000000 moveread_dfy-0.1.0/src/moveread/dfy/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.0/src/moveread/dfy/scripts/connect_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2462 2024-05-07 18:15:24.000000 moveread_dfy-0.1.0/src/moveread/dfy/scripts/doer_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/src/moveread/dfy/server/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3225 2024-05-12 09:12:22.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      757 2024-05-11 16:53:30.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/pgns.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4340 2024-05-11 16:56:41.000000 moveread_dfy-0.1.0/src/moveread/dfy/server/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-12 08:53:00.000000 moveread_dfy-0.1.0/src/moveread/dfy/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 09:38:19.035494 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1025 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      233 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-12 09:38:19.000000 moveread_dfy-0.1.0/src/moveread_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-13 14:43:44.000000 moveread_dfy-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/moveread/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.2/src/moveread/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.2/src/moveread/dfy/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/doer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1985 2024-05-12 16:19:17.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_puller.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1297 2024-05-12 14:09:05.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_pusher.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1015 2024-05-12 14:23:00.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_run_connect.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.2/src/moveread/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1866 2024-05-07 17:56:09.000000 moveread_dfy-0.1.2/src/moveread/dfy/integrations/core.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1535 2024-05-12 10:43:00.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/api_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/connect_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3140 2024-05-12 14:35:12.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/doer_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/server/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3316 2024-05-13 12:55:43.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      751 2024-05-12 10:41:22.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/pgns.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4477 2024-05-13 12:52:26.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2437 2024-05-13 12:47:37.000000 moveread_dfy-0.1.2/src/moveread/dfy/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/top_level.txt
```

### Comparing `moveread_dfy-0.1.0/PKG-INFO` & `moveread_dfy-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.0
+Version: 0.1.2
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
@@ -18,16 +18,21 @@
 Provides-Extra: server
 Requires-Dist: pure-cv; extra == "server"
 Requires-Dist: fastapi; extra == "server"
 Requires-Dist: python-multipart; extra == "server"
 Requires-Dist: uvicorn[standard]; extra == "server"
 Requires-Dist: kv-azure-blob; extra == "server"
 Requires-Dist: psycopg2-binary; extra == "server"
+Requires-Dist: dslog; extra == "server"
 Provides-Extra: local
 Requires-Dist: kv-fs; extra == "local"
+Requires-Dist: python-dotenv; extra == "local"
+Requires-Dist: kv-fs; extra == "local"
+Provides-Extra: doer
+Requires-Dist: moveread-pipelines-dfy; extra == "doer"
 Provides-Extra: client
 Provides-Extra: clientgen
 Requires-Dist: openapi-ts; extra == "clientgen"
 
 # Moveread DFY
 
 > Moveread DFY data models and API
```

### Comparing `moveread_dfy-0.1.0/pyproject.toml` & `moveread_dfy-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-dfy"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread DFY data models and API"
 dependencies = [
   "lazy-loader", "pydantic",
   "chess-pairings", "dslog",
@@ -19,16 +19,17 @@
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/moveread-dfy.git"
 
 [project.optional-dependencies]
-server = ["pure-cv", "fastapi", "python-multipart", "uvicorn[standard]", "kv-azure-blob", "psycopg2-binary"]
-local = ["kv-fs"]
+server = ["pure-cv", "fastapi", "python-multipart", "uvicorn[standard]", "kv-azure-blob", "psycopg2-binary", "dslog"]
+local = ["kv-fs", "python-dotenv", "kv-fs"]
+doer = ["moveread-pipelines-dfy"]
 client = []
 clientgen = ["openapi-ts"]
 
 [project.scripts]
 dfy-api = "moveread.dfy.scripts.api_cli:main"
 dfy-clientgen = "moveread.dfy.scripts.clientgen_cli:main"
 dfy-connect = "moveread.dfy.scripts.connect_cli:main"
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/doer/_puller.py` & `moveread_dfy-0.1.2/src/moveread/dfy/doer/_puller.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 from datetime import timedelta
 import asyncio
+from uuid import uuid4
 from sqlalchemy import Engine
 from sqlalchemy.exc import DatabaseError
 from sqlmodel import select, Session
 from haskellian import Left, either as E
 from dslog import Logger
+from kv.api import KV
 from q.api import WriteQueue
 from moveread.pipelines.dfy import Input
+from moveread.pipelines.input_validation import GameId
 from scoresheet_models import ModelID
-from ..types import Game, GameId
+from ..types import Game
+
+def randomId(tournId: str, group: str, round: str, board: str) -> str:
+  return f'{tournId}/{group}/{round}/{board}_{uuid4()}'
 
 async def puller(
   Qin: WriteQueue[Input], engine: Engine, *,
+  online_images: KV[bytes], local_images: KV[bytes],
   tournId: str, model: ModelID, polling_interval: timedelta = timedelta(seconds=30),
   logger = Logger.rich().prefix('[PULLER]')
 ):
   @E.do()
   async def pull_once():
     try:
       with Session(engine) as ses:
-        stmt = select(Game).where(Game.tournId == tournId, Game.status == None)
+        stmt = select(Game).where(Game.tournId == tournId, Game.status == Game.Status.uploaded)
         games = ses.exec(stmt).all()
         for game in games:
-          id = GameId.of(game)
-          task = Input(gameId=id.dict(), model=model, imgs=[img.url for img in game.imgs]) # type: ignore (id's are structurally identical)
+          gameId = GameId(group=game.group, round=game.round, board=game.board)
+          id = randomId(tournId, **gameId)
+          urls = [img.url for img in game.imgs]
+          task = Input(gameId=gameId, model=model, imgs=urls)
+          tasks = [online_images.copy(url, local_images, url).run() for url in urls]
+          results = await asyncio.gather(*tasks)
+          E.sequence(results).unsafe()
+
           logger(f'Inputting new task for "{id}":', task)
-          (await Qin.push(id.stringify(), task)).unsafe()
+          (await Qin.push(id, task)).unsafe()
           game.status = Game.Status.doing
           ses.add(game)
         ses.commit()
+
+
     except DatabaseError as e:
       Left(e).unsafe()
 
+
   while True:
+    logger('Polling', level='DEBUG')
     r = await pull_once()
+    logger('Polled', level='DEBUG')
     if r.tag == 'left':
       logger('Error while pulling', r.value, level='ERROR')
     
     await asyncio.sleep(polling_interval.total_seconds())
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/doer/_pusher.py` & `moveread_dfy-0.1.2/src/moveread/dfy/doer/_pusher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import asyncio
 from sqlalchemy import Engine
 from sqlmodel import select, Session
 from dslog import Logger
 from haskellian import either as E, Left
 from q.api import ReadQueue
 from moveread.pipelines.dfy import Result
-from ..types import Game
+from ..types import Game, PGN
+
+def exact_game(tournId: str, group: str, round: str, board: str):
+  return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
 
 async def pusher(
   Qout: ReadQueue[Result], engine: Engine, *,
   tournId: str,
   logger = Logger.rich().prefix('[DFY PUSHER]')
 ):
   
   @E.do()
   async def push_one():
     id, result = (await Qout.read()).unsafe()
     gid = result.gameId
     logger(f'Pushing result for {gid}')
     try:
       with Session(engine) as ses:
-        stmt = select(Game).where(Game.tournId == tournId, Game.group == gid.group, Game.round == gid.round, Game.board == gid.board)
+        stmt = select(Game).where(*exact_game(tournId, **gid))
         game = ses.exec(stmt).first()
         if game is None:
           logger(f'Game not found: {gid}', level='ERROR')
           return
 
-        game.pgn = ' '.join(result.pgn)
+        game.pgn = PGN(moves=result.pgn)
         game.status = Game.Status.done
         ses.add(game)
         ses.commit()
     except Exception as e:
       Left(e).unsafe()
 
     (await Qout.pop(id)).unsafe()
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/doer/_run_connect.py` & `moveread_dfy-0.1.2/src/moveread/dfy/doer/_run_connect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import asyncio
 from datetime import timedelta
 from sqlmodel import SQLModel
 from sqlalchemy import Engine
 from dslog import Logger
 from haskellian import promise as P
+from kv.api import KV
 from q.api import ReadQueue, WriteQueue
 from scoresheet_models import ModelID
 from moveread.pipelines.dfy import Input, Result
 from ._puller import puller
 from ._pusher import pusher
 
 @P.run
 async def run_connect(
   Qin: WriteQueue[Input], Qout: ReadQueue[Result], *,
   engine: Engine, tournId: str, model: ModelID,
+  local_images: KV[bytes], online_images: KV[bytes],
   logger = Logger.rich().prefix('[DFY]'),
   polling_interval = timedelta(seconds=30)
 ):
   
   SQLModel.metadata.create_all(engine)
 
   tasks = (
     puller(
       Qin, engine, tournId=tournId, polling_interval=polling_interval,
-      model=model, logger=logger.prefix('[PULLER]')
+      model=model, logger=logger.prefix('[PULLER]'),
+      online_images=online_images, local_images=local_images
     ),
     pusher(Qout, engine, tournId=tournId, logger=logger.prefix('[PUSHER]'))
   )
   await asyncio.gather(*tasks)
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/integrations/core.py` & `moveread_dfy-0.1.2/src/moveread/dfy/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/scripts/api_cli.py` & `moveread_dfy-0.1.2/src/moveread/dfy/scripts/api_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 
   parser.add_argument('-p', '--port', default=8000, type=int)
   parser.add_argument('--host', default='0.0.0.0', type=str)
 
 
   args = parser.parse_args()
   db = args.db
-  print(f'Running API...')
-  print(f'- DB URL: "{db}"')
+
+  from dslog import Logger, formatters
+  logger = Logger.stderr().format(formatters.click)
+
+  logger(f'Running API...')
+  logger(f'- DB URL: "{db}"')
 
   if args.images:
     images_path = os.path.join(os.getcwd(), args.images)
-    print(f'- Images path: "{images_path}"')
+    logger(f'- Images path: "{images_path}"')
     from kv.fs import FilesystemKV
     images = FilesystemKV[bytes](images_path)
   else:
     images_path = None
     from kv.azure.blob import BlobKV
     images = BlobKV[bytes].from_conn_str(args.blobs)
-    print(f'- Azure Blob account: {images.client.account_name}')
+    logger(f'- Azure Blob account: {images.client.account_name}')
 
   from sqlalchemy import create_engine
   from moveread.dfy import run_api
   engine = create_engine(db)
-  run_api(images, engine, images_path=images_path, port=args.port, host=args.host)  
+  run_api(images, engine, images_path=images_path, port=args.port, host=args.host, logger=logger)
 
 if __name__ == '__main__':
   import sys
   from dotenv import load_dotenv
   load_dotenv()
-  os.chdir('/home/m4rs/mr-github/modes/dfy/moveread-dfy/local')
   SQL_CONN_STR = os.environ['SQL_CONN_STR']
   BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
   sys.argv.extend(f'--blobs {BLOB_CONN_STR} --db {SQL_CONN_STR}'.split(' '))
   main()
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/scripts/connect_cli.py` & `moveread_dfy-0.1.2/src/moveread/dfy/scripts/connect_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/scripts/doer_cli.py` & `moveread_dfy-0.1.2/src/moveread/dfy/scripts/doer_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,61 +2,89 @@
 from argparse import ArgumentParser
 
 def main():
   parser = ArgumentParser()
   parser.add_argument('-i', '--input', required=True)
   parser.add_argument('-o', '--output', required=True)
   parser.add_argument('-b', '--base-path', required=True)
-  parser.add_argument('-d', '--database', required=True, help='Database URL')
+  parser.add_argument('-d', '--db', required=True, help='Database URL')
   parser.add_argument('-t', '--tournament', required=True, help='Tournament ID')
   parser.add_argument('-m', '--model', required=True, choices=MODEL_IDS, help='Model ID')
-  parser.add_argument('--images', required=True)
   parser.add_argument('--protocol', default='sqlite', required=False, choices=['sqlite', 'fs'], help='Protocol used in queues')
+  parser.add_argument('--images', type=str, help='Local path to images')
+  parser.add_argument('--blobs', type=str, help='Azure Blob connection string')
 
   args = parser.parse_args()
 
 
   import os
   from dslog import Logger
   input_path = os.path.join(os.getcwd(), args.input)
   output_path = os.path.join(os.getcwd(), args.output)
   base_path = os.path.join(os.getcwd(), args.base_path)
-  images_path = os.path.join(os.getcwd(), args.images)
   proto = args.protocol
-  db_url = args.database
+  db_url = args.db
   tournId = args.tournament
+  images_path = os.path.join(os.getcwd(), args.images)
   
   logger = Logger.click().prefix('[DFY]')
   logger(f'Running...')
   logger(f'- Tournament ID: "{tournId}"')
   logger(f'- Database URL: "{db_url}"')
   logger(f'- Images path: "{images_path}"')
+
+  
   logger(f'- Queues protocol: "{proto}"')
   logger(f'- Input path: "{input_path}"')
   logger(f'- Internal path: "{base_path}"')
   logger(f'- Output path: "{output_path}"')
   
-  from kv.fs import FilesystemKV
+  from kv.azure.blob import BlobKV
+  online_images = BlobKV[bytes].from_conn_str(args.blobs)
+  
+  logger(f'- Azure Blob account: {online_images.client.account_name}')
+  
   from sqlmodel import create_engine
   from moveread.dfy import run_connect
   from moveread.pipelines.dfy import run_local, input_queue, output_queue
   from multiprocessing import Process
+  from kv.fs import FilesystemKV
+  local_images = FilesystemKV[bytes](images_path)
 
   Qin = input_queue(input_path, protocol=proto)
   Qout = output_queue(output_path, protocol=proto)
   engine = create_engine(db_url)
-  images = FilesystemKV[bytes](images_path)
   ps = (
-    Process(target=run_connect, args=(Qin, Qout), kwargs=dict(engine=engine, tournId=tournId, logger=logger.prefix('[I/O]'), model=args.model)),
-    Process(target=run_local, args=(Qin, Qout), kwargs=dict(base_path=base_path, images=images, images_path=images_path, logger=logger)),
+    Process(
+      target=run_connect, args=(Qin, Qout), kwargs=dict(
+        engine=engine, tournId=tournId, logger=logger.prefix('[I/O]'), model=args.model,
+        local_images=local_images, online_images=online_images
+      )
+    ),
+    Process(
+      target=run_local, args=(Qin, Qout), kwargs=dict(
+        base_path=base_path, images=local_images,
+        images_path=images_path, logger=logger
+      )
+    ),
   )
   for p in ps:
     p.start()
   for p in ps:
     p.join()
 
 if __name__ == '__main__':
   import sys
   import os
-  os.chdir('/home/m4rs/mr-github/modes/dfy/moveread-dfy/')
-  sys.argv.extend('-b test/internal -i test/in -o test/out -d sqlite:///db.sqlite -t llobregat -m llobregat23 --images test/images'.split(' '))
+  from dotenv import load_dotenv
+  os.chdir('/home/m4rs/mr-github/modes/moveread-dfy/infra/doer')
+  load_dotenv()
+  SQL_CONN_STR = os.environ['SQL_CONN_STR']
+  BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
+  args = f'-i queues/in -o queues/out -b queues/internal \
+      -t llobregat23 -m llobregat23 \
+      --db {SQL_CONN_STR} \
+      --blobs {BLOB_CONN_STR} \
+      --images images'.replace('\n', '').split(' ')
+  args = [arg for arg in args if arg]
+  sys.argv.extend(args)
   main()
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/server/api.py` & `moveread_dfy-0.1.2/src/moveread/dfy/server/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     app.mount('/images', StaticFiles(directory=images_path))
 
   @app.get('/authorize/{tournId}')
   def authorize(token: str, tournId: str, r: Response) -> bool:
     authed = sdk.authorize(token, tournId)
     return authed
 
+  @app.get('/')
+  def tournaments() -> Sequence[Tournament]:
+    return sdk.tournaments()
+
   @app.get('/{tournId}')
   def tournament(tournId: str) -> Tournament | None:
     return sdk.tournament(tournId)
   
   @app.get('/{tournId}/{group}')
   def group(tournId: str, group: str) -> Group | None:
     return sdk.group(tournId, group)
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/server/main.py` & `moveread_dfy-0.1.2/src/moveread/dfy/server/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/server/pgns.py` & `moveread_dfy-0.1.2/src/moveread/dfy/server/pgns.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,14 @@
   pair = game.pairing.root
   if game.pgn is None or pair.tag == 'unpaired':
     return None
   site = tnmt and tnmt.site
   event = tnmt and tnmt.name
   headers = PGNHeaders(
     Event=event, Site=site, White=pair.white, Black=pair.black,
-    Round=f'{game.round}.{game.board}', Result=pair.result or '*'
+    Round=f'{game.round}.{game.board}', Result=pair.result,
   )
   comment = '[...]' if game.pgn.early else None
   return export_pgn(game.pgn.moves, headers, comment)
 
 def export_all(games: Iterable[Game], tnmt: Tournament | None = None) -> str:
   return '\n\n'.join(pgn for game in games if (pgn := export(game, tnmt)) is not None)
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/server/sdk.py` & `moveread_dfy-0.1.2/src/moveread/dfy/server/sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     self._engine = engine
 
   def authorize(self, token: str, tournId: str) -> bool:
     with Session(self._engine) as ses:
       results = ses.exec(select(Token).where(Token.token == token, Token.tournId == tournId))
       return results.first() is not None
 
+  def tournaments(self) -> Sequence[Tournament]:
+    with Session(self._engine) as ses:
+      return ses.exec(select(Tournament)).all()
+
   def tournament(self, tournId: str) -> Tournament | None:
     with Session(self._engine) as ses:
       return ses.exec(select_tnmt(tournId)).first()
     
   def group(self, tournId: str, group: str) -> Group | None:
     with Session(self._engine) as ses:
       return ses.exec(select(Group).where(Group.tournId == tournId, Group.name == group)).first()
```

### Comparing `moveread_dfy-0.1.0/src/moveread/dfy/types.py` & `moveread_dfy-0.1.2/src/moveread/dfy/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import Sequence, TypedDict
 from enum import StrEnum
+from datetime import date
 from pydantic import RootModel, Field as PydanticField
 from sqlmodel import Field, SQLModel, Relationship
 from sqltypes import SpaceDelimitedList, PydanticModel
 from chess_pairings import Paired, Unpaired
 
 class Pairing(RootModel):
   root: Paired | Unpaired = PydanticField(discriminator='tag')
 
 class Tournament(SQLModel, table=True):
   tournId: str = Field(primary_key=True)
   name: str
   site: str | None = None
+  start_date: date | None = None
+  end_date: date | None = None
   groups: Sequence[str] = Field(sa_type=SpaceDelimitedList)
 
 class Group(SQLModel, table=True):
   tournId: str = Field(primary_key=True, foreign_key='tournament.tournId')
   name: str = Field(primary_key=True)
   rounds: Sequence[str] = Field(sa_type=SpaceDelimitedList)
```

### Comparing `moveread_dfy-0.1.0/src/moveread_dfy.egg-info/PKG-INFO` & `moveread_dfy-0.1.2/src/moveread_dfy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.0
+Version: 0.1.2
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
@@ -18,16 +18,21 @@
 Provides-Extra: server
 Requires-Dist: pure-cv; extra == "server"
 Requires-Dist: fastapi; extra == "server"
 Requires-Dist: python-multipart; extra == "server"
 Requires-Dist: uvicorn[standard]; extra == "server"
 Requires-Dist: kv-azure-blob; extra == "server"
 Requires-Dist: psycopg2-binary; extra == "server"
+Requires-Dist: dslog; extra == "server"
 Provides-Extra: local
 Requires-Dist: kv-fs; extra == "local"
+Requires-Dist: python-dotenv; extra == "local"
+Requires-Dist: kv-fs; extra == "local"
+Provides-Extra: doer
+Requires-Dist: moveread-pipelines-dfy; extra == "doer"
 Provides-Extra: client
 Provides-Extra: clientgen
 Requires-Dist: openapi-ts; extra == "clientgen"
 
 # Moveread DFY
 
 > Moveread DFY data models and API
```

### Comparing `moveread_dfy-0.1.0/src/moveread_dfy.egg-info/SOURCES.txt` & `moveread_dfy-0.1.2/src/moveread_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

