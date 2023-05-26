# Comparing `tmp/all-fives-domino-1.0.4.tar.gz` & `tmp/all-fives-domino-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all-fives-domino-1.0.4.tar", last modified: Thu May 25 21:11:03 2023, max compression
+gzip compressed data, was "all-fives-domino-1.0.5.tar", last modified: Fri May 26 21:15:55 2023, max compression
```

## Comparing `all-fives-domino-1.0.4.tar` & `all-fives-domino-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.141143 all-fives-domino-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-25 21:10:49.000000 all-fives-domino-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/all_fives_domino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-25 21:11:03.000000 all-fives-domino-1.0.4/all_fives_domino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 21:11:03.141143 all-fives-domino-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/main/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.133143 all-fives-domino-1.0.4/src/main/game/
--rw-r--r--   0 root         (0) root         (0)     1147 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/game/DominoRound.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/game/Piece.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/main/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-25 21:10:48.000000 all-fives-domino-1.0.4/src/main/game/__pycache__/Piece.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/main/game/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/main/player/
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Brain.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Hand.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-25 21:10:41.000000 all-fives-domino-1.0.4/src/main/player/Player.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/main/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/game/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:11:03.137143 all-fives-domino-1.0.4/src/test/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 20:34:42.000000 all-fives-domino-1.0.4/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 20:33:44.000000 all-fives-domino-1.0.4/src/test/game/test_pieces.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-25 21:10:50.000000 all-fives-domino-1.0.4/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-26 21:15:41.000000 all-fives-domino-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/all_fives_domino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-26 21:15:55.000000 all-fives-domino-1.0.5/all_fives_domino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/main/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/game/
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/game/DominoRound.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/game/Piece.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.917680 all-fives-domino-1.0.5/src/main/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4014 2023-05-26 21:15:41.000000 all-fives-domino-1.0.5/src/main/game/__pycache__/Piece.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/main/game/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/main/player/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.5/src/main/player/Brain.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/player/Hand.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-26 21:15:33.000000 all-fives-domino-1.0.5/src/main/player/Player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/main/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 21:15:55.921680 all-fives-domino-1.0.5/src/test/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 20:34:42.000000 all-fives-domino-1.0.5/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 20:33:44.000000 all-fives-domino-1.0.5/src/test/game/test_pieces.py
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-26 21:15:43.000000 all-fives-domino-1.0.5/version.txt
```

### Comparing `all-fives-domino-1.0.4/LICENSE` & `all-fives-domino-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.4/PKG-INFO` & `all-fives-domino-1.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.4
+Version: 1.0.5
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=1+failed%2C+1+tests&color=critical&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=32%25&color=orange&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=25%25&color=red&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.4/all_fives_domino.egg-info/PKG-INFO` & `all-fives-domino-1.0.5/all_fives_domino.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.4
+Version: 1.0.5
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=1+failed%2C+1+tests&color=critical&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=32%25&color=orange&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=25%25&color=red&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.4/all_fives_domino.egg-info/SOURCES.txt` & `all-fives-domino-1.0.5/all_fives_domino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.4/setup.py` & `all-fives-domino-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.4/src/main/game/DominoRound.py` & `all-fives-domino-1.0.5/src/main/game/DominoRound.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,89 @@
 from typing import Union, List, Tuple
 
-from src.main.game.Piece import domino_set
+from src.main.game.Piece import domino_set, Piece
 from src.main.player.Player import Player
 from src.main.player.Brain import Brain
 from src.main.player.Hand import Hand
 
 
 class DominoRound:
-    def __init__(self, player1: Player, player2: Player, begins: Union[Player, None]):
+    def __init__(self, brain1: Brain, brain2: Brain, begins: Union[Brain, None]):
         self.pool = domino_set()
-        self.source_piece: List[Tuple[int, int]] = []
-        self.player1 = player1
-        self.player2 = player2
-        self.current_player = begins
+        self.origin: Union[Piece, None] = None
+        self.player1 = Player(brain1, self)
+        self.player2 = Player(brain2, self)
+        self.current_player = self.player1 if begins == brain1 else (self.player2 if begins == brain2 else None)
+        self.has_crossing = False
 
     def deal_hand(self):
-        # Each player receives 7 pieces
+        # Each player receives 7 initial pieces
         for i in range(7):
             self.player1.draw()
             self.player2.draw()
 
-    def neutral_start(self):
+    def get_required_starting_piece(self):
         """
-        If no starting player is defined, the player with [5|5] begins.
+        Find the piece a player is required to start with.
 
+        If no starting player is defined, the player with [5|5] begins.
         If neither player has [5|5], the order goes [1|1], [2|2], ..., [6|6], [0|0].
         If neither player has any double pieces, they draw a piece each until one does.
         """
+        if self.current_player is not None:
+            return None
+
         while self.current_player is None:
-            pass
+            for i in [5, 1, 2, 3, 4, 6, 0]:
+                piece = Piece(i, i)
+
+                if piece in self.player1.hand:
+                    self.current_player = self.player1
+                    return piece
+                if piece in self.player2.hand:
+                    self.current_player = self.player1
+                    return piece
+
+    def score_piece(self, piece: Piece, depth=28):
+        piece_score = 0
+
+
+
+        return piece_score
+
+    def score(self):
+        score = self.score_piece(self.origin)
+        self.current_player.score += score
+
+    def play(self, player: Player, piece: Piece, origin: Union[Piece, None], close = False):
+        if piece not in player.hand:
+            raise Exception(f"Player attempted to play {piece}, but it's not in their hand")
+
+        if piece.is_double and self.has_crossing and close:
+            piece.closed = True
+
+        player.hand.pop(piece)
+
+        if origin is None:
+            if self.origin is not None:
+                raise Exception(f"Player attempted to play {piece} as origin, "
+                                f"but there is already origin piece {self.origin}")
+            self.origin = piece
+        else:
+            origin.append(piece)
+        self.score()
+
+        if self.current_player == self.player1:
+            self.current_player = self.player2
+        else:
+            self.current_player = self.player1
 
     def valid_options(self, hand):
         return []
 
-    def play(self):
+    def run(self):
+        starting_piece = self.get_required_starting_piece()
+        if starting_piece is not None:
+            self.play(self.current_player, starting_piece, None)
+
         while True:
-            self.current_player.play()
+            pass
```

### Comparing `all-fives-domino-1.0.4/src/main/game/Piece.py` & `all-fives-domino-1.0.5/src/main/game/Piece.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,52 @@
-from typing import List
+from typing import List, Union
 
 
 class Piece:
     def __init__(self, a: int, b: int):
         """
         Constructor
 
         a: int                  -> First number on the piece
         b: int                  -> Second number on the piece
 
         linked: List[Piece]     -> Pieces played from this Piece
         is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece
         is_double: Bool         -> Whether both sides of the piece show the same number
+        closed: Bool            -> If a double piece is closed (face down), nothing can be appended to it
         points: int             -> Point value of the piece, which is the combined value of both sides
         """
         self.sides = sorted([a, b])
         self.linked: List[Piece] = []
+        self.linked_to: Union[Piece, None] = None
         self.is_crossing = False
         self.is_double = self.sides[0] == self.sides[1]
+        self.closed = False
         self.points = sum(self.sides)
 
     def append(self, piece):
         self.linked.append(piece)
 
     def __repr__(self):
-        """Simple visual representation, e.g. [4|6]"""
-        return f"[{self.sides[0]}|{self.sides[1]}]"
+        """Simple visual representation using die face Unicode symbols"""
+        if self.closed:
+            closed = u"\u25A9"
+            return f"[{closed}|{closed}]"
+
+        sides = [
+            u"\u25A1",
+            u"\u2680",
+            u"\u2681",
+            u"\u2682",
+            u"\u2683",
+            u"\u2684",
+            u"\u2685"
+        ]
+
+        return f"[{sides[self.sides[0]]}|{sides[self.sides[1]]}]"
 
     def __hash__(self):
         """Integer representation, e.g. 64 for a [4|6] piece"""
         return self.sides[1] * 10 + self.sides[0]
 
     def __eq__(self, other):
         """Returns whether the pieces are equal based on their hash"""
@@ -46,8 +63,13 @@
 
 def domino_set():
     pieces = set()
     for i in range(7):
         for j in range(7):
             if i <= j:
                 pieces.add(Piece(i, j))
+
+    piece = Piece(7, 7)
+    piece.closed = True
+    pieces.add(piece)
+
     return sorted(pieces)
```

### Comparing `all-fives-domino-1.0.4/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.5/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

