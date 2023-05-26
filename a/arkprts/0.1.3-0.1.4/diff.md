# Comparing `tmp/arkprts-0.1.3.tar.gz` & `tmp/arkprts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.3.tar", last modified: Sun May 21 17:13:42 2023, max compression
+gzip compressed data, was "arkprts-0.1.4.tar", last modified: Fri May 26 14:45:21 2023, max compression
```

## Comparing `arkprts-0.1.3.tar` & `arkprts-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.396297 arkprts-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-05-21 17:13:42.393309 arkprts-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.235389 arkprts-0.1.3/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.3/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-05-19 18:21:49.000000 arkprts-0.1.3/arkprts/__main__.py
--rw-rw-rw-   0        0        0    12390 2023-05-19 19:14:56.000000 arkprts-0.1.3/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.3/arkprts/errors.py
--rw-rw-rw-   0        0        0     6605 2023-05-21 14:06:41.000000 arkprts-0.1.3/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.358318 arkprts-0.1.3/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.3/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.3/arkprts/models/base.py
--rw-rw-rw-   0        0        0    10890 2023-05-21 17:06:34.000000 arkprts-0.1.3/arkprts/models/data.py
--rw-rw-rw-   0        0        0     6953 2023-05-21 13:50:03.000000 arkprts-0.1.3/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.3/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.307348 arkprts-0.1.3/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 17:13:42.000000 arkprts-0.1.3/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 17:13:42.397296 arkprts-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-21 17:12:18.000000 arkprts-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:13:42.383303 arkprts-0.1.3/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.3/tests/test_config.py
--rw-rw-rw-   0        0        0      357 2023-05-19 18:47:11.000000 arkprts-0.1.3/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.628323 arkprts-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-05-26 14:45:21.616330 arkprts-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.482407 arkprts-0.1.4/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.4/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-05-26 13:50:36.000000 arkprts-0.1.4/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    12518 2023-05-26 14:00:15.000000 arkprts-0.1.4/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.4/arkprts/errors.py
+-rw-rw-rw-   0        0        0     6994 2023-05-26 14:35:04.000000 arkprts-0.1.4/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.591352 arkprts-0.1.4/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.4/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.4/arkprts/models/base.py
+-rw-rw-rw-   0        0        0    11504 2023-05-26 14:36:53.000000 arkprts-0.1.4/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     7120 2023-05-26 13:50:27.000000 arkprts-0.1.4/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.4/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.554367 arkprts-0.1.4/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:45:21.628323 arkprts-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-05-26 14:38:54.000000 arkprts-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.606339 arkprts-0.1.4/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.4/tests/test_config.py
+-rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.4/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.3/LICENSE` & `arkprts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.3/PKG-INFO` & `arkprts-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.3/README.md` & `arkprts-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.3/arkprts/__main__.py` & `arkprts-0.1.4/arkprts/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if user.level < 5:
             continue
 
         print(f"{user.nickname}#{user.nick_number} ({user.uid}) Lvl {user.level}")
         print(f"Resume: {user.resume}")
         print(
             f"Current stage: {user.main_stage_progress} | Characters: {user.char_cnt} | Furniture: {user.furn_cnt} | "
-            f"Secretary: {client.gamedata.get_operator(user.secretary).name}",
+            f"Secretary: {client.gamedata.character_table[user.secretary].name}",
         )
         print(f"Playing since: {user.register_ts.isoformat()}")
         print(f"Last Online: {user.last_online_time.isoformat()}")
 
         print("Support Operators: ", end="")
         for char in user.assist_char_list:
             if not char:
```

### Comparing `arkprts-0.1.3/arkprts/client.py` & `arkprts-0.1.4/arkprts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,32 @@
     proxy: str | None = None
 
     uid: str | None
     secret: str | None
 
     _seqnum: int
 
-    def __init__(self, *, pure: bool = False, **config: object) -> None:
+    def __init__(
+        self,
+        *,
+        config: Config | None = None,
+        gamedata: GameData | None = None,
+        pure: bool = False,
+    ) -> None:
         """Initialize the client.
 
         If `pure` is set to `True`, the client will not attempt to download game data.
         """
-        self.config = Config(**config)
+        self.config = config or Config()
+        self.gamedata = gamedata or GameData()
+        self.pure = pure
 
         self.uid = None
         self.secret = None
         self._seqnum = 1
-        self.pure = pure
-        self.gamedata = GameData()
 
     async def _request(
         self,
         method: str,
         url: str,
         *,
         headers: typing.Mapping[str, str] | None = None,
@@ -101,15 +107,15 @@
                 return data
 
     async def request(self, endpoint: str, *, method: str = "POST", **kwargs: typing.Any) -> typing.Any:
         """Make a request towards the game server."""
         if self.uid is None or self.secret is None:
             raise errors.NotLoggedInError("Not logged in.")
 
-        logger.debug("Sending request #%d to %s.", self._seqnum, endpoint)
+        logger.debug("[%s] Sending request #%d to %s.", self.uid, self._seqnum, endpoint)
         headers = {
             "secret": self.secret,
             "seqnum": str(self._seqnum),
             "uid": self.uid,
         }
         self._seqnum += 1  # tfw no x++
```

### Comparing `arkprts-0.1.3/arkprts/errors.py` & `arkprts-0.1.4/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.3/arkprts/gamedata.py` & `arkprts-0.1.4/arkprts/gamedata.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,36 +120,48 @@
 
         # sometimes the contents are identical, we still want to update the mtime
         self.commit_file.write_text(commit)
         os.utime(self.commit_file, (time.time(), time.time()))
 
         logger.info("Downloaded game data")
 
-    def _get_data(self, name: str, *, server: str | None = None) -> models.DDict:
+    def _get_data(self, filename: str, *, server: str | None = None) -> models.DDict:
         """Get a file."""
         server = server or self.server
 
-        if self._cache.get(server, {}).get(name):
-            return models.DDict(self._cache[server][name])
+        if self._cache.get(server, {}).get(filename):
+            return models.DDict(self._cache[server][filename])
 
-        path = self.directory / server / "gamedata" / f"{name}.json"
+        path = self.directory / server / "gamedata" / filename
         if not path.exists():
             raise FileNotFoundError("Static gamedata has not been loaded.")
 
         with path.open(encoding="utf-8") as file:
             data = json.load(file)
 
-        self._cache.setdefault(server, {})[name] = data
+        self._cache.setdefault(server, {})[filename] = data
 
         return models.DDict(data)
 
     def get_excel(self, name: str, *, server: str | None = None) -> models.DDict:
         """Get an excel table file."""
-        return self._get_data(f"excel/{name}", server=server)
+        return self._get_data(f"excel/{name}.json", server=server)
 
+    def __getitem__(self, name: str) -> models.DDict:
+        """Get an excel table file."""
+        return self.get_excel(name)
+
+    def __getattr__(self, name: str) -> models.DDict:
+        """Get an excel table file."""
+        try:
+            return self[name]
+        except KeyError as e:
+            raise AttributeError(name) from e
+
+    # helper stuff
     def get_operator(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get an operator."""
         data = self.get_excel("character_table", server=server)
         return data[id]
 
     def get_item(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get an item."""
```

### Comparing `arkprts-0.1.3/arkprts/models/base.py` & `arkprts-0.1.4/arkprts/models/base.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.3/arkprts/models/data.py` & `arkprts-0.1.4/arkprts/models/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,26 +40,26 @@
     """Amount of expedited completion permits."""
     hgg_shard: int = pydantic.Field(alias="hggShard")
     """Amount of yellow distinction certificates."""
     lgg_shard: int = pydantic.Field(alias="lggShard")
     """Amount of green commendation certificates.."""
     recruit_license: int = pydantic.Field(alias="recruitLicense")
     """Amount of recruitment permit."""
-    progress: int
+    progress: int = pydantic.Field(repr=False)
     """IDK."""
-    buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes")
-    """Remaining pulls until guaranteed 5 star operator."""
-    ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag")
+    buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes", repr=False)
+    """IDK. Ap refers to sanity."""
+    ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag", repr=False)
     """IDK. Ap refers to sanity."""
     uid: str
     """User ID."""
-    flags: typing.Mapping[str, bool]
+    flags: typing.Mapping[str, bool] = pydantic.Field(repr=False)
     """Completed stories."""
     ap: int
-    """Current sanity."""
+    """Current sanity. Actually not a true value."""
     max_ap: int = pydantic.Field(alias="maxAp")
     """Max sanity."""
     pay_diamond: int = pydantic.Field(alias="payDiamond")
     """Bough originium prime."""
     free_diamond: int = pydantic.Field(alias="freeDiamond")
     """Earned originium prime."""
     diamond_shard: int = pydantic.Field(alias="diamondShard")
@@ -68,21 +68,21 @@
     """Amount of LMD."""
     practice_ticket: int = pydantic.Field(alias="practiceTicket")
     """Amount of training permits."""
     last_refresh_ts: datetime.datetime = pydantic.Field(alias="lastRefreshTs")
     """IDK. When sanity was last incremented."""
     last_ap_add_time: datetime.datetime = pydantic.Field(alias="lastApAddTime")
     """IDK."""
-    main_stage_progress: str = pydantic.Field(alias="mainStageProgress")
+    main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
     """Current main story stage ID. None if completed."""
     register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
     """Account creation time."""
     server_name: str = pydantic.Field(alias="serverName")
     """Server name. Should always be Terra."""
-    avatar_id: str = pydantic.Field(alias="avatarId")
+    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
     """IDK. Always 0."""
     resume: str
     """Player display bio."""
     friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
     """How many friend slots are open."""
     secretary: str
     """ID of the secretary operator."""
@@ -119,14 +119,23 @@
     char_inst_id: int = pydantic.Field(alias="charInstId")
     """Operator index."""
     skill_index: int = pydantic.Field(alias="skillIndex")
     """Index of chosen skill."""
     current_equip: typing.Optional[str] = None
     """Currently equipped module ID."""
 
+    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
+    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
+        """Flatten Amiya to only keep her guard form."""
+        if values and values.get("tmpl"):
+            current = values["tmpl"][values["currentTmpl"]]
+            values.update(current)
+
+        return values
+
 
 class Squads(base.BaseModel):
     """Operator squad data."""
 
     squad_id: str = pydantic.Field(alias="squadId")
     """Squad ID."""
     name: str
@@ -138,16 +147,16 @@
 class Skill(base.BaseModel):
     """Operator skill data."""
 
     skill_id: str = pydantic.Field(alias="skillId")
     """Skill ID."""
     unlock: bool
     """Whether the skill is unlocked."""
-    state: bool
-    """IDK."""
+    state: bool = pydantic.Field(repr=False)
+    """IDK. Always false."""
     specialize_level: int = pydantic.Field(alias="specializeLevel")
     """Skill mastery level."""
     complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
     """IDK. Time left until skill upgrade is complete. Is -1 if not upgrading."""
 
     @pydantic.validator("complete_upgrade_time", pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _complete_upgrade_time(cls, v: int) -> typing.Optional[int]:
@@ -155,15 +164,15 @@
             return None
 
         return v
 
     @property
     def static(self) -> base.DDict:
         """Static data for this skill."""
-        return self.client.gamedata.get_skill(self.skill_id)
+        return self.client.gamedata.skill_table[self.skill_id]
 
 
 class Equip(base.BaseModel):
     """Operator module data."""
 
     hide: bool
     """Whether the module is hidden."""
@@ -206,19 +215,29 @@
     """Operator modules."""
     star_mark: bool = pydantic.Field(False, alias="starMark")
     """Whether the operator is marked as favorite."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this operator."""
-        return self.client.gamedata.get_operator(self.char_id)
+        return self.client.gamedata.character_table[self.char_id]
+
+    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
+    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
+        """Flatten Amiya to only keep her guard form."""
+        if values and values.get("tmpl"):
+            current = values["tmpl"][values["currentTmpl"]]
+            values.update(current)
+            values["skin"] = current["skinId"]  # why even?
+
+        return values
 
 
 class CharGroup(base.BaseModel):
-    """Operator group data."""
+    """Additional operator data."""
 
     favor_point: int = pydantic.Field(alias="favorPoint")
     """Operator trust."""
 
 
 class Troops(base.BaseModel):
     """Operator data."""
@@ -229,29 +248,19 @@
     """Amount of squads. Should be always 4."""
     squads: typing.Mapping[int, Squads]
     """Squad data."""
     chars: typing.Mapping[int, Character]
     """Operator data."""
     char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
     """Additional operator data."""
-    char_mission: typing.Mapping[str, typing.Mapping[str, bool]] = pydantic.Field(alias="charMission")
-    """Special operation missions."""
-    addon: base.DDict = pydantic.Field(default_factory=base.DDict)
+    char_mission: typing.Mapping[str, typing.Mapping[str, int]] = pydantic.Field(alias="charMission", repr=False)
+    """IDK. Special operation missions."""
+    addon: base.DDict = pydantic.Field(default_factory=base.DDict, repr=False)
     """IDK."""
 
-    @pydantic.validator("chars", pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _fix_amiya(cls, value: typing.Any) -> typing.Any:
-        """Flatten amiya to only keep her guard form."""
-        for v in value.values():
-            if v and v.get("tmpl"):
-                current = v["tmpl"][v["currentTmpl"]]
-                v.update(current)
-
-        return value
-
 
 class Skins(base.BaseModel):
     """Operator skin data."""
 
     character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
     """Owned skins."""
     skin_ts: typing.Mapping[str, datetime.datetime] = pydantic.Field(alias="skinTs")
@@ -272,15 +281,15 @@
 class Social(base.BaseModel):
     """Social data."""
 
     assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
     """Support operators."""
     yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
     """IDK. Clue exchange data."""
-    y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs")
+    y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs", repr=False)
     """IDK."""
     medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
     """Medal board."""
 
 
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
```

### Comparing `arkprts-0.1.3/arkprts/models/social.py` & `arkprts-0.1.4/arkprts/models/social.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 class Skill(base.BaseModel):
     """Skill of a character."""
 
     skill_id: str = pydantic.Field(alias="skillId")
     """Skill ID."""
     unlock: bool
     """Whether the skill is unlocked."""
-    state: bool
-    """IDK. Skill state."""
+    state: bool = pydantic.Field(repr=False)
+    """IDK. Always false."""
     specialize_level: int = pydantic.Field(alias="specializeLevel")
     """Skill mastery level."""
     complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
     """IDK. Time left until skill upgrade is complete. Is -1 if not upgrading."""
 
     @pydantic.validator("complete_upgrade_time", pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _complete_upgrade_time(cls, v: int) -> typing.Optional[int]:
@@ -39,15 +39,15 @@
             return None
 
         return v
 
     @property
     def static(self) -> base.DDict:
         """Static data for this skill."""
-        return self.client.gamedata.get_skill(self.skill_id)
+        return self.client.gamedata.skill_table[self.skill_id]
 
 
 class UniEquip(base.BaseModel):
     """Equipped modules."""
 
     hide: bool
     """IDK. Whether the module is publicly hidden."""
@@ -74,39 +74,48 @@
     """Elite phase."""
     favor_point: int = pydantic.Field(alias="favorPoint")
     """Raw trust points (25570 is 200% Trust)"""
     potential_rank: int = pydantic.Field(alias="potentialRank")
     """Operator potential. Starts at 0."""
     level: int
     """Operator level."""
-    crisis_record: base.DDict = pydantic.Field(alias="crisisRecord")
+    crisis_record: base.DDict = pydantic.Field(alias="crisisRecord", repr=False)
     """IDK. selectedCrisis is used for contingency contracts elsewhere."""
     current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
     """ID of the currently equipped module."""
     equip: typing.Mapping[str, UniEquip]
     """Equipped modules. Module ID to module info."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this operator."""
-        return self.client.gamedata.get_operator(self.char_id)
+        return self.client.gamedata.character_table[self.char_id]
+
+    @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
+    def _fix_amiya(cls, values: typing.Any) -> typing.Any:
+        """Flatten Amiya to only keep her guard form."""
+        if values and values.get("tmpl"):
+            current = values["tmpl"][values["currentTmpl"]]
+            values.update(current)
+
+        return values
 
 
 class PlacedMedal(base.BaseModel):
     """A single medal on a board."""
 
     id: str
     """Medal ID."""
     pos: typing.Tuple[int, int]
     """Medal position on the board."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this medal."""
-        return self.client.gamedata.get_medal(self.id)
+        return self.client.gamedata.medal_table.medal_list[self.id]
 
 
 class MedalBoardCustom(base.BaseModel):
     """Custom medal board layout."""
 
     layout: typing.Sequence[PlacedMedal]
     """Medals on the board."""
@@ -119,15 +128,16 @@
     """Medal board template ID."""
     medal_list: typing.Sequence[str] = pydantic.Field(alias="medalList")
     """Medal IDs on the board."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this medal board."""
-        return self.client.gamedata.get_medal_group(self.group_id)
+        groups = self.client.gamedata.medal_table.medal_type_data.activity_medal.group_data
+        return next(i for i in groups if i.group_id == self.group_id)
 
 
 class MedalBoard(base.BaseModel):
     """Medal board info."""
 
     type: typing.Literal["CUSTOM", "TEMPLATE", "EMPTY"]
     """Medal board layout type."""
@@ -148,34 +158,25 @@
     """Player UID."""
     friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
     """How many friend slots are open."""
     server_name: str = pydantic.Field(alias="serverName")
     """Server name. Should always be Terra."""
     level: int
     """Player level."""
-    avatar_id: str = pydantic.Field(alias="avatarId")
+    avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
     """IDK. Always 0."""
     avatar: typing.Optional[Avatar] = None
     """Selected avatar."""
     assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
     """Assist operator list."""
     last_online_time: datetime.datetime = pydantic.Field(alias="lastOnlineTime")
     """Last online time."""
     medal_board: MedalBoard = pydantic.Field(alias="medalBoard")
     """Medal board."""
 
-    @pydantic.validator("assist_char_list", pre=True, each_item=True)  # pyright: ignore[reportUnknownMemberType]
-    def _fix_amiya(cls, v: typing.Any) -> typing.Any:
-        """Flatten amiya to only keep her guard form."""
-        if v and v.get("tmpl"):
-            current = v["tmpl"][v["currentTmpl"]]
-            v.update(current)
-
-        return v
-
 
 class Player(PartialPlayer):
     """Player info."""
 
     register_ts: datetime.datetime = pydantic.Field(alias="registerTs")
     """Account creation time."""
     main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
@@ -189,14 +190,14 @@
     secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
     """ID of the secretary operator's skin."""
     resume: str
     """Player display bio."""
     team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
     """Amount of characters owned in each faction."""
     board: typing.Sequence[str]
-    """IDK. Factions with full trust. Shows up blue in-game."""
+    """Factions with full trust. Shows up blue in-game."""
     info_share: datetime.datetime = pydantic.Field(alias="infoShare")
     """IDK."""
     recent_visited: bool = pydantic.Field(alias="recentVisited")
     """IDK."""
     info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
     """IDK."""
```

### Comparing `arkprts-0.1.3/arkprts.egg-info/PKG-INFO` & `arkprts-0.1.4/arkprts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.3/pyproject.toml` & `arkprts-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.3/setup.py` & `arkprts-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.3",
+    version="0.1.4",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

