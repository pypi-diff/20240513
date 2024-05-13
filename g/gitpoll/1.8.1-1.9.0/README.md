# Comparing `tmp/gitpoll-1.8.1-py3-none-any.whl.zip` & `tmp/gitpoll-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7784 bytes, number of entries: 14
+Zip file size: 8012 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       32 b- defN 24-Apr-30 16:31 gitpoll/__init__.py
 -rw-r--r--  2.0 unx     1527 b- defN 24-May-03 07:39 gitpoll/args.py
--rw-r--r--  2.0 unx      483 b- defN 24-May-03 07:39 gitpoll/config.py
+-rw-r--r--  2.0 unx      514 b- defN 24-May-03 09:17 gitpoll/config.py
 -rw-r--r--  2.0 unx      877 b- defN 24-May-03 02:43 gitpoll/git.py
 -rw-r--r--  2.0 unx      889 b- defN 24-May-03 02:09 gitpoll/log.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-03 07:37 gitpoll/main.py
+-rw-r--r--  2.0 unx     2251 b- defN 24-May-03 09:04 gitpoll/main.py
 -rw-r--r--  2.0 unx     2072 b- defN 24-May-03 02:17 gitpoll/shell.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-03 08:58 gitpoll/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4576 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1057 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/RECORD
-14 files, 14868 bytes uncompressed, 6044 bytes compressed:  59.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-03 09:31 gitpoll/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4878 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1057 b- defN 24-May-03 09:31 gitpoll-1.9.0.dist-info/RECORD
+14 files, 15333 bytes uncompressed, 6272 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: gitpoll/shell.py
 Comment: 
 
 Filename: gitpoll/version.py
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/LICENSE
+Filename: gitpoll-1.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/METADATA
+Filename: gitpoll-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/WHEEL
+Filename: gitpoll-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/entry_points.txt
+Filename: gitpoll-1.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/top_level.txt
+Filename: gitpoll-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gitpoll-1.8.1.dist-info/RECORD
+Filename: gitpoll-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitpoll/config.py

```diff
@@ -1,12 +1,12 @@
 # Logging
 import os
 
 LOGGER_FILE = 'gitpoll.log'
 LOGGER_NAME = 'gitpoll'
 MAX_LOG_SIZE = 10 * 1024 * 1024 * 1024  # 10 GB
 MAX_LOG_FILES = 3  # Rotate over three files
-LOGGER_SET_LEVEL = 'DEBUG'
+LOGGER_SET_LEVEL = os.getenv('GITPOLL_LOG_LEVEL', 'INFO')
 # Optimized log format: Date-Time Level[Logger]Module:Function:Line-Message
 # Example output: 2024-04-30 06:21 - INFO[gitpoll]main:main:22-Checking for changes in the repository.
 LOGGER_FORMAT = "%(asctime)s %(levelname)s %(module)s:%(funcName)s %(message)s"
 DATE_FORMAT = '%m-%d %H:%M:%S'
```

## gitpoll/main.py

```diff
@@ -58,14 +58,18 @@
         return 1
 
     logger.debug("Changing to repository path: {}".format(repo_path))
     os.chdir(repo_path)
 
     logger.debug('args: {}'.format(args.__dict__))
 
+    if args.interval:
+        print('Polling every {} seconds...'.format(args.interval))
+    else:
+        print('Running once...')
     while True:
         logger.debug("Main loop iteration | ARGS {}".format(args.__dict__))
         _mainloop(args)
 
 
 if __name__ == "__main__":
     main()
```

## gitpoll/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.8.1'
+__version__ = '1.9.0'
```

## Comparing `gitpoll-1.8.1.dist-info/LICENSE` & `gitpoll-1.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gitpoll-1.8.1.dist-info/METADATA` & `gitpoll-1.9.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitpoll
-Version: 1.8.1
+Version: 1.9.0
 Summary: A tool to watch a GitHub repository for changes and perform actions before and after pulling updates.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://github.com/cc-d/gitpoll
 Project-URL: Repository, https://github.com/cc-d/gitpoll
 Project-URL: Issues, https://github.com/cc-d/gitpoll/issues
 Project-URL: Documentation, https://github.com/cc-d/gitpoll
 Project-URL: Changelog, https://github.com/cc-d/gitpoll/blob/main/CHANGELOG.md
@@ -41,15 +41,14 @@
 - All behavior is configurable via command-line options.
 
 ## Installation
 
 ### Requirements
 
 - Python 3.5 or higher
-- Dependencies: `pyshared`, `logfunc`
 
 ### Setup
 
 #### Install from PyPI using pip:
 
 ```bash
 pip install gitpoll
@@ -86,14 +85,18 @@
   -p PRE_ACTION, --pre-action PRE_ACTION
                         Command or path to the pre-action shell script or command.
   -P POST_ACTION, --post-action POST_ACTION
                         Command or path to the post-action shell script or command.
   -f, --force           Force execution pre and post actions regardless of changes.
 ```
 
+### Environment Variables
+
+- `GITPOLL_LOG_LEVEL`: Set the log level (default: `INFO`)
+
 ### Basic Usage
 
 To monitor a repository and execute actions based on changes:
 
 ```bash
 gitpoll /path/to/repo
 ```
@@ -102,14 +105,28 @@
 
 Monitor a repository at `/home/user/myrepo`, check every 300 seconds, and run specified scripts:
 
 ```bash
 gitpoll /home/user/myrepo -i 300 -p /path/to/pre_script.sh -P /path/to/post_script.sh
 ```
 
+### Pre/Post Actions
+
+These are executed as if being executed from the current shell gitpoll is running within. Either a `.sh` script location or the shell command itself.
+
+```
+-p test.sh
+```
+
+is valid as well as
+
+```
+-p 'sudo systemctl restart x'
+```
+
 ### No-Pull Mode
 
 Execute pre and post actions without pulling changes from the repository:
 
 ```bash
 gitpoll /path/to/repo --no-pull
 ```
```

