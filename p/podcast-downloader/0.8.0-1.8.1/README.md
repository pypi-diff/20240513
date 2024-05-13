# Comparing `tmp/podcast_downloader-0.8.0.tar.gz` & `tmp/podcast_downloader-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_downloader-0.8.0.tar", last modified: Tue Mar 12 18:30:15 2024, max compression
+gzip compressed data, was "podcast_downloader-1.8.1.tar", last modified: Mon May 13 18:04:28 2024, max compression
```

## Comparing `podcast_downloader-0.8.0.tar` & `podcast_downloader-1.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:30:15.951343 podcast_downloader-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-03-12 18:30:15.951343 podcast_downloader-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:30:15.947343 podcast_downloader-0.8.0/podcast_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/downloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/podcast_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:30:15.951343 podcast_downloader-0.8.0/podcast_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-03-12 18:30:15.000000 podcast_downloader-0.8.0/podcast_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-12 18:30:15.000000 podcast_downloader-0.8.0/podcast_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 18:30:15.000000 podcast_downloader-0.8.0/podcast_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 18:30:15.000000 podcast_downloader-0.8.0/podcast_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-12 18:30:15.000000 podcast_downloader-0.8.0/podcast_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:30:15.951343 podcast_downloader-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-12 18:30:03.000000 podcast_downloader-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:04:28.198723 podcast_downloader-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17532 2024-05-13 18:04:28.198723 podcast_downloader-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16919 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:04:28.194723 podcast_downloader-1.8.1/podcast_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/downloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/podcast_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:04:28.198723 podcast_downloader-1.8.1/podcast_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17532 2024-05-13 18:04:28.000000 podcast_downloader-1.8.1/podcast_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 18:04:28.000000 podcast_downloader-1.8.1/podcast_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:04:28.000000 podcast_downloader-1.8.1/podcast_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 18:04:28.000000 podcast_downloader-1.8.1/podcast_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 18:04:28.000000 podcast_downloader-1.8.1/podcast_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:04:28.198723 podcast_downloader-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 18:04:20.000000 podcast_downloader-1.8.1/setup.py
```

### Comparing `podcast_downloader-0.8.0/LICENSE` & `podcast_downloader-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.8.0/PKG-INFO` & `podcast_downloader-1.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast_downloader
-Version: 0.8.0
+Version: 1.8.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -19,103 +19,126 @@
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
 [![Downloads](https://img.shields.io/pypi/dm/podcast-downloader.svg)](https://pypi.python.org/pypi/podcast-downloader)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-The Python module for downloading files from given RSS feeds.
-It is not using database of any sort. It require configuration file.
+The Python module designed for downloading files from given RSS feeds, particularly targeted at podcasts.
+It does not use any sort of database but requires a configuration file.
 
-The script is analyzing the directory where it put the previously downloaded files.
-It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
+The script is intended to be run periodically. Upon starting, it analyzes the directory where it previously stored downloaded files.
+It then compares these files with those listed in the RSS feed, identifying any missing ones and downloading them.
 
-As name suggested, the script is designed for podcasts. The files searched by default are `mp3`.
+The files searched by default are `mp3`.
+
+The result of using the [example below](#configuration), on empty directories, will be:
+
+```log
+dplocki@ghost-wheel:~$ python -m podcast_downloader
+[2024-04-08 21:19:10] Loading configuration (from file: "~/.podcast_downloader_config.json")
+[2024-04-08 21:19:15] Checking "The Skeptic Guide"
+[2024-04-08 21:19:15] Last downloaded file "<none>"
+[2024-04-08 21:19:15] The Skeptic Guide: Downloading file: "https://traffic.libsyn.com/secure/skepticsguide/skepticast2024-04-06.mp3" saved as "skepticast2024-04-06.mp3"
+[2024-04-08 21:19:41] Checking "The Real Python Podcast"
+[2024-04-08 21:19:41] Last downloaded file "<none>"
+[2024-04-08 21:19:41] The Real Python Podcast: Downloading file: "https://chtbl.com/track/92DB94/files.realpython.com/podcasts/RPP_E199_03_Calvin.eef1db4d6679.mp3" saved as "[20240405] rpp_e199_03_calvin.eef1db4d6679.mp3"
+[2024-04-08 21:20:04] Finished
+```
+
+The result:
+
+```
+dplocki@ghost-wheel:~$ tree podcasts/
+podcasts/
+├── RealPython
+│   └── [20240405] rpp_e199_03_calvin.eef1db4d6679.mp3
+└── SGTTU
+    └── skepticast2024-04-06.mp3
+
+2 directories, 2 files
+```
 
 ## Setup
 
-### Installation from PyPI
+Installation from PyPI:
 
 ```bash
 pip install podcast_downloader
 ```
 
 ## Running the script
 
-The script [require configuration file](#configuration) in order to work.
-After installation, the script can be called as any Python module:
+The script [requires configuration file](#configuration) in order to work.
+After installation, the script can be run as any Python module:
 
 ```bash
 python -m podcast_downloader
 ```
 
-### In action
+It is also possible to run the script with given configuration file:
 
-Using the [example above](#example), the result will be:
-
-```log
-[2020-06-16 19:54:35] Loading configuration (from file: "~/.podcast_downloader_config.json")
-[2020-06-16 19:54:35] Checking "The Skeptic Guide"
-[2020-06-16 19:54:35] Last downloaded file "skepticast2020-06-13.mp3"
-[2020-06-16 19:54:39] The Skeptic Guide: Nothing new
-[2020-06-16 19:54:39] ------------------------------
-[2020-06-16 19:54:39] Finished
+```bash
+python -m podcast_downloader --config my_config.json
 ```
 
 ## Configuration
 
-### The configuration file
-
-The configuration file is placed in home directory.
-
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
-
-### An example of configuration file
+An example of configuration file
 
 ```json
 {
   "if_directory_empty": "download_from_4_days",
   "podcasts": [
     {
-      "name": "Python for dummies",
-      "rss_link": "http://python-for-dummies/atom.rss",
-      "path": "~/podcasts/PythonForDummies"
-    },
-    {
       "name": "The Skeptic Guide",
       "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
       "path": "~/podcasts/SGTTU"
+    },
+    {
+      "rss_link": "https://realpython.com/podcasts/rpp/feed",
+      "path": "~/podcasts/RealPython",
+      "file_name_template": "[%publish_date%] %file_name%.%file_extension%"
     }
   ]
 }
 ```
 
+### The configuration file
+
+By default the configuration file is placed in home directory. It's file name is: `.podcast_downloader_config.json`.
+
+The config file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
+
+The path to configuration file can be specified by [script argument](#script-arguments).
+
 ### The settings hierarchy
 
-The script will replace default values by read from configuration file.
-Those will be cover by all values given by command line.
+The script replaces default values by those read from configuration file.
+Those will be overload by values given from command line.
 
 ```
- command line parameters > configuration file > default values
+command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                                | Note |
-|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                               |      |
-| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
-| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
-| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
-| `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| Property             | Type       | Required? | Default                                | Note |
+|:---------------------|:----------:|:---------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no        | infinity                               |      |
+| `if_directory_empty` | string     | no        | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no        | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
+| `podcasts`           | subsection | yes       | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no        | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
+| `fill_up_gaps`       | boolean    | no        | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| `download_delay`     | number     | no        | `0`                                    | See [Download delay](#download-delay) |
 
 ### Podcasts sub category
 
-`Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
+The `podcasts` segment is the part of configuration file where you provide the array of objects with fallowing content:
 
 | Property             | Type       | Required | Default                                | Note |
 |:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
 | `name`               | string     | yes      | -                                      | The name of channel (use in logger) |
 | `rss_link`           | string     | yes      | -                                      | The URL of RSS feed |
 | `path`               | string     | yes      | -                                      | The path to directory, where podcast are stored, will be downloaded |
 | `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, see [File name template](#file-name-template)|
@@ -124,149 +147,164 @@
 | `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
 | `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
 | `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 | `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
 
 ### HTTP request headers
 
-Some servers may don't like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is way, there is a possibility to present the script client as something else.
+Some servers may not like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is why, there is a possibility for the script to pose as something else: by specifying the HTTP headers during downloading files.
 
-There is an option to specify HTTP headers when downloading files.
-You can provide them using the `http_headers` value in the configuration file.
-The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+Use the `http_headers` option in the configuration file. The value should be a dictionary object where each header is presented as a key-value pair. The key being the header title and the value being the header value.
 
-Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+By default the value is: `{"User-Agent": "podcast-downloader"}`. Providing anything else for `http_headers` will override all the default values (they do not merge).
 
-Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+On other hand in the podcast sub-configuration, the `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
 
 Example:
 
 ```json
 {
   "http_headers": {
     "User-Agent": "podcast-downloader"
+
   },
   "podcasts": [
     {
-      "name": "Unu Podcast",
-      "rss_link": "http://www.unupodcast.org/feed.rss",
-      "path": "~/podcasts/unu_podcast",
+      "name": "Unua Podcast",
+      "rss_link": "http://www.unuapodcast.org/feed.rss",
+      "path": "~/podcasts/unua_podcast",
+      "https_headers": {
+        "User-Agent": "Mozilla/5.0"
+      }
+    },
+    {
+      "name": "Dua Podcast",
+      "rss_link": "http://www.duapodcast.org/feed.rss",
+      "path": "~/podcasts/dua_podcast",
       "https_headers": {
-        "User-Agent": "User-Agent: Mozilla/5.0",
+        "Authorization": "Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ=="
       }
     }
   ]
 }
 ```
 
-## Script arguments
+In this example, the Unua Podcast will be download just with the header: `User-Agent: Mozilla/5.0`, and the Dua Podcast with: `User-Agent: podcast-downloader` and `Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==`.
+
+### Download delay
 
-The script accept following command line arguments:
+When you had a lot of files to download from a single server, it may be better to set up the small delay between downloads to avoid being recognized as an attacker by the server. In the script there is an option called `download_delay`, which represents the **number of seconds** the script will wait between downloads.
 
-| Short version | Long name              | Parameter           | Default         | Note |
-|:--------------|:-----------------------|:-------------------:|:---------------:|:-----|
-|               | `--downloads_limit`    | number              | infinity        | The maximum number of downloaded mp3 files |
-|               | `--if_directory_empty` | string              | `download_last` | The general approach on empty directory |
+The default value is `0`.
 
-## Adding date to file name
+Notes:
 
-If RSS channel doesn't have single and constant name convention, it may causing the script to working incorrectly. The solution is force files to have common and meaningful prefix. The script is able to adding the date on beginning of downloaded file name.
+ * this delay applies per podcast, not between two different podcasts
+ * the value can be provided as [script argument](#script-arguments)
 
-Use [File name template](#file-name-template) and option `%publish_date%`.
+## Script arguments
+
+The script accepts following command line arguments:
+
+| Short version | Long name              | Parameter           | Default                             | Note |
+|:--------------|:-----------------------|:-------------------:|:-----------------------------------:|:-----|
+|               | `--config`             | string              | `~/.podcast_downloader_config.json` | The placement of the configuration file |
+|               | `--downloads_limit`    | number              | infinity                            | The maximum number of downloaded mp3 files |
+|               | `--if_directory_empty` | string              | `download_last`                     | The general approach on empty directory |
+|               | `--download_delay`     | number              | `0`                                 | The waiting time (seconds) between downloads |
 
 ## File name template
 
-Use to change the name of downloaded file after its downloading.
+Use to adjust the file name after downloading.
 
-Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is taken from the link to podcast file.
+Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is based on the link to podcast file.
 
 Template values:
 
 | Name               | Notes                                                   |
 |:-------------------|:--------------------------------------------------------|
-| `%file_name%`      | The file name taken from link, without extension        |
-| `%file_extension%` | The extension for the file, taken from link             |
+| `%file_name%`      | The file name from the link, without extension          |
+| `%file_extension%` | The extension for the file, from link                   |
 | `%publish_date%`   | The publish date of the RSS entry                       |
 | `%title%`          | The title of the RSS entry                              |
 
-### Non default the publish_date
-
-The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change the date you can provide the new format after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
+### Non-default the publish_date
 
+The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change it you can provide the new one after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
 
 | The standard code | The script code | Notes                                      |
 |:------------------|:----------------|:-------------------------------------------|
 | `%Y%m%d`          | `$Y$m$d`        | The default value of the `%publish_date%`  |
 | `%A`              | `$A`            | Adds the weekday (local language settings) |
 | `%x`              | `$x`            | The local date represent. **Warning**: in some settings, the `/` is used here, so it may caused problem in the file name |
 
 ### Examples
 
 * `[%publish_date%] %file_name%.%file_extension%`
 * `[%publish_date%] %title%.%file_extension%`
 
 ## File types filter
 
-Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
+Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader looks just for them, ignoring all others types.
 
-If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
+If your podcast supports other types of media files, you can specified the file filters. Provide the  extension of the file (like `.mp3`) and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
-If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
+If you don't know the type of the file, you can look for it in the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-  <enclosure
-    url="https://an.apple.supporter.page/podcast/episode23.m4a"
-    length="14527149"
-    type="audio/x-m4a" />
+  <enclosure url="https://www.vidocast.url/podcast/episode23.m4a"
+             length="14527149"
+             type="audio/x-m4a" />
 ```
 
-Notes: the dot on the file extension is require.
+**Note**: the dot on the file extension is require.
 
 ### Example
 
 ```json
   "podcast_extensions": {
     ".mp3": "audio/mpeg",
     ".m4a": "audio/x-m4a"
   }
 ```
 
 ## In case of empty directory
 
-If a directory for podcast is empty, the script needs to recognize what to do. Due to lack of database, you can:
+If a directory for podcast is empty, the script needs to know what to do. Due to lack of database, you can:
 
 * [download all episodes from feed](#download-all-from-feed)
-* [download only the last episode](#only-last)
-* [download last n episodes](#download-n-last-episodes)
+* [download only the last episode](#download-last)
+* [download last n episodes](#download-last-n-episodes)
 * [download all new episode from last n days](#download-all-from-n-days)
 * [download all new episode since day after, the last episode should appear](#download-all-episode-since-last-excepted)
 
+Default behavior is: `download_last`
+
 ### Download all from feed
 
 The script will download all episodes from the feed.
 
 Set by `download_all_from_feed`.
 
-### Only last
+### Download last
 
 The script will download only the last episode from the feed.
-It is a good approach when you wish to start listening the podcast.
 It is also default approach of the script.
 
 Set by `download_last`.
 
 ### Download last n episodes
 
-The script will download exactly given number of episodes from the feed.
+The script will download exactly the given number of episodes from the feed.
 
-Set by `download_last_n_episodes`. The *n* must be replaced by number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five last episodes will be downloaded.
+Set by `download_last_n_episodes`. The *n* must be replaced by a number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five most recent episodes will be downloaded.
 
 ### Download all from n days
 
-The script will download all episodes which appear in last *n* days. I can be use when you are downloading on regular schedule.
+The script will download all episodes which appear in recent *n* days. It can be use when you are downloading on regular schedule.
 The *n* number is given within the setup value: `download_from_n_days`. For example: `download_from_3_days` means download all episodes from last 3 days.
 
 ### Download all episode since last excepted
 
 The script will download all episodes which appear after the day of release of last episode.
 
 The *n* number is the day of the normal episode.
@@ -292,21 +330,21 @@
 |------------------------|---------|
 | `download_from_monday` | New episodes appear in Monday. The script will download all episodes since last Tuesday (including it) |
 | `download_from_Fri`    | New episodes appear in Friday. The script will download all episodes since last Saturday (including it) |
 | `download_from_12`     | New episodes appear each 12th of month. The script will download all episodes since 13 month before |
 
 ## Download files from gaps
 
-The script recognizes the stream of downloaded files (based on the feed). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situations where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed).
+The script recognizes the stream of downloaded files (based on the feed data). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situation where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed), the most earlier episode.
 
 Default value: `false`.
 
 ## The analyze of the RSS feed
 
-The script is look through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
+The script looks through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
 
 ## Converting the OPML
 
 The [OPML](https://en.wikipedia.org/wiki/OPML) files can be converted into [configuration](#configuration). The output file needs to be adjusted (missing the `path`).
 
 ```py
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `podcast_downloader-0.8.0/README.md` & `podcast_downloader-1.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,103 +2,126 @@
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
 [![Downloads](https://img.shields.io/pypi/dm/podcast-downloader.svg)](https://pypi.python.org/pypi/podcast-downloader)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-The Python module for downloading files from given RSS feeds.
-It is not using database of any sort. It require configuration file.
+The Python module designed for downloading files from given RSS feeds, particularly targeted at podcasts.
+It does not use any sort of database but requires a configuration file.
 
-The script is analyzing the directory where it put the previously downloaded files.
-It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
+The script is intended to be run periodically. Upon starting, it analyzes the directory where it previously stored downloaded files.
+It then compares these files with those listed in the RSS feed, identifying any missing ones and downloading them.
 
-As name suggested, the script is designed for podcasts. The files searched by default are `mp3`.
+The files searched by default are `mp3`.
+
+The result of using the [example below](#configuration), on empty directories, will be:
+
+```log
+dplocki@ghost-wheel:~$ python -m podcast_downloader
+[2024-04-08 21:19:10] Loading configuration (from file: "~/.podcast_downloader_config.json")
+[2024-04-08 21:19:15] Checking "The Skeptic Guide"
+[2024-04-08 21:19:15] Last downloaded file "<none>"
+[2024-04-08 21:19:15] The Skeptic Guide: Downloading file: "https://traffic.libsyn.com/secure/skepticsguide/skepticast2024-04-06.mp3" saved as "skepticast2024-04-06.mp3"
+[2024-04-08 21:19:41] Checking "The Real Python Podcast"
+[2024-04-08 21:19:41] Last downloaded file "<none>"
+[2024-04-08 21:19:41] The Real Python Podcast: Downloading file: "https://chtbl.com/track/92DB94/files.realpython.com/podcasts/RPP_E199_03_Calvin.eef1db4d6679.mp3" saved as "[20240405] rpp_e199_03_calvin.eef1db4d6679.mp3"
+[2024-04-08 21:20:04] Finished
+```
+
+The result:
+
+```
+dplocki@ghost-wheel:~$ tree podcasts/
+podcasts/
+├── RealPython
+│   └── [20240405] rpp_e199_03_calvin.eef1db4d6679.mp3
+└── SGTTU
+    └── skepticast2024-04-06.mp3
+
+2 directories, 2 files
+```
 
 ## Setup
 
-### Installation from PyPI
+Installation from PyPI:
 
 ```bash
 pip install podcast_downloader
 ```
 
 ## Running the script
 
-The script [require configuration file](#configuration) in order to work.
-After installation, the script can be called as any Python module:
+The script [requires configuration file](#configuration) in order to work.
+After installation, the script can be run as any Python module:
 
 ```bash
 python -m podcast_downloader
 ```
 
-### In action
+It is also possible to run the script with given configuration file:
 
-Using the [example above](#example), the result will be:
-
-```log
-[2020-06-16 19:54:35] Loading configuration (from file: "~/.podcast_downloader_config.json")
-[2020-06-16 19:54:35] Checking "The Skeptic Guide"
-[2020-06-16 19:54:35] Last downloaded file "skepticast2020-06-13.mp3"
-[2020-06-16 19:54:39] The Skeptic Guide: Nothing new
-[2020-06-16 19:54:39] ------------------------------
-[2020-06-16 19:54:39] Finished
+```bash
+python -m podcast_downloader --config my_config.json
 ```
 
 ## Configuration
 
-### The configuration file
-
-The configuration file is placed in home directory.
-
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
-
-### An example of configuration file
+An example of configuration file
 
 ```json
 {
   "if_directory_empty": "download_from_4_days",
   "podcasts": [
     {
-      "name": "Python for dummies",
-      "rss_link": "http://python-for-dummies/atom.rss",
-      "path": "~/podcasts/PythonForDummies"
-    },
-    {
       "name": "The Skeptic Guide",
       "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
       "path": "~/podcasts/SGTTU"
+    },
+    {
+      "rss_link": "https://realpython.com/podcasts/rpp/feed",
+      "path": "~/podcasts/RealPython",
+      "file_name_template": "[%publish_date%] %file_name%.%file_extension%"
     }
   ]
 }
 ```
 
+### The configuration file
+
+By default the configuration file is placed in home directory. It's file name is: `.podcast_downloader_config.json`.
+
+The config file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
+
+The path to configuration file can be specified by [script argument](#script-arguments).
+
 ### The settings hierarchy
 
-The script will replace default values by read from configuration file.
-Those will be cover by all values given by command line.
+The script replaces default values by those read from configuration file.
+Those will be overload by values given from command line.
 
 ```
- command line parameters > configuration file > default values
+command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                                | Note |
-|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                               |      |
-| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
-| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
-| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
-| `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| Property             | Type       | Required? | Default                                | Note |
+|:---------------------|:----------:|:---------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no        | infinity                               |      |
+| `if_directory_empty` | string     | no        | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no        | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
+| `podcasts`           | subsection | yes       | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no        | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
+| `fill_up_gaps`       | boolean    | no        | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| `download_delay`     | number     | no        | `0`                                    | See [Download delay](#download-delay) |
 
 ### Podcasts sub category
 
-`Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
+The `podcasts` segment is the part of configuration file where you provide the array of objects with fallowing content:
 
 | Property             | Type       | Required | Default                                | Note |
 |:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
 | `name`               | string     | yes      | -                                      | The name of channel (use in logger) |
 | `rss_link`           | string     | yes      | -                                      | The URL of RSS feed |
 | `path`               | string     | yes      | -                                      | The path to directory, where podcast are stored, will be downloaded |
 | `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, see [File name template](#file-name-template)|
@@ -107,149 +130,164 @@
 | `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
 | `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
 | `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 | `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
 
 ### HTTP request headers
 
-Some servers may don't like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is way, there is a possibility to present the script client as something else.
+Some servers may not like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is why, there is a possibility for the script to pose as something else: by specifying the HTTP headers during downloading files.
 
-There is an option to specify HTTP headers when downloading files.
-You can provide them using the `http_headers` value in the configuration file.
-The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+Use the `http_headers` option in the configuration file. The value should be a dictionary object where each header is presented as a key-value pair. The key being the header title and the value being the header value.
 
-Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+By default the value is: `{"User-Agent": "podcast-downloader"}`. Providing anything else for `http_headers` will override all the default values (they do not merge).
 
-Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+On other hand in the podcast sub-configuration, the `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
 
 Example:
 
 ```json
 {
   "http_headers": {
     "User-Agent": "podcast-downloader"
+
   },
   "podcasts": [
     {
-      "name": "Unu Podcast",
-      "rss_link": "http://www.unupodcast.org/feed.rss",
-      "path": "~/podcasts/unu_podcast",
+      "name": "Unua Podcast",
+      "rss_link": "http://www.unuapodcast.org/feed.rss",
+      "path": "~/podcasts/unua_podcast",
+      "https_headers": {
+        "User-Agent": "Mozilla/5.0"
+      }
+    },
+    {
+      "name": "Dua Podcast",
+      "rss_link": "http://www.duapodcast.org/feed.rss",
+      "path": "~/podcasts/dua_podcast",
       "https_headers": {
-        "User-Agent": "User-Agent: Mozilla/5.0",
+        "Authorization": "Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ=="
       }
     }
   ]
 }
 ```
 
-## Script arguments
+In this example, the Unua Podcast will be download just with the header: `User-Agent: Mozilla/5.0`, and the Dua Podcast with: `User-Agent: podcast-downloader` and `Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==`.
+
+### Download delay
 
-The script accept following command line arguments:
+When you had a lot of files to download from a single server, it may be better to set up the small delay between downloads to avoid being recognized as an attacker by the server. In the script there is an option called `download_delay`, which represents the **number of seconds** the script will wait between downloads.
 
-| Short version | Long name              | Parameter           | Default         | Note |
-|:--------------|:-----------------------|:-------------------:|:---------------:|:-----|
-|               | `--downloads_limit`    | number              | infinity        | The maximum number of downloaded mp3 files |
-|               | `--if_directory_empty` | string              | `download_last` | The general approach on empty directory |
+The default value is `0`.
 
-## Adding date to file name
+Notes:
 
-If RSS channel doesn't have single and constant name convention, it may causing the script to working incorrectly. The solution is force files to have common and meaningful prefix. The script is able to adding the date on beginning of downloaded file name.
+ * this delay applies per podcast, not between two different podcasts
+ * the value can be provided as [script argument](#script-arguments)
 
-Use [File name template](#file-name-template) and option `%publish_date%`.
+## Script arguments
+
+The script accepts following command line arguments:
+
+| Short version | Long name              | Parameter           | Default                             | Note |
+|:--------------|:-----------------------|:-------------------:|:-----------------------------------:|:-----|
+|               | `--config`             | string              | `~/.podcast_downloader_config.json` | The placement of the configuration file |
+|               | `--downloads_limit`    | number              | infinity                            | The maximum number of downloaded mp3 files |
+|               | `--if_directory_empty` | string              | `download_last`                     | The general approach on empty directory |
+|               | `--download_delay`     | number              | `0`                                 | The waiting time (seconds) between downloads |
 
 ## File name template
 
-Use to change the name of downloaded file after its downloading.
+Use to adjust the file name after downloading.
 
-Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is taken from the link to podcast file.
+Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is based on the link to podcast file.
 
 Template values:
 
 | Name               | Notes                                                   |
 |:-------------------|:--------------------------------------------------------|
-| `%file_name%`      | The file name taken from link, without extension        |
-| `%file_extension%` | The extension for the file, taken from link             |
+| `%file_name%`      | The file name from the link, without extension          |
+| `%file_extension%` | The extension for the file, from link                   |
 | `%publish_date%`   | The publish date of the RSS entry                       |
 | `%title%`          | The title of the RSS entry                              |
 
-### Non default the publish_date
-
-The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change the date you can provide the new format after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
+### Non-default the publish_date
 
+The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change it you can provide the new one after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
 
 | The standard code | The script code | Notes                                      |
 |:------------------|:----------------|:-------------------------------------------|
 | `%Y%m%d`          | `$Y$m$d`        | The default value of the `%publish_date%`  |
 | `%A`              | `$A`            | Adds the weekday (local language settings) |
 | `%x`              | `$x`            | The local date represent. **Warning**: in some settings, the `/` is used here, so it may caused problem in the file name |
 
 ### Examples
 
 * `[%publish_date%] %file_name%.%file_extension%`
 * `[%publish_date%] %title%.%file_extension%`
 
 ## File types filter
 
-Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
+Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader looks just for them, ignoring all others types.
 
-If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
+If your podcast supports other types of media files, you can specified the file filters. Provide the  extension of the file (like `.mp3`) and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
-If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
+If you don't know the type of the file, you can look for it in the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-  <enclosure
-    url="https://an.apple.supporter.page/podcast/episode23.m4a"
-    length="14527149"
-    type="audio/x-m4a" />
+  <enclosure url="https://www.vidocast.url/podcast/episode23.m4a"
+             length="14527149"
+             type="audio/x-m4a" />
 ```
 
-Notes: the dot on the file extension is require.
+**Note**: the dot on the file extension is require.
 
 ### Example
 
 ```json
   "podcast_extensions": {
     ".mp3": "audio/mpeg",
     ".m4a": "audio/x-m4a"
   }
 ```
 
 ## In case of empty directory
 
-If a directory for podcast is empty, the script needs to recognize what to do. Due to lack of database, you can:
+If a directory for podcast is empty, the script needs to know what to do. Due to lack of database, you can:
 
 * [download all episodes from feed](#download-all-from-feed)
-* [download only the last episode](#only-last)
-* [download last n episodes](#download-n-last-episodes)
+* [download only the last episode](#download-last)
+* [download last n episodes](#download-last-n-episodes)
 * [download all new episode from last n days](#download-all-from-n-days)
 * [download all new episode since day after, the last episode should appear](#download-all-episode-since-last-excepted)
 
+Default behavior is: `download_last`
+
 ### Download all from feed
 
 The script will download all episodes from the feed.
 
 Set by `download_all_from_feed`.
 
-### Only last
+### Download last
 
 The script will download only the last episode from the feed.
-It is a good approach when you wish to start listening the podcast.
 It is also default approach of the script.
 
 Set by `download_last`.
 
 ### Download last n episodes
 
-The script will download exactly given number of episodes from the feed.
+The script will download exactly the given number of episodes from the feed.
 
-Set by `download_last_n_episodes`. The *n* must be replaced by number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five last episodes will be downloaded.
+Set by `download_last_n_episodes`. The *n* must be replaced by a number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five most recent episodes will be downloaded.
 
 ### Download all from n days
 
-The script will download all episodes which appear in last *n* days. I can be use when you are downloading on regular schedule.
+The script will download all episodes which appear in recent *n* days. It can be use when you are downloading on regular schedule.
 The *n* number is given within the setup value: `download_from_n_days`. For example: `download_from_3_days` means download all episodes from last 3 days.
 
 ### Download all episode since last excepted
 
 The script will download all episodes which appear after the day of release of last episode.
 
 The *n* number is the day of the normal episode.
@@ -275,21 +313,21 @@
 |------------------------|---------|
 | `download_from_monday` | New episodes appear in Monday. The script will download all episodes since last Tuesday (including it) |
 | `download_from_Fri`    | New episodes appear in Friday. The script will download all episodes since last Saturday (including it) |
 | `download_from_12`     | New episodes appear each 12th of month. The script will download all episodes since 13 month before |
 
 ## Download files from gaps
 
-The script recognizes the stream of downloaded files (based on the feed). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situations where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed).
+The script recognizes the stream of downloaded files (based on the feed data). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situation where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed), the most earlier episode.
 
 Default value: `false`.
 
 ## The analyze of the RSS feed
 
-The script is look through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
+The script looks through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
 
 ## Converting the OPML
 
 The [OPML](https://en.wikipedia.org/wiki/OPML) files can be converted into [configuration](#configuration). The output file needs to be adjusted (missing the `path`).
 
 ```py
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `podcast_downloader-0.8.0/podcast_downloader/__main__.py` & `podcast_downloader-1.8.1/podcast_downloader/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,28 @@
     parser.add_argument(
         "--if_directory_empty",
         required=False,
         type=str,
         help="The general approach on empty directory",
     )
 
+    parser.add_argument(
+        "--config",
+        required=False,
+        type=str,
+        help="The path to configuration file",
+    )
+
+    parser.add_argument(
+        "--download_delay",
+        required=False,
+        type=int,
+        help="The waiting time (seconds) between downloads",
+    )
+
     return parser
 
 
 def configuration_to_function_on_empty_directory(
     configuration_value: str,
 ) -> Callable[[Iterable[RSSEntity]], Iterable[RSSEntity]]:
     if configuration_value == "download_last":
@@ -156,24 +170,32 @@
     DEFAULT_CONFIGURATION = {
         configuration.CONFIG_DOWNLOADS_LIMIT: sys.maxsize,
         configuration.CONFIG_IF_DIRECTORY_EMPTY: "download_last",
         configuration.CONFIG_PODCAST_EXTENSIONS: {".mp3": "audio/mpeg"},
         configuration.CONFIG_FILE_NAME_TEMPLATE: "%file_name%.%file_extension%",
         configuration.CONFIG_HTTP_HEADER: {"User-Agent": "podcast-downloader"},
         configuration.CONFIG_FILL_UP_GAPS: False,
+        configuration.CONFIG_DOWNLOAD_DELAY: 0,
         configuration.CONFIG_PODCASTS: [],
     }
 
-    CONFIG_FILE = "~/.podcast_downloader_config.json"
-    logger.info('Loading configuration (from file: "%s")', CONFIG_FILE)
+    PARAMETERS_CONFIGURATION = parse_argv(build_parser())
+
+    config_file_name = PARAMETERS_CONFIGURATION.get(
+        "config", "~/.podcast_downloader_config.json"
+    )
+    logger.info('Loading configuration (from file: "%s")', config_file_name)
+    CONFIGURATION_FROM_FILE = load_configuration_file(
+        os.path.expanduser(config_file_name)
+    )
 
     CONFIGURATION = merge_parameters_collection(
         DEFAULT_CONFIGURATION,
-        load_configuration_file(os.path.expanduser(CONFIG_FILE)),
-        parse_argv(build_parser()),
+        CONFIGURATION_FROM_FILE,
+        PARAMETERS_CONFIGURATION,
     )
 
     is_valid, error = configuration_verification(CONFIGURATION)
     if not is_valid:
         logger.info("There is a problem with configuration file: %s", error)
         exit(1)
 
@@ -204,28 +226,33 @@
             CONFIGURATION[configuration.CONFIG_HTTP_HEADER],
             rss_source.get(configuration.CONFIG_HTTP_HEADER, {}),
         )
         rss_fill_up_gaps = rss_source.get(
             CONFIGURATION[configuration.CONFIG_FILL_UP_GAPS],
             rss_source.get(configuration.CONFIG_FILL_UP_GAPS, False),
         )
+        rss_download_delay = rss_source.get(
+            CONFIGURATION[configuration.CONFIG_DOWNLOAD_DELAY],
+            rss_source.get(configuration.CONFIG_DOWNLOAD_DELAY, 0),
+        )
 
         if rss_disable:
-            logger.info('Skipping the "%s"', rss_source_name)
+            logger.info('Skipping the "%s"', rss_source_name or rss_source_link)
             continue
 
-        try:
-            feed = load_feed(rss_source_link)
-            if not rss_source_name:
-                rss_source_name = get_feed_title_from_feed(feed)
-
-        except error:
-            logger.error(f"Error while checking the link: '{rss_source_link}': {error}")
+        feed = load_feed(rss_source_link)
+        if feed.bozo and len(feed.entries) == 0:
+            logger.error(
+                f"Error while checking the link: '{rss_source_link}': {feed['bozo_exception']}"
+            )
             continue
 
+        if not rss_source_name:
+            rss_source_name = get_feed_title_from_feed(feed)
+
         logger.info('Checking "%s"', rss_source_name)
 
         to_name_function = configuration_to_function_rss_to_name(
             rss_file_name_template_value, rss_source
         )
 
         on_directory_empty = configuration_to_function_on_empty_directory(
@@ -276,15 +303,24 @@
         if missing_files_links:
             download_podcast = partial(
                 download_rss_entity_to_path,
                 rss_https_header,
                 to_real_podcast_file_name,
             )
 
+            first_element = True
             for rss_entry in reversed(missing_files_links):
+                if rss_download_delay > 0:
+                    if not first_element:
+                        logger.info(
+                            "The download is sleeping (%d second)", rss_download_delay
+                        )
+                        time.sleep(rss_download_delay)
+                        first_element = False
+
                 wanted_podcast_file_name = to_name_function(rss_entry)
                 if wanted_podcast_file_name in downloaded_files:
                     continue
 
                 if DOWNLOADS_LIMITS == 0:
                     continue
```

### Comparing `podcast_downloader-0.8.0/podcast_downloader/configuration.py` & `podcast_downloader-1.8.1/podcast_downloader/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 CONFIG_IF_DIRECTORY_EMPTY = "if_directory_empty"
 CONFIG_DOWNLOADS_LIMIT = "downloads_limit"
 CONFIG_FILE_NAME_TEMPLATE = "file_name_template"
 CONFIG_PODCAST_EXTENSIONS = "podcast_extensions"
 CONFIG_HTTP_HEADER = "http_headers"
 CONFIG_FILL_UP_GAPS = "fill_up_gaps"
+CONFIG_DOWNLOAD_DELAY = "download_delay"
 
 CONFIG_PODCASTS = "podcasts"
 CONFIG_PODCASTS_NAME = "name"
 CONFIG_PODCASTS_PATH = "path"
 CONFIG_PODCASTS_RSS_LINK = "rss_link"
 CONFIG_PODCASTS_REQUIRE_DATE = "require_date"
 CONFIG_PODCASTS_DISABLE = "disable"
```

### Comparing `podcast_downloader-0.8.0/podcast_downloader/downloaded.py` & `podcast_downloader-1.8.1/podcast_downloader/downloaded.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.8.0/podcast_downloader/parameters.py` & `podcast_downloader-1.8.1/podcast_downloader/parameters.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.8.0/podcast_downloader/rss.py` & `podcast_downloader-1.8.1/podcast_downloader/rss.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.8.0/podcast_downloader/utils.py` & `podcast_downloader-1.8.1/podcast_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `podcast_downloader-0.8.0/podcast_downloader.egg-info/PKG-INFO` & `podcast_downloader-1.8.1/podcast_downloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast_downloader
-Version: 0.8.0
+Version: 1.8.1
 Summary: The script for downloading the recent mp3 from given RSS channels
 Home-page: https://github.com/dplocki/podcast-downloader
 Author: Dawid Plocki
 Author-email: dawid.plocki@gmail.com
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -19,103 +19,126 @@
 
 ![GitHub](https://img.shields.io/github/license/dplocki/podcast-downloader)
 ![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fdplocki%2Fpodcast-downloader%2Fbadge%3Fref%3Dmaster&style=flat)
 ![PyPI](https://img.shields.io/pypi/v/podcast-downloader)
 [![Downloads](https://img.shields.io/pypi/dm/podcast-downloader.svg)](https://pypi.python.org/pypi/podcast-downloader)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-The Python module for downloading files from given RSS feeds.
-It is not using database of any sort. It require configuration file.
+The Python module designed for downloading files from given RSS feeds, particularly targeted at podcasts.
+It does not use any sort of database but requires a configuration file.
 
-The script is analyzing the directory where it put the previously downloaded files.
-It is compering the last added file with the rss feed, finding the missing ones, and downloading them.
+The script is intended to be run periodically. Upon starting, it analyzes the directory where it previously stored downloaded files.
+It then compares these files with those listed in the RSS feed, identifying any missing ones and downloading them.
 
-As name suggested, the script is designed for podcasts. The files searched by default are `mp3`.
+The files searched by default are `mp3`.
+
+The result of using the [example below](#configuration), on empty directories, will be:
+
+```log
+dplocki@ghost-wheel:~$ python -m podcast_downloader
+[2024-04-08 21:19:10] Loading configuration (from file: "~/.podcast_downloader_config.json")
+[2024-04-08 21:19:15] Checking "The Skeptic Guide"
+[2024-04-08 21:19:15] Last downloaded file "<none>"
+[2024-04-08 21:19:15] The Skeptic Guide: Downloading file: "https://traffic.libsyn.com/secure/skepticsguide/skepticast2024-04-06.mp3" saved as "skepticast2024-04-06.mp3"
+[2024-04-08 21:19:41] Checking "The Real Python Podcast"
+[2024-04-08 21:19:41] Last downloaded file "<none>"
+[2024-04-08 21:19:41] The Real Python Podcast: Downloading file: "https://chtbl.com/track/92DB94/files.realpython.com/podcasts/RPP_E199_03_Calvin.eef1db4d6679.mp3" saved as "[20240405] rpp_e199_03_calvin.eef1db4d6679.mp3"
+[2024-04-08 21:20:04] Finished
+```
+
+The result:
+
+```
+dplocki@ghost-wheel:~$ tree podcasts/
+podcasts/
+├── RealPython
+│   └── [20240405] rpp_e199_03_calvin.eef1db4d6679.mp3
+└── SGTTU
+    └── skepticast2024-04-06.mp3
+
+2 directories, 2 files
+```
 
 ## Setup
 
-### Installation from PyPI
+Installation from PyPI:
 
 ```bash
 pip install podcast_downloader
 ```
 
 ## Running the script
 
-The script [require configuration file](#configuration) in order to work.
-After installation, the script can be called as any Python module:
+The script [requires configuration file](#configuration) in order to work.
+After installation, the script can be run as any Python module:
 
 ```bash
 python -m podcast_downloader
 ```
 
-### In action
+It is also possible to run the script with given configuration file:
 
-Using the [example above](#example), the result will be:
-
-```log
-[2020-06-16 19:54:35] Loading configuration (from file: "~/.podcast_downloader_config.json")
-[2020-06-16 19:54:35] Checking "The Skeptic Guide"
-[2020-06-16 19:54:35] Last downloaded file "skepticast2020-06-13.mp3"
-[2020-06-16 19:54:39] The Skeptic Guide: Nothing new
-[2020-06-16 19:54:39] ------------------------------
-[2020-06-16 19:54:39] Finished
+```bash
+python -m podcast_downloader --config my_config.json
 ```
 
 ## Configuration
 
-### The configuration file
-
-The configuration file is placed in home directory.
-
-The name: `.podcast_downloader_config.json`. The file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
-
-### An example of configuration file
+An example of configuration file
 
 ```json
 {
   "if_directory_empty": "download_from_4_days",
   "podcasts": [
     {
-      "name": "Python for dummies",
-      "rss_link": "http://python-for-dummies/atom.rss",
-      "path": "~/podcasts/PythonForDummies"
-    },
-    {
       "name": "The Skeptic Guide",
       "rss_link": "https://feed.theskepticsguide.org/feed/rss.aspx",
       "path": "~/podcasts/SGTTU"
+    },
+    {
+      "rss_link": "https://realpython.com/podcasts/rpp/feed",
+      "path": "~/podcasts/RealPython",
+      "file_name_template": "[%publish_date%] %file_name%.%file_extension%"
     }
   ]
 }
 ```
 
+### The configuration file
+
+By default the configuration file is placed in home directory. It's file name is: `.podcast_downloader_config.json`.
+
+The config file is format in [JSON](https://en.wikipedia.org/wiki/JSON). The expected encoding is [utf-8](https://en.wikipedia.org/wiki/UTF-8).
+
+The path to configuration file can be specified by [script argument](#script-arguments).
+
 ### The settings hierarchy
 
-The script will replace default values by read from configuration file.
-Those will be cover by all values given by command line.
+The script replaces default values by those read from configuration file.
+Those will be overload by values given from command line.
 
 ```
- command line parameters > configuration file > default values
+command line parameters > configuration file > default values
 ```
 
 ### The main options
 
-| Property             | Type       | Required | Default                                | Note |
-|:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
-| `downloads_limit`    | number     | no       | infinity                               |      |
-| `if_directory_empty` | string     | no       | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
-| `podcast_extensions` | key-value  | no       | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
-| `podcasts`           | subsection | yes      | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
-| `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
-| `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| Property             | Type       | Required? | Default                                | Note |
+|:---------------------|:----------:|:---------:|:--------------------------------------:|:-----|
+| `downloads_limit`    | number     | no        | infinity                               |      |
+| `if_directory_empty` | string     | no        | download_last                          | See [In case of empty directory](#in-case-of-empty-directory) |
+| `podcast_extensions` | key-value  | no        | `{".mp3": "audio/mpeg"}`               | See [File types filter](#file-types-filter) |
+| `podcasts`           | subsection | yes       | `[]`                                   | See [Podcasts sub category](#podcasts-sub-category) |
+| `http_headers`       | key-value  | no        | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
+| `fill_up_gaps`       | boolean    | no        | false                                  | See [Download files from gaps](#download-files-from-gaps) |
+| `download_delay`     | number     | no        | `0`                                    | See [Download delay](#download-delay) |
 
 ### Podcasts sub category
 
-`Podcasts` is the part of configuration file where you provide the array of objects with fallowing content:
+The `podcasts` segment is the part of configuration file where you provide the array of objects with fallowing content:
 
 | Property             | Type       | Required | Default                                | Note |
 |:---------------------|:----------:|:--------:|:--------------------------------------:|:-----|
 | `name`               | string     | yes      | -                                      | The name of channel (use in logger) |
 | `rss_link`           | string     | yes      | -                                      | The URL of RSS feed |
 | `path`               | string     | yes      | -                                      | The path to directory, where podcast are stored, will be downloaded |
 | `file_name_template` | string     | no       | `%file_name%.%file_extension%`         | The template for the downloaded files, see [File name template](#file-name-template)|
@@ -124,149 +147,164 @@
 | `if_directory_empty` | string     | no       | `download_last`                        | See [In case of empty directory](#in-case-of-empty-directory) |
 | `require_date`       | boolean    | no       | `false`                                | **Deprecated** Is date of podcast should be added into name of file - use the `file_name_template`: `[%publish_date%] %file_name%.%file_extension%"` |
 | `http_headers`       | key-value  | no       | `{"User-Agent": "podcast-downloader"}` | See [HTTP request headers](#http-request-headers) |
 | `fill_up_gaps`       | boolean    | no       | false                                  | See [Download files from gaps](#download-files-from-gaps) |
 
 ### HTTP request headers
 
-Some servers may don't like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is way, there is a possibility to present the script client as something else.
+Some servers may not like how the urllib is presenting itself to them (the HTTP User-Agent header). This may lead into problems like: `urllib.error.HTTPError: HTTP Error 403: Forbidden`. That is why, there is a possibility for the script to pose as something else: by specifying the HTTP headers during downloading files.
 
-There is an option to specify HTTP headers when downloading files.
-You can provide them using the `http_headers` value in the configuration file.
-The option value should be a dictionary where each header is presented as a key-value pair, with the key being the header title and the value being the header value.
+Use the `http_headers` option in the configuration file. The value should be a dictionary object where each header is presented as a key-value pair. The key being the header title and the value being the header value.
 
-Default value: `{"User-Agent": "podcast-downloader"}`. Providing any value for `http_headers` will override the default value.
+By default the value is: `{"User-Agent": "podcast-downloader"}`. Providing anything else for `http_headers` will override all the default values (they do not merge).
 
-Podcast `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
+On other hand in the podcast sub-configuration, the `http_headers` will be merged with the global `http_headers`. In case of a conflict (same key name), the vale from podcast sub-configuration will override the global one.
 
 Example:
 
 ```json
 {
   "http_headers": {
     "User-Agent": "podcast-downloader"
+
   },
   "podcasts": [
     {
-      "name": "Unu Podcast",
-      "rss_link": "http://www.unupodcast.org/feed.rss",
-      "path": "~/podcasts/unu_podcast",
+      "name": "Unua Podcast",
+      "rss_link": "http://www.unuapodcast.org/feed.rss",
+      "path": "~/podcasts/unua_podcast",
+      "https_headers": {
+        "User-Agent": "Mozilla/5.0"
+      }
+    },
+    {
+      "name": "Dua Podcast",
+      "rss_link": "http://www.duapodcast.org/feed.rss",
+      "path": "~/podcasts/dua_podcast",
       "https_headers": {
-        "User-Agent": "User-Agent: Mozilla/5.0",
+        "Authorization": "Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ=="
       }
     }
   ]
 }
 ```
 
-## Script arguments
+In this example, the Unua Podcast will be download just with the header: `User-Agent: Mozilla/5.0`, and the Dua Podcast with: `User-Agent: podcast-downloader` and `Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==`.
+
+### Download delay
 
-The script accept following command line arguments:
+When you had a lot of files to download from a single server, it may be better to set up the small delay between downloads to avoid being recognized as an attacker by the server. In the script there is an option called `download_delay`, which represents the **number of seconds** the script will wait between downloads.
 
-| Short version | Long name              | Parameter           | Default         | Note |
-|:--------------|:-----------------------|:-------------------:|:---------------:|:-----|
-|               | `--downloads_limit`    | number              | infinity        | The maximum number of downloaded mp3 files |
-|               | `--if_directory_empty` | string              | `download_last` | The general approach on empty directory |
+The default value is `0`.
 
-## Adding date to file name
+Notes:
 
-If RSS channel doesn't have single and constant name convention, it may causing the script to working incorrectly. The solution is force files to have common and meaningful prefix. The script is able to adding the date on beginning of downloaded file name.
+ * this delay applies per podcast, not between two different podcasts
+ * the value can be provided as [script argument](#script-arguments)
 
-Use [File name template](#file-name-template) and option `%publish_date%`.
+## Script arguments
+
+The script accepts following command line arguments:
+
+| Short version | Long name              | Parameter           | Default                             | Note |
+|:--------------|:-----------------------|:-------------------:|:-----------------------------------:|:-----|
+|               | `--config`             | string              | `~/.podcast_downloader_config.json` | The placement of the configuration file |
+|               | `--downloads_limit`    | number              | infinity                            | The maximum number of downloaded mp3 files |
+|               | `--if_directory_empty` | string              | `download_last`                     | The general approach on empty directory |
+|               | `--download_delay`     | number              | `0`                                 | The waiting time (seconds) between downloads |
 
 ## File name template
 
-Use to change the name of downloaded file after its downloading.
+Use to adjust the file name after downloading.
 
-Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is taken from the link to podcast file.
+Default value (the `%file_name%.%file_extension%`) will simple save up the file as it was uploaded by original creator. The file name and its extension is based on the link to podcast file.
 
 Template values:
 
 | Name               | Notes                                                   |
 |:-------------------|:--------------------------------------------------------|
-| `%file_name%`      | The file name taken from link, without extension        |
-| `%file_extension%` | The extension for the file, taken from link             |
+| `%file_name%`      | The file name from the link, without extension          |
+| `%file_extension%` | The extension for the file, from link                   |
 | `%publish_date%`   | The publish date of the RSS entry                       |
 | `%title%`          | The title of the RSS entry                              |
 
-### Non default the publish_date
-
-The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change the date you can provide the new format after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
+### Non-default the publish_date
 
+The `%publish_date%` by default gives result in format `YEARMMDD`. In order to change it you can provide the new one after the colon (the `:` character). The script respect the codes [of the 1989 C standard](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes), but the percent sign (`%`) must be replaced by dollar sign (`$`). This is because of my unfortunate decision to use the percent character as marker of the code.
 
 | The standard code | The script code | Notes                                      |
 |:------------------|:----------------|:-------------------------------------------|
 | `%Y%m%d`          | `$Y$m$d`        | The default value of the `%publish_date%`  |
 | `%A`              | `$A`            | Adds the weekday (local language settings) |
 | `%x`              | `$x`            | The local date represent. **Warning**: in some settings, the `/` is used here, so it may caused problem in the file name |
 
 ### Examples
 
 * `[%publish_date%] %file_name%.%file_extension%`
 * `[%publish_date%] %title%.%file_extension%`
 
 ## File types filter
 
-Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader will look just for them.
+Podcasts are mostly stored as `*.mp3` files. By default Podcast Downloader looks just for them, ignoring all others types.
 
-If your podcast support other types of media files, you can precised your own podcast file filter, by providing extension for the file (like `.mp3`), and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
+If your podcast supports other types of media files, you can specified the file filters. Provide the  extension of the file (like `.mp3`) and type of link in RSS feed itself (for `mp3` it is `audio/mpeg`).
 
-If you don't know the type of the file, you can check the RSS file. Seek for `enclosure` tags, should looks like this:
+If you don't know the type of the file, you can look for it in the RSS file. Seek for `enclosure` tags, should looks like this:
 
 ```xml
-  <enclosure
-    url="https://an.apple.supporter.page/podcast/episode23.m4a"
-    length="14527149"
-    type="audio/x-m4a" />
+  <enclosure url="https://www.vidocast.url/podcast/episode23.m4a"
+             length="14527149"
+             type="audio/x-m4a" />
 ```
 
-Notes: the dot on the file extension is require.
+**Note**: the dot on the file extension is require.
 
 ### Example
 
 ```json
   "podcast_extensions": {
     ".mp3": "audio/mpeg",
     ".m4a": "audio/x-m4a"
   }
 ```
 
 ## In case of empty directory
 
-If a directory for podcast is empty, the script needs to recognize what to do. Due to lack of database, you can:
+If a directory for podcast is empty, the script needs to know what to do. Due to lack of database, you can:
 
 * [download all episodes from feed](#download-all-from-feed)
-* [download only the last episode](#only-last)
-* [download last n episodes](#download-n-last-episodes)
+* [download only the last episode](#download-last)
+* [download last n episodes](#download-last-n-episodes)
 * [download all new episode from last n days](#download-all-from-n-days)
 * [download all new episode since day after, the last episode should appear](#download-all-episode-since-last-excepted)
 
+Default behavior is: `download_last`
+
 ### Download all from feed
 
 The script will download all episodes from the feed.
 
 Set by `download_all_from_feed`.
 
-### Only last
+### Download last
 
 The script will download only the last episode from the feed.
-It is a good approach when you wish to start listening the podcast.
 It is also default approach of the script.
 
 Set by `download_last`.
 
 ### Download last n episodes
 
-The script will download exactly given number of episodes from the feed.
+The script will download exactly the given number of episodes from the feed.
 
-Set by `download_last_n_episodes`. The *n* must be replaced by number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five last episodes will be downloaded.
+Set by `download_last_n_episodes`. The *n* must be replaced by a number of episodes, which you wanted to have downloaded. For example: `download_last_5_episodes` means that five most recent episodes will be downloaded.
 
 ### Download all from n days
 
-The script will download all episodes which appear in last *n* days. I can be use when you are downloading on regular schedule.
+The script will download all episodes which appear in recent *n* days. It can be use when you are downloading on regular schedule.
 The *n* number is given within the setup value: `download_from_n_days`. For example: `download_from_3_days` means download all episodes from last 3 days.
 
 ### Download all episode since last excepted
 
 The script will download all episodes which appear after the day of release of last episode.
 
 The *n* number is the day of the normal episode.
@@ -292,21 +330,21 @@
 |------------------------|---------|
 | `download_from_monday` | New episodes appear in Monday. The script will download all episodes since last Tuesday (including it) |
 | `download_from_Fri`    | New episodes appear in Friday. The script will download all episodes since last Saturday (including it) |
 | `download_from_12`     | New episodes appear each 12th of month. The script will download all episodes since 13 month before |
 
 ## Download files from gaps
 
-The script recognizes the stream of downloaded files (based on the feed). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situations where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed).
+The script recognizes the stream of downloaded files (based on the feed data). By default, the last downloaded file (according to the feed) marks the start of downloading. In case of gaps, situation where there are missing files before the last downloaded one, the script will ignore them by default. However, there is a possibility to change this behavior to download all missing files between already downloaded ones. To enable this, you need to set the `fill_up_gaps` value to **true**. It's important to note that the script will not download files before the first one (according to the feed), the most earlier episode.
 
 Default value: `false`.
 
 ## The analyze of the RSS feed
 
-The script is look through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
+The script looks through all the `items` nodes in RSS file. The `item` node can contain the `enclosure` node. Those nodes are used to passing the files. According to the convention the single `item` should contain only one `enclosure`, but script (as [the library used](https://pypi.org/project/feedparser/) under it) can handle the multiple files attached into podcast `item`.
 
 ## Converting the OPML
 
 The [OPML](https://en.wikipedia.org/wiki/OPML) files can be converted into [configuration](#configuration). The output file needs to be adjusted (missing the `path`).
 
 ```py
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `podcast_downloader-0.8.0/setup.py` & `podcast_downloader-1.8.1/setup.py`

 * *Files identical despite different names*

