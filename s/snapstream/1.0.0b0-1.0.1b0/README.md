# Comparing `tmp/snapstream-1.0.0b0.tar.gz` & `tmp/snapstream-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-1.0.0b0.tar", max compression
+gzip compressed data, was "snapstream-1.0.1b0.tar", max compression
```

## Comparing `snapstream-1.0.0b0.tar` & `snapstream-1.0.1b0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-03-22 22:36:56.125909 snapstream-1.0.0b0/LICENSE
--rw-r--r--   0        0        0     2536 2024-03-22 22:36:56.125909 snapstream-1.0.0b0/README.md
--rw-r--r--   0        0        0     2039 2024-03-22 22:37:07.985930 snapstream-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     2280 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/__init__.py
--rw-r--r--   0        0        0     8333 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/__main__.py
--rw-r--r--   0        0        0    10462 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/caching.py
--rw-r--r--   0        0        0     2889 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/codecs.py
--rw-r--r--   0        0        0    11072 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/core.py
--rw-r--r--   0        0        0     3623 2024-03-22 22:36:56.133909 snapstream-1.0.0b0/snapstream/utils.py
--rw-r--r--   0        0        0     4201 1970-01-01 00:00:00.000000 snapstream-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-13 14:01:12.185822 snapstream-1.0.1b0/LICENSE
+-rw-r--r--   0        0        0     2536 2024-05-13 14:01:12.189822 snapstream-1.0.1b0/README.md
+-rw-r--r--   0        0        0     2033 2024-05-13 14:01:26.405852 snapstream-1.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     2280 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/__init__.py
+-rw-r--r--   0        0        0     8347 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/__main__.py
+-rw-r--r--   0        0        0    10445 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/caching.py
+-rw-r--r--   0        0        0     2889 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/codecs.py
+-rw-r--r--   0        0        0    11259 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/core.py
+-rw-r--r--   0        0        0     3623 2024-05-13 14:01:12.193822 snapstream-1.0.1b0/snapstream/utils.py
+-rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 snapstream-1.0.1b0/PKG-INFO
```

### Comparing `snapstream-1.0.0b0/LICENSE` & `snapstream-1.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0b0/README.md` & `snapstream-1.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0b0/pyproject.toml` & `snapstream-1.0.1b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "1.0.0-beta"
+version = "1.0.1-beta"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
@@ -27,32 +27,31 @@
 [tool.poetry.dependencies]
 python = "^3.8.1"
 confluent-kafka = "^2.0.2"
 rocksdict = "^0.3.10"
 pypubsub = "^4.0.3"
 avro = "^1.11.1"
 toolz = "^0.12.0"
-pyright = "^1.1.302"
 
 [tool.poetry.group.dev.dependencies]
-pydocstyle = "^6.3.0"
-autopep8 = "^2.0.2"
-pyright = "^1.1.300"
-flake8 = "^6.0.0"
-bandit = "^1.7.5"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
-pre-commit = "^3.2.1"
-ipykernel = "^6.22.0"
-sphinx = "^6.2.1"
-sphinx-rtd-theme = "^1.2.0"
-sphinx-autoapi = "^2.1.0"
-sphinx-autobuild = "^2021.3.14"
-testcontainers = {extras = ["kafka"], version = "^3.7.1"}
+pydocstyle = ">=6.3.0"
+autopep8 = ">=2.0.2"
+pyright = ">=1.1.300"
+flake8 = ">=6.0.0"
+bandit = ">=1.7.5"
+pytest = ">=7.2.2"
+pytest-cov = ">=4.0.0"
+pytest-mock = ">=3.10.0"
+pre-commit = ">=3.2.1"
+ipykernel = ">=6.22.0"
+sphinx = ">=6.2.1"
+sphinx-rtd-theme = ">=1.2.0"
+sphinx-autoapi = ">=2.1.0"
+sphinx-autobuild = ">=2021.3.14"
+testcontainers = {extras = ["kafka"], version = ">=3.7.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["snapstream"]
```

### Comparing `snapstream-1.0.0b0/snapstream/__init__.py` & `snapstream-1.0.1b0/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0b0/snapstream/__main__.py` & `snapstream-1.0.1b0/snapstream/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,32 +187,32 @@
     """Read records from cache."""
     if not path.isdir(args.path):
         raise OSError(f'Folder doesn\'t exist: {args.path}')
     cache = Cache(
         args.path,
         access_type=AccessType.read_only(),
     )
+    if args.stats:
+        print()
+        print('Statistics:')
+        print(dumps(cache.live_files(), indent=4))
+        print('Folder size:', folder_size(args.path + '/**/*', 'mb'), 'mb')
+        return
     key_filter = curry(regex_filter)(args.key_filter)
     val_filter = curry(regex_filter)(args.val_filter)
     for key, val in cache.items():
         if key_filter(str(key)) and val_filter(str(val)):
             if args.columns and not isinstance(val, dict):
                 raise ValueError(f'Columns could not be extracted from {type(val)}: {val}')
             print()
             print('>>> key:', key)
             print(val) if not args.columns else print({
                 k: v for k, v in val.items() if k in args.columns.split(',')
             })
 
-    if args.stats:
-        print()
-        print('Statistics:')
-        print(dumps(cache.live_files(), indent=4))
-        print('Folder size:', folder_size(args.path + '/**/*', 'mb'), 'mb')
-
 
 def main():
     """Run main program."""
     args = get_args()
     try:
         # Construct config path
         config_path = path.join(
```

### Comparing `snapstream-1.0.0b0/snapstream/caching.py` & `snapstream-1.0.1b0/snapstream/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     def transaction(self, key) -> Any:
         """Lock the db entry while using the context manager."""
         with self._get_lock(key):
             yield self
 
     def get(
         self,
-        key: Union[str, int, float, bytes, bool, List[str], List[int], List[float], List[bytes], List[bool]],
+        key: Union[str, int, float, bytes, bool, List[Union[str, int, float, bytes, bool]]],
         default: Any = None,
         read_opt: Union[ReadOptions, None] = None
     ) -> Optional[Any]:
         """Get item from database by key."""
         return self.db.get(key, default, read_opt)
 
     def put(
```

### Comparing `snapstream-1.0.0b0/snapstream/codecs.py` & `snapstream-1.0.1b0/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0b0/snapstream/core.py` & `snapstream-1.0.1b0/snapstream/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Callable,
     Dict,
     Iterable,
     Iterator,
     Optional,
     Set,
     Tuple,
+    cast,
 )
 
 from confluent_kafka import Consumer, Producer
 from confluent_kafka.admin import AdminClient, NewTopic
 from confluent_kafka.error import KafkaException
 from pubsub import pub
 from toolz import pipe
@@ -148,21 +149,15 @@
         - Should serialize using topic codec.
         - Should skip sending message when dry is True.
         - Should show a warning when skipped.
         """
         raise NotImplementedError
 
 
-def _consumer_handler(c, conf, poll_timeout, codec, raise_error):
-    manual_commit = pipe(
-        conf.get('enable.auto.commit'),
-        str,
-        str.lower
-    ) == 'false'
-
+def _consumer_handler(c, poll_timeout, codec, raise_error, commit_each_message):
     while True:
         msg = c.poll(poll_timeout)
         if msg is None:
             continue
         if err := msg.error():
             if raise_error or err.fatal() or not err.retriable():
                 raise KafkaException(err)
@@ -171,49 +166,18 @@
                 continue
         if codec:
             decoded_val = codec.decode(msg.value())
             msg.set_value(decoded_val)
 
         yield msg
 
-        if manual_commit:
+        if commit_each_message:
             c.commit()
 
 
-@contextmanager
-def get_consumer(
-    topic: str,
-    conf: dict,
-    offset=None,
-    codec: Optional[ICodec] = None,
-    poll_timeout: float = 1.0,
-    poller=_consumer_handler,
-    raise_error=False
-) -> Iterator[Iterable[Any]]:
-    """Yield an iterable to consume from kafka."""
-    c = Consumer(conf, logger=logger)
-
-    def consume():
-        def on_assign(c, ps):
-            for p in ps:
-                if offset is not None:
-                    p.offset = offset
-            c.assign(ps)
-
-        logger.debug(f'Subscribing to topic: {topic}.')
-        c.subscribe([topic], on_assign=on_assign)
-        logger.debug(f'Consuming from topic: {topic}.')
-        yield from poller(c, conf, poll_timeout, codec, raise_error)
-
-    try:
-        yield consume()
-    finally:
-        c.close()
-
-
 def _producer_handler(p, topic, poll_timeout, codec, dry):
     def callback(err, msg):
         if err is not None:
             logger.error(f'Failed to deliver message: {err}.')
             # Raise exception by default
             raise KafkaException(err)
         else:
@@ -227,31 +191,14 @@
             logger.warning(f'Skipped sending message to {topic} [dry=True].')
             return
         p.produce(topic=topic, key=key, value=val, *args, **kwargs, callback=callback)
         p.poll(poll_timeout)
     return produce
 
 
-@contextmanager
-def get_producer(
-    topic: str,
-    conf: dict,
-    dry=False,
-    codec: Optional[ICodec] = None,
-    poll_timeout: float = 1.0,
-    flush_timeout: float = -1.0,
-    pusher=_producer_handler
-) -> Iterator[Callable[[Any, Any], None]]:
-    """Yield kafka produce method."""
-    p = Producer(conf, logger=logger)
-    yield pusher(p, topic, poll_timeout, codec, dry)
-    logger.debug(f'Flushing messages to kafka, flush_timeout={flush_timeout}.')
-    p.flush(flush_timeout)
-
-
 class Topic(ITopic):
     """Act as a consumer and producer.
 
     >>> topic = Topic('emoji', {
     ...     'bootstrap.servers': 'localhost:29091',
     ...     'auto.offset.reset': 'earliest',
     ...     'group.id': 'demo',
@@ -274,31 +221,34 @@
         offset: Optional[int] = None,
         codec: Optional[ICodec] = None,
         flush_timeout: float = -1.0,
         poll_timeout: float = 1.0,
         pusher=_producer_handler,
         poller=_consumer_handler,
         dry: bool = False,
-        raise_error: bool = False
+        raise_error: bool = False,
+        commit_each_message: bool = False
     ) -> None:
         """Pass topic related configuration."""
         c = Conf()
         self.name = name
         self.conf = {**c.conf, **conf}
         self.starting_offset = offset
         self.flush_timeout = flush_timeout
         self.poll_timeout = poll_timeout
-        self.consumer = None
-        self.producer = None
-        self._producer_ctx = None
+        self._consumer = None
+        self._producer = None
+        self._producer_callable = None
+        self._producer_ctx_mgr = None
         self.pusher = pusher
         self.poller = poller
         self.codec = codec
         self.dry = dry
         self.raise_error = raise_error
+        self.commit_each_message = commit_each_message
 
     def admin(self):
         """Get admin client."""
         return AdminClient(self.conf)
 
     def create_topic(self, *args, **kwargs) -> None:
         """Create topic."""
@@ -310,60 +260,95 @@
             except KafkaException as e:
                 if "TOPIC_ALREADY_EXISTS" in str(e):
                     logger.warning(e)
                 else:
                     logger.error(e)
                     raise
 
+    @contextmanager
+    def _get_consumer(self) -> Iterator[Iterable[Any]]:
+        """Yield an iterable to consume from kafka."""
+        self._consumer = Consumer(self.conf, logger=logger)
+        commit_each_message = pipe(
+            self.conf.get('enable.auto.commit'),
+            str,
+            str.lower
+        ) == 'false' and self.commit_each_message
+
+        def consume():
+            def on_assign(c, ps):
+                for p in ps:
+                    if self.starting_offset is not None:
+                        p.offset = self.starting_offset
+                c.assign(ps)
+
+            logger.debug(f'Subscribing to topic: {self.name}.')
+            cast(Consumer, self._consumer).subscribe([self.name], on_assign=on_assign)
+            logger.debug(f'Consuming from topic: {self.name}.')
+            yield from self.poller(self._consumer, self.poll_timeout, self.codec,
+                                   self.raise_error, commit_each_message)
+        yield consume()
+        leave_msg = (
+            'Leaving group'
+            if commit_each_message
+            else 'Committing offsets and leaving group'
+        )
+        logger.debug(f'{leave_msg}, flush_timeout={self.flush_timeout}.')
+        self._consumer.close()
+
+    @contextmanager
+    def _get_producer(self) -> Iterator[Callable[[Any, Any], None]]:
+        """Yield kafka produce method."""
+        self._producer = self._producer or Producer(self.conf, logger=logger)
+        yield self.pusher(self._producer, self.name, self.poll_timeout, self.codec, self.dry)
+        logger.debug(f'Flushing messages to kafka, flush_timeout={self.flush_timeout}.')
+        self._producer.flush(self.flush_timeout)
+
     def __iter__(self) -> Iterator[Any]:
         """Consume from topic."""
-        c = get_consumer(self.name, self.conf, self.starting_offset, self.codec,
-                         self.poll_timeout, self.poller, self.raise_error)
+        c = self._get_consumer()
         with c as consumer:
             for msg in consumer:
                 yield msg
 
     def __next__(self) -> Any:
         """Consume next message from topic."""
-        self.consumer = self.consumer or self.__iter__()
-        return next(self.consumer)
+        c = self._get_consumer()
+        with c as consumer:
+            for msg in consumer:
+                return msg
 
     def __getitem__(self, i) -> Any:
         """Consume specific range of messages from topic."""
         if not isinstance(i, (slice, int)):
             raise TypeError('Expected slice or int.')
         start, step, stop = (
             i,
             None,
             i + 1 if i >= 0 else None
         ) if isinstance(i, int) else (
             i.start,
             i.step,
             i.stop
         )
-        c = get_consumer(self.name, self.conf, start, self.codec,
-                         self.poll_timeout, self.poller, self.raise_error)
+        c = self._get_consumer()
         with c as consumer:
             for msg in consumer:
+                if start and start > msg.offset():
+                    continue
                 if stop and msg.offset() >= stop:
                     return
                 if step and (msg.offset() - max(0, start)) % step != 0:
                     continue
                 yield msg
 
     def __call__(self, val, key=None, *args, **kwargs) -> None:
         """Produce to topic."""
-        self._producer_ctx = (
-            self._producer_ctx
-            or get_producer(self.name, self.conf, self.dry, self.codec,
-                            self.poll_timeout, self.flush_timeout, self.pusher)
-        )
-        self.producer = (
-            self.producer or
-            self._producer_ctx.__enter__()
-        )
-        self.producer(key, val, *args, **kwargs)
+        if not self._producer_callable:
+            self._producer_ctx_mgr = self._get_producer()
+            self._producer_callable = self._producer_ctx_mgr.__enter__()
+        self._producer_callable(key, val, *args, **kwargs)
 
     def __del__(self):
-        """Exit potential producer instance."""
-        if self._producer_ctx:
-            self._producer_ctx.__exit__(None, None, None)
+        """Cleanup and finalization."""
+        if self._producer_ctx_mgr:
+            self._producer_ctx_mgr.__exit__(None, None, None)
```

### Comparing `snapstream-1.0.0b0/snapstream/utils.py` & `snapstream-1.0.1b0/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-1.0.0b0/PKG-INFO` & `snapstream-1.0.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 1.0.0b0
+Version: 1.0.1b0
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -21,15 +21,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: avro (>=1.11.1,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.0.2,<3.0.0)
 Requires-Dist: pypubsub (>=4.0.3,<5.0.0)
-Requires-Dist: pyright (>=1.1.302,<2.0.0)
 Requires-Dist: rocksdict (>=0.3.10,<0.4.0)
 Requires-Dist: toolz (>=0.12.0,<0.13.0)
 Project-URL: Documentation, https://snapstream.readthedocs.io
 Project-URL: Repository, https://github.com/Menziess/snapstream
 Description-Content-Type: text/markdown
 
 [![Test Python Package](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml/badge.svg)](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml) [![Documentation Status](https://readthedocs.org/projects/snapstream/badge/?version=latest)](https://snapstream.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/snapstream?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/snapstream)
```

