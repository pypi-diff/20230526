# Comparing `tmp/PrSpiders-0.5.2.2.tar.gz` & `tmp/PrSpiders-0.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.2.tar", last modified: Thu May 25 08:03:03 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.3.tar", last modified: Fri May 26 09:31:22 2023, max compression
```

## Comparing `PrSpiders-0.5.2.2.tar` & `PrSpiders-0.5.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.712763 PrSpiders-0.5.2.2/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5497 2023-05-25 08:03:03.710763 PrSpiders-0.5.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.562764 PrSpiders-0.5.2.2/PrSpider/
--rw-rw-rw-   0        0        0    11104 2023-05-25 03:27:10.000000 PrSpiders-0.5.2.2/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.2/PrSpider/__init__.py
--rw-rw-rw-   0        0        0     2362 2023-05-25 03:27:14.000000 PrSpiders-0.5.2.2/PrSpider/log.py
--rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.2/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.2/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2.2/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.2/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.617764 PrSpiders-0.5.2.2/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5497 2023-05-25 08:03:02.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-05-25 08:03:03.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 08:03:02.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-25 08:03:02.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-25 08:03:03.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-25 08:03:03.000000 PrSpiders-0.5.2.2/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.630764 PrSpiders-0.5.2.2/pkg/
--rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.2/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.666767 PrSpiders-0.5.2.2/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.2/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.2/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.2/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.2/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-25 08:03:03.700766 PrSpiders-0.5.2.2/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.2/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.2/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.2/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.2/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-25 08:03:03.718764 PrSpiders-0.5.2.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-25 08:02:57.000000 PrSpiders-0.5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.051569 PrSpiders-0.5.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5497 2023-05-26 09:31:22.047565 PrSpiders-0.5.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.763574 PrSpiders-0.5.2.3/PrSpider/
+-rw-rw-rw-   0        0        0    11294 2023-05-26 09:30:37.000000 PrSpiders-0.5.2.3/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.3/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-05-26 09:30:30.000000 PrSpiders-0.5.2.3/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.3/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.3/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2.3/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.3/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.957568 PrSpiders-0.5.2.3/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5497 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-26 09:31:21.000000 PrSpiders-0.5.2.3/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:21.971568 PrSpiders-0.5.2.3/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.3/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.011568 PrSpiders-0.5.2.3/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.3/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.3/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.3/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.3/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:31:22.041564 PrSpiders-0.5.2.3/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.3/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.3/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.3/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.3/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 09:31:22.053566 PrSpiders-0.5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-26 09:30:52.000000 PrSpiders-0.5.2.3/setup.py
```

### Comparing `PrSpiders-0.5.2.2/LICENSE.txt` & `PrSpiders-0.5.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/PKG-INFO` & `PrSpiders-0.5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.2/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2.3/PrSpider/PrSpiders.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,25 +44,25 @@
         settions.workers = self.workers
         settions.download_delay = self.download_delay
         settions.executor = ThreadPoolExecutor(settions.workers)
         settions.download_num = self.download_num
         settions.logger = self.logger
         settions.log_stdout = self.log_stdout
         settions.log_level = self.log_level
-        loguer.warning(
-            "\033[31m~~~ @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s @Download_Num %s @LOG_LEVEL %s ~~~\033[0m"
-            % (
-                self.workers,
-                self.retry,
-                self.pid,
-                self.download_delay,
-                self.download_num,
-                self.log_level.upper(),
-            )
-        )
+        loguercor.log('Start',
+                      "<red>~~~ @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s @Download_Num %s @LOG_LEVEL %s ~~~</red>"
+                      % (
+                          self.workers,
+                          self.retry,
+                          self.pid,
+                          self.download_delay,
+                          self.download_num,
+                          self.log_level.upper(),
+                      )
+                      )
         if not self.start_urls and not hasattr(self, "start_requests"):
             raise AttributeError("Crawling could not start: 'start_urls' not found ")
         else:
             self.start_requests(**kwargs)
 
     def start_requests(self, **kwargs):
         if isinstance(self.start_urls, str):
@@ -123,22 +123,23 @@
                         retry_interval=retry_interval,
                         **kwargs,
                     )
                     futures.add(task)
                     cls.futures.add(task)
 
                 if len(cls.futures) > cls.workers:
-                    loguer.error(f'ThreadPoolExecutor workers not enough {len(cls.futures), cls.workers}.')
+                    loguercor.error(
+                        f'<yellow>ThreadPoolExecutor workers not enough {len(cls.futures), cls.workers}.</yellow>')
 
                 for future in as_completed(futures):
                     futures.remove(future)
                     worker_exception = future.exception()
                     cls.futures.remove(future) if future in cls.futures else cls.futures
                     if worker_exception:
-                        loguer.error(f"[PrSpider Exception] %s" % worker_exception)
+                        loguercor.error(f"<red>[PrSpider Exception] %s</red>" % worker_exception)
 
     @classmethod
     def Requests(
             cls,
             url=None,
             callback=None,
             headers=None,
@@ -172,22 +173,23 @@
                     retry_interval=retry_interval,
                     **kwargs,
                 )
                 futures.add(task)
                 cls.futures.add(task)
 
             if len(cls.futures) > cls.workers:
-                loguer.error(f'ThreadPoolExecutor workers not enough <green>{len(cls.futures)}</green>, {cls.workers}.')
+                loguercor.error(
+                    f'<yellow>ThreadPoolExecutor workers not enough {len(cls.futures)}</yellow>, {cls.workers}.')
 
             for future in as_completed(futures):
                 futures.remove(future)
                 worker_exception = future.exception()
                 cls.futures.remove(future) if future in cls.futures else cls.futures
                 if worker_exception:
-                    loguer.error(f"[PrSpider Exception] %s" % worker_exception)
+                    loguercor.error(f"<red>[PrSpider Exception] %s<red>" % worker_exception)
 
     @classmethod
     def fetch(
             self,
             url,
             callback,
             headers=None,
@@ -212,27 +214,24 @@
             settion=settions,
             **kwargs,
         )
         self.retry_num += int(response.meta.get("retry_num"))
         if response:
             if response.ok:
                 settions.success_num += 1
-                loguer.info(
-                    f"\033[31m{method.upper()}\033[0m | \033[33m{response.code}\033[0m | \033[34m{url}\033[0m")
+                loguercor.log('Crawl',
+                              f"<red>{method.upper()}</red> <yellow>{response.code}</yellow> <blue>{url}</blue>")
                 return callable(callback(response))
             else:
                 settions.false_num += 1
-                loguer.error(
-                    f"\033[31m{method.upper()}\033[0m \033[33m{response.code}\033[0m \033[34m{url}\033[0m"
-                )
+                loguercor.error(f"<red>{method.upper()}</red> <yellow>{response.code}</yellow> <blue>{url}</blue>")
                 return callable(callback(response))
         else:
             settions.false_num += 1
-            loguer.error(
-                f"\033[31m{method.upper()}\033[0m \033[33m{response.code}\033[0m \033[34m{url}\033[0m")
+            loguercor.error(f"<red>{method.upper()}</red> <yellow>{response.code}</yellow> <blue>{url}</blue>")
             callback(response)
             return self
 
     @classmethod
     def parse(self, response):
         raise NotImplementedError(
             f"{self.__class__.__name__}.parse callback is not defined"
@@ -250,36 +249,36 @@
     def __del__(self):
         end_time = time.time()
         spend_time = end_time - self.start_time
         try:
             average_time = spend_time / self.request_num
         except ZeroDivisionError:
             average_time = 0
-        m = """<Spider End>
+        m = """<green><Spider End>
 | ------------------ | ----------------------                               
 | `Workers`          | `%s`                                             
 | `Download Delay`   | `%s`                                             
 | `Download Num`     | `%s`                                             
 | `Request Num`      | `%s`                                             
 | `Success Num`      | `%s`                                             
 | `False Num`        | `%s`                                              
 | `Retry Num`        | `%s`                                              
 | `Start Time`       | `%s`                                              
 | `End Time`         | `%s`                                             
 | `Spend Time`       | `%.3fs`                                          
 | `Average Time`     | `%.3fs`         
-| ------------------ | ----------------------                            
+| ------------------ | ---------------------- </green>                          
         """ % (
             self.workers,
             self.download_delay,
             self.download_num,
             self.request_num,
             self.success_num,
             self.false_num,
             self.retry_num,
             self.process_timestamp(self.start_time),
             self.process_timestamp(end_time),
             spend_time,
             average_time,
         )
-        loguer.info(m)
+        loguer.opt(colors=True).info(m)
         self.executor.shutdown(wait=True)
```

### Comparing `PrSpiders-0.5.2.2/PrSpider/log.py` & `PrSpiders-0.5.2.3/PrSpider/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 import sys, os, re
 from loguru import logger as loguer
 
+loguercor = loguer.opt(colors=True)
 
 
 class Log():
     def __init__(self, log_stdout=True, log_level='INFO', log_file=False) -> None:
         self.level_dict = {
             "warn": 'WARNING',
             "info": 'INFO',
             "debug": 'DEBUG',
             "error": 'ERROR',
             "critical": 'CRITICAL',
+            "success": 'SUCCESS',
         }
         self.level_stdout = {
-            "critical": ['Print', 'CRITICAL'],
-            "error": ['Print', 'ERROR', 'CRITICAL', ],
-            "warn": ['Print', 'WARNING', 'ERROR', 'CRITICAL'],
-            "info": ['Print', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-            "debug": ['Print', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
+            "critical": ['Start', 'Print', 'CRITICAL'],
+            "error": ['Start', 'Print', 'ERROR', 'CRITICAL', ],
+            "success": ['Start', 'Print', 'Crawl', 'CRITICAL', ],
+            "warn": ['Start', 'Print', 'SUCCESS', 'WARNING', 'ERROR', 'CRITICAL'],
+            "info": ['Start', 'Print', 'SUCCESS', 'Crawl', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
+            "debug": ['Start', 'Print', 'SUCCESS', 'Crawl', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
         }
         self.log_stdout, self.log_level, self.log_file = log_stdout, log_level, log_file
-        loguer.level("TRACE", color="<blue>")
         loguer.level("DEBUG", color="<green>")
         loguer.level("INFO", color="<cyan>")
         loguer.level("SUCCESS", color="<light-green>")
         loguer.level("WARNING", color="<yellow>")
         loguer.level("ERROR", color="<red>")
         loguer.level("CRITICAL", color="<red>")
         loguer.level("Print", no=30, color="<green>")
-
+        loguer.level("Crawl", no=40, color="<green>")
+        loguer.level("Start", no=50, color="<yellow>")
 
     def loggering(self):
         levels = self.level_dict.get(self.log_level.lower())
         slevel = self.level_stdout.get(self.log_level.lower())
+        format = "<b><green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green></b><b><level> | {level: ^8} | </level></b><b><i>{message}</i></b>"
         stdout_handler = {
             "sink": sys.stdout,
+            "colorize": True,
             "filter": lambda record: record["level"].name in slevel,
-            "format": "<light-green><b>{time:YYYY-MM-DD HH:mm:ss.SSS}</b></light-green> | <b><level>{level: ^8}</level></b> | <b>{message}</b>"
+            "format": format
         }
         loguer.configure(handlers=[stdout_handler])
         if self.log_stdout:
             sys.stdout = InterceptHandler()
         if self.log_file:
             file_log = os.path.basename(__file__) if self.log_file is True else self.log_file
             file_log = (
                 re.sub("\..*", ".log", file_log)
                 if "." in file_log
                 else file_log + ".log"
             )
             filename = f"./{file_log}"
-            loguer.add(filename, level=levels)
+            loguer.add(filename, level=levels, format=format)
         return loguer
 
 
 class InterceptHandler():
     def write(self, message):
         if message.strip():
             loguer.log("Print", message.strip())
```

### Comparing `PrSpiders-0.5.2.2/PrSpider/pxpath.py` & `PrSpiders-0.5.2.3/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/PrSpider/pyconn.py` & `PrSpiders-0.5.2.3/PrSpider/pyconn.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/PrSpider/requestXpath.py` & `PrSpiders-0.5.2.3/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/PrSpider/useragent.py` & `PrSpiders-0.5.2.3/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2.3/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.2
+Version: 0.5.2.3
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.2/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2.3/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/README.md` & `PrSpiders-0.5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2.3/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/pkg/prspider/start.py` & `PrSpiders-0.5.2.3/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/requestXpath/__init__.py` & `PrSpiders-0.5.2.3/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/requestXpath/pxpath.py` & `PrSpiders-0.5.2.3/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/requestXpath/requestXpath.py` & `PrSpiders-0.5.2.3/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/requestXpath/useragent.py` & `PrSpiders-0.5.2.3/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.2/setup.py` & `PrSpiders-0.5.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.2.2"
+__version__ = "0.5.2.3"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

