# Comparing `tmp/calcure-2.9.2.tar.gz` & `tmp/calcure-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcure-2.9.2.tar", last modified: Mon May  8 07:58:30 2023, max compression
+gzip compressed data, was "calcure-2.9.3.tar", last modified: Fri May 26 06:42:19 2023, max compression
```

## Comparing `calcure-2.9.2.tar` & `calcure-2.9.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.196696 calcure-2.9.2/
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9.2/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-08 07:58:30.196696 calcure-2.9.2/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9.2/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.193363 calcure-2.9.2/calcure/
--rw-r--r--   0 r         (1000) r         (1000)    42043 2023-05-08 07:56:13.000000 calcure-2.9.2/calcure/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9.2/calcure/calendars.py
--rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9.2/calcure/colors.py
--rw-r--r--   0 r         (1000) r         (1000)    20458 2023-05-08 07:56:23.000000 calcure-2.9.2/calcure/configuration.py
--rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-08 07:56:33.000000 calcure-2.9.2/calcure/controls.py
--rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-08 07:53:30.000000 calcure-2.9.2/calcure/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3512 2023-05-08 07:54:09.000000 calcure-2.9.2/calcure/dialogues.py
--rw-r--r--   0 r         (1000) r         (1000)     1572 2023-05-08 07:55:03.000000 calcure-2.9.2/calcure/errors.py
--rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9.2/calcure/importers.py
--rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9.2/calcure/loaders.py
--rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9.2/calcure/savers.py
--rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-06 11:03:23.000000 calcure-2.9.2/calcure/screen.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.196696 calcure-2.9.2/calcure/translations/
--rw-r--r--   0 r         (1000) r         (1000)     5832 2023-05-08 07:19:10.000000 calcure-2.9.2/calcure/translations/br.py
--rw-r--r--   0 r         (1000) r         (1000)     5328 2023-05-08 07:19:11.000000 calcure-2.9.2/calcure/translations/en.py
--rw-r--r--   0 r         (1000) r         (1000)     6293 2023-05-08 07:19:09.000000 calcure-2.9.2/calcure/translations/fr.py
--rw-r--r--   0 r         (1000) r         (1000)     6325 2023-05-08 07:19:08.000000 calcure-2.9.2/calcure/translations/it.py
--rw-r--r--   0 r         (1000) r         (1000)     8334 2023-05-08 07:19:07.000000 calcure-2.9.2/calcure/translations/ru.py
--rw-r--r--   0 r         (1000) r         (1000)     6173 2023-05-08 07:20:42.000000 calcure-2.9.2/calcure/translations/tr.py
--rw-r--r--   0 r         (1000) r         (1000)     5472 2023-05-08 07:19:38.000000 calcure-2.9.2/calcure/translations/zh.py
--rw-r--r--   0 r         (1000) r         (1000)      989 2023-05-06 06:48:14.000000 calcure-2.9.2/calcure/weather.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-08 07:58:30.193363 calcure-2.9.2/calcure.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-08 07:58:30.000000 calcure-2.9.2/calcure.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9.2/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-08 07:58:30.196696 calcure-2.9.2/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9.2/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-26 06:42:19.195923 calcure-2.9.3/
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9.3/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-26 06:42:19.195923 calcure-2.9.3/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9.3/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-26 06:42:19.195923 calcure-2.9.3/calcure/
+-rw-r--r--   0 r         (1000) r         (1000)    42031 2023-05-26 06:39:48.000000 calcure-2.9.3/calcure/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9.3/calcure/calendars.py
+-rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9.3/calcure/colors.py
+-rw-r--r--   0 r         (1000) r         (1000)    20452 2023-05-26 06:39:12.000000 calcure-2.9.3/calcure/configuration.py
+-rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-08 07:56:33.000000 calcure-2.9.3/calcure/controls.py
+-rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-08 07:53:30.000000 calcure-2.9.3/calcure/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3512 2023-05-08 07:54:09.000000 calcure-2.9.3/calcure/dialogues.py
+-rw-r--r--   0 r         (1000) r         (1000)     1572 2023-05-08 07:55:03.000000 calcure-2.9.3/calcure/errors.py
+-rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9.3/calcure/importers.py
+-rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9.3/calcure/loaders.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9.3/calcure/savers.py
+-rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-06 11:03:23.000000 calcure-2.9.3/calcure/screen.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-26 06:42:19.195923 calcure-2.9.3/calcure/translations/
+-rw-r--r--   0 r         (1000) r         (1000)     5832 2023-05-08 07:19:10.000000 calcure-2.9.3/calcure/translations/br.py
+-rw-r--r--   0 r         (1000) r         (1000)     5328 2023-05-08 07:19:11.000000 calcure-2.9.3/calcure/translations/en.py
+-rw-r--r--   0 r         (1000) r         (1000)     6293 2023-05-08 07:19:09.000000 calcure-2.9.3/calcure/translations/fr.py
+-rw-r--r--   0 r         (1000) r         (1000)     6325 2023-05-08 07:19:08.000000 calcure-2.9.3/calcure/translations/it.py
+-rw-r--r--   0 r         (1000) r         (1000)     8334 2023-05-08 07:19:07.000000 calcure-2.9.3/calcure/translations/ru.py
+-rw-r--r--   0 r         (1000) r         (1000)     6173 2023-05-08 07:20:42.000000 calcure-2.9.3/calcure/translations/tr.py
+-rw-r--r--   0 r         (1000) r         (1000)     5472 2023-05-08 07:19:38.000000 calcure-2.9.3/calcure/translations/zh.py
+-rw-r--r--   0 r         (1000) r         (1000)      989 2023-05-06 06:48:14.000000 calcure-2.9.3/calcure/weather.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-26 06:42:19.195923 calcure-2.9.3/calcure.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-26 06:42:19.000000 calcure-2.9.3/calcure.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9.3/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-26 06:42:19.195923 calcure-2.9.3/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9.3/setup.py
```

### Comparing `calcure-2.9.2/LICENSE` & `calcure-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/PKG-INFO` & `calcure-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9.2
+Version: 2.9.3
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9.2/README.md` & `calcure-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/__main__.py` & `calcure-2.9.3/calcure/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from calcure.translations.tr import *
 elif cf.LANG == "zh":
     from calcure.translations.zh import *
 else:
     from calcure.translations.en import *
 
 
-__version__ = "2.9.2"
+__version__ = "2.9.3"
 
 
 def read_items_from_user_arguments(screen, user_tasks, user_events, task_saver_csv, event_saver_csv):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
         opts, _ = getopt.getopt(sys.argv[1:], "pjhvi", ["folder=", "config=", "task=", "event="])
         for opt, arg in opts:
@@ -155,15 +155,15 @@
 
     @property
     def info(self):
         """Icon and name of the task, which is decorated if needed"""
         name = self.task.name[self.indent:]
         if self.screen.privacy or self.task.privacy:
             return f'{cf.TODO_ICON} {cf.PRIVACY_ICON * len(name)}'
-        if self.task.status == Status.DONE and cf.STRIKETHROUGH_DONE_TASKS:
+        if self.task.status == Status.DONE and cf.STRIKETHROUGH_DONE:
             strike = "\u0336"
             return f'{self.icon} {strike}{strike.join(name)}{strike}'
         return f'{self.icon} {name}'
 
     def render(self):
         """Render a line with an icon, task, deadline, and timer"""
         self.display_line(self.y, self.x + self.indent, self.info, self.color)
@@ -272,15 +272,15 @@
             for color in Color:
                 if color.value == Color.ICS_CALENDARS0.value + self.event.calendar_number:
                     return color
             return Color.EVENTS
 
     def decorate_info(self):
         """Icon and name of the event, which is decorated if needed"""
-        if self.event.status == Status.DONE and cf.STRIKETHROUGH_DONE_TASKS:
+        if self.event.status == Status.DONE and cf.STRIKETHROUGH_DONE:
             strike = "\u0336"
             self.info = f'{self.icon} {strike}{strike.join(self.event.name)}{strike}'
 
     def obfuscate_info(self):
         """Obfuscate the info if privacy mode is on"""
         if self.screen.privacy or self.event.privacy:
             self.info = f'{cf.EVENT_ICON} {cf.PRIVACY_ICON * len(self.event.name)}'
```

### Comparing `calcure-2.9.2/calcure/calendars.py` & `calcure-2.9.3/calcure/calendars.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/colors.py` & `calcure-2.9.3/calcure/colors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/configuration.py` & `calcure-2.9.3/calcure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 "underlined_today":         "No",
                 "underlined_days":          "No",
                 "underlined_day_names":     "No",
                 "underlined_weekends":      "No",
                 "underlined_weekend_names": "No",
                 "underlined_title":         "No",
                 "underlined_active_pane":   "No",
-                "strikethrough_done_tasks": "Yes",
+                "strikethrough_done":       "No",
                 }
 
         conf["Event icons"] = {
                 "travel":      "✈",
                 "plane":       "✈",
                 "voyage":      "✈",
                 "flight":      "✈",
@@ -275,15 +275,15 @@
             self.UNDERLINED_TODAY         = conf.getboolean("Styles", "underlined_today", fallback=False)
             self.UNDERLINED_DAYS          = conf.getboolean("Styles", "underlined_days", fallback=False)
             self.UNDERLINED_DAY_NAMES     = conf.getboolean("Styles", "underlined_day_names", fallback=False)
             self.UNDERLINED_WEEKENDS      = conf.getboolean("Styles", "underlined_weekends", fallback=False)
             self.UNDERLINED_WEEKEND_NAMES = conf.getboolean("Styles", "underlined_weekend_names", fallback=False)
             self.UNDERLINED_TITLE         = conf.getboolean("Styles", "underlined_title", fallback=False)
             self.UNDERLINED_ACTIVE_PANE   = conf.getboolean("Styles", "underlined_active_pane", fallback=False)
-            self.STRIKETHROUGH_DONE_TASKS = conf.getboolean("Styles", "strikethrough_done_tasks", fallback=True)
+            self.STRIKETHROUGH_DONE       = conf.getboolean("Styles", "strikethrough_done", fallback=False)
 
             # Icons:
             self.TODAY_ICON       = conf.get("Parameters", "today_icon", fallback="•") if self.DISPLAY_ICONS else "·"
             self.PRIVACY_ICON     = conf.get("Parameters", "privacy_icon", fallback="•") if self.DISPLAY_ICONS else "·"
             self.HIDDEN_ICON      = conf.get("Parameters", "hidden_icon", fallback="...")
             self.EVENT_ICON       = conf.get("Parameters", "event_icon", fallback="•") if self.DISPLAY_ICONS else "·"
             self.BIRTHDAY_ICON    = conf.get("Parameters", "birthday_icon", fallback="★") if self.DISPLAY_ICONS else "·"
```

### Comparing `calcure-2.9.2/calcure/controls.py` & `calcure-2.9.3/calcure/controls.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/data.py` & `calcure-2.9.3/calcure/data.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/dialogues.py` & `calcure-2.9.3/calcure/dialogues.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/errors.py` & `calcure-2.9.3/calcure/errors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/importers.py` & `calcure-2.9.3/calcure/importers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/loaders.py` & `calcure-2.9.3/calcure/loaders.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/savers.py` & `calcure-2.9.3/calcure/savers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/screen.py` & `calcure-2.9.3/calcure/screen.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/br.py` & `calcure-2.9.3/calcure/translations/br.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/en.py` & `calcure-2.9.3/calcure/translations/en.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/fr.py` & `calcure-2.9.3/calcure/translations/fr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/it.py` & `calcure-2.9.3/calcure/translations/it.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/ru.py` & `calcure-2.9.3/calcure/translations/ru.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/tr.py` & `calcure-2.9.3/calcure/translations/tr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/translations/zh.py` & `calcure-2.9.3/calcure/translations/zh.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure/weather.py` & `calcure-2.9.3/calcure/weather.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/calcure.egg-info/PKG-INFO` & `calcure-2.9.3/calcure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9.2
+Version: 2.9.3
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9.2/calcure.egg-info/SOURCES.txt` & `calcure-2.9.3/calcure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcure-2.9.2/setup.py` & `calcure-2.9.3/setup.py`

 * *Files identical despite different names*

