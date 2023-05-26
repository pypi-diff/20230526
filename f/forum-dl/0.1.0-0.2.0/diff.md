# Comparing `tmp/forum_dl-0.1.0.tar.gz` & `tmp/forum_dl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forum_dl-0.1.0.tar", last modified: Fri May 19 00:26:44 2023, max compression
+gzip compressed data, was "forum_dl-0.2.0.tar", last modified: Fri May 26 17:46:54 2023, max compression
```

## Comparing `forum_dl-0.1.0.tar` & `forum_dl-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-19 00:26:44.629667 forum_dl-0.1.0/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1072 2023-02-05 02:04:17.000000 forum_dl-0.1.0/LICENSE
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3315 2023-05-19 00:26:44.626334 forum_dl-0.1.0/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2975 2023-05-17 19:02:56.000000 forum_dl-0.1.0/README.md
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-19 00:26:44.623000 forum_dl-0.1.0/forum_dl/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1432 2023-05-18 19:08:10.000000 forum_dl-0.1.0/forum_dl/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       85 2023-05-18 01:32:50.000000 forum_dl-0.1.0/forum_dl/__main__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      442 2023-04-26 17:44:14.000000 forum_dl-0.1.0/forum_dl/exceptions.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-19 00:26:44.626334 forum_dl-0.1.0/forum_dl/extractors/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1244 2023-04-26 17:47:41.000000 forum_dl-0.1.0/forum_dl/extractors/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     9397 2023-05-18 19:25:36.000000 forum_dl-0.1.0/forum_dl/extractors/common.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8081 2023-05-16 00:08:31.000000 forum_dl-0.1.0/forum_dl/extractors/discourse.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10688 2023-05-16 01:15:05.000000 forum_dl-0.1.0/forum_dl/extractors/hackernews.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11021 2023-05-12 14:05:14.000000 forum_dl-0.1.0/forum_dl/extractors/hyperkitty.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7085 2023-05-18 19:25:55.000000 forum_dl-0.1.0/forum_dl/extractors/hypermail.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8430 2023-05-16 00:27:49.000000 forum_dl-0.1.0/forum_dl/extractors/invision.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13455 2023-05-17 19:03:08.000000 forum_dl-0.1.0/forum_dl/extractors/phpbb.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11594 2023-05-18 19:25:47.000000 forum_dl-0.1.0/forum_dl/extractors/pipermail.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13255 2023-05-13 22:43:53.000000 forum_dl-0.1.0/forum_dl/extractors/proboards.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     9935 2023-05-18 19:26:03.000000 forum_dl-0.1.0/forum_dl/extractors/simplemachines.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13986 2023-05-16 00:37:45.000000 forum_dl-0.1.0/forum_dl/extractors/vbulletin.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13787 2023-05-14 20:25:39.000000 forum_dl-0.1.0/forum_dl/extractors/xenforo.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1475 2023-05-18 18:51:44.000000 forum_dl-0.1.0/forum_dl/forumdl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3157 2023-05-16 18:50:37.000000 forum_dl-0.1.0/forum_dl/options.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3319 2023-05-18 19:25:16.000000 forum_dl-0.1.0/forum_dl/session.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5207 2023-05-18 23:13:35.000000 forum_dl-0.1.0/forum_dl/soup.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       93 2023-04-20 02:45:45.000000 forum_dl-0.1.0/forum_dl/version.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-19 00:26:44.626334 forum_dl-0.1.0/forum_dl/writers/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1049 2023-04-29 13:42:22.000000 forum_dl-0.1.0/forum_dl/writers/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      487 2023-04-28 23:15:46.000000 forum_dl-0.1.0/forum_dl/writers/babyl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7797 2023-05-18 19:51:25.000000 forum_dl-0.1.0/forum_dl/writers/common.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      293 2023-05-04 19:53:33.000000 forum_dl-0.1.0/forum_dl/writers/jsonl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      544 2023-04-28 23:39:06.000000 forum_dl-0.1.0/forum_dl/writers/maildir.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      466 2023-04-28 23:15:14.000000 forum_dl-0.1.0/forum_dl/writers/mbox.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      519 2023-04-28 23:39:11.000000 forum_dl-0.1.0/forum_dl/writers/mh.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      482 2023-04-28 23:15:32.000000 forum_dl-0.1.0/forum_dl/writers/mmdf.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-19 00:26:44.623000 forum_dl-0.1.0/forum_dl.egg-info/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     3315 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1022 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/SOURCES.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/entry_points.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       82 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/requires.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        9 2023-05-19 00:26:44.000000 forum_dl-0.1.0/forum_dl.egg-info/top_level.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      625 2023-05-19 00:00:07.000000 forum_dl-0.1.0/pyproject.toml
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-05-19 00:26:44.629667 forum_dl-0.1.0/setup.cfg
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1072 2023-02-05 02:04:17.000000 forum_dl-0.2.0/LICENSE
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4939 2023-05-26 17:46:54.116119 forum_dl-0.2.0/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4323 2023-05-26 17:36:07.000000 forum_dl-0.2.0/README.md
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.112786 forum_dl-0.2.0/forum_dl/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1776 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       85 2023-05-18 01:32:50.000000 forum_dl-0.2.0/forum_dl/__main__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      489 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/exceptions.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/forum_dl/extractors/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1244 2023-04-26 17:47:41.000000 forum_dl-0.2.0/forum_dl/extractors/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10283 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/common.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8521 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/discourse.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10911 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hackernews.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11669 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hyperkitty.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7394 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hypermail.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8648 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/invision.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13814 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/phpbb.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11956 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/pipermail.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13624 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/proboards.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    17288 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/simplemachines.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    14240 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/vbulletin.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    14012 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/xenforo.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1475 2023-05-18 18:51:44.000000 forum_dl-0.2.0/forum_dl/forumdl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4323 2023-05-26 17:33:51.000000 forum_dl-0.2.0/forum_dl/options.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4780 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/session.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5207 2023-05-18 23:13:35.000000 forum_dl-0.2.0/forum_dl/soup.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       93 2023-04-20 02:45:45.000000 forum_dl-0.2.0/forum_dl/version.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/forum_dl/writers/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1057 2023-05-26 01:03:26.000000 forum_dl-0.2.0/forum_dl/writers/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      487 2023-04-28 23:15:46.000000 forum_dl-0.2.0/forum_dl/writers/babyl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8243 2023-05-21 03:00:29.000000 forum_dl-0.2.0/forum_dl/writers/common.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      293 2023-05-04 19:53:33.000000 forum_dl-0.2.0/forum_dl/writers/jsonl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      544 2023-04-28 23:39:06.000000 forum_dl-0.2.0/forum_dl/writers/maildir.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      466 2023-04-28 23:15:14.000000 forum_dl-0.2.0/forum_dl/writers/mbox.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      519 2023-04-28 23:39:11.000000 forum_dl-0.2.0/forum_dl/writers/mh.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      482 2023-04-28 23:15:32.000000 forum_dl-0.2.0/forum_dl/writers/mmdf.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      278 2023-05-26 01:03:30.000000 forum_dl-0.2.0/forum_dl/writers/warc.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.112786 forum_dl-0.2.0/forum_dl.egg-info/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4939 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1047 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/entry_points.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       92 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/requires.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        9 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/top_level.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      992 2023-05-26 17:46:46.000000 forum_dl-0.2.0/pyproject.toml
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-05-26 17:46:54.116119 forum_dl-0.2.0/setup.cfg
```

### Comparing `forum_dl-0.1.0/LICENSE` & `forum_dl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/PKG-INFO` & `forum_dl-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-Metadata-Version: 2.1
-Name: forum_dl
-Version: 0.1.0
-Summary: Download posts and threads from forums, news aggregators, mail archives
-Author-email: Mikolaj Wielgus <wielgusmikolaj@gmail.com>
-License: MIT
-Requires-Python: >=3.10.11
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: html2text
-License-File: LICENSE
-
 # forum-dl
 
-Forum-dl is a downloader (scraper) for forums, mailing lists, and news aggregators. It can be used to crawl, extract, and archive individual threads and entire boards into a variety of output formats.
+Forum-dl is a scraper and archiver for forums (including Discourse, PhpBB, SMF), mailing lists, and news aggregators ([list](#forum-software)). It can be used to extract and archive all posts from individual threads and entire boards into JSONL, Mbox, Maildir, WARC ([complete list](#output-formats)).
+
+<sub>The project is currently in alpha stage. Please do not hesitate to [file](https://github.com/mikwielgus/forum-dl/issues) bug reports and feature requests.</sub>
+
+![image](https://github.com/mikwielgus/forum-dl/assets/58011230/e677d1aa-efa3-4cfc-9283-38408842b278)
 
 # Installation
 
-Clone the repository:
+You can install Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
+
+## PIP
+
+Install the latest stable version of Forum-dl from PIP:
 
 ```
-git clone https://github.com/mikwielgus/forum-dl
+pip install forum-dl
 ```
 
-Then, in the same directory, install the repository directly: 
+## Repository 
+
+Clone the repository and install it in editable mode:
 
 ```
-pip install -e forum-dl
+git clone https://github.com/mikwielgus/forum-dl && pip install -e forum-dl
 ```
 
-# Quick start
+# Usage examples
 
-Download a Simple Machines forum thread in JSONL format:
+Download a Simple Machines Forum thread in JSONL format:
 
 ```
 forum-dl "https://www.simplemachines.org/community/index.php?topic=584230.0"
 ```
 
-Download an entire PhpBB forum board in JSONL format, write to stdout (`-o -`).
+Download an entire PhpBB board into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
 
 ```
 forum-dl -o - "https://www.phpbb.com/community/viewforum.php?f=696"
 ```
 
-<sub>(due to current architecture limitations, `forum-dl` will shallowly scan the entire forum hierarchy before downloading the board. This will be fixed in future releases)</sub>
+<sub>(due to current architectural limitations, `forum-dl` will scan the first page of each board in the entire forum before downloading the target board. This will be fixed in future releases)</sub>
 
 Download Hacker News top stories and write them to a Maildir directory `hn`:
 
 ```
 forum-dl --textify --content-as-title -f maildir -o hn "https://news.ycombinator.com/news"
 ```
 
@@ -75,43 +73,58 @@
 
 - Babyl
 - JSONL
 - Maildir
 - Mbox
 - MH
 - MMDF
+- WARC
 
 # Usage
 
 ```
-forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE]
-         [-f FORMAT] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [-R RETRIES] [--retry-sleep RETRY_SLEEP]
+         [--retry-sleep-multiplier RETRY_SLEEP_MULTIPLIER] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE] [-f FORMAT]
+         [--warc-output FILE] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+         [--author-as-addr-spec]
 ```
 
 ## General Options:
 
 ```
   --help                Show this help message and exit
   --version             Print program version and exit
   --list-extractors     List all supported extractors and exit
   --list-output-formats
                         List all supported output formats and exit
-  --user-agent USER_AGENT
-                        User-Agent request header
+```
+
+## Session Options:
+
+```
+  -R N, --retries N     Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)
+  --retry-sleep SECONDS
+                        Time to sleep between retries, in seconds (default: 1)
+  --retry-sleep-multiplier K
+                        A constant by which sleep time is multiplied on each retry (default: 2)
+  --user-agent UA       User-Agent request header
 ```
 
 ## Output Options:
 
 ```
   -q, --quiet           Activate quiet mode
   -v, --verbose         Print various debugging information
   -g, --get-urls        Print URLs instead of downloading
   -o FILE, --output FILE
                         Output all results concatenated to FILE, or stdout if FILE is -
   -f FORMAT, --output-format FORMAT
-                        Output format
+                        Output format. Use --list-output-formats for a list of possible arguments
+  --warc-output FILE    Record HTTP requests, store them in FILE in WARC format
   --no-boards           Do not write board objects
   --no-threads          Do not write thread objects
   --no-posts            Do not write post objects
   --textify             Lossily convert HTML content to plaintext
   --content-as-title    Write 98 initial characters of content in title field of each post
+  --author-as-addr-spec
+                        Append author and domain as an addr-spec in the From header
 ```
```

### Comparing `forum_dl-0.1.0/forum_dl/__init__.py` & `forum_dl-0.2.0/forum_dl/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,26 +24,33 @@
         print("\n".join(forumdl.list_output_formats()))
     elif not args.urls:
         parser.error(
             "The following arguments are required: URL\n"
             "Use 'forum-dl --help' to get a list of all options."
         )
     else:
+        warc_output = args.output if args.output_format == "warc" else args.warc_output
+
         forumdl.download(
             urls=args.urls,
             output_format=args.output_format,
             session_options=SessionOptions(
+                retries=args.retries,
+                retry_sleep=args.retry_sleep,
+                retry_sleep_multiplier=args.retry_sleep_multiplier,
+                warc_output=warc_output,
                 user_agent=args.user_agent,
                 get_urls=args.get_urls,
             ),
             extractor_options=ExtractorOptions(
                 path=False,
             ),
             writer_options=WriterOptions(
                 output_path=args.output,
                 write_board_objects=args.boards,
                 write_thread_objects=args.threads,
                 write_post_objects=args.posts,
-                content_as_title=args.content_as_title,
                 textify=args.textify,
+                content_as_title=args.content_as_title,
+                author_as_addr_spec=args.author_as_addr_spec,
             ),
         )
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/__init__.py` & `forum_dl-0.2.0/forum_dl/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/forum_dl/extractors/common.py` & `forum_dl-0.2.0/forum_dl/extractors/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from urllib.parse import urlparse, urlunparse, parse_qs, urlencode
 from pathlib import PurePosixPath
+import logging
+import traceback
 
 from ..session import Session
 from ..exceptions import SearchError
 from ..version import __version__
 
 
 def get_relative_url(url: str, base_url: str):
@@ -64,14 +66,27 @@
 
         if result:
             return result
 
     raise ValueError
 
 
+def regex_search(pattern: Pattern[str], strings: list[str] | str):
+    if isinstance(strings, str):
+        strings = [strings]
+
+    for string in strings:
+        result = pattern.search(string)
+
+        if result:
+            return result
+
+    raise ValueError
+
+
 @dataclass
 class ExtractorOptions:
     path: bool
 
 
 @dataclass  # (kw_only=True)
 class PageState:
@@ -86,14 +101,15 @@
     data: dict[str, Any]
 
 
 @dataclass
 class Post(Item):
     subpath: tuple[str, ...]
     author: str
+    creation_time: str
     content: str
 
 
 @dataclass
 class Thread(Item):
     title: str
 
@@ -204,16 +220,24 @@
                 self._fetch_subboards(cur_board)
 
             i += 1
 
         if not board.path:
             self._are_all_boards_fetched = True
 
-    @abstractmethod
+    @final
     def _fetch_subboards(self, board: Board):
+        try:
+            self._do_fetch_subboards(board)
+        except Exception as e:
+            logging.warning(repr(e))
+            logging.warning(traceback.format_exc())
+
+    @abstractmethod
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _resolve_url(self, url: str):
         return url
 
     @abstractmethod
     def _get_node_from_url(self, url: str) -> Item | tuple[str, ...]:
@@ -262,26 +286,26 @@
         node = self._get_node_from_url(self._resolve_url(url))
 
         if isinstance(node, Board):
             return self.find_board(node.path)
 
         return node
 
-    def _fetch_lazy_subboard(self, board: Board, id: str) -> Board | None:
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str) -> Board | None:
         if not self._are_subboards_fetched[board.path]:
             for _ in self._fetch_lazy_subboards(board):
                 pass
 
             self._are_subboards_fetched[board.path] = True
 
-        return self._subboards[board.path][id]
+        return self._subboards[board.path][subboard_id]
 
     @abstractmethod
     def _fetch_lazy_subboards(self, board: Board) -> Generator[Board, None, None]:
-        self._fetch_subboards(board)
+        self._do_fetch_subboards(board)
         return iter(self._subboards[board.path])
 
     @final
     def subboards(self, board: Board):
         if not self._are_subboards_fetched[board.path]:
             for _ in self._fetch_lazy_subboards(board):
                 pass
@@ -296,35 +320,43 @@
     ) -> Generator[Thread, None, PageState | None]:
         pass
 
     @final
     def _fetch_board_threads(
         self, board: Board, initial_state: PageState | None = None
     ):
-        self.board_state = initial_state or PageState(url=board.url)
-        while self.board_state:
-            self.board_state = yield from self._fetch_board_page_threads(
-                board, self.board_state
-            )
+        try:
+            self.board_state = initial_state or PageState(url=board.url)
+            while self.board_state:
+                self.board_state = yield from self._fetch_board_page_threads(
+                    board, self.board_state
+                )
+        except Exception as e:
+            logging.warning(repr(e))
+            logging.warning(traceback.format_exc())
 
     @abstractmethod
     def _fetch_thread_page_posts(
         self, thread: Thread, state: PageState
     ) -> Generator[Post, None, PageState | None]:
         pass
 
     @final
     def _fetch_thread_posts(
         self, thread: Thread, initial_state: PageState | None = None
     ):
-        self.thread_state = initial_state or PageState(url=thread.url)
-        while self.thread_state:
-            self.thread_state = yield from self._fetch_thread_page_posts(
-                thread, self.thread_state
-            )
+        try:
+            self.thread_state = initial_state or PageState(url=thread.url)
+            while self.thread_state:
+                self.thread_state = yield from self._fetch_thread_page_posts(
+                    thread, self.thread_state
+                )
+        except Exception as e:
+            logging.warning(repr(e))
+            logging.warning(traceback.format_exc())
 
     @final
     def threads(self, board: Board, initial_state: PageState | None = None):
         yield from self._fetch_board_threads(board, initial_state)
 
     @final
     def posts(self, thread: Thread, initial_state: PageState | None = None):
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/discourse.py` & `forum_dl-0.2.0/forum_dl/extractors/discourse.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     ]
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         url = url.removesuffix("/").removesuffix(".json")
         url = url.removesuffix(".json")
 
-        response = session.get_noretry(normalize_url(url))
+        response = session.try_get(
+            normalize_url(url), should_cache=True, should_retry=False
+        )
         soup = Soup(response.content)
 
         crawler_nav = soup.find("nav", class_="crawler-nav")
         home_anchor = crawler_nav.find("a")
         base_url = urljoin(response.url, home_anchor.get("href"))
 
         return DiscourseExtractor(session, normalize_url(base_url), options)
@@ -74,41 +76,43 @@
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
         response = self._session.get(urljoin(self.base_url, "site.json"))
         site_json = response.json()
 
         for category_data in site_json["categories"]:
             if "parent_category_id" not in category_data:
-                id = str(category_data["id"])
+                category_id = str(category_data["id"])
 
                 self._set_board(
-                    path=(id,),
-                    url=urljoin(self.base_url, f"c/{category_data['slug']}/{id}"),
+                    path=(category_id,),
+                    url=urljoin(
+                        self.base_url, f"c/{category_data['slug']}/{category_id}"
+                    ),
                     origin=response.url,
                     data=category_data,
                     title=category_data["name"],
                     are_subboards_fetched=True,
                 )
 
         for category_data in site_json["categories"]:
             if "parent_category_id" in category_data:
                 slug = category_data["slug"]
-                id = str(category_data["id"])
+                category_id = str(category_data["id"])
                 parent_id = str(category_data["parent_category_id"])
 
                 self._set_board(
-                    path=(parent_id, id),
-                    url=urljoin(self.base_url, f"c/{slug}/{id}"),
+                    path=(parent_id, category_id),
+                    url=urljoin(self.base_url, f"c/{slug}/{category_id}"),
                     origin=response.url,
                     data=category_data,
                     title=category_data["name"],
                     are_subboards_fetched=True,
                 )
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
         url = url.removesuffix(".json")
 
         relative_url = get_relative_url(url, self.base_url)
         url_parts = PurePosixPath(relative_url).parts
@@ -123,43 +127,43 @@
                 if board.data["slug"] == slug:
                     return board
 
                 for _, subboard in self._subboards[board.path].items():
                     if subboard.data["slug"] == slug:
                         return subboard
         elif url_parts[0] == "t":
-            id = url_parts[1]
-            json_url = urljoin(self.base_url, f"t/{id}.json")
-            response = self._session.get(json_url)
+            topic_id = url_parts[1]
+            json_url = urljoin(self.base_url, f"t/{topic_id}.json")
+            response = self._session.get(json_url, should_cache=True)
             data = response.json()
 
             slug = data["slug"]
             category_id = str(data["category_id"])
 
             if category_id in self._subboards[self.root.path]:
-                path = (category_id, f"{id}")
+                path = (category_id, f"{topic_id}")
             else:
                 for _, subboard in self._subboards[self.root.path].items():
                     if category_id in self._subboards[self.root.path]:
-                        path = subboard.path + (category_id, f"{id}")
+                        path = subboard.path + (category_id, f"{topic_id}")
                         break
                 else:
                     raise ValueError
 
             return Thread(
                 path=path,
                 url=url,
                 origin=response.url,
                 data=data,
                 title=data["title"],
             )
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if state.url == board.url:
@@ -171,18 +175,18 @@
 
             state.url = f"{state.url}.json"
 
         response = self._session.get(state.url)
         page_json = response.json()
 
         for data in page_json["topic_list"]["topics"]:
-            id = str(data["id"])
+            topic_id = str(data["id"])
             yield Thread(
-                path=board.path + (id,),
-                url=urljoin(self.base_url, f"t/{data['slug']}/{id}"),
+                path=board.path + (topic_id,),
+                url=urljoin(self.base_url, f"t/{data['slug']}/{topic_id}"),
                 origin=response.url,
                 data=data,
                 title=data["title"],
             )
 
         if more_topics_url := page_json["topic_list"].get("more_topics_url", None):
             parsed_more_topics_url = urlparse(str(more_topics_url))
@@ -202,32 +206,37 @@
             state = DiscourseThreadPageState(
                 url=response.url, stream_data=page_json["post_stream"]["stream"]
             )
         else:
             origin = state.url
             state = cast(DiscourseThreadPageState, state)
             post_ids = tuple(state.stream_data[:20])
-            response = self._session.uncached_get(
-                origin, params={"post_ids[]": post_ids}
+            response = self._session.get(
+                origin,
+                params={"post_ids[]": post_ids},
+                should_cache=False,
             )
             page_json = response.json()
 
         datas = page_json["post_stream"]["posts"]
 
         for data in datas:
             topic_slug = data["topic_slug"]
+            topic_id = data["topic_id"]
+            post_number = data["post_number"]
 
             state.stream_data.pop(0)
             yield Post(
                 path=thread.path,
                 subpath=(str(data["id"]),),
-                url=urljoin(self.base_url, f"t/{topic_slug}/{id}"),
+                url=urljoin(self.base_url, f"t/{topic_slug}/{topic_id}/{post_number}"),
                 origin=response.url,
                 data=data,
                 author=data.get("username", None),
+                creation_time=data.get("created_at", None),
                 content=data.get("cooked", None),
             )
 
         topic_id = str(page_json["id"])
 
         if state.stream_data:
             state.url = urljoin(self.base_url, f"t/{topic_id}/posts.json")
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/hackernews.py` & `forum_dl-0.2.0/forum_dl/extractors/hackernews.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from abc import abstractmethod
 from urllib.parse import urljoin, urlparse, parse_qs
 import logging
+from datetime import datetime
 
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 
 
 class HackernewsExtractor(Extractor):
     tests = [
@@ -109,15 +110,15 @@
         return (item_id - 1) // self.PAGE_SIZE
 
     def _fetch_top_boards(self):
         firebase_url = f"https://hacker-news.firebaseio.com/v0/maxitem.json"
         self._max_item_id = int(self._session.get(firebase_url).content)
         self.pages: list[list[int]] = [[]] * (1 + self._calc_page_id(self._max_item_id))
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
         parsed_url = urlparse(url)
 
         # The whole site.
         # TODO: Do this `if` properly by normalizing the URL beforehand.
@@ -128,15 +129,15 @@
             parsed_query = parse_qs(parsed_url.query)
             item_id = str(parsed_query["id"][0])
 
             return self._fetch_item_thread(int(item_id))
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _get_is_fetchable(self, item_id: int):
         if item_id > self._max_item_id:
@@ -157,15 +158,15 @@
 
         self.pages[page_id].append(item_id)
         return True
 
     def _fetch_item_thread(self, item_id: int):
         while True:
             firebase_url = f"https://hacker-news.firebaseio.com/v0/item/{item_id}.json"
-            response = self._session.get(firebase_url)
+            response = self._session.get(firebase_url, should_cache=True)
             data = response.json()
 
             if "parent" in data:
                 item_id = data["parent"]
             else:
                 page_id = self._calc_page_id(item_id)
                 self.pages[page_id].append(item_id)
@@ -219,40 +220,43 @@
         post_paths: list[tuple[str, ...]] = [()]
 
         i = 0
         while True:
             post_path = post_paths[i]
 
             if post_path:
-                id = post_path[-1]
+                post_id = post_path[-1]
             else:
-                id = thread.path[-1]
+                post_id = thread.path[-1]
 
-            firebase_url = f"https://hacker-news.firebaseio.com/v0/item/{id}.json"
+            firebase_url = f"https://hacker-news.firebaseio.com/v0/item/{post_id}.json"
 
             response = self._session.get(firebase_url)
             data = response.json()
 
             if data:
-                self._register_item(int(id))
+                self._register_item(int(post_id))
                 yield Post(
                     path=thread.path,
                     subpath=post_path,
                     url=thread.url,
                     origin=response.url,
                     data=data,
                     author=data.get("by", ""),
+                    creation_time=datetime.utcfromtimestamp(
+                        data.get("time")
+                    ).isoformat(),
                     content=data.get("text", ""),
                 )
 
                 for kid_id in data.get("kids", []):
                     post_paths.append(post_path + (str(kid_id),))
 
             else:
-                logging.warning(f"Item at id={post_path[-1]} is null")
+                logging.warning(f"Item at post_id={post_path[-1]} is null")
 
             i += 1
             if i == len(post_paths):
                 break
 
 
 class HackernewsSpecificExtractor(HackernewsExtractor):
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/hyperkitty.py` & `forum_dl-0.2.0/forum_dl/extractors/hyperkitty.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse
+import dateutil.parser
 import re
 
 from .common import normalize_url
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 from ..soup import Soup
 
@@ -67,15 +68,19 @@
         },
     ]
 
     _reply_level_regex = re.compile(r"reply-level-(\d+)")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(normalize_url(url, append_slash=False))
+        response = session.try_get(
+            normalize_url(url, append_slash=False),
+            should_cache=True,
+            should_retry=False,
+        )
         soup = Soup(response.content)
 
         if extractor := HyperkittyExtractor.detect_postorius(
             session, url, soup, options
         ):
             return extractor
 
@@ -115,19 +120,19 @@
 
         base_url = normalize_url(urljoin(url, navbar_brand_anchor.get("href")))
         return HyperkittyExtractor(session, base_url, options)
 
     def _fetch_top_boards(self):
         pass
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         resolved_url = normalize_url(response.url)
 
         if resolved_url == self.base_url:
             return self.root
 
         parsed_url = urlparse(resolved_url)
         path = PurePosixPath(parsed_url.path)
@@ -148,53 +153,50 @@
                 title=thread_h3.string,
             )
         elif len(path.parts) >= 2 and path.parts[-2] == "list":
             return self.find_board((path.parts[-1],))
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
-        url = normalize_url(urljoin(self.base_url, f"list/{id}"))
-        response = self._session.get(url)
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
+        url = normalize_url(urljoin(self.base_url, f"list/{subboard_id}"))
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         title = ""
 
         if title_section := soup.try_find("section", id="title"):
             if h1 := title_section.try_find("h1"):
                 title = h1.string.strip()
             elif h2 := title_section.try_find("h2"):
                 title = h2.string.strip()
 
-        # description = ""
-
-        # if description_section := soup.find("p", id="description"):
-        # description = description_section.string
-
         return self._set_board(
-            path=(id,),
+            path=(subboard_id,),
             url=url,
             origin=response.url,
             data={},
             # data={"description": description},
             title=title,
         )
 
     def _fetch_lazy_subboards(self, board: Board):
         href: str = ""
         url: str = self.base_url
 
         while href != "#":
-            response = self._session.get(url)
+            response = self._session.get(url, should_cache=True)
             soup = Soup(response.content)
             list_anchors = soup.find_all("a", class_="list-name")
 
             for list_anchor in list_anchors:
-                id = PurePosixPath(urlparse(list_anchor.get("href")).path).parts[-1]
-                yield self._fetch_lazy_subboard(board, id)
+                list_id = PurePosixPath(urlparse(list_anchor.get("href")).path).parts[
+                    -1
+                ]
+                yield self._fetch_lazy_subboard(board, list_id)
 
             page_link_anchors = soup.find_all("a", class_="page-link")
             next_page_anchor = page_link_anchors[-1]
 
             href = next_page_anchor.get("href")
             url = urljoin(self.base_url, href)
 
@@ -242,26 +244,31 @@
         origin = state.url
         response = self._session.get(origin)
 
         if state.url == thread.url:
             soup = Soup(response.content)
 
             email_author_div = soup.find("div", class_="email-author")
+            email_time_div = soup.find("div", class_="time")
+            email_time_span = email_time_div.find("span")
+            time = email_time_span.get("title").removeprefix("Sender's time: ")
+
             email_body_div = soup.find("div", class_="email-body")
 
             yield Post(
                 path=thread.path,
                 subpath=(),
                 url=urljoin(
                     origin,
                     soup.find("div", class_="messagelink").find("a").get("href"),
                 ),
                 origin=origin,
                 data={},
                 author=str(email_author_div.find("a").string),
+                creation_time=dateutil.parser.parse(time).isoformat(),
                 content="".join(str(v) for v in email_body_div.contents),
             )
 
             return PageState(url=urljoin(state.url, "replies?sort=thread"))
 
         json = response.json()
 
@@ -277,33 +284,39 @@
                 if match := self._reply_level_regex.match(klass):
                     cur_reply_level = int(match.group(1))
                     break
             else:
                 cur_reply_level = 0
 
             email_header_div = reply_level_div.find("div", class_="email-header")
-            id = email_header_div.get("id")
+            post_id = email_header_div.get("id")
 
             if cur_reply_level > prev_reply_level:
-                subpath.append(id)
+                subpath.append(post_id)
             else:
-                subpath[-(prev_reply_level - cur_reply_level - 1) :] = [id]
+                subpath[-(prev_reply_level - cur_reply_level - 1) :] = [post_id]
 
             email_author_div = reply_level_div.find("div", class_="email-author")
+
+            email_time_div = soup.find("div", class_="time")
+            email_time_span = email_time_div.find("span")
+            time = email_time_span.get("title").removeprefix("Sender's time: ")
+
             email_body_div = reply_level_div.find("div", class_="email-body")
 
             yield Post(
                 path=thread.path,
                 subpath=tuple(subpath),
                 url=urljoin(
                     origin, soup.find("div", class_="messagelink").find("a").get("href")
                 ),
                 origin=origin,
                 data={},
                 author=str(email_author_div.find("a").string),
+                creation_time=dateutil.parser.parse(time).isoformat(),
                 content="".join(str(v) for v in email_body_div.contents),
             )
 
             prev_reply_level = cur_reply_level
 
         if json["more_pending"]:
             next_offset = json["next_offset"]
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/hypermail.py` & `forum_dl-0.2.0/forum_dl/extractors/hypermail.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,18 @@
     ]
 
     _page_href_regex = re.compile(r"^(\d+)/index.html$")
     _post_href_regex = re.compile(r"^(\d+).html$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(
-            normalize_url(url, remove_suffixes=[], append_slash=False)
+        response = session.try_get(
+            normalize_url(url, remove_suffixes=[], append_slash=False),
+            should_cache=True,
+            should_retry=False,
         )
         soup = Soup(response.content)
 
         _ = soup.find(
             "meta",
             attrs={"name": "generator", "content": re.compile("^hypermail.*$")},
         )
@@ -74,40 +76,40 @@
             return HypermailExtractor(session, base_url, options)
 
         return HypermailExtractor(session, response.url, options)
 
     def _fetch_top_boards(self):
         pass
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         resolved_url = normalize_url(response.url, append_slash=False)
 
         if resolved_url == self.base_url:
             return self.root
 
         parsed_url = urlparse(resolved_url)
         path = PurePosixPath(parsed_url.path)
 
         if len(path.parts) >= 2 and self._post_href_regex.match(path.parts[-1]):
-            id = path.parts[-1].removesuffix(".html")
+            thread_id = path.parts[-1].removesuffix(".html")
             return Thread(
-                path=(id,),
+                path=(thread_id,),
                 url=url,
                 origin=resolved_url,
                 data={},
                 title="",  # TODO.
             )
 
         return self.root
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if state.url == board.url:
@@ -140,17 +142,17 @@
                 thread_anchor := child_ul.try_find(
                     "a", attrs={"href": self._post_href_regex}
                 )
             ):
                 continue
 
             href = thread_anchor.get("href")
-            id = regex_match(self._post_href_regex, href).group(1)
+            thread_id = regex_match(self._post_href_regex, href).group(1)
             yield Thread(
-                path=(id,),
+                path=(thread_id,),
                 url=urljoin(self.base_url, href),
                 origin=response.url,
                 data={},
                 title="",  # TODO.
             )
 
         if state.relative_urls:
@@ -180,20 +182,20 @@
         subpath: list[str] = []
 
         for child_anchor in child_anchors:
             child_pos = len(list(child_anchor.parents))
             cur_depth = (child_pos - root_pos) // 2
 
             href = child_anchor.get("href")
-            id = regex_match(self._post_href_regex, href).group(1)
+            post_id = regex_match(self._post_href_regex, href).group(1)
 
             if cur_depth > prev_depth:
-                subpath.append(id)
+                subpath.append(post_id)
             else:
-                subpath[-(prev_depth - cur_depth - 1) :] = [id]
+                subpath[-(prev_depth - cur_depth - 1) :] = [post_id]
 
             yield self._fetch_post(
                 state, thread.path, tuple(subpath), urljoin(state.url, href)
             )
 
             prev_depth = cur_depth
 
@@ -205,18 +207,22 @@
         url: str,
     ):
         response = self._session.get(url)
         soup = Soup(response.content)
 
         author_meta = soup.find("meta", attrs={"name": "Author"})
 
+        # TODO: We can use the isosent=... comment instead.
+        date_meta = soup.find("meta", attrs={"name": "Date"})
+
         address = soup.find("address")
 
         return Post(
             path=path,
             subpath=subpath,
             url=url,
             origin=response.url,
             data={},
             author=author_meta.get("content"),
+            creation_time=date_meta.get("content"),
             content="".join(str(v) for v in islice(address.next_siblings, 1, None)),
         )
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/invision.py` & `forum_dl-0.2.0/forum_dl/extractors/invision.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             "test_contents_hash": "1e0e0413cf82cf82bf83cfdf69813309594a06e4",
             "test_item_count": 52,
         },
     ]
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(url)
+        response = session.try_get(url, should_cache=True, should_retry=False)
         soup = Soup(response.content)
 
         breadcrumbs_ul = soup.find("ul", attrs={"data-role": "breadcrumbList"})
         breadcrumb_lis = breadcrumbs_ul.find_all("li")
         base_url = url
 
         if len(breadcrumb_lis) >= 2:
@@ -83,15 +83,15 @@
 
         if soup.find("a", attrs={"title": "Invision Community"}):
             return InvisionExtractor(session, base_url, options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
-        response = self._session.get(self.base_url)
+        response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
         category_lis = soup.find_all("li", class_="cForumRow")
         for category_li in category_lis:
             category_id = category_li.get("data-categoryid")
             category_anchor = category_li.find("h2").find_all("a")[1]
 
@@ -117,19 +117,19 @@
                     data={},
                     title=category_anchor.string,
                     are_subboards_fetched=True,
                 )
 
         self._fetch_lower_boards(self.root)
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         if board is self.root:
             return
 
-        response = self._session.get(board.url)
+        response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
         subboard_divs = soup.find_all("div", class_="cForumGrid")
         for subboard_div in subboard_divs:
             subboard_id = subboard_div.get("data-forumid")
             subboard_h3 = subboard_div.find("h3")
             subboard_anchor = subboard_h3.find("a")
@@ -140,15 +140,15 @@
                 origin=response.url,
                 data={},
                 title=subboard_anchor.string,
                 are_subboards_fetched=True,
             )
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         breadcrumbs_ul = soup.find("ul", attrs={"data-role": "breadcrumbList"})
         breadcrumb_lis = breadcrumbs_ul.find_all("li")
 
         if len(breadcrumb_lis) <= 2:
             return self.root
@@ -172,15 +172,15 @@
         else:
             for cur_board in self._boards:
                 if cur_board.url == url:
                     return cur_board
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if board is self.root:
@@ -216,26 +216,29 @@
         content_articles = soup.find_all("article", class_="ipsComment")
 
         for content_article in content_articles:
             content_div = content_article.find(
                 "div", attrs={"data-role": "commentContent"}
             )
             author_div = content_article.find("div", class_="cAuthorPane_content")
+            time_tag = author_div.find("time")
+
             author_h3 = author_div.find("h3", class_="cAuthorPane_author")
             url_div = author_div.find("div")
-            id = regex_match(
+            post_id = regex_match(
                 re.compile(r"^elComment_(\d+)"), content_article.get("id")
             ).group(1)
 
             yield Post(
                 path=thread.path,
-                subpath=(id,),
+                subpath=(post_id,),
                 url=url_div.find("a").get("href"),
                 origin=response.url,
                 data={},
                 author=author_h3.find("a").string,
+                creation_time=time_tag.get("datetime"),
                 content="".join(str(v) for v in content_div.contents),
             )
 
         next_page_link = soup.try_find("link", attrs={"rel": "next"})
         if next_page_link:
             return PageState(url=next_page_link.get("href"))
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/phpbb.py` & `forum_dl-0.2.0/forum_dl/extractors/phpbb.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         # Check for the existence of "viewforum.php".
         response = session.try_get(
             urljoin(
                 normalize_url(url, remove_suffixes=["viewforum.php", "viewtopic.php"]),
                 "viewforum.php",
-            )
+            ),
+            should_cache=True,
+            should_retry=False,
         )
 
         # A rather crude way to detect: we look for a <html> tag with "dir" attribute.
         soup = Soup(response.text)
         soup.find("html", attrs={"dir": True})
 
         return PhpbbExtractor(
@@ -150,15 +152,15 @@
             return False
 
         return True
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
-        response = self._session.get(self.base_url)
+        response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
         board_lis = soup.find_all("div", class_="forabg")
 
         for board_li in board_lis:
             header_li = board_li.find("li", class_="header")
             board_anchor = header_li.find("a")
@@ -199,19 +201,19 @@
                     ),
                     url=subboard_url,
                     origin=response.url,
                     data={},
                     title=subboard_title,
                 )
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         if board is self.root:
             return
 
-        response = self._session.get(board.url)
+        response = self._session.get(board.url, should_cache=True)
 
         try:
             get_relative_url(response.url, self.base_url)
         except ValueError:
             return
 
         soup = Soup(response.content)
@@ -236,40 +238,42 @@
                 origin=response.url,
                 data={},
                 title=subboard_title,
                 are_subboards_fetched=True,
             )
 
     def _resolve_url(self, url: str):
-        return normalize_url(self._session.get(url).url, keep_queries=["f", "t"])
+        return normalize_url(
+            self._session.get(url, should_cache=True).url, keep_queries=["f", "t"]
+        )
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         resolved_url = normalize_url(response.url, keep_queries=["f", "t"])
 
         parsed_url = urlparse(resolved_url)
         parts = PurePosixPath(parsed_url.path).parts
 
         if parts[-1] == "viewforum.php":
             self._fetch_lower_boards(self.root)
 
             parsed_query = parse_qs(parsed_url.query)
 
             if "f" not in parsed_query:
                 return self.root
 
-            id = parsed_query["f"][0]
+            board_id = parsed_query["f"][0]
 
             for board in self._boards:
-                if board is not self.root and board.path[-1] == id:
+                if board is not self.root and board.path[-1] == board_id:
                     return board
 
             raise ValueError
         elif parts[-1] == "viewtopic.php":
-            id = parse_qs(parsed_url.query)["t"][0]
+            topic_id = parse_qs(parsed_url.query)["t"][0]
             soup = Soup(response.content)
             breadcrumbs = soup.find(class_="breadcrumbs")
 
             breadcrumb_anchors = breadcrumbs.find_all("a", attrs={"itemprop": "item"})
 
             breadcrumb_urls = [
                 self._resolve_url(urljoin(url, anchor.get("href")))
@@ -277,26 +281,26 @@
             ]
             board = self.find_board_from_urls(tuple(breadcrumb_urls[1:]))
 
             title_h2 = soup.find("h2", class_="topic-title")
             title = title_h2.find("a").string
 
             return Thread(
-                path=board.path + (id,),
+                path=board.path + (topic_id,),
                 url=resolved_url,
                 origin=resolved_url,
                 data={},
                 title=title,
             )
         elif normalize_url(resolved_url) == self.base_url:
             return self.root
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if board == self.root:
@@ -371,28 +375,32 @@
         post_divs = soup.find_all("div", class_="post")
 
         for post_div in post_divs:
             id_div_regex = re.compile(r"^post_content(\d+)$")
             id_div = post_div.find("div", id=id_div_regex)
             content_div = post_div.find("div", class_="content")
 
-            username_tag = post_div.find(
+            author_p = post_div.find("p", class_="author")
+
+            username_tag = author_p.find(
                 {"a", "span"}, class_={"username", "username-coloured"}
             )
+            time_tag = author_p.find("time")
 
             url_h3 = post_div.find("h3")
             url_anchor = url_h3.find("a")
 
             yield Post(
                 path=thread.path,
                 subpath=(regex_match(id_div_regex, id_div.get("id")).group(1),),
                 url=urljoin(response.url, url_anchor.get("href")),
                 origin=response.url,
                 data={},
                 author=username_tag.string,
+                creation_time=time_tag.get("datetime"),
                 content=str("".join(str(v) for v in content_div.contents)),
             )
 
         pagination_anchors = soup.find_all(
             "a",
             attrs={"href": self._is_viewtopic_pagination_url},
         )
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/pipermail.py` & `forum_dl-0.2.0/forum_dl/extractors/pipermail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse, urlunparse
 from dataclasses import dataclass
+import dateutil.parser
 import bs4
 import re
 
 from .common import normalize_url, regex_match
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..exceptions import TagSearchError
 from ..session import Session
@@ -57,15 +58,15 @@
     )
     _post_href_regex = re.compile(r"^(\d+).html$")
     _root_post_comment_regex = re.compile(r"^0 ([^-]+)- $")
     _child_post_comment_regex = re.compile(r"^(1|2|3) ([^-]+)-(.*?)-? $")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(url)
+        response = session.try_get(url, should_cache=True, should_retry=False)
         resolved_url = normalize_url(response.url, append_slash=False)
 
         parsed_url = urlparse(resolved_url)
         path = PurePosixPath(parsed_url.path)
 
         if len(path.parts) >= 4 and path.parts[-4] == "pipermail":
             return PipermailExtractor(
@@ -111,42 +112,42 @@
                 ),
                 options,
             )
 
     def _fetch_top_boards(self):
         pass
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         normalized_url = normalize_url(response.url)
 
         if normalized_url == self.base_url:
             return self.root
 
         parsed_url = urlparse(normalized_url)
         path = PurePosixPath(parsed_url.path)
 
         if len(path.parts) >= 4 and path.parts[-4] == "pipermail":
             if path.parts[-1] == "thread.html":
                 return self.find_board((path.parts[-3],))
 
-            id = path.parts[-1].removesuffix(".html")
+            thread_id = path.parts[-1].removesuffix(".html")
             board_id = path.parts[-3]
 
             # TODO: Properly read board name instead.
             board_id.replace("_", "@")
 
             soup = Soup(response.content)
             title = soup.find("title").string
 
             return Thread(
-                path=(board_id, id),
+                path=(board_id, thread_id),
                 url=url,
                 origin=response.url,
                 data={},
                 title=title,
             )
         elif len(path.parts) >= 3 and path.parts[-3] == "pipermail":
             return self.find_board((path.parts[-2],))
@@ -160,69 +161,71 @@
             if path.parts[-2] == "pipermail":
                 return self.find_board((path.parts[-1],))
 
             return self.root
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
-        nice_id = id.replace("@", "_")
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
+        nice_id = subboard_id.replace("@", "_")
 
         url = normalize_url(urljoin(self.base_url, f"mailman/listinfo/{nice_id}"))
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         title_title = soup.find("title")
         title = regex_match(self._listinfo_title_regex, title_title.string).group(1)
 
         # body = str(soup.find_all("p")[2].contents[1])
         return self._set_board(
-            path=(id,),
+            path=(subboard_id,),
             url=url,
             origin=response.url,
             data={},
             # data={"body": body},
             title=title,
         )
 
     def _fetch_lazy_subboards(self, board: Board):
         # TODO use a for loop over _fetch_lazy_subboard() instead
         url = normalize_url(urljoin(self.base_url, f"mailman/listinfo"))
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         listinfo_anchors = soup.find_all("a", attrs={"href": self._listinfo_href_regex})
 
         for listinfo_anchor in listinfo_anchors:
             href = listinfo_anchor.get("href")
-            id = regex_match(self._listinfo_href_regex, href).group(1)
-            yield self._fetch_lazy_subboard(board, id)
+            list_id = regex_match(self._listinfo_href_regex, href).group(1)
+            yield self._fetch_lazy_subboard(board, list_id)
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if board == self.root:
             return None
 
         if state.url == board.url:
-            id = board.path[0]
-            pipermail_url = urljoin(self.base_url, f"pipermail/{id}")
+            board_id = board.path[0]
+            pipermail_url = urljoin(self.base_url, f"pipermail/{board_id}")
 
             response = self._session.get(pipermail_url)
             soup = Soup(response.content)
 
             page_anchors = soup.find_all(
                 "a", attrs={"href": self._pipermail_page_href_regex}
             )
 
             relative_urls = list(
                 reversed([page_anchor.get("href") for page_anchor in page_anchors])
             )
 
             relative_url = relative_urls.pop()
             return PipermailPageState(
-                url=urljoin(urljoin(self.base_url, f"pipermail/{id}/"), relative_url),
+                url=urljoin(
+                    urljoin(self.base_url, f"pipermail/{board_id}/"), relative_url
+                ),
                 relative_urls=relative_urls,
             )
 
         state = cast(PipermailPageState, state)
 
         response = self._session.get(state.url)
         soup = Soup(response.content)
@@ -233,18 +236,18 @@
         )
 
         for root_comment in root_comments:
             thread_anchor = root_comment.find_next(
                 "a", attrs={"href": self._post_href_regex}
             )
             href = thread_anchor.get("href")
-            id = regex_match(self._post_href_regex, href).group(1)
+            thread_id = regex_match(self._post_href_regex, href).group(1)
 
             yield Thread(
-                path=board.path + (id,),
+                path=board.path + (thread_id,),
                 url=urljoin(state.url, href),
                 origin=response.url,
                 data={},
                 title=thread_anchor.string,
             )
 
         if state.relative_urls:
@@ -297,20 +300,20 @@
                 .split("-")
             )
 
             child_anchor = child_comment.find_next(
                 "a", attrs={"href": self._post_href_regex}
             )
             href = child_anchor.get("href")
-            id = regex_match(self._post_href_regex, href).group(1)
+            post_id = regex_match(self._post_href_regex, href).group(1)
 
             if len(cur_long_ids) > len(prev_long_ids):
-                subpath.append(id)
+                subpath.append(post_id)
             else:
-                subpath[-(len(prev_long_ids) - len(cur_long_ids) - 1) :] = [id]
+                subpath[-(len(prev_long_ids) - len(cur_long_ids) - 1) :] = [post_id]
 
             yield self._fetch_post(
                 state, thread.path, tuple(subpath), urljoin(state.url, href)
             )
 
             prev_long_ids = cur_long_ids
 
@@ -325,17 +328,19 @@
         soup = Soup(response.content)
 
         content_pre = soup.find("pre")
         content = "".join(str(v) for v in content_pre.contents)
         content = re.sub(r"><i>(.*?\n)</i>", r">\1", content)
 
         author_b = soup.find("b")
+        date_i = soup.find("i")
 
         return Post(
             path=path,
             subpath=subpath,
             url=url,
             origin=response.url,
             data={},
             author=str(author_b.string),
+            creation_time=dateutil.parser.parse(date_i.string).isoformat(),
             content=content,
         )
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/proboards.py` & `forum_dl-0.2.0/forum_dl/extractors/proboards.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse
+from datetime import datetime
 import re
 
 from .common import regex_match
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 from ..soup import Soup
 
@@ -198,15 +199,17 @@
 
         if parsed_url.netloc.endswith("proboards.com"):
             return ProboardsExtractor(session, urljoin(url, "/"), options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
-        response = self._session.get(self.base_url)
+        response = self._session.try_get(
+            self.base_url, should_cache=True, should_retry=False
+        )
         soup = Soup(response.content)
 
         category_anchors = soup.find_all("a", attrs={"name": self._category_name_regex})
 
         for category_anchor in category_anchors:
             category_id = regex_match(
                 self._category_name_regex, category_anchor.get("name")
@@ -239,19 +242,19 @@
                     data={},
                     title=board_anchor.string,
                     are_subboards_fetched=True,
                 )
 
         self._fetch_lower_boards(self.root)
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         if not board.url:
             return
 
-        response = self._session.get(board.url)
+        response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
         subboard_trs = soup.find_all("tr", id=self._board_id_regex)
         for subboard_tr in subboard_trs:
             subboard_id = regex_match(
                 self._board_id_regex, subboard_tr.get("id")
             ).group(1)
@@ -270,15 +273,15 @@
         parsed_url = urlparse(url)
         url_parts = PurePosixPath(parsed_url.path).parts
 
         if len(url_parts) <= 1:
             return self.root
 
         if url_parts[1] == "thread":
-            response = self._session.get(url)
+            response = self._session.get(url, should_cache=True)
             soup = Soup(response.content)
 
             breadcrumbs_div = soup.find("div", class_="nav-tree-wrapper")
             breadcrumb_anchors = breadcrumbs_div.find_all(
                 "a", attrs={"itemprop": "item"}
             )
 
@@ -303,15 +306,15 @@
         elif url_parts[1] == "board":
             for cur_board in self._boards:
                 if cur_board.path[-1] == url_parts[1]:
                     return cur_board
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if board == self.root:
@@ -347,24 +350,28 @@
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         response = self._session.get(state.url)
         soup = Soup(response.content)
 
         post_trs = soup.find_all("tr", class_="item")
         for post_tr in post_trs:
             user_anchor = post_tr.try_find("a", class_="o-user-link")
+            time_abbr = post_tr.find("abbr", class_="time")
             message_div = post_tr.find("div", class_="message")
-            id = regex_match(self._post_id_regex, post_tr.get("id")).group(1)
+            post_id = regex_match(self._post_id_regex, post_tr.get("id")).group(1)
 
             yield Post(
                 path=thread.path,
-                subpath=(id,),
-                url=urljoin(self.base_url, f"post/{id}/thread"),
+                subpath=(post_id,),
+                url=urljoin(self.base_url, f"post/{post_id}/thread"),
                 origin=response.url,
                 data={},
                 author=user_anchor.string if user_anchor else "",
+                creation_time=datetime.fromtimestamp(
+                    int(time_abbr.get("data-timestamp")) / 1000
+                ).isoformat(),
                 content=str("".join(str(v) for v in message_div.contents)),
             )
 
         next_page_li = soup.try_find("li", class_="next")
         if not next_page_li:
             return None
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/vbulletin.py` & `forum_dl-0.2.0/forum_dl/extractors/vbulletin.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,28 +210,28 @@
         },
     ]
 
     _forum_id_regex = re.compile(r"^forum(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(url)
+        response = session.try_get(url, should_cache=True, should_retry=False)
         soup = Soup(response.content)
 
         generator_meta = soup.find("meta", attrs={"name": "generator"})
         if not generator_meta.get("content").startswith("vBulletin"):
             return None
 
         base = soup.find("base")
         return VbulletinExtractor(session, base.get("href"), options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
-        response = self._session.get(self.base_url)
+        response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
         trs = soup.find_all("tr", class_=["category-header", "forum-item"])
         category_id = ""
 
         for tr in trs:
             if "category-header" in tr.get_list("class"):
@@ -258,20 +258,20 @@
                     path=(category_id, board_id),
                     url=board_anchor.get("href"),
                     origin=response.url,
                     data={},
                     title=title,
                 )
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         # Don't fetch top boards.
         if len(board.path) <= 1:
             return
 
-        response = self._session.get(board.url)
+        response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
         trs = soup.find_all("tr", class_="forum-item")
         for tr in trs:
             subboard_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
 
             subboard_anchor = tr.find("a", class_="forum-title")
@@ -280,34 +280,34 @@
                 url=subboard_anchor.get("href"),
                 origin=response.url,
                 data={},
                 title=subboard_anchor.string.strip(),
             )
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         breadcrumb_anchors = soup.find_all("a", class_="crumb-link")
 
         if len(breadcrumb_anchors) <= 1:
             return self.root
 
         # Thread.
         if soup.try_find("h2", class_="b-post__title"):
             breadcrumb_urls = [
                 self._resolve_url(anchor.get("href")) for anchor in breadcrumb_anchors
             ]
             board = self.find_board_from_urls(tuple(breadcrumb_urls[2:]))
 
-            id = soup.find("input", attrs={"name": "nodeid"}).get("value")
+            thread_id = soup.find("input", attrs={"name": "nodeid"}).get("value")
             title_h1 = soup.find("h1", class_="main-title")
 
             return Thread(
-                path=board.path + (id,),
+                path=board.path + (thread_id,),
                 url=urljoin(self.base_url, url),
                 origin=response.url,
                 data={},
                 title=title_h1.string,
             )
         # Board.
         else:
@@ -360,22 +360,24 @@
             # No support for comments for now.
             if "b-comment" in post_li.get_list("class"):
                 continue
 
             url_anchor = post_li.find("a", class_="b-post__count")
             content_div = post_li.find("div", class_="js-post__content-text")
             author_anchor = post_li.find("div", class_="author").find("a")
-            id = post_li.get("data-node-id")
+            time_tag = post_li.find("time", attrs={"itemprop": "dateCreated"})
+            post_id = post_li.get("data-node-id")
 
             yield Post(
                 path=thread.path,
-                subpath=(id,),
+                subpath=(post_id,),
                 url=url_anchor.get("href"),
                 origin=response.url,
                 data={},
                 author=author_anchor.string,
+                creation_time=time_tag.get("datetime"),
                 content="".join(str(v) for v in content_div.contents).strip(),
             )
 
         next_page_anchor = soup.try_find("a", class_="right-arrow")
         if next_page_anchor and next_page_anchor.try_get("href"):
             return PageState(url=next_page_anchor.get("href"))
```

### Comparing `forum_dl-0.1.0/forum_dl/extractors/xenforo.py` & `forum_dl-0.2.0/forum_dl/extractors/xenforo.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,16 +202,18 @@
     _board_class_regex = re.compile(r"^node--id(\d+)$")
     _thread_class_regex = re.compile(r"^js-threadListItem-(\d+)$")
     _thread_key_regex = re.compile(r"^thread-(\d+)$")
     _post_id_regex = re.compile(r"^post-(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
-        response = session.get_noretry(
-            normalize_url(url, remove_suffixes=[], append_slash=False)
+        response = session.try_get(
+            normalize_url(url, remove_suffixes=[], append_slash=False),
+            should_cache=True,
+            should_retry=False,
         )
         soup = Soup(response.content)
 
         data_nav_id_anchor = soup.find("a", attrs={"data-nav-id": "forums"})
         base_url = normalize_url(urljoin(url, data_nav_id_anchor.get("href")))
         if not base_url:
             return None
@@ -220,15 +222,15 @@
             return None
 
         return XenforoExtractor(session, base_url, options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
-        response = self._session.get(self.base_url)
+        response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
         block_category_divs = soup.find_all("div", class_=self._category_class_regex)
         for block_category_div in block_category_divs:
             category_header = block_category_div.find("h2", class_="block-header")
             category_anchor = category_header.find("a")
             category_id = regex_match(
@@ -266,19 +268,19 @@
                     origin=response.url,
                     data={},
                     title=node_description_anchor.string.strip(),
                 )
 
         self._fetch_lower_boards(self.root)
 
-    def _fetch_subboards(self, board: Board):
+    def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
-        response = self._session.get(url)
+        response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
         breadcrumbs_ul = soup.find("ul", class_="p-breadcrumbs")
         breadcrumb_anchors = breadcrumbs_ul.find_all("a", attrs={"itemprop": "item"})
 
         if len(breadcrumb_anchors) <= 1:
             return self.root
@@ -307,15 +309,15 @@
 
             for cur_board in self._boards:
                 if cur_board.url == board_href:
                     return cur_board
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, id: str):
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
     def _fetch_board_page_threads(self, board: Board, state: PageState):
         if board == self.root:
@@ -360,26 +362,28 @@
 
         for message_article in message_articles:
             bbwrapper_div = message_article.find("div", class_="bbWrapper")
             message_attribution_ul = message_article.find(
                 "ul", class_="message-attribution-main"
             )
             url_anchor = message_attribution_ul.find("a")
+            time_tag = message_attribution_ul.find("time")
 
             yield Post(
                 path=thread.path,
                 subpath=(
                     regex_match(
                         self._post_id_regex, message_article.get("data-content")
                     ).group(1),
                 ),
                 url=urljoin(state.url, url_anchor.get("href")),
                 origin=response.url,
                 data={},
                 author=message_article.get("data-author"),
+                creation_time=time_tag.get("datetime"),
                 content=str(bbwrapper_div.encode_contents()),
             )
 
         next_page_anchor = soup.try_find("a", class_="pageNav-jump--next")
         if next_page_anchor:
             return PageState(
                 url=urljoin(self.base_url, next_page_anchor.get("href")),
```

### Comparing `forum_dl-0.1.0/forum_dl/forumdl.py` & `forum_dl-0.2.0/forum_dl/forumdl.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/forum_dl/soup.py` & `forum_dl-0.2.0/forum_dl/soup.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/forum_dl/writers/__init__.py` & `forum_dl-0.2.0/forum_dl/writers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..extractors.common import Extractor
 from ..exceptions import WriterNotFoundError
 from ..session import SessionOptions
 
 # from .strictyaml import StrictYamlWriter
 import inspect
 
-modules = ["babyl", "maildir", "mbox", "mh", "mmdf", "jsonl"]
+modules = ["babyl", "jsonl", "maildir", "mbox", "mh", "mmdf", "warc"]
 
 
 def find(
     extractor: Extractor,
     module_name: str,
     session_options: SessionOptions,
     writer_options: WriterOptions,
```

### Comparing `forum_dl-0.1.0/forum_dl/writers/common.py` & `forum_dl-0.2.0/forum_dl/writers/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from mailbox import Mailbox, Message
+from urllib.parse import urlparse
+import email.utils
 
 try:
     from html2text import html2text
 except ImportError:
     pass
 
 from datetime import datetime, timezone
@@ -20,16 +22,17 @@
 
 @dataclass  # (kw_only=True)
 class WriterOptions:
     output_path: str
     write_board_objects: bool
     write_thread_objects: bool
     write_post_objects: bool
-    content_as_title: bool
     textify: bool
+    content_as_title: bool
+    author_as_addr_spec: bool
 
 
 @dataclass  # (kw_only=True)
 class WriterState:
     board_path: tuple[str, ...] | None = None
     board_page: PageState | None = None
     thread_page: PageState | None = None
@@ -232,15 +235,25 @@
 
     def _build_message(self, thread: Thread, post: Post):
         msg = self._new_message()
 
         path = post.path + post.subpath
 
         msg["Message-ID"] = "<" + ".".join(path) + ">"
-        msg["From"] = post.author
+        msg["Content-Location"] = post.url
+        msg["Date"] = email.utils.formatdate(
+            datetime.fromisoformat(post.creation_time).timestamp()
+        )
+
+        if self._options.author_as_addr_spec:
+            domain = urlparse(self._extractor.base_url).netloc
+
+            msg["From"] = f"{post.author} <{post.author}@{domain}>"
+        else:
+            msg["From"] = post.author
 
         if len(path) >= 2:
             msg["In-Reply-To"] = f"<{'.'.join(path[:-1])}>"
 
             refs = f"{path[0]}"
             for ref in post.path[1:-1]:
                 refs += f" <{ref}>"
```

### Comparing `forum_dl-0.1.0/forum_dl/writers/maildir.py` & `forum_dl-0.2.0/forum_dl/writers/maildir.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/forum_dl/writers/mh.py` & `forum_dl-0.2.0/forum_dl/writers/mh.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.1.0/forum_dl.egg-info/PKG-INFO` & `forum_dl-0.2.0/forum_dl.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 Metadata-Version: 2.1
 Name: forum-dl
-Version: 0.1.0
+Version: 0.2.0
 Summary: Download posts and threads from forums, news aggregators, mail archives
 Author-email: Mikolaj Wielgus <wielgusmikolaj@gmail.com>
 License: MIT
+Project-URL: repository, https://github.com/mikwielgus/forum-dl
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.10.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: html2text
 License-File: LICENSE
 
 # forum-dl
 
-Forum-dl is a downloader (scraper) for forums, mailing lists, and news aggregators. It can be used to crawl, extract, and archive individual threads and entire boards into a variety of output formats.
+Forum-dl is a scraper and archiver for forums (including Discourse, PhpBB, SMF), mailing lists, and news aggregators ([list](#forum-software)). It can be used to extract and archive all posts from individual threads and entire boards into JSONL, Mbox, Maildir, WARC ([complete list](#output-formats)).
+
+<sub>The project is currently in alpha stage. Please do not hesitate to [file](https://github.com/mikwielgus/forum-dl/issues) bug reports and feature requests.</sub>
+
+![image](https://github.com/mikwielgus/forum-dl/assets/58011230/e677d1aa-efa3-4cfc-9283-38408842b278)
 
 # Installation
 
-Clone the repository:
+You can install Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
+
+## PIP
+
+Install the latest stable version of Forum-dl from PIP:
 
 ```
-git clone https://github.com/mikwielgus/forum-dl
+pip install forum-dl
 ```
 
-Then, in the same directory, install the repository directly: 
+## Repository 
+
+Clone the repository and install it in editable mode:
 
 ```
-pip install -e forum-dl
+git clone https://github.com/mikwielgus/forum-dl && pip install -e forum-dl
 ```
 
-# Quick start
+# Usage examples
 
-Download a Simple Machines forum thread in JSONL format:
+Download a Simple Machines Forum thread in JSONL format:
 
 ```
 forum-dl "https://www.simplemachines.org/community/index.php?topic=584230.0"
 ```
 
-Download an entire PhpBB forum board in JSONL format, write to stdout (`-o -`).
+Download an entire PhpBB board into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
 
 ```
 forum-dl -o - "https://www.phpbb.com/community/viewforum.php?f=696"
 ```
 
-<sub>(due to current architecture limitations, `forum-dl` will shallowly scan the entire forum hierarchy before downloading the board. This will be fixed in future releases)</sub>
+<sub>(due to current architectural limitations, `forum-dl` will scan the first page of each board in the entire forum before downloading the target board. This will be fixed in future releases)</sub>
 
 Download Hacker News top stories and write them to a Maildir directory `hn`:
 
 ```
 forum-dl --textify --content-as-title -f maildir -o hn "https://news.ycombinator.com/news"
 ```
 
@@ -75,43 +90,58 @@
 
 - Babyl
 - JSONL
 - Maildir
 - Mbox
 - MH
 - MMDF
+- WARC
 
 # Usage
 
 ```
-forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE]
-         [-f FORMAT] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [-R RETRIES] [--retry-sleep RETRY_SLEEP]
+         [--retry-sleep-multiplier RETRY_SLEEP_MULTIPLIER] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE] [-f FORMAT]
+         [--warc-output FILE] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+         [--author-as-addr-spec]
 ```
 
 ## General Options:
 
 ```
   --help                Show this help message and exit
   --version             Print program version and exit
   --list-extractors     List all supported extractors and exit
   --list-output-formats
                         List all supported output formats and exit
-  --user-agent USER_AGENT
-                        User-Agent request header
+```
+
+## Session Options:
+
+```
+  -R N, --retries N     Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)
+  --retry-sleep SECONDS
+                        Time to sleep between retries, in seconds (default: 1)
+  --retry-sleep-multiplier K
+                        A constant by which sleep time is multiplied on each retry (default: 2)
+  --user-agent UA       User-Agent request header
 ```
 
 ## Output Options:
 
 ```
   -q, --quiet           Activate quiet mode
   -v, --verbose         Print various debugging information
   -g, --get-urls        Print URLs instead of downloading
   -o FILE, --output FILE
                         Output all results concatenated to FILE, or stdout if FILE is -
   -f FORMAT, --output-format FORMAT
-                        Output format
+                        Output format. Use --list-output-formats for a list of possible arguments
+  --warc-output FILE    Record HTTP requests, store them in FILE in WARC format
   --no-boards           Do not write board objects
   --no-threads          Do not write thread objects
   --no-posts            Do not write post objects
   --textify             Lossily convert HTML content to plaintext
   --content-as-title    Write 98 initial characters of content in title field of each post
+  --author-as-addr-spec
+                        Append author and domain as an addr-spec in the From header
 ```
```

### Comparing `forum_dl-0.1.0/forum_dl.egg-info/SOURCES.txt` & `forum_dl-0.2.0/forum_dl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 forum_dl/writers/__init__.py
 forum_dl/writers/babyl.py
 forum_dl/writers/common.py
 forum_dl/writers/jsonl.py
 forum_dl/writers/maildir.py
 forum_dl/writers/mbox.py
 forum_dl/writers/mh.py
-forum_dl/writers/mmdf.py
+forum_dl/writers/mmdf.py
+forum_dl/writers/warc.py
```

