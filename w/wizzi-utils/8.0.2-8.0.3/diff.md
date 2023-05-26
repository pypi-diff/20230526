# Comparing `tmp/wizzi_utils-8.0.2.tar.gz` & `tmp/wizzi_utils-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wizzi_utils-8.0.2.tar", last modified: Fri Jan  6 10:08:53 2023, max compression
+gzip compressed data, was "dist\wizzi_utils-8.0.3.tar", last modified: Fri May 26 18:27:41 2023, max compression
```

## Comparing `wizzi_utils-8.0.2.tar` & `wizzi_utils-8.0.3.tar`

### file list

```diff
@@ -1,92 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.254422 wizzi_utils-8.0.2/
--rw-rw-rw-   0        0        0     1077 2021-02-22 10:25:17.000000 wizzi_utils-8.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     7022 2023-01-06 10:08:53.255389 wizzi_utils-8.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6190 2022-10-10 17:27:16.000000 wizzi_utils-8.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-01-06 10:08:53.256392 wizzi_utils-8.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2721 2023-01-06 10:07:22.000000 wizzi_utils-8.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.689772 wizzi_utils-8.0.2/wizzi_utils/
--rw-rw-rw-   0        0        0     2215 2023-01-06 08:23:42.000000 wizzi_utils-8.0.2/wizzi_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.718318 wizzi_utils-8.0.2/wizzi_utils/google/
--rw-rw-rw-   0        0        0      140 2023-01-06 10:04:31.000000 wizzi_utils-8.0.2/wizzi_utils/google/__init__.py
--rw-rw-rw-   0        0        0    29127 2023-01-06 10:03:22.000000 wizzi_utils-8.0.2/wizzi_utils/google/google_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.723384 wizzi_utils-8.0.2/wizzi_utils/google/test/
--rw-rw-rw-   0        0        0      111 2023-01-06 10:04:40.000000 wizzi_utils-8.0.2/wizzi_utils/google/test/__init__.py
--rw-rw-rw-   0        0        0    12386 2023-01-06 10:05:26.000000 wizzi_utils-8.0.2/wizzi_utils/google/test/test_google_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.744562 wizzi_utils-8.0.2/wizzi_utils/json/
--rw-rw-rw-   0        0        0      134 2021-07-20 13:56:12.000000 wizzi_utils-8.0.2/wizzi_utils/json/__init__.py
--rw-rw-rw-   0        0        0     3035 2021-06-20 09:51:39.000000 wizzi_utils-8.0.2/wizzi_utils/json/json_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.770411 wizzi_utils-8.0.2/wizzi_utils/json/test/
--rw-rw-rw-   0        0        0      107 2021-07-20 13:56:12.000000 wizzi_utils-8.0.2/wizzi_utils/json/test/__init__.py
--rw-rw-rw-   0        0        0     1815 2021-06-04 08:44:35.000000 wizzi_utils-8.0.2/wizzi_utils/json/test/test_json_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.783453 wizzi_utils-8.0.2/wizzi_utils/misc/
--rw-rw-rw-   0        0        0      134 2021-04-25 10:54:11.000000 wizzi_utils-8.0.2/wizzi_utils/misc/__init__.py
--rw-rw-rw-   0        0        0    89235 2023-01-06 10:07:28.000000 wizzi_utils-8.0.2/wizzi_utils/misc/misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.815979 wizzi_utils-8.0.2/wizzi_utils/misc/test/
--rw-rw-rw-   0        0        0      107 2021-04-25 10:50:19.000000 wizzi_utils-8.0.2/wizzi_utils/misc/test/__init__.py
--rw-rw-rw-   0        0        0    41103 2022-12-30 13:22:06.000000 wizzi_utils-8.0.2/wizzi_utils/misc/test/test_misc_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.860234 wizzi_utils-8.0.2/wizzi_utils/models/
--rw-rw-rw-   0        0        0      316 2021-08-10 23:21:36.000000 wizzi_utils-8.0.2/wizzi_utils/models/__init__.py
--rw-rw-rw-   0        0        0    32920 2022-05-26 16:04:02.000000 wizzi_utils-8.0.2/wizzi_utils/models/base_models.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.911011 wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/
--rw-rw-rw-   0        0        0      447 2021-08-10 23:21:36.000000 wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/__init__.py
--rw-rw-rw-   0        0        0    11967 2021-08-10 23:14:47.000000 wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/object_detection.py
--rw-rw-rw-   0        0        0    30085 2021-08-10 21:23:15.000000 wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/pose_detection.py
--rw-rw-rw-   0        0        0    13099 2022-05-26 16:04:02.000000 wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/tracking.py
--rw-rw-rw-   0        0        0    41515 2021-07-01 16:56:54.000000 wizzi_utils-8.0.2/wizzi_utils/models/labels_bank.py
--rw-rw-rw-   0        0        0    53088 2021-08-06 10:02:29.000000 wizzi_utils-8.0.2/wizzi_utils/models/models_configs.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.977030 wizzi_utils-8.0.2/wizzi_utils/models/test/
--rw-rw-rw-   0        0        0      201 2021-08-11 11:50:12.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/__init__.py
--rw-rw-rw-   0        0        0     9974 2022-07-07 19:03:32.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/shared_code_for_tests.py
--rw-rw-rw-   0        0        0     3796 2021-08-11 11:36:11.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_od.py
--rw-rw-rw-   0        0        0     4868 2021-08-11 11:12:59.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_pd.py
--rw-rw-rw-   0        0        0     5884 2022-10-10 17:54:59.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_tracking.py
--rw-rw-rw-   0        0        0     1916 2021-08-11 11:44:40.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_models.py
--rw-rw-rw-   0        0        0     3683 2021-08-11 11:39:43.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_tflite_od.py
--rw-rw-rw-   0        0        0     4392 2021-08-11 11:09:51.000000 wizzi_utils-8.0.2/wizzi_utils/models/test/test_tflite_pd.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.002681 wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/
--rw-rw-rw-   0        0        0      308 2021-08-10 23:21:36.000000 wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/__init__.py
--rw-rw-rw-   0        0        0    12906 2022-05-26 16:39:19.000000 wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/object_detection.py
--rw-rw-rw-   0        0        0    19806 2022-05-26 16:39:19.000000 wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/pose_detection.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.021000 wizzi_utils-8.0.2/wizzi_utils/open_cv/
--rw-rw-rw-   0        0        0      143 2021-07-20 13:58:01.000000 wizzi_utils-8.0.2/wizzi_utils/open_cv/__init__.py
--rw-rw-rw-   0        0        0    53206 2022-10-10 16:08:57.000000 wizzi_utils-8.0.2/wizzi_utils/open_cv/open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.039246 wizzi_utils-8.0.2/wizzi_utils/open_cv/test/
--rw-rw-rw-   0        0        0      113 2021-07-20 13:57:56.000000 wizzi_utils-8.0.2/wizzi_utils/open_cv/test/__init__.py
--rw-rw-rw-   0        0        0    40415 2022-12-30 13:17:47.000000 wizzi_utils-8.0.2/wizzi_utils/open_cv/test/test_open_cv_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.077921 wizzi_utils-8.0.2/wizzi_utils/pyplot/
--rw-rw-rw-   0        0        0      140 2021-07-20 13:59:48.000000 wizzi_utils-8.0.2/wizzi_utils/pyplot/__init__.py
--rw-rw-rw-   0        0        0    67152 2022-10-10 17:19:31.000000 wizzi_utils-8.0.2/wizzi_utils/pyplot/pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.095880 wizzi_utils-8.0.2/wizzi_utils/pyplot/test/
--rw-rw-rw-   0        0        0      111 2021-07-20 13:59:59.000000 wizzi_utils-8.0.2/wizzi_utils/pyplot/test/__init__.py
--rw-rw-rw-   0        0        0    38480 2022-10-10 17:25:23.000000 wizzi_utils-8.0.2/wizzi_utils/pyplot/test/test_pyplot_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.125326 wizzi_utils-8.0.2/wizzi_utils/socket/
--rw-rw-rw-   0        0        0      140 2021-07-20 14:03:00.000000 wizzi_utils-8.0.2/wizzi_utils/socket/__init__.py
--rw-rw-rw-   0        0        0    24420 2022-12-30 11:13:12.000000 wizzi_utils-8.0.2/wizzi_utils/socket/socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.149979 wizzi_utils-8.0.2/wizzi_utils/socket/test/
--rw-rw-rw-   0        0        0      111 2021-07-20 14:03:04.000000 wizzi_utils-8.0.2/wizzi_utils/socket/test/__init__.py
--rw-rw-rw-   0        0        0    10439 2022-12-30 11:20:16.000000 wizzi_utils-8.0.2/wizzi_utils/socket/test/test_socket_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.166193 wizzi_utils-8.0.2/wizzi_utils/tflite/
--rw-rw-rw-   0        0        0      264 2022-10-10 17:45:09.000000 wizzi_utils-8.0.2/wizzi_utils/tflite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.181481 wizzi_utils-8.0.2/wizzi_utils/tflite/test/
--rw-rw-rw-   0        0        0      105 2021-07-20 14:06:44.000000 wizzi_utils-8.0.2/wizzi_utils/tflite/test/__init__.py
--rw-rw-rw-   0        0        0      403 2021-07-06 09:00:59.000000 wizzi_utils-8.0.2/wizzi_utils/tflite/test/test_tflite.py
--rw-rw-rw-   0        0        0     2952 2022-10-10 16:19:42.000000 wizzi_utils-8.0.2/wizzi_utils/tflite/tflite_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.183475 wizzi_utils-8.0.2/wizzi_utils/torch/
--rw-rw-rw-   0        0        0      463 2022-09-21 10:27:11.000000 wizzi_utils-8.0.2/wizzi_utils/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.209471 wizzi_utils-8.0.2/wizzi_utils/torch/test/
--rw-rw-rw-   0        0        0      109 2021-07-20 14:05:29.000000 wizzi_utils-8.0.2/wizzi_utils/torch/test/__init__.py
--rw-rw-rw-   0        0        0    16352 2021-08-11 12:19:47.000000 wizzi_utils-8.0.2/wizzi_utils/torch/test/test_torch_tools.py
--rw-rw-rw-   0        0        0    26441 2022-06-23 17:47:26.000000 wizzi_utils-8.0.2/wizzi_utils/torch/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.227410 wizzi_utils-8.0.2/wizzi_utils/tts/
--rw-rw-rw-   0        0        0      125 2021-07-20 14:07:03.000000 wizzi_utils-8.0.2/wizzi_utils/tts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:53.242423 wizzi_utils-8.0.2/wizzi_utils/tts/test/
--rw-rw-rw-   0        0        0       99 2021-07-20 14:07:07.000000 wizzi_utils-8.0.2/wizzi_utils/tts/test/__init__.py
--rw-rw-rw-   0        0        0     3175 2022-07-02 20:01:08.000000 wizzi_utils-8.0.2/wizzi_utils/tts/test/test_tts.py
--rw-rw-rw-   0        0        0    21575 2022-07-02 15:29:07.000000 wizzi_utils-8.0.2/wizzi_utils/tts/tts.py
--rw-rw-rw-   0        0        0     2477 2022-12-30 13:22:24.000000 wizzi_utils-8.0.2/wizzi_utils/wizzi_utils_requirements.txt
-drwxrwxrwx   0        0        0        0 2023-01-06 10:08:52.711519 wizzi_utils-8.0.2/wizzi_utils.egg-info/
--rw-rw-rw-   0        0        0     7022 2023-01-06 10:08:52.000000 wizzi_utils-8.0.2/wizzi_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4254 2023-01-06 10:08:52.000000 wizzi_utils-8.0.2/wizzi_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 10:08:52.000000 wizzi_utils-8.0.2/wizzi_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-01-06 10:08:52.000000 wizzi_utils-8.0.2/wizzi_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0      491 2023-01-06 10:08:52.000000 wizzi_utils-8.0.2/wizzi_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.019103 wizzi_utils-8.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     6815 2023-05-26 18:27:41.019103 wizzi_utils-8.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5979 2023-05-18 12:16:03.000000 wizzi_utils-8.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-26 18:27:41.019103 wizzi_utils-8.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2721 2023-05-26 18:26:10.000000 wizzi_utils-8.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.972233 wizzi_utils-8.0.3/wizzi_utils/
+-rw-rw-rw-   0        0        0     2215 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.972233 wizzi_utils-8.0.3/wizzi_utils/google/
+-rw-rw-rw-   0        0        0      140 2023-05-18 12:28:31.000000 wizzi_utils-8.0.3/wizzi_utils/google/__init__.py
+-rw-rw-rw-   0        0        0    29127 2023-05-18 12:36:17.000000 wizzi_utils-8.0.3/wizzi_utils/google/google_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.972233 wizzi_utils-8.0.3/wizzi_utils/google/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/google/test/__init__.py
+-rw-rw-rw-   0        0        0    12539 2023-05-18 12:32:45.000000 wizzi_utils-8.0.3/wizzi_utils/google/test/test_google_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.972233 wizzi_utils-8.0.3/wizzi_utils/json/
+-rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/json/__init__.py
+-rw-rw-rw-   0        0        0     3035 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/json/json_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/json/test/
+-rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/json/test/__init__.py
+-rw-rw-rw-   0        0        0     1815 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/json/test/test_json_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/misc/
+-rw-rw-rw-   0        0        0      134 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/misc/__init__.py
+-rw-rw-rw-   0        0        0    93269 2023-05-26 18:26:24.000000 wizzi_utils-8.0.3/wizzi_utils/misc/misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/misc/test/
+-rw-rw-rw-   0        0        0      107 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/misc/test/__init__.py
+-rw-rw-rw-   0        0        0    41133 2023-05-18 11:21:37.000000 wizzi_utils-8.0.3/wizzi_utils/misc/test/test_misc_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/models/
+-rw-rw-rw-   0        0        0      316 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/__init__.py
+-rw-rw-rw-   0        0        0    32920 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/base_models.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/
+-rw-rw-rw-   0        0        0      447 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/__init__.py
+-rw-rw-rw-   0        0        0    11967 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/object_detection.py
+-rw-rw-rw-   0        0        0    30085 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/pose_detection.py
+-rw-rw-rw-   0        0        0    13099 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/tracking.py
+-rw-rw-rw-   0        0        0    41515 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/labels_bank.py
+-rw-rw-rw-   0        0        0    53088 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/models_configs.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.987856 wizzi_utils-8.0.3/wizzi_utils/models/test/
+-rw-rw-rw-   0        0        0      201 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/__init__.py
+-rw-rw-rw-   0        0        0     9974 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/shared_code_for_tests.py
+-rw-rw-rw-   0        0        0     3796 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_od.py
+-rw-rw-rw-   0        0        0     4868 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_pd.py
+-rw-rw-rw-   0        0        0     5884 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_tracking.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_models.py
+-rw-rw-rw-   0        0        0     3683 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_tflite_od.py
+-rw-rw-rw-   0        0        0     4392 2023-05-18 13:12:36.000000 wizzi_utils-8.0.3/wizzi_utils/models/test/test_tflite_pd.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/
+-rw-rw-rw-   0        0        0      308 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/__init__.py
+-rw-rw-rw-   0        0        0    12906 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/object_detection.py
+-rw-rw-rw-   0        0        0    19806 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/pose_detection.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/open_cv/
+-rw-rw-rw-   0        0        0      143 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/open_cv/__init__.py
+-rw-rw-rw-   0        0        0    53198 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/open_cv/open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/open_cv/test/
+-rw-rw-rw-   0        0        0      113 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/open_cv/test/__init__.py
+-rw-rw-rw-   0        0        0    40649 2023-05-18 12:57:14.000000 wizzi_utils-8.0.3/wizzi_utils/open_cv/test/test_open_cv_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/pyplot/
+-rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/pyplot/__init__.py
+-rw-rw-rw-   0        0        0    67152 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/pyplot/pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/pyplot/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/pyplot/test/__init__.py
+-rw-rw-rw-   0        0        0    38480 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/pyplot/test/test_pyplot_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/socket/
+-rw-rw-rw-   0        0        0      140 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/socket/__init__.py
+-rw-rw-rw-   0        0        0    24353 2023-05-18 11:25:24.000000 wizzi_utils-8.0.3/wizzi_utils/socket/socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/socket/test/
+-rw-rw-rw-   0        0        0      111 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/socket/test/__init__.py
+-rw-rw-rw-   0        0        0    10494 2023-05-18 11:29:49.000000 wizzi_utils-8.0.3/wizzi_utils/socket/test/test_socket_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/tflite/
+-rw-rw-rw-   0        0        0      264 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tflite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/tflite/test/
+-rw-rw-rw-   0        0        0      105 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tflite/test/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tflite/test/test_tflite.py
+-rw-rw-rw-   0        0        0     2952 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tflite/tflite_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/torch/
+-rw-rw-rw-   0        0        0      636 2023-05-26 18:23:15.000000 wizzi_utils-8.0.3/wizzi_utils/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/torch/test/
+-rw-rw-rw-   0        0        0      109 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/torch/test/__init__.py
+-rw-rw-rw-   0        0        0    16354 2023-05-18 13:15:33.000000 wizzi_utils-8.0.3/wizzi_utils/torch/test/test_torch_tools.py
+-rw-rw-rw-   0        0        0    26441 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/torch/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/tts/
+-rw-rw-rw-   0        0        0      125 2023-05-18 13:05:38.000000 wizzi_utils-8.0.3/wizzi_utils/tts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:41.003480 wizzi_utils-8.0.3/wizzi_utils/tts/test/
+-rw-rw-rw-   0        0        0       99 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tts/test/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 08:10:35.000000 wizzi_utils-8.0.3/wizzi_utils/tts/test/test_tts.py
+-rw-rw-rw-   0        0        0    21592 2023-05-18 13:17:11.000000 wizzi_utils-8.0.3/wizzi_utils/tts/tts.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:27:40.972233 wizzi_utils-8.0.3/wizzi_utils.egg-info/
+-rw-rw-rw-   0        0        0     6815 2023-05-26 18:27:40.000000 wizzi_utils-8.0.3/wizzi_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4360 2023-05-26 18:27:40.000000 wizzi_utils-8.0.3/wizzi_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:27:40.000000 wizzi_utils-8.0.3/wizzi_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-26 18:27:40.000000 wizzi_utils-8.0.3/wizzi_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      491 2023-05-26 18:27:40.000000 wizzi_utils-8.0.3/wizzi_utils.egg-info/top_level.txt
```

### Comparing `wizzi_utils-8.0.2/LICENSE.txt` & `wizzi_utils-8.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/PKG-INFO` & `wizzi_utils-8.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: wizzi_utils
-Version: 8.0.2
+Version: 8.0.3
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.2.tar.gz
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.3.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Package wizzi utils:
+# Package [wizzi utils](https://github.com/2easy4wizzi/wizzi_utils_pypi/tree/main):
+
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/2easy4wizzi.jpeg)
 
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true)
-<!--- <img src="https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true" width="155" height="90" /> -->
 ## Brief
 
 * "wizzi_utils" main usage is for debugging and fast coding.
 * The package is cross-platform (most of the functions tested on Windows and linux).
 * The package is well documented and contain many easy access common functions.
     * In addition, almost every function is used in a test(more an example) I've written for learning purposes.
 * Package includes tools for json, open_cv, pyplot, socket, torch, text to speach and more.
@@ -42,15 +42,15 @@
 # The above import, will give access to all wizzi utils main module and the extra modules 
 # only if the packages are installed
 print(wu.to_str(var=2, title='my_int'))  # this will 100% work
 wu.test.to_str_test()  # for a wide example of to_str function
 print(wu.tt.to_str(var=3, title='my_int'))  # tt for torch tools. will work if torch installed
 wu.tt.test.to_str_test()  # for a wide example of tt.to_str function
 # If facing packages issues and want to know what packages I used, call the following
-wu.wizzi_utils_requirements()  # updated on 10/10/2022 
+wu.download_wizzi_utils_env_snapshot()  # updated on 10/10/2022 
 ```
 
 ### list of all the packages
 
 ```python
 import wizzi_utils as wu
 
@@ -98,16 +98,15 @@
         tf_v=True,
         cv2_v=True,
         with_pip_list=False,
         with_profiler=False
     )
 ```
 
-<!--- ![main wrapper img](resources/readme_images/main_wrapper.PNG) -->
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/main_wrapper.PNG?raw=true)
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/main_wrapper.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # fps measurements:
 fps = wu.FPS(last_k=3, cache_size=5, summary_title='classFPS_test')
 for t in range(10):
@@ -119,16 +118,15 @@
         wu.sleep(seconds=1)
     fps.update(ack_progress=ack)
     if t == 5:
         print('\tget_fps() = {:.4f}'.format(fps.get_fps()))
 fps.finalize()
 ```
 
-<!--- ![fps img](resources/readme_images/fps.PNG) -->
-![fps img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/fps.PNG?raw=true)
+![fps img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/fps.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * cv2 show image with extra control:
 * concatenation of several images(e.g. 2 cameras frames)
@@ -153,16 +151,15 @@
     resize=1.5,  # 150%
     grid=(3, 1),  # 3 rows 1 col
     header='cool, no?',
     separator_c='aqua',
 )
 ```
 
-<!--- ![display images img](resources/readme_images/display_images.PNG) -->
-![display images img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/display_images.PNG?raw=true)
+![display images img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/display_images.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * object detection models
 * pose detection models
@@ -172,21 +169,22 @@
 wu.models.test.test_cv2_pose_detection_models()
 wu.models.test.test_cv2_tracking_models()
 ```
 
 <!--- ![object detection img](resources/readme_images/yolov4.PNG) -->
 <!--- ![pose estimation img](resources/readme_images/pose.PNG) -->
 <!--- ![tracking img](resources/readme_images/tracking.PNG) -->
-![object detection img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/yolov4.PNG?raw=true)
-![pose estimation img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/pose.PNG?raw=true)
-![tracking img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tracking.PNG?raw=true)
+![object detection img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/yolov4.PNG?raw=true)
+![pose estimation img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/pose.PNG?raw=true)
+![tracking img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tracking.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # text to speak gui over pyttsx3 and pyQt5 packages
 wu.tts.test.run_machine_buddy_gui_test()
 ```
 
-<!--- ![tts img](resources/readme_images/tts.PNG) -->
-![tts img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tts.PNG?raw=true)
+![tts img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tts.PNG?raw=true)
+
+
```

### Comparing `wizzi_utils-8.0.2/README.md` & `wizzi_utils-8.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Package wizzi utils:
+# Package [wizzi utils](https://github.com/2easy4wizzi/wizzi_utils_pypi/tree/main):
+
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/2easy4wizzi.jpeg)
 
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true)
-<!--- <img src="https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true" width="155" height="90" /> -->
 ## Brief
 
 * "wizzi_utils" main usage is for debugging and fast coding.
 * The package is cross-platform (most of the functions tested on Windows and linux).
 * The package is well documented and contain many easy access common functions.
     * In addition, almost every function is used in a test(more an example) I've written for learning purposes.
 * Package includes tools for json, open_cv, pyplot, socket, torch, text to speach and more.
@@ -21,15 +21,15 @@
 # The above import, will give access to all wizzi utils main module and the extra modules 
 # only if the packages are installed
 print(wu.to_str(var=2, title='my_int'))  # this will 100% work
 wu.test.to_str_test()  # for a wide example of to_str function
 print(wu.tt.to_str(var=3, title='my_int'))  # tt for torch tools. will work if torch installed
 wu.tt.test.to_str_test()  # for a wide example of tt.to_str function
 # If facing packages issues and want to know what packages I used, call the following
-wu.wizzi_utils_requirements()  # updated on 10/10/2022 
+wu.download_wizzi_utils_env_snapshot()  # updated on 10/10/2022 
 ```
 
 ### list of all the packages
 
 ```python
 import wizzi_utils as wu
 
@@ -77,16 +77,15 @@
         tf_v=True,
         cv2_v=True,
         with_pip_list=False,
         with_profiler=False
     )
 ```
 
-<!--- ![main wrapper img](resources/readme_images/main_wrapper.PNG) -->
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/main_wrapper.PNG?raw=true)
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/main_wrapper.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # fps measurements:
 fps = wu.FPS(last_k=3, cache_size=5, summary_title='classFPS_test')
 for t in range(10):
@@ -98,16 +97,15 @@
         wu.sleep(seconds=1)
     fps.update(ack_progress=ack)
     if t == 5:
         print('\tget_fps() = {:.4f}'.format(fps.get_fps()))
 fps.finalize()
 ```
 
-<!--- ![fps img](resources/readme_images/fps.PNG) -->
-![fps img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/fps.PNG?raw=true)
+![fps img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/fps.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * cv2 show image with extra control:
 * concatenation of several images(e.g. 2 cameras frames)
@@ -132,16 +130,15 @@
     resize=1.5,  # 150%
     grid=(3, 1),  # 3 rows 1 col
     header='cool, no?',
     separator_c='aqua',
 )
 ```
 
-<!--- ![display images img](resources/readme_images/display_images.PNG) -->
-![display images img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/display_images.PNG?raw=true)
+![display images img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/display_images.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * object detection models
 * pose detection models
@@ -151,21 +148,20 @@
 wu.models.test.test_cv2_pose_detection_models()
 wu.models.test.test_cv2_tracking_models()
 ```
 
 <!--- ![object detection img](resources/readme_images/yolov4.PNG) -->
 <!--- ![pose estimation img](resources/readme_images/pose.PNG) -->
 <!--- ![tracking img](resources/readme_images/tracking.PNG) -->
-![object detection img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/yolov4.PNG?raw=true)
-![pose estimation img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/pose.PNG?raw=true)
-![tracking img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tracking.PNG?raw=true)
+![object detection img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/yolov4.PNG?raw=true)
+![pose estimation img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/pose.PNG?raw=true)
+![tracking img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tracking.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # text to speak gui over pyttsx3 and pyQt5 packages
 wu.tts.test.run_machine_buddy_gui_test()
 ```
 
-<!--- ![tts img](resources/readme_images/tts.PNG) -->
-![tts img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tts.PNG?raw=true)
+![tts img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tts.PNG?raw=true)
```

### Comparing `wizzi_utils-8.0.2/setup.py` & `wizzi_utils-8.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         'wizzi_utils/tts',
         'wizzi_utils/tts/test',
         'wizzi_utils/models',
         'wizzi_utils/models/cv2_models',
         'wizzi_utils/models/tflite_models',
         'wizzi_utils/models/test',
     ],
-    version='8.0.2',
+    version='8.0.3',
     license='MIT',  # https://help.github.com/articles/licensing-a-repository
     description='Debugging tools and fast coding',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Gilad Eini',
     author_email='giladEini@gmail.com',
     url='https://github.com/2easy4wizzi/wizzi_utils_pypi',  # link to github
-    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.2.tar.gz',
+    download_url='https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.3.tar.gz',
     keywords=[  # Keywords that define your package best
         'debugging tools',
         'json',
         'open cv',
         'pyplot',
         'socket',
         'torch',
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/__init__.py` & `wizzi_utils-8.0.3/wizzi_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/google/google_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/google/google_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         * HOST could be a CLIENT
      HOST:
          1 https://console.cloud.google.com/
          2 Dashboard - create project
          3 enter project -
          4 type in search "enable Api and services" and click
          5 find google drive API below in the list and click. up in the tool bar click enable api
-         4 on the left(in the same place) click CREDENTIALS - client id -
+         6 on the left(in the same place) click CREDENTIALS - client id -
             desktop app and download the dot json file. you can rename to client_secret.json
             this file will be the "client_config_file" in your settings.yaml file
      CLIENT:
          1 HOST must add CLIENT (including himself):
             in the same screen as step 4 from HOST, click under CREDENTIALS on "OAuth consent screen"
              +Add users, under test users, add user email (that will be logging from the python)
          2 pip install pydrive
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/google/test/test_google_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/google/test/test_google_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from wizzi_utils.misc import misc_tools as mt
 from wizzi_utils.misc.test import test_misc_tools as mtt
 from wizzi_utils.socket import socket_tools as st
 import os
 
 
 def build_gh() -> got.GDriveHandler:
+    # set env variable to the dir containing the settings.yaml file
+    gdrive_secrets_dir = mt.get_env_variable(key='GDRIVE_DIR')
     gh = got.GDriveHandler(
-        yaml_path='./GDrive2/settings.yaml',
+        yaml_path='{}/settings.yaml'.format(gdrive_secrets_dir),
         tabs=1,
         dir_color='reverse',
         file_color='light_blue',
         title_color=['underlined', 'light_yellow']
 
     )
     print(gh)
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/json/json_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/json/json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/json/test/test_json_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/json/test/test_json_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/misc/misc_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/misc/misc_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from traceback import TracebackException
 # noinspection PyProtectedMember
 # from pip import _internal
 import subprocess
 import pkg_resources
 from enum import Enum
 
+import wizzi_utils
+
 LINES = '-' * 80
 NOT_FOUND = '{} Not found'
 CREATED = '{} Created'
 EXISTS = '{} Exists'
 DELETED = '{} Deleted'
 MOVED = '{} Moved to {}'
 COPIED = '{} Copied to {}'
@@ -261,65 +263,119 @@
                     pa = ls_spl[2]
         f_obj.close()
         if ma and mi and pa:
             cudnn_v = '{}.{}.{}'.format(ma, mi, pa)
     return cudnn_v
 
 
+def extract_cuda_version_linux(cuda_path: str) -> str:
+    cuda_v = None
+
+    if os.path.isfile('{}/version.txt'.format(cuda_path)):
+        cuda_v_file = '{}/version.txt'.format(cuda_path)
+        f_obj = open(cuda_v_file, 'r')
+        for line in f_obj:
+            ls = line.strip()
+            if ls.startswith('CUDA Version'):
+                ls_spl = ls.split(' ')
+                if len(ls_spl) == 3:
+                    cuda_v = line.strip().split(' ')[2]
+                    break
+    elif os.path.isfile('{}/version.json'.format(cuda_path)):
+        import json
+        cuda_v_file = '{}/version.json'.format(cuda_path)
+        j_obj = json.load(fp=open(cuda_v_file))
+        cuda_v = j_obj['cuda']['version']
+
+    return cuda_v
+
+
 def get_cuda_version(ack: bool = False, tabs: int = 1) -> str:
     """
     :param ack:
     :param tabs:
     :return: cuda version if found on environment variables
     see get_cuda_version_test()
     """
-    cuda_v = None
-    cudnn_v = None
+    cuda_str = add_color('* No CUDA found', ops=FAIL_C)
+    try:
+        cuda_path, cuda_v, cudnn_v = None, None, None
+        if is_windows():
+            # e.g. C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v10.2
+            cuda_path = get_env_variable(key='CUDA_PATH')
+            if cuda_path is not None and os.path.isdir(cuda_path):
+                cuda_v = os.path.basename(cuda_path)  # version taken from dir name
+                cudnn_path = '{}/include/cudnn_version.h'.format(cuda_path)
+                if os.path.isfile(cudnn_path):
+                    cudnn_v = get_cudnn_version(cudnn_path=cudnn_path)
 
-    if is_windows():
-        cuda_path = get_env_variable(key='CUDA_PATH')
-        if cuda_path is not None:
-            cuda_v = os.path.basename(cuda_path)
+        elif is_linux():
+            # try to locate cuda version file
+            known_options = [
+                '/usr/local/cuda',
+            ]
+
+            # e.g. /usr/local/cuda-11.7 or /usr/local/cuda
+            cuda_path = get_env_variable(key='CUDA_ROOT')  # first try with env variable
+            if cuda_path is None or not os.path.isdir(cuda_path):
+                for option in known_options:  # second try known paths
+                    if os.path.isdir(option):
+                        cuda_path = option
+                        break  # found cuda dir
+
+            if cuda_path is not None and os.path.isdir(cuda_path):  # if we have the cuda dir
+                cuda_v = extract_cuda_version_linux(cuda_path)
+
+        # windows and linux
+        if cuda_v is not None and cuda_path is not None:
+            # first attempt
             cudnn_v = get_cudnn_version(cudnn_path='{}/include/cudnn.h'.format(cuda_path))
 
-    elif is_linux():
-        cuda_path = get_env_variable(key='CUDA_ROOT')
-        cuda_v_file = '{}/version.txt'.format(cuda_path)
-        if os.path.exists(cuda_v_file):
-            f_obj = open(cuda_v_file, 'r')
-            for line in f_obj:
-                ls = line.strip()
-                if ls.startswith('CUDA Version'):
-                    ls_spl = ls.split(' ')
-                    if len(ls_spl) == 3:
-                        cuda_v = line.strip().split(' ')[2]
-                        break
-        if cuda_v is not None:
-            cudnn_path = '{}/include/cudnn.h'.format(cuda_path)
-            if is_jetson_nano():  # cudnn location on jetson_nano
-                cudnn_path = '/usr/include/aarch64-linux-gnu/cudnn_version_v8.h'
-            cudnn_v = get_cudnn_version(cudnn_path=cudnn_path)
-            if cudnn_v is None:  # TRY via env variable
+            # second attempt
+            if cudnn_v is None:
+                cudnn_v = get_cudnn_version(cudnn_path='{}/include/cudnn_version.h'.format(cuda_path))
+
+            # third - env variable
+            if cudnn_v is None:
                 cudnn_path = get_env_variable(key='CUDNN_FILE_PATH')
                 if cudnn_path is not None:
                     cudnn_v = get_cudnn_version(cudnn_path=cudnn_path)
 
-    if cuda_v is None:
-        cuda_v = add_color('* No CUDA_PATH found', ops=FAIL_C)
-    else:
-        cuda_v = '{}* CUDA Version: {}'.format(tabs * '\t', cuda_v)
-        if cudnn_v is not None:
-            cuda_v += ' (cuDNN Version {})'.format(cudnn_v)
-        else:
-            cuda_v += ' (No cuDNN found)'
-        cuda_v = add_color(cuda_v, ops=SUCCESS_C)
+        if cuda_v is not None:
+            cuda_str = '{}* CUDA Version: {}'.format(tabs * '\t', cuda_v)
+            if cudnn_v is not None:
+                cuda_str += ' (cuDNN Version {})'.format(cudnn_v)
+            else:
+                cuda_str += ' (No cuDNN found)'
+            cuda_str = add_color(cuda_str, ops=SUCCESS_C)
+
+        if ack:
+            print(cuda_str)
+    except Exception:
+        pass
+    return cuda_str
 
-    if ack:
-        print(cuda_v)
-    return cuda_v
+
+def get_nvidia_gpus() -> str:
+    try:
+        cmd = 'nvidia-smi --query-gpu=gpu_name,memory.total --format=csv,noheader'
+        gpu_str_lines = run_shell_command_and_get_out(cmd=cmd, ack_cmd=False)
+        # gpu_str_lines = ['Quadro RTX 4000, 8192 Mib', 'Quadro RTX 4000, 8192 Mib']
+
+        gpu_str_all = ''
+        for i, gpu_str in enumerate(gpu_str_lines):
+            gpu_name, gpu_size = gpu_str.split(', ')
+            gpu_str_all += '[device {}] {} ({})'.format(i, gpu_name, gpu_size)
+            if i + 1 < len(gpu_str_lines):
+                gpu_str_all += ', '
+
+        gpu_str_all = add_color(f'* Nvidia GPUs: {gpu_str_all}', ops=SUCCESS_C)
+    except Exception:
+        gpu_str_all = add_color('* Nvidia GPUs: (Nvidia-smi not available)', ops=FAIL_C)
+    return gpu_str_all
 
 
 def get_env_variables(ack: bool = False, tabs: int = 1) -> dict:
     """
     :param ack:
     :param tabs:
     :return: dict with envs
@@ -456,15 +512,15 @@
 
 
 def version() -> str:
     """
     :return:
     """
     # v = pkg_resources.require("wizzi_utils")[0].version
-    v = '8.0.2'
+    v = '8.0.3'
     return v
 
 
 def is_windows() -> bool:
     """
     :return:
     see os_test() - tested
@@ -560,25 +616,27 @@
 
 
 def main_wrapper(
         main_function: Callable,
         seed: int = -1,
         ipv4: bool = False,
         cuda_off: bool = False,
+        nvid_gpu: bool = True,
         torch_v: bool = False,
         tf_v: bool = False,
         cv2_v: bool = False,
         with_pip_list: bool = False,
         with_profiler: bool = False
 ) -> None:
     """
     :param main_function: the function to run
     :param seed: if -1 no seed, else set_seed(seed=seed)
     :param ipv4: print computer ipv4
     :param cuda_off: make gpu invisible and force run on cpu
+    :param nvid_gpu: info on nvidia gpus. uses nvidia-smi
     :param torch_v: print torch version
     :param tf_v: print tensorflow lite version
     :param cv2_v: print opencv version
     :param with_pip_list: print pip list (all libraries installed)
     :param with_profiler: run profiler
     template:
     wu.main_wrapper(
@@ -623,14 +681,18 @@
 
     cuda_msg = get_cuda_version(ack=False, tabs=0)
     if cuda_off:
         make_cuda_invisible()
         cuda_msg += ' (Turned off)'
     print(cuda_msg)
 
+    if nvid_gpu:
+        nvidia_gpus_info = get_nvidia_gpus()
+        print(nvidia_gpus_info)
+
     if torch_v:
         try:
             from wizzi_utils.torch.torch_tools import get_torch_version
             print(get_torch_version(ack=False, tabs=0))
         except (ImportError, ModuleNotFoundError, NameError, AttributeError) as err:
             print(add_color('* torch not Found. error: {}'.format(err), 'r'))
 
@@ -1881,26 +1943,14 @@
         for i, percentage in enumerate(per_core_raw):
             # print(f"Core {i}: {percentage}%")
             per_core += 'C{}-{}% '.format(i, percentage)
         string += '\n{}\tCPU Usage per core {}'.format(tabs * '\t', per_core)
     return string
 
 
-def wizzi_utils_requirements():
-    print('A snapshot of my environment packages:')
-
-    misc_file = get_file_name(depth=1)
-    misc_dir = os.path.dirname(misc_file)
-    main_src_dir = '{}/../'.format(misc_dir)
-
-    req_file = '{}/wizzi_utils_requirements.txt'.format(main_src_dir)
-    _ = read_file_lines(fp=req_file, ack=True)
-    return
-
-
 def last_exception(tabs: int = 1):
     """
     prints last_exception occurred
     :return:
     """
     exception_error(sys.exc_info()[1], tabs=tabs)
     return
@@ -2304,14 +2354,18 @@
         except (ImportError, ModuleNotFoundError, NameError, AttributeError) as err:
             out.write('# * {}\n'.format(err))
 
         cuda_msg = get_cuda_version(ack=False, tabs=0)
         cuda_msg = remove_colors(cuda_msg)
         out.write('# {}\n'.format(cuda_msg))
 
+        nvidia_gpus_info = get_nvidia_gpus()
+        nvidia_gpus_info = remove_colors(nvidia_gpus_info)
+        out.write('# {}\n'.format(nvidia_gpus_info))
+
         try:
             from wizzi_utils.open_cv.open_cv_tools import get_cv_version
             cv_v = get_cv_version(ack=False, tabs=0)
             cv_v = remove_colors(cv_v)
             out.write('# {}\n'.format(cv_v))
         except (ImportError, ModuleNotFoundError, NameError, AttributeError) as err:
             out.write('# * opencv-python not Found. error: {}\n'.format(err))
@@ -2615,22 +2669,23 @@
     :param repo_name:
     :param ack:
     :return:
     anywhere from the project - we should have prefix/repo_name/suffix
     return prefix/repo_name
     prefix change on each system
     """
-    repo_root_path = get_file_name(depth=1)
-    if repo_name in repo_root_path:
-        while not repo_root_path.endswith(repo_name):  # strip dir until we get to repo_name
-            repo_root_path = os.path.dirname(repo_root_path)
+    cwd = os.getcwd()
+    if repo_name in cwd:
+        cwd_split = cwd.split(repo_name)
+        repo_root_path = os.path.join(cwd_split[0], repo_name)
         if ack:
             print('\tRepoRoot={}'.format(repo_root_path))
     else:
         exception_error('{} not found in current path'.format(repo_name))
+        repo_root_path = 'N/A'
     return repo_root_path
 
 
 def rename_folder(dir_path: str, new_name: str, ack: bool = True) -> str:
     """
     renames a folder and returns the path of the new folder
     :param dir_path: path of the target folder
@@ -2648,7 +2703,53 @@
             exception_error(e='new folder name {} exist. can\'t rename...'.format(new_name_fp))
         else:
             os.rename(dir_path, new_name_fp)
             if ack:
                 files_n = len(find_files_in_folder(dir_path=new_name_fp, file_suffix=''))
                 print('\t{} renamed to {} ({} files)'.format(dir_path, new_name_fp, files_n))
     return new_name_fp
+
+
+def download_wizzi_utils_env_snapshot(ack: bool = False):
+    """
+    snapshot of a working environment
+    """
+    try:
+        from wizzi_utils.socket.socket_tools import download_file
+        snapshot_file_path = './wizzi_utils_env_snapshot.txt'
+        if not os.path.exists(snapshot_file_path):
+            git_pref = 'https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi'
+            success = download_file(
+                url=f'{git_pref}/main/resources/wizzi_utils_env_snapshot.txt',
+                dst_path=snapshot_file_path)
+            if success and ack:
+                read_file_lines(fp=snapshot_file_path, ack=True)
+        else:
+            print(f'file {os.path.abspath(snapshot_file_path)} exists')
+
+    except (ImportError, ModuleNotFoundError, NameError, AttributeError) as err:
+        print(add_color('* tflite_runtime not Found. error: {}'.format(err), 'r'))
+
+    return
+
+
+def download_wizzi_utils_requirements_txt(ack: bool = False):
+    """
+    snapshot of a working environment
+    """
+    try:
+        from wizzi_utils.socket.socket_tools import download_file
+        req_file_path = './requirements.txt'
+        if not os.path.exists(req_file_path):
+            git_pref = 'https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi'
+            success = download_file(
+                url=f'{git_pref}/main/resources/requirements.txt',
+                dst_path=req_file_path)
+            if success and ack:
+                read_file_lines(fp=req_file_path, ack=True)
+        else:
+            print(f'file {os.path.abspath(req_file_path)} exists')
+
+    except (ImportError, ModuleNotFoundError, NameError, AttributeError) as err:
+        print(add_color('* tflite_runtime not Found. error: {}'.format(err), 'r'))
+
+    return
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/misc/test/test_misc_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/misc/test/test_misc_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1057,16 +1057,16 @@
 
     _, _, _, _ = mt.get_path_file_system_info(path='./fake_file.py', ack=True)
     return
 
 
 def get_repo_root_test():
     mt.get_function_name_and_line(ack=True, tabs=0)
-    mt.get_repo_root(repo_name='NO_REPO', ack=True)
-    mt.get_repo_root(repo_name='wizzi_utils_pypi', ack=True)
+    ret = mt.get_repo_root(repo_name='wizzi_utils_pypi', ack=True)  # will return 'N/A' outside wizzi utils repo
+    print('\t{}'.format(ret))
     return
 
 
 def rename_folder_test():
     mt.get_function_name_and_line(ack=True, tabs=0)
 
     _ = mt.rename_folder(dir_path='./NoSuchDir', new_name='NoSuchDir2')  # expected exception
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/base_models.py` & `wizzi_utils-8.0.3/wizzi_utils/models/base_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/object_detection.py` & `wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/pose_detection.py` & `wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/cv2_models/tracking.py` & `wizzi_utils-8.0.3/wizzi_utils/models/cv2_models/tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/labels_bank.py` & `wizzi_utils-8.0.3/wizzi_utils/models/labels_bank.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/models_configs.py` & `wizzi_utils-8.0.3/wizzi_utils/models/models_configs.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/shared_code_for_tests.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/shared_code_for_tests.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_od.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_pd.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_pd.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_cv2_tracking.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_cv2_tracking.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_models.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_models.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_tflite_od.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_tflite_od.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/test/test_tflite_pd.py` & `wizzi_utils-8.0.3/wizzi_utils/models/test/test_tflite_pd.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from wizzi_utils.models.test.shared_code_for_tests import od_or_pd_Model_video_test
 from wizzi_utils.models.test.shared_code_for_tests import od_or_pd_Model_cam_test
 
 
 def __get_pd_dict(op: int = 1):
     if op == 1:
         pd_solo = {
-            'model_names': ['pose_landmark_lite'],
+            # 'model_names': ['pose_landmark_lite'],
             # 'model_names': ['pose_landmark_full'],
             # 'model_names': ['pose_landmark_heavy'],
-            # 'model_names': ['posenet'],
+            'model_names': ['posenet'],
             'dis_size': (640, 480),
             'grid': (1, 1),
         }
         pd_meta_dict = pd_solo
     elif op == 2:
         pd_dual = {
             'model_names': [
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/object_detection.py` & `wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/object_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/models/tflite_models/pose_detection.py` & `wizzi_utils-8.0.3/wizzi_utils/models/tflite_models/pose_detection.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/open_cv/open_cv_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/open_cv/open_cv_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,24 +683,24 @@
 def get_frames_from_cap_cv2(cap: cv2.VideoCapture) -> int:
     """
     :param cap:
     :return:
     """
     video_total_frames = None
     if cap.isOpened():
-        video_total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT)) - 1
+        video_total_frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     return video_total_frames
 
 
 def get_frames_from_cap_imutils(cap) -> int:
     """
     :param cap:
     :return:
     """
-    video_total_frames = int(cap.stream.get(cv2.CAP_PROP_FRAME_COUNT)) - 1
+    video_total_frames = int(cap.stream.get(cv2.CAP_PROP_FRAME_COUNT))
     return video_total_frames
 
 
 def get_fps_from_cap_cv2(cap: cv2.VideoCapture) -> float:
     fps = None
     if cap.isOpened():
         fps = cap.get(cv2.CAP_PROP_FPS)
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/open_cv/test/test_open_cv_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/open_cv/test/test_open_cv_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from wizzi_utils.socket import socket_tools as st
 from wizzi_utils.pyplot import pyplot_tools as pyplt
 import numpy as np
 import os
 from collections import OrderedDict
 # noinspection PyPackageRequirements
 import cv2
+import ssl
+
+# noinspection PyProtectedMember
+ssl._create_default_https_context = ssl._create_unverified_context
 
 LOOP_TESTS = 50
 BLOCK_MS_NORMAL = 2000  # 0 to block
 ITERS_CAM_TEST = 10  # 0 to block
 
 
 def load_img_from_web(name: str, ack: bool = True) -> np.array:
@@ -578,20 +582,20 @@
     return
 
 
 def video_creator_size_test():
     wu.get_function_name(ack=True, tabs=0)
 
     # NOTICE MKV FIX ON WINDOWS on python 3.8
-    # download the file below to any dir. let DIR be its path
+    # download the file below to any dir. let DIR be its path. set env var MKV_DLL_DIR=DIR
     # https://github.com/2easy4wizzi/wizzi_utils_pypi/raw/main/resources/openh264-1.8.0-win64.dll
-    # uncomment the following:
-    # if wu.is_windows():
-    #     adding this folder - contains dll for h264 for python 3.8
-    #     wu.add_resource_folder_to_path(resources_dir=DIR)
+    MKV_DLL_DIR = wu.get_env_variable(key='MKV_DLL_DIR')
+    if MKV_DLL_DIR is not None and os.path.isdir(MKV_DLL_DIR) and wu.is_windows():
+        # adding this folder - contains dll for h264 for python 3.8
+        wu.add_resource_folder_to_path(resources_dir=MKV_DLL_DIR)
 
     # now open video file
     vid_name = mtt.DOG1
     video_path = get_vid_from_web(name=vid_name)
 
     if not os.path.exists(video_path):
         wu.exception_error(wu.NOT_FOUND.format(video_path), real_exception=False)
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/pyplot/pyplot_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/pyplot/pyplot_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/pyplot/test/test_pyplot_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/pyplot/test/test_pyplot_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/socket/socket_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/socket/socket_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,16 +547,15 @@
     """
     based on https://cloud.google.com/bigquery/docs/reference/libraries#client-libraries-install-python
     bigQ test online: https://console.cloud.google.com/bigquery
     bigQ generate new key: https://console.cloud.google.com/projectselector2/iam-admin/serviceaccounts
         service and project name > keys > add key > download
     bigQ table keys https://packaging.python.org/en/latest/guides/analyzing-pypi-package-downloads/
     dependencies
-    # pip install google # maybe
-    # pip install --upgrade google-cloud-speech # maybe
+    pip install google
     pip install pandas
     pip install google-cloud-bigquery
     pip install db-dtypes (on administrative mode)
 
     important: assumes you have credentials file on env variable GOOGLE_APPLICATION_CREDENTIALS
     see big_query_package_by_month_test() to see how do insert dynamically
     """
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/socket/test/test_socket_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/socket/test/test_socket_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,26 +302,23 @@
     18   6436  2021-04-01
     19   1748  2021-03-01
     20    231  2021-02-01
     time for all: 0:03:32
     """
 
     mt.get_function_name(ack=True, tabs=0)
-
-    cred_file = '{}/secret_keys/credentialsBigQ.json'.format(mt.get_repo_root(repo_name='wizzi_utils'))
-    if not os.path.exists(cred_file):
-        mt.exception_error(e='credentials file not found {}'.format(os.path.abspath(cred_file)))
+    # don't forget to set GOOGLE_APPLICATION_CREDENTIALS to your big query cred_file
+    # see instruction how to generate on st.runQ() function documentation
+    cred_file = mt.get_env_variable(key='GOOGLE_APPLICATION_CREDENTIALS')
+    if cred_file is None or not os.path.isfile(cred_file):
+        err = 'GOOGLE_APPLICATION_CREDENTIALS env variable not found or file not exists'
+        mt.exception_error(e=err)
         return
 
-    mt.set_env_variable(
-        key='GOOGLE_APPLICATION_CREDENTIALS',
-        val=cred_file,
-        ack=True
-    )
-    months_from_wu_release = 3
+    months_from_wu_release = 2
     # def diff_month(d1: datetime, d2: datetime) -> int:
     #     return (d1.year - d2.year) * 12 + d1.month - d2.month
     # WU_PUBLISH_DATE = datetime(year=2021, month=2, day=22)
     # months_from_wu_release = diff_month(datetime.today(), WU_PUBLISH_DATE) + 1  # +1: include this month
 
     st.big_query_package_by_month(
         package_name='wizzi-utils',  # package first release Feb 22, 2021
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/tflite/tflite_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/tflite/tflite_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/torch/test/test_torch_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/torch/test/test_torch_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from wizzi_utils.misc.test import test_misc_tools as mtt
 import numpy as np
 # noinspection PyPackageRequirements
 import torch
 # noinspection PyPackageRequirements
 import torch.nn as nn
 # noinspection PyPackageRequirements
-import torch.nn.functional as F
+import torch.nn.functional as func
 
 
 def cuda_on_test():
     mt.get_function_name(ack=True, tabs=0)
     print('\tcuda available ? {}'.format(tt.cuda_on()))
     return
 
@@ -321,139 +321,139 @@
 
 def get_torch_version_test():
     mt.get_function_name(ack=True, tabs=0)
     tt.get_torch_version(ack=True, tabs=1)
     return
 
 
-class Mnist_example(nn.Module):
+class MnistExample(nn.Module):
     # noinspection PyTypeChecker
     def __init__(self):
-        super(Mnist_example, self).__init__()
+        super(MnistExample, self).__init__()
         self.conv1 = nn.Conv2d(1, 32, 3, 1)
         self.conv2 = nn.Conv2d(32, 64, 3, 1)
         self.dropout1 = nn.Dropout(0.25)
         self.dropout2 = nn.Dropout(0.5)
         self.fc1 = nn.Linear(9216, 128)
         self.fc2 = nn.Linear(128, 10)
 
     def forward(self, x):
         x = self.conv1(x)
-        x = F.relu(x)
+        x = func.relu(x)
         x = self.conv2(x)
-        x = F.relu(x)
-        x = F.max_pool2d(x, 2)
+        x = func.relu(x)
+        x = func.max_pool2d(x, 2)
         x = self.dropout1(x)
         x = torch.flatten(x, 1)
         x = self.fc1(x)
-        x = F.relu(x)
+        x = func.relu(x)
         x = self.dropout2(x)
         x = self.fc2(x)
-        output = F.log_softmax(x, dim=1)
+        output = func.log_softmax(x, dim=1)
         return output
 
 
 def save_load_model_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     tt.layer_info(net1, layer='conv1', title='net1 conv1 values', wv=True, tabs=1)
     mt.create_dir(mtt.TEMP_FOLDER1)
     path = '{}/{}.pt'.format(mtt.TEMP_FOLDER1, mtt.JUST_A_NAME)
     tt.save_model(net1, path=path)
 
-    net2 = Mnist_example()
+    net2 = MnistExample()
     if tt.cuda_on():
         net2 = net2.cuda()
 
     tt.layer_info(net2, layer='conv1', title='net2 conv1 values', wv=True, tabs=1)
     tt.load_model(net2, path)
     tt.layer_info(net2, layer='conv1', title='net2 conv1 values(after load)', wv=True, tabs=1)
     mt.delete_dir_with_files(mtt.TEMP_FOLDER1, tabs=2)
     return
 
 
 def model_info_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     tt.model_info(net1, 'Mnist model', wv=True, tabs=1)
     return
 
 
 def layer_info_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     tt.layer_info(net1, layer='conv2', wv=True, tabs=1)
     return
 
 
 def model_summary_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example().float()  # if cuda_on(): model_summary need float variables
+    net1 = MnistExample().float()  # if cuda_on(): model_summary need float variables
     tt.model_summary(net1, input_size=(1, 28, 28), batch_size=256)
     return
 
 
 def model_params_count_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     print('\ttotal params {:,}'.format(tt.model_params_count(net1)))
     return
 
 
 def model_status_str_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     print('\tstatus = {}'.format(tt.model_status_str(net1)))
     return
 
 
 def set_model_status_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     print('\tstatus = {}'.format(tt.model_status_str(net1)))
     tt.set_model_status(net1, status=False)
     print('\tstatus = {}'.format(tt.model_status_str(net1)))
     tt.set_model_status(net1, status=True)
     print('\tstatus = {}'.format(tt.model_status_str(net1)))
     return
 
 
 def set_layer_status_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     tt.layer_info(net1, layer='conv2', title='net2')
     tt.set_layer_status(net1, layers=['conv2'], status=False)
     tt.model_info(net1, title='net2(post freezing conv2)')
     return
 
 
 def model_clone_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
+    net1 = MnistExample()
     print('\tnet1 address {}'.format(hex(id(net1))))
     net2 = tt.model_clone(net1)
     print('\tnet2 address {}'.format(hex(id(net2))))
     return
 
 
 def model_copy_layers_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
-    net2 = Mnist_example()
+    net1 = MnistExample()
+    net2 = MnistExample()
     tt.model_info(net1, title='net1', wv=True, tabs=1)
     tt.model_info(net2, title='net2', wv=True, tabs=1)
     tt.model_copy_layers(net1, net2, layers=['conv1'])
     tt.model_info(net2, title='net2(after copy conv1)', wv=True, tabs=1)
     return
 
 
 def model_copy_except_layers_test():
     mt.get_function_name(ack=True, tabs=0)
-    net1 = Mnist_example()
-    net2 = Mnist_example()
+    net1 = MnistExample()
+    net2 = MnistExample()
     tt.model_info(net1, title='net1', wv=True, tabs=1)
     tt.model_info(net2, title='net2', wv=True, tabs=1)
     tt.model_copy_except_layers(net1, net2, layers=['conv1'])
     tt.model_info(net2, title='net2(after copy all net1 except conv1)', wv=True, tabs=1)
     return
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils/torch/torch_tools.py` & `wizzi_utils-8.0.3/wizzi_utils/torch/torch_tools.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/tts/test/test_tts.py` & `wizzi_utils-8.0.3/wizzi_utils/tts/test/test_tts.py`

 * *Files identical despite different names*

### Comparing `wizzi_utils-8.0.2/wizzi_utils/tts/tts.py` & `wizzi_utils-8.0.3/wizzi_utils/tts/tts.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,16 @@
         def common_say_button_clicked(self):
             common_say = self.common_combo.currentText()
             if common_say:
                 print('common say {}'.format(common_say))
                 self.machine_buddy.say(text=common_say)
             return
 
-        def keyPressEvent(self, event: QtGui.QKeyEvent):
+        @staticmethod
+        def keyPressEvent(event: QtGui.QKeyEvent):
             if event.key() in [QtCore.Qt.Key_Escape]:
                 print('keyPressEvent(): Qt plot: Esc was clicked. Terminating...')
                 MachineBuddyGui.get_qt_app().quit()
 
         @staticmethod
         def get_qt_app() -> QtWidgets.QApplication:
             app = QtWidgets.QApplication.instance()  # main app must init before creating GLViewWidget
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils.egg-info/PKG-INFO` & `wizzi_utils-8.0.3/wizzi_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: wizzi-utils
-Version: 8.0.2
+Version: 8.0.3
 Summary: Debugging tools and fast coding
 Home-page: https://github.com/2easy4wizzi/wizzi_utils_pypi
-Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.2.tar.gz
 Author: Gilad Eini
 Author-email: giladEini@gmail.com
 License: MIT
+Download-URL: https://github.com/2easy4wizzi/wizzi_utils_pypi/archive/refs/tags/v_8.0.3.tar.gz
 Keywords: debugging tools,json,open cv,pyplot,socket,torch,tf lite
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Package wizzi utils:
+# Package [wizzi utils](https://github.com/2easy4wizzi/wizzi_utils_pypi/tree/main):
+
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/2easy4wizzi.jpeg)
 
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true)
-<!--- <img src="https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/2easy4wizzi.jpeg?raw=true" width="155" height="90" /> -->
 ## Brief
 
 * "wizzi_utils" main usage is for debugging and fast coding.
 * The package is cross-platform (most of the functions tested on Windows and linux).
 * The package is well documented and contain many easy access common functions.
     * In addition, almost every function is used in a test(more an example) I've written for learning purposes.
 * Package includes tools for json, open_cv, pyplot, socket, torch, text to speach and more.
@@ -42,15 +42,15 @@
 # The above import, will give access to all wizzi utils main module and the extra modules 
 # only if the packages are installed
 print(wu.to_str(var=2, title='my_int'))  # this will 100% work
 wu.test.to_str_test()  # for a wide example of to_str function
 print(wu.tt.to_str(var=3, title='my_int'))  # tt for torch tools. will work if torch installed
 wu.tt.test.to_str_test()  # for a wide example of tt.to_str function
 # If facing packages issues and want to know what packages I used, call the following
-wu.wizzi_utils_requirements()  # updated on 10/10/2022 
+wu.download_wizzi_utils_env_snapshot()  # updated on 10/10/2022 
 ```
 
 ### list of all the packages
 
 ```python
 import wizzi_utils as wu
 
@@ -98,16 +98,15 @@
         tf_v=True,
         cv2_v=True,
         with_pip_list=False,
         with_profiler=False
     )
 ```
 
-<!--- ![main wrapper img](resources/readme_images/main_wrapper.PNG) -->
-![main wrapper img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/main_wrapper.PNG?raw=true)
+![main wrapper img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/main_wrapper.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # fps measurements:
 fps = wu.FPS(last_k=3, cache_size=5, summary_title='classFPS_test')
 for t in range(10):
@@ -119,16 +118,15 @@
         wu.sleep(seconds=1)
     fps.update(ack_progress=ack)
     if t == 5:
         print('\tget_fps() = {:.4f}'.format(fps.get_fps()))
 fps.finalize()
 ```
 
-<!--- ![fps img](resources/readme_images/fps.PNG) -->
-![fps img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/fps.PNG?raw=true)
+![fps img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/fps.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * cv2 show image with extra control:
 * concatenation of several images(e.g. 2 cameras frames)
@@ -153,16 +151,15 @@
     resize=1.5,  # 150%
     grid=(3, 1),  # 3 rows 1 col
     header='cool, no?',
     separator_c='aqua',
 )
 ```
 
-<!--- ![display images img](resources/readme_images/display_images.PNG) -->
-![display images img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/display_images.PNG?raw=true)
+![display images img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/display_images.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 """
 * object detection models
 * pose detection models
@@ -172,21 +169,22 @@
 wu.models.test.test_cv2_pose_detection_models()
 wu.models.test.test_cv2_tracking_models()
 ```
 
 <!--- ![object detection img](resources/readme_images/yolov4.PNG) -->
 <!--- ![pose estimation img](resources/readme_images/pose.PNG) -->
 <!--- ![tracking img](resources/readme_images/tracking.PNG) -->
-![object detection img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/yolov4.PNG?raw=true)
-![pose estimation img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/pose.PNG?raw=true)
-![tracking img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tracking.PNG?raw=true)
+![object detection img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/yolov4.PNG?raw=true)
+![pose estimation img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/pose.PNG?raw=true)
+![tracking img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tracking.PNG?raw=true)
 
 ```python
 import wizzi_utils as wu
 
 # text to speak gui over pyttsx3 and pyQt5 packages
 wu.tts.test.run_machine_buddy_gui_test()
 ```
 
-<!--- ![tts img](resources/readme_images/tts.PNG) -->
-![tts img](https://github.com/2easy4wizzi/2easy4wizzi.github.io/blob/master/images_wu/tts.PNG?raw=true)
+![tts img](https://raw.githubusercontent.com/2easy4wizzi/wizzi_utils_pypi/main/resources/readme_images/tts.PNG?raw=true)
+
+
```

### Comparing `wizzi_utils-8.0.2/wizzi_utils.egg-info/SOURCES.txt` & `wizzi_utils-8.0.3/wizzi_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 wizzi_utils/__init__.py
-wizzi_utils/wizzi_utils_requirements.txt
 wizzi_utils.egg-info/PKG-INFO
 wizzi_utils.egg-info/SOURCES.txt
 wizzi_utils.egg-info/dependency_links.txt
 wizzi_utils.egg-info/requires.txt
 wizzi_utils.egg-info/top_level.txt
 wizzi_utils/google/__init__.py
 wizzi_utils/google/google_tools.py
@@ -60,14 +59,18 @@
 wizzi_utils/torch/torch_tools.py
 wizzi_utils/torch/test/__init__.py
 wizzi_utils/torch/test/test_torch_tools.py
 wizzi_utils/tts/__init__.py
 wizzi_utils/tts/tts.py
 wizzi_utils/tts/test/__init__.py
 wizzi_utils/tts/test/test_tts.py
+wizzi_utils/google/__init__.py
+wizzi_utils/google/google_tools.py
+wizzi_utils/google/test/__init__.py
+wizzi_utils/google/test/test_google_tools.py
 wizzi_utils/json/__init__.py
 wizzi_utils/json/json_tools.py
 wizzi_utils/json/test/__init__.py
 wizzi_utils/json/test/test_json_tools.py
 wizzi_utils/misc/__init__.py
 wizzi_utils/misc/misc_tools.py
 wizzi_utils/misc/test/__init__.py
```

