# Comparing `tmp/malclient-upgraded-1.4a1.tar.gz` & `tmp/malclient-upgraded-1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malclient-upgraded-1.4a1.tar", last modified: Thu May 25 23:50:41 2023, max compression
+gzip compressed data, was "malclient-upgraded-1.4a2.tar", last modified: Fri May 26 01:30:33 2023, max compression
```

## Comparing `malclient-upgraded-1.4a1.tar` & `malclient-upgraded-1.4a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.894634 malclient-upgraded-1.4a1/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1087 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a1/LICENSE
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4655 2023-05-25 23:50:41.894634 malclient-upgraded-1.4a1/PKG-INFO
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4165 2023-05-25 23:49:17.000000 malclient-upgraded-1.4a1/README.md
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.861095 malclient-upgraded-1.4a1/malclient/
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.884628 malclient-upgraded-1.4a1/malclient/Datamodels/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      105 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/Datamodels/__init__.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7420 2022-11-22 17:28:58.000000 malclient-upgraded-1.4a1/malclient/Datamodels/enums.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    15784 2023-05-25 23:44:42.000000 malclient-upgraded-1.4a1/malclient/Datamodels/fields.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    13014 2023-05-25 23:02:33.000000 malclient-upgraded-1.4a1/malclient/Datamodels/models.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1275 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/Datamodels/pagination.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       77 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/__init__.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     8757 2023-05-25 23:44:42.000000 malclient-upgraded-1.4a1/malclient/anime.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3336 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a1/malclient/boards.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7808 2023-05-25 22:05:50.000000 malclient-upgraded-1.4a1/malclient/client.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     2068 2023-01-22 22:26:02.000000 malclient-upgraded-1.4a1/malclient/exceptions.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3849 2022-11-22 20:46:54.000000 malclient-upgraded-1.4a1/malclient/manga.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    12218 2022-11-22 20:47:13.000000 malclient-upgraded-1.4a1/malclient/my_list.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3581 2023-01-22 22:26:40.000000 malclient-upgraded-1.4a1/malclient/request_handler.py
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-25 23:50:41.893636 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4655 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/PKG-INFO
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      594 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/SOURCES.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        1 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/dependency_links.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       18 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/requires.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       10 2023-05-25 23:50:41.000000 malclient-upgraded-1.4a1/malclient_upgraded.egg-info/top_level.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      148 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a1/pyproject.toml
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       79 2023-05-25 23:50:41.895674 malclient-upgraded-1.4a1/setup.cfg
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      889 2023-05-25 23:46:38.000000 malclient-upgraded-1.4a1/setup.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.058825 malclient-upgraded-1.4a2/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1087 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a2/LICENSE
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-26 01:30:33.058825 malclient-upgraded-1.4a2/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4233 2023-05-26 00:21:49.000000 malclient-upgraded-1.4a2/README.md
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.025213 malclient-upgraded-1.4a2/malclient/
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.048213 malclient-upgraded-1.4a2/malclient/Datamodels/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      105 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/Datamodels/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7420 2022-11-22 17:28:58.000000 malclient-upgraded-1.4a2/malclient/Datamodels/enums.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    15855 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/Datamodels/fields.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    13483 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/Datamodels/models.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1275 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/Datamodels/pagination.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       77 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     8789 2023-05-26 00:17:31.000000 malclient-upgraded-1.4a2/malclient/anime.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3336 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/boards.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7808 2023-05-25 22:05:50.000000 malclient-upgraded-1.4a2/malclient/client.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     2068 2023-01-22 22:26:02.000000 malclient-upgraded-1.4a2/malclient/exceptions.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3849 2022-11-22 20:46:54.000000 malclient-upgraded-1.4a2/malclient/manga.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    12218 2022-11-22 20:47:13.000000 malclient-upgraded-1.4a2/malclient/my_list.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     6527 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/request_handler.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.057826 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      594 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        1 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       18 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/requires.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       10 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/top_level.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      148 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a2/pyproject.toml
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       79 2023-05-26 01:30:33.059825 malclient-upgraded-1.4a2/setup.cfg
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      889 2023-05-26 01:30:16.000000 malclient-upgraded-1.4a2/setup.py
```

### Comparing `malclient-upgraded-1.4a1/LICENSE` & `malclient-upgraded-1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/PKG-INFO` & `malclient-upgraded-1.4a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.4a1
+Version: 1.4a2
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
@@ -108,14 +108,16 @@
 print(repr(anime))
 
 # Update anime List based off of search results
 anime = client.search_anime("Monogatari", limit=1)
 ```
 
 ### Most Imoprtant To-Do's
+- [ ] Implement people endpoint
+- [ ] Implement episodes endpoint
 - [ ] Implement additional search endpoint
 
 ### Useful resources
 - [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
 - [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
 - [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
```

### Comparing `malclient-upgraded-1.4a1/README.md` & `malclient-upgraded-1.4a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 print(repr(anime))
 
 # Update anime List based off of search results
 anime = client.search_anime("Monogatari", limit=1)
 ```
 
 ### Most Imoprtant To-Do's
+- [ ] Implement people endpoint
+- [ ] Implement episodes endpoint
 - [ ] Implement additional search endpoint
 
 ### Useful resources
 - [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
 - [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
 - [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
```

### Comparing `malclient-upgraded-1.4a1/malclient/Datamodels/enums.py` & `malclient-upgraded-1.4a2/malclient/Datamodels/enums.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/Datamodels/fields.py` & `malclient-upgraded-1.4a2/malclient/Datamodels/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,14 +354,15 @@
         self.first_name: bool = kwargs.get("first_name", False)
         self.last_name: bool = kwargs.get("last_name", False)
         self.alternative_name: bool = kwargs.get("alternative_name", False)
         self.main_picture: bool = kwargs.get("main_picture", False)
         self.biography: bool = kwargs.get("biography", False)
         self.pictures: bool = kwargs.get("pictures", False)
         self._animeography: Fields = self._generate_subclass(Fields, kwargs.get("animeography", False))
+        self.num_favorites: bool = kwargs.get("num_favorites", False)
 
     @property
     def animeography(self) -> Fields:
         return self._animeography
 
     @animeography.setter
     def animeography(self, value: Fields):
```

### Comparing `malclient-upgraded-1.4a1/malclient/Datamodels/models.py` & `malclient-upgraded-1.4a2/malclient/Datamodels/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -477,17 +477,30 @@
 
 
 class ForumCategory(MALBaseModel):
     title: str
     boards: list[ForumBoard]
 
 
+# This is added to avoid further expanding of AnimeObject
+class Animeography(AnimeObject):
+    """
+    Object represents animeography of character.
+    It might be populated same way as AnimeObject, depending on fields requested.
+    However it always contains role field, which represents role given to character in anime.
+
+    This object is only available in Character object.
+    """
+    role: Optional[str]
+
+
 class Character(MALBaseModel):
     id: int
-    role: str
+    role: Optional[str]
     first_name: Optional[str]
     last_name: Optional[str]
     alternative_name: Optional[list[str]]
-    main_picture: Optional[HttpUrl]
+    main_picture: Optional[Asset]
     biography: Optional[str]
-    pictures: Optional[list[HttpUrl]]
-    animeography: Optional[list[AnimeObject]]
+    pictures: Optional[list[Asset]]
+    animeography: Optional[list[Animeography]]
+    num_favorites: Optional[int]
```

### Comparing `malclient-upgraded-1.4a1/malclient/Datamodels/pagination.py` & `malclient-upgraded-1.4a2/malclient/Datamodels/pagination.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/anime.py` & `malclient-upgraded-1.4a2/malclient/anime.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,30 +157,30 @@
                   "fields": fields.to_payload(),
                   "nsfw": nsfw if nsfw is not None else self.nsfw}
 
         temp = self._api_handler.call(uri=uri, params=params)
         r_class = Node if fields == Fields.node() else AnimeObject
         return PagedResult([r_class(**anime) for anime in temp["data"]], temp['paging'])
 
-    def get_anime_characters(self, anime_id: int, *, fields: CharacterFields = CharacterFields, limit: int = 500, offset: int = 0) -> PagedResult[Character]:
+    def get_anime_characters(self, anime_id: int, *, fields: CharacterFields = CharacterFields.all(), limit: int = 500, offset: int = 0) -> PagedResult[Character]:
         """
         Gets list of characters from specified anime
 
         :param int anime_id: Id of anime to fetch characters from
         :param Fields fields: Fields returned alongside results
         :param int limit: number of queries returned
         :param int offset: Position from which search results will be presented
 
         :return: List of entries fetched from MyAnimeList with paging support
         :rtype: PagedResult[Character]
         """
         uri = f'anime/{anime_id}/characters'
         params = {"limit": limit,
                   "offset": offset,
-                  "fields": fields}
+                  "fields": fields.to_payload()}
 
         temp = self._api_handler.call(uri=uri, params=params)
         return PagedResult([Character(**character) for character in temp["data"]], temp['paging'])
 
     def get_character_details(self, character_id: int, *, fields: CharacterFields = CharacterFields.all()) -> Character:
         """
         Gets details of specified character
@@ -188,10 +188,10 @@
         :param int character_id: Id of character to fetch
         :param Fields fields: Fields returned alongside results
 
         :return: List of entries fetched from MyAnimeList with paging support
         :rtype: PagedResult[Character]
         """
         uri = f'characters/{character_id}'
-        params = {"fields": fields}
+        params = {"fields": fields.to_payload()}
 
         return Character(**self._api_handler.call(uri=uri, params=params))
```

### Comparing `malclient-upgraded-1.4a1/malclient/boards.py` & `malclient-upgraded-1.4a2/malclient/boards.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/client.py` & `malclient-upgraded-1.4a2/malclient/client.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/exceptions.py` & `malclient-upgraded-1.4a2/malclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/manga.py` & `malclient-upgraded-1.4a2/malclient/manga.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient/my_list.py` & `malclient-upgraded-1.4a2/malclient/my_list.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/malclient_upgraded.egg-info/PKG-INFO` & `malclient-upgraded-1.4a2/malclient_upgraded.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.4a1
+Version: 1.4a2
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
@@ -108,14 +108,16 @@
 print(repr(anime))
 
 # Update anime List based off of search results
 anime = client.search_anime("Monogatari", limit=1)
 ```
 
 ### Most Imoprtant To-Do's
+- [ ] Implement people endpoint
+- [ ] Implement episodes endpoint
 - [ ] Implement additional search endpoint
 
 ### Useful resources
 - [MAL auth guide](https://myanimelist.net/blog.php?eid=835707)
 - [Unofficial API Discord](https://discord.gg/XqzqDkzuFx)
 - [Official MAL API Club](https://myanimelist.net/clubs.php?cid=13727)
```

### Comparing `malclient-upgraded-1.4a1/malclient_upgraded.egg-info/SOURCES.txt` & `malclient-upgraded-1.4a2/malclient_upgraded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a1/setup.py` & `malclient-upgraded-1.4a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="malclient-upgraded",
-    version="1.4a1",
+    version="1.4a2",
     author="ModerNews",
     author_email="polski.gruzin.biz@gmail.com",
     description=
     "Modified and rewritten using modern models version of James Fotherby malclient",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ModerNews/MAL-API-Client-Upgraded",
```

