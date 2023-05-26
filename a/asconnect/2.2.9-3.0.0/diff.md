# Comparing `tmp/asconnect-2.2.9.tar.gz` & `tmp/asconnect-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asconnect-2.2.9.tar", max compression
+gzip compressed data, was "asconnect-3.0.0.tar", max compression
```

## Comparing `asconnect-2.2.9.tar` & `asconnect-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0     1141 2020-09-30 13:33:16.848652 asconnect-2.2.9/LICENSE
--rw-r--r--   0        0        0     4502 2021-07-08 12:23:19.634821 asconnect-2.2.9/README.md
--rwxr-xr-x   0        0        0      297 2020-10-16 13:31:57.508255 asconnect-2.2.9/asconnect/__init__.py
--rw-r--r--   0        0        0     3165 2022-01-25 09:30:52.395345 asconnect-2.2.9/asconnect/altool.py
--rwxr-xr-x   0        0        0     3406 2021-07-08 12:24:00.974744 asconnect-2.2.9/asconnect/app_client.py
--rwxr-xr-x   0        0        0     5930 2021-07-08 12:23:27.324782 asconnect-2.2.9/asconnect/app_info_client.py
--rwxr-xr-x   0        0        0    10487 2021-07-08 12:23:27.323700 asconnect-2.2.9/asconnect/beta_review_client.py
--rwxr-xr-x   0        0        0     6296 2022-01-25 09:30:52.436718 asconnect-2.2.9/asconnect/build_client.py
--rwxr-xr-x   0        0        0     2301 2021-11-23 15:48:57.548392 asconnect-2.2.9/asconnect/client.py
--rw-r--r--   0        0        0     1301 2021-09-15 10:35:15.311279 asconnect-2.2.9/asconnect/exceptions.py
--rwxr-xr-x   0        0        0    12681 2021-11-25 15:58:40.305681 asconnect-2.2.9/asconnect/httpclient.py
--rw-r--r--   0        0        0      537 2021-10-05 12:17:03.862444 asconnect-2.2.9/asconnect/models/__init__.py
--rw-r--r--   0        0        0     2166 2021-07-08 12:38:54.734204 asconnect-2.2.9/asconnect/models/app_info.py
--rw-r--r--   0        0        0     4313 2021-07-08 12:39:08.683657 asconnect-2.2.9/asconnect/models/app_store.py
--rw-r--r--   0        0        0      903 2021-07-08 12:39:02.519876 asconnect-2.2.9/asconnect/models/app_store_version_localizations.py
--rw-r--r--   0        0        0     2721 2021-07-08 12:39:33.172840 asconnect-2.2.9/asconnect/models/apps.py
--rw-r--r--   0        0        0     1178 2021-07-08 12:39:40.941398 asconnect-2.2.9/asconnect/models/beta_app_review.py
--rw-r--r--   0        0        0     1866 2021-07-08 12:39:48.437450 asconnect-2.2.9/asconnect/models/beta_detail.py
--rw-r--r--   0        0        0     1277 2021-07-08 12:39:56.175568 asconnect-2.2.9/asconnect/models/beta_groups.py
--rw-r--r--   0        0        0     1225 2021-07-08 12:40:04.219871 asconnect-2.2.9/asconnect/models/builds.py
--rw-r--r--   0        0        0     1221 2021-07-08 12:38:40.406073 asconnect-2.2.9/asconnect/models/common.py
--rw-r--r--   0        0        0      978 2021-07-08 12:40:20.452423 asconnect-2.2.9/asconnect/models/idfa.py
--rw-r--r--   0        0        0     1373 2021-07-08 12:40:27.075321 asconnect-2.2.9/asconnect/models/localization.py
--rw-r--r--   0        0        0     4280 2021-07-08 12:40:45.165084 asconnect-2.2.9/asconnect/models/screenshots.py
--rw-r--r--   0        0        0     1364 2021-10-19 11:02:07.515543 asconnect-2.2.9/asconnect/models/users.py
--rwxr-xr-x   0        0        0     9963 2021-09-15 10:35:37.326234 asconnect-2.2.9/asconnect/screenshot_client.py
--rw-r--r--   0        0        0      352 2021-07-08 12:20:48.317779 asconnect-2.2.9/asconnect/sorting.py
--rwxr-xr-x   0        0        0     1216 2021-10-19 11:02:40.906719 asconnect-2.2.9/asconnect/users_client.py
--rw-r--r--   0        0        0     2170 2020-10-16 13:25:57.722356 asconnect-2.2.9/asconnect/utilities.py
--rwxr-xr-x   0        0        0    15965 2022-02-28 09:26:20.342765 asconnect-2.2.9/asconnect/version_client.py
--rw-r--r--   0        0        0     1125 2022-02-28 09:26:31.683491 asconnect-2.2.9/pyproject.toml
--rw-r--r--   0        0        0     5427 2022-02-28 09:26:55.356837 asconnect-2.2.9/setup.py
--rw-r--r--   0        0        0     5663 2022-02-28 09:26:55.357365 asconnect-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-05-26 09:25:30.302768 asconnect-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4502 2023-05-26 09:25:30.306768 asconnect-3.0.0/README.md
+-rwxr-xr-x   0        0        0      297 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/altool.py
+-rwxr-xr-x   0        0        0     3406 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/app_client.py
+-rwxr-xr-x   0        0        0     5930 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/app_info_client.py
+-rwxr-xr-x   0        0        0    10487 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/beta_review_client.py
+-rwxr-xr-x   0        0        0     6296 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/build_client.py
+-rwxr-xr-x   0        0        0     2301 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/client.py
+-rw-r--r--   0        0        0     1301 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/exceptions.py
+-rwxr-xr-x   0        0        0    12747 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/httpclient.py
+-rw-r--r--   0        0        0      537 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/__init__.py
+-rw-r--r--   0        0        0     2166 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_info.py
+-rw-r--r--   0        0        0     4313 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_store.py
+-rw-r--r--   0        0        0      933 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_store_version_localizations.py
+-rw-r--r--   0        0        0     2721 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/apps.py
+-rw-r--r--   0        0        0     1178 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_app_review.py
+-rw-r--r--   0        0        0     1866 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_detail.py
+-rw-r--r--   0        0        0     1277 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_groups.py
+-rw-r--r--   0        0        0     1225 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/builds.py
+-rw-r--r--   0        0        0     1221 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/common.py
+-rw-r--r--   0        0        0      978 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/idfa.py
+-rw-r--r--   0        0        0     1373 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/localization.py
+-rw-r--r--   0        0        0     4440 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/screenshots.py
+-rw-r--r--   0        0        0     1364 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/users.py
+-rwxr-xr-x   0        0        0     9963 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/screenshot_client.py
+-rw-r--r--   0        0        0      352 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/sorting.py
+-rwxr-xr-x   0        0        0     1216 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/users_client.py
+-rw-r--r--   0        0        0     2219 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/utilities.py
+-rwxr-xr-x   0        0        0    16470 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/version_client.py
+-rw-r--r--   0        0        0     1342 2023-05-26 09:25:30.306768 asconnect-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 asconnect-3.0.0/PKG-INFO
```

### Comparing `asconnect-2.2.9/LICENSE` & `asconnect-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/README.md` & `asconnect-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/altool.py` & `asconnect-3.0.0/asconnect/altool.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/app_client.py` & `asconnect-3.0.0/asconnect/app_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/app_info_client.py` & `asconnect-3.0.0/asconnect/app_info_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/beta_review_client.py` & `asconnect-3.0.0/asconnect/beta_review_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/build_client.py` & `asconnect-3.0.0/asconnect/build_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/client.py` & `asconnect-3.0.0/asconnect/client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/exceptions.py` & `asconnect-3.0.0/asconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/httpclient.py` & `asconnect-3.0.0/asconnect/httpclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,18 @@
                 "iss": self.issuer_id,
                 "exp": int(expiration.timestamp()),
                 "aud": "appstoreconnect-v1",
             },
             self.key_contents,
             algorithm="ES256",
             headers={"kid": self.key_id, "typ": "JWT"},
-        ).decode("utf-8")
+        )
+
+        if not isinstance(token, str):
+            token = token.decode("utf-8")
 
         self.log.debug(f"Generating new token. Expiration: {expiration}")
         self._cached_token_info = (token, expiration)
 
         return token
 
     def generate_url(self, endpoint: str) -> str:
```

### Comparing `asconnect-2.2.9/asconnect/models/__init__.py` & `asconnect-3.0.0/asconnect/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/app_info.py` & `asconnect-3.0.0/asconnect/models/app_info.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/app_store.py` & `asconnect-3.0.0/asconnect/models/app_store.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/app_store_version_localizations.py` & `asconnect-3.0.0/asconnect/models/app_store_version_localizations.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     @deserialize.key("marketing_url", "marketingUrl")
     @deserialize.key("promotional_text", "promotionalText")
     @deserialize.key("support_url", "supportUrl")
     @deserialize.key("whats_new", "whatsNew")
     class Attributes(BaseAttributes):
         """Attributes."""
 
-        description: str
-        keywords: str
+        description: Optional[str]
+        keywords: Optional[str]
         locale: str
         marketing_url: Optional[str]
         promotional_text: Optional[str]
-        support_url: str
+        support_url: Optional[str]
         whats_new: Optional[str]
 
     identifier: str
     attributes: Attributes
     relationships: Optional[Dict[str, Relationship]]
     links: Links
```

### Comparing `asconnect-2.2.9/asconnect/models/apps.py` & `asconnect-3.0.0/asconnect/models/apps.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/beta_app_review.py` & `asconnect-3.0.0/asconnect/models/beta_app_review.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/beta_detail.py` & `asconnect-3.0.0/asconnect/models/beta_detail.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/beta_groups.py` & `asconnect-3.0.0/asconnect/models/beta_groups.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/builds.py` & `asconnect-3.0.0/asconnect/models/builds.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/common.py` & `asconnect-3.0.0/asconnect/models/common.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/idfa.py` & `asconnect-3.0.0/asconnect/models/idfa.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/localization.py` & `asconnect-3.0.0/asconnect/models/localization.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/models/screenshots.py` & `asconnect-3.0.0/asconnect/models/screenshots.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 
     APP_IPHONE_65 = "APP_IPHONE_65"
     APP_IPHONE_58 = "APP_IPHONE_58"
     APP_IPHONE_55 = "APP_IPHONE_55"
     APP_IPHONE_47 = "APP_IPHONE_47"
     APP_IPHONE_40 = "APP_IPHONE_40"
     APP_IPHONE_35 = "APP_IPHONE_35"
+    APP_IPAD_PRO_6GEN_129 = "APP_IPAD_PRO_6GEN_129"
     APP_IPAD_PRO_3GEN_129 = "APP_IPAD_PRO_3GEN_129"
+    APP_IPAD_PRO_2GEN_129 = "APP_IPAD_PRO_2GEN_129"
     APP_IPAD_PRO_3GEN_11 = "APP_IPAD_PRO_3GEN_11"
     APP_IPAD_PRO_129 = "APP_IPAD_PRO_129"
     APP_IPAD_105 = "APP_IPAD_105"
     APP_IPAD_97 = "APP_IPAD_97"
     APP_DESKTOP = "APP_DESKTOP"
+    APP_WATCH_SERIES_7 = "APP_WATCH_SERIES_7"
     APP_WATCH_SERIES_4 = "APP_WATCH_SERIES_4"
     APP_WATCH_SERIES_3 = "APP_WATCH_SERIES_3"
     APP_APPLE_TV = "APP_APPLE_TV"
     IMESSAGE_APP_IPHONE_65 = "IMESSAGE_APP_IPHONE_65"
     IMESSAGE_APP_IPHONE_58 = "IMESSAGE_APP_IPHONE_58"
     IMESSAGE_APP_IPHONE_55 = "IMESSAGE_APP_IPHONE_55"
     IMESSAGE_APP_IPHONE_47 = "IMESSAGE_APP_IPHONE_47"
@@ -131,15 +134,15 @@
     class Attributes(BaseAttributes):
         """Attributes."""
 
         asset_delivery_state: AppMediaAssetState
         asset_token: str
         asset_type: str
         file_name: str
-        file_size: int
+        file_size: Optional[int]
         image_asset: Optional[ImageAsset]
         source_file_checksum: Optional[str]
         uploaded: Optional[bool]
         upload_operations: Optional[List[UploadOperation]]
 
     identifier: str
     attributes: Attributes
```

### Comparing `asconnect-2.2.9/asconnect/models/users.py` & `asconnect-3.0.0/asconnect/models/users.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/screenshot_client.py` & `asconnect-3.0.0/asconnect/screenshot_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/users_client.py` & `asconnect-3.0.0/asconnect/users_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-2.2.9/asconnect/utilities.py` & `asconnect-3.0.0/asconnect/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Utilities for the library."""
 
 import hashlib
 import os
 from typing import Dict, Iterator, Optional, TypeVar
 import urllib.parse
 
-IteratorType = TypeVar("IteratorType")
-
+IteratorType = TypeVar("IteratorType")  # pylint: disable=invalid-name
 
 def next_or_none(iterator: Iterator[IteratorType]) -> Optional[IteratorType]:
     """Get the next value from an iterator, or return None when it is exhausted.
 
     :param iterator: The iterator to get the next value from
 
     :returns: The next value or None if exhausted
@@ -65,11 +64,11 @@
 
     folder_path = os.path.expanduser("~/.appstoreconnect/private_keys")
     os.makedirs(folder_path, exist_ok=True)
 
     key_file_name = f"AuthKey_{key_id}.p8"
     key_file_path = os.path.join(folder_path, key_file_name)
 
-    with open(key_file_path, "w") as key_file:
+    with open(key_file_path, "w", encoding="utf-8") as key_file:
         key_file.write(key_contents)
 
     return key_file_path
```

### Comparing `asconnect-2.2.9/asconnect/version_client.py` & `asconnect-3.0.0/asconnect/version_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Wrapper around the Apple App Store Connect APIs."""
 
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 import logging
+import time
 from typing import Iterator, List, Optional
 
 from asconnect.exceptions import AppStoreConnectError
 from asconnect.httpclient import HttpClient
 from asconnect.models import (
     AppStoreVersion,
     AppStoreVersionPhasedRelease,
     PhasedReleaseState,
     Platform,
     AppStoreVersionLocalization,
     AppStoreReviewDetails,
     IdfaDeclaration,
+    Build,
 )
 from asconnect.utilities import next_or_none, update_query_parameters
 
 
 class VersionClient:
     """Wrapper class around the ASC API."""
 
@@ -195,20 +197,33 @@
     def get_localizations(self, *, version_id: str) -> Iterator[AppStoreVersionLocalization]:
         """Get the version localizations for an app version.
 
         :param version_id: The version ID to get the localizations for
 
         :returns: An AppStoreVersion
         """
-        self.log.info("Getting localizations for version {version_id}...")
+        self.log.info(f"Getting localizations for version {version_id}...")
         url = self.http_client.generate_url(
             f"appStoreVersions/{version_id}/appStoreVersionLocalizations"
         )
         yield from self.http_client.get(url=url, data_type=List[AppStoreVersionLocalization])
 
+    def get_attached_build(self, *, version_id: str) -> Optional[Build]:
+        """Get the build that is attached to a specific App Store version.
+
+        :param version_id: The version ID to get the build for
+
+        :returns: A Build
+        """
+        self.log.info(f"Getting build for version {version_id}...")
+
+        url = self.http_client.generate_url(f"appStoreVersions/{version_id}/build")
+
+        return next_or_none(self.http_client.get(url=url, data_type=Build))
+
     def set_build(self, *, version_id: str, build_id: str) -> None:
         """Set the build for a version
 
         :param version_id: The ID of the version to set the build on
         :param build_id: The ID of the build to set
         """
 
@@ -448,8 +463,7 @@
                 data_type=None,
             )
         except AppStoreConnectError as ex:
             if attempt < max_attempts and ex.response.status_code >= 500 and ex.response.status_code < 600:
                 self.log.info("Submit failed due to server-side intermittent issue. Will sleep for 1 minute and try again.")
                 time.sleep(60)
                 self.submit_for_review(version_id=version_id)
-
```

### Comparing `asconnect-2.2.9/pyproject.toml` & `asconnect-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asconnect"
-version = "2.2.9"
+version = "3.0.0"
 description = "A wrapper around the Apple App Store Connect APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -18,33 +18,41 @@
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Environment :: MacOS X',
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-cryptography = "^3.0.0"
-deserialize = "^1.2.0"
-pyjwt = "^1.7.0"
-requests = "^2.20.0"
-tenacity = "^6.2.0"
-
-[tool.poetry.dev-dependencies]
-black = "=21.5b2"
-mypy = "=0.812"
-pylint = "=2.8.3"
-pytest = "=6.2.4"
-pytest-cov = "=2.12.1"
-pytest-dependency = "=0.5.1"
-
+python = "^3.8"
+cryptography = "^40.0.0"
+deserialize = "^2.0.1"
+pyjwt = "^2.6.0"
+requests = "^2.28.2"
+tenacity = "^8.2.2"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.1.0"
+mypy = "^1.1.1"
+pylint = "^2.17.1"
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+pytest-dependency = "^0.5.1"
+types-requests = "^2.28.11.16"
+
+[[tool.mypy.overrides]]
+module = [
+    "deserialize"
+]
+ignore_missing_imports = true
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `asconnect-2.2.9/setup.py` & `asconnect-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,139 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asconnect
+Version: 3.0.0
+Summary: A wrapper around the Apple App Store Connect APIs
+Home-page: https://github.com/microsoft/asconnect
+License: MIT
+Keywords: apple,app store,itunes,connect
+Author: Dale Myers
+Author-email: dalemy@microsoft.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: cryptography (>=40.0.0,<41.0.0)
+Requires-Dist: deserialize (>=2.0.1,<3.0.0)
+Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Project-URL: Repository, https://github.com/microsoft/asconnect
+Description-Content-Type: text/markdown
 
-packages = \
-['asconnect', 'asconnect.models']
+# asconnect
 
-package_data = \
-{'': ['*']}
+asconnect is a Python wrapper around the [Apple App Store Connect REST APIs](https://developer.apple.com/documentation/appstoreconnectapi).
 
-install_requires = \
-['cryptography>=3.0.0,<4.0.0',
- 'deserialize>=1.2.0,<2.0.0',
- 'pyjwt>=1.7.0,<2.0.0',
- 'requests>=2.20.0,<3.0.0',
- 'tenacity>=6.2.0,<7.0.0']
-
-setup_kwargs = {
-    'name': 'asconnect',
-    'version': '2.2.9',
-    'description': 'A wrapper around the Apple App Store Connect APIs',
-    'long_description': '# asconnect\n\nasconnect is a Python wrapper around the [Apple App Store Connect REST APIs](https://developer.apple.com/documentation/appstoreconnectapi).\n\nThis wrapper does not cover every API, but does cover the basics, including:\n\n* Uploading a build\n* Creating a new TestFlight version\n* Setting TestFlight review information\n* Creating a new app store version\n* Setting the app review information\n* Submitting for app review\n\n## Getting Started\n\n### Installation\n\nThe package is available on PyPI, so you can run `pip install asconnect` to get the latest version.\n\n### Creating a client\n\nTo begin, you need to [generate a key](https://developer.apple.com/documentation/appstoreconnectapi/creating_api_keys_for_app_store_connect_api), then get it\'s ID, the contents of the key itself, and the issuer ID.\n\nOnce you have those, you can create a new client by running:\n\n```python\nclient = asconnect.Client(key_id="...", key_contents="...", issuer_id="...")\n```\n\n### Getting your App\n\nMost operations require an app identifier. This is not the same as the bundle ID you choose, but is an ID generated by Apple. The easiest way to get this is to run this code:\n\n```python\napp = client.app.get_from_bundle_id("com.example.my_bundle_id")\n```\n\n### Uploading a Build\n\nUploading a build isn\'t technically part of the App Store Connect APIs, but a wrapper around altool is included to make things as easy as possible. Let\'s upload a build for your app:\n\n```python\nclient.build.upload(\n  ipa_path="/path/to/the/app.ipa",\n  platform=asconnect.Platform.ios,\n)\n```\n\nAnd if you want to wait for your build to finish processing:\n\n```python\nbuild = client.build.wait_for_build_to_process("com.example.my_bundle_id", build_number)\n```\n\n`build_number` is the build number you gave your build when you created it. It\'s used by the app store to identify the build.\n\n### App Store Submission\n\nLet\'s take that build, create a new app store version and submit it,\n\n```python\n# Create a new version\nversion = client.app.create_new_version(version="1.2.3", app_id=app.identifier)\n\n# Set the build for that version\nclient.version.set_build(version_id=version.identifier, build_id=build.identifier)\n\n# Submit for review\nclient.version.submit_for_review(version_id=version.identifier)\n```\n\nIt\'s that easy. Most of the time at least. If you don\'t have previous version to inherit information from you\'ll need to do things like set screenshots, reviewer info, etc. All of which is possible through this library.\n### Phased Distribution\n```python\n# Create a new version\nversion = client.app.create_new_version(version="1.2.3", app_id=app.identifier)\n\n# Start a versions\' phased release, the initial state of which is INACTIVE\nphased_release = client.version.create_phased_release(version_id=version.identifier)\n\n# Check on a phased release\nphased_release = client.version.get_phased_release(version_id=version.identifier)\n\n# Advance or modify a phased release\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.active)\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.pause)\nphased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.complete)\n\n# Delete\nclient.version.delete_phased_release(phased_release_id=phased_release.identifier)\n```\n# Getting Started\n\nFor development `asconnect` uses [`poetry`](https://github.com/python-poetry/poetry)\n\n# Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.\n\nWhen you submit a pull request, a CLA bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n',
-    'author': 'Dale Myers',
-    'author_email': 'dalemy@microsoft.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/microsoft/asconnect',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
+This wrapper does not cover every API, but does cover the basics, including:
 
+* Uploading a build
+* Creating a new TestFlight version
+* Setting TestFlight review information
+* Creating a new app store version
+* Setting the app review information
+* Submitting for app review
+
+## Getting Started
+
+### Installation
+
+The package is available on PyPI, so you can run `pip install asconnect` to get the latest version.
+
+### Creating a client
+
+To begin, you need to [generate a key](https://developer.apple.com/documentation/appstoreconnectapi/creating_api_keys_for_app_store_connect_api), then get it's ID, the contents of the key itself, and the issuer ID.
+
+Once you have those, you can create a new client by running:
+
+```python
+client = asconnect.Client(key_id="...", key_contents="...", issuer_id="...")
+```
+
+### Getting your App
+
+Most operations require an app identifier. This is not the same as the bundle ID you choose, but is an ID generated by Apple. The easiest way to get this is to run this code:
+
+```python
+app = client.app.get_from_bundle_id("com.example.my_bundle_id")
+```
+
+### Uploading a Build
+
+Uploading a build isn't technically part of the App Store Connect APIs, but a wrapper around altool is included to make things as easy as possible. Let's upload a build for your app:
+
+```python
+client.build.upload(
+  ipa_path="/path/to/the/app.ipa",
+  platform=asconnect.Platform.ios,
+)
+```
+
+And if you want to wait for your build to finish processing:
+
+```python
+build = client.build.wait_for_build_to_process("com.example.my_bundle_id", build_number)
+```
+
+`build_number` is the build number you gave your build when you created it. It's used by the app store to identify the build.
+
+### App Store Submission
+
+Let's take that build, create a new app store version and submit it,
+
+```python
+# Create a new version
+version = client.app.create_new_version(version="1.2.3", app_id=app.identifier)
+
+# Set the build for that version
+client.version.set_build(version_id=version.identifier, build_id=build.identifier)
+
+# Submit for review
+client.version.submit_for_review(version_id=version.identifier)
+```
+
+It's that easy. Most of the time at least. If you don't have previous version to inherit information from you'll need to do things like set screenshots, reviewer info, etc. All of which is possible through this library.
+### Phased Distribution
+```python
+# Create a new version
+version = client.app.create_new_version(version="1.2.3", app_id=app.identifier)
+
+# Start a versions' phased release, the initial state of which is INACTIVE
+phased_release = client.version.create_phased_release(version_id=version.identifier)
+
+# Check on a phased release
+phased_release = client.version.get_phased_release(version_id=version.identifier)
+
+# Advance or modify a phased release
+phased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.active)
+phased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.pause)
+phased_release = client.version.patch_phased_release(phased_release_id=phased_release.identifier, phased_release_state=PhasedReleaseState.complete)
+
+# Delete
+client.version.delete_phased_release(phased_release_id=phased_release.identifier)
+```
+# Getting Started
+
+For development `asconnect` uses [`poetry`](https://github.com/python-poetry/poetry)
+
+# Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
+
+When you submit a pull request, a CLA bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
-setup(**setup_kwargs)
```

