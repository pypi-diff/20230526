# Comparing `tmp/pgx-0.7.4.tar.gz` & `tmp/pgx-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.7.4.tar", last modified: Mon May 15 21:08:32 2023, max compression
+gzip compressed data, was "pgx-0.8.0.tar", last modified: Fri May 26 04:16:33 2023, max compression
```

## Comparing `pgx-0.7.4.tar` & `pgx-0.8.0.tar`

### file list

```diff
@@ -1,144 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.931589 pgx-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 21:08:22.000000 pgx-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-15 21:08:32.931589 pgx-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-05-15 21:08:22.000000 pgx-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.911588 pgx-0.7.4/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.911588 pgx-0.7.4/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.911588 pgx-0.7.4/pgx/_mahjong/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_mahjong/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.911588 pgx-0.7.4/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.915588 pgx-0.7.4/pgx/_src/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/assets/between.npy
--rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/assets/can_move.npy
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.919588 pgx-0.7.4/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.919588 pgx-0.7.4/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.919588 pgx-0.7.4/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.923588 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37353 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.927589 pgx-0.7.4/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.927589 pgx-0.7.4/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-05-15 21:08:22.000000 pgx-0.7.4/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.911588 pgx-0.7.4/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-15 21:08:32.000000 pgx-0.7.4/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-15 21:08:32.000000 pgx-0.7.4/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:08:32.000000 pgx-0.7.4/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 21:08:32.000000 pgx-0.7.4/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 21:08:32.000000 pgx-0.7.4/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-15 21:08:22.000000 pgx-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:08:32.931589 pgx-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-15 21:08:22.000000 pgx-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:32.931589 pgx-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61927 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29776 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-15 21:08:22.000000 pgx-0.7.4/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.569276 pgx-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 04:16:21.000000 pgx-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-26 04:16:33.569276 pgx-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-05-26 04:16:21.000000 pgx-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.533276 pgx-0.8.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx/_mahjong/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.541276 pgx-0.8.0/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.545276 pgx-0.8.0/pgx/_src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/assets/between.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/assets/can_move.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.549276 pgx-0.8.0/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.549276 pgx-0.8.0/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.553276 pgx-0.8.0/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.557276 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/gardner_chess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38512 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.557276 pgx-0.8.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.561276 pgx-0.8.0/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-26 04:16:22.000000 pgx-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 04:16:33.569276 pgx-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-26 04:16:22.000000 pgx-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.565276 pgx-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74697 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34016 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.7.4/LICENSE` & `pgx-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/PKG-INFO` & `pgx-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.7.4
+Version: 0.8.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,21 +58,19 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not (state.terminated | state.terminated).all():
+while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
-
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
@@ -106,31 +104,32 @@
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
 |<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
-|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `beta` | *Animal-themed child-friendly shogi.* |
+|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
 |<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
-|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `beta` | *Checkmate opponent's king to win.* |
-|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `beta` | *Connect discs, win with four.* |
-|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `beta` | *Strategically place stones, claim territory.* |
-|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `beta` | *Connect opposite sides, block opponent.* |
+|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
+|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
+|<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
+|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
+|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
 |<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
 |<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
-|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `beta` | *Flip and conquer opponent's pieces.* |
-|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `beta` | *Japanese chess with captured pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
 |<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
-|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `beta` | *Three in a row wins.* |
+|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.7.4 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.8.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -27,64 +27,64 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.terminated).all():
+# vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
-â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in May 2023. Opinions and
-comments are more than welcome!  ## Supported games | Backgammon | Chess |
-Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
+## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
+| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
+/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
-friendly shogi.* | |Backgammon
+main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
+shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif]| `beta` | *Checkmate opponent's king to win.* |
-|Connect_Four
+assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
+Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/connect_four_light.gif]| `beta` | *Connect discs, win with
-four.* | |Go
+main/docs/assets/connect_four_light.gif]| `v0` | *Connect discs, win with
+four.* | |Gardner_Chess
+`"gardner_chess"`|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/gardner_chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
+main/docs/assets/gardner_chess_light.gif]| `v0` | *5x5 chess variant, excluding
+castling.* | |Go
 `"go_9x9"` `"go_19x19"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
 docs/assets/go-19x19_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/go-19x19_light.gif]| `beta` | *Strategically place stones,
-claim territory.* | |Hex
+main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
+territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-hex_light.gif]| `beta` | *Connect opposite sides, block opponent.* | |Kuhn
-Poker
+hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
 bluffing game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
@@ -102,27 +102,27 @@
 docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
 dodge bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/othello_light.gif]| `beta` | *Flip and conquer opponent's pieces.* |
+assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_light.gif] | `beta` | *Japanese chess with captured pieces.* |
+assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
 pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/tic_tac_toe_light.gif]| `beta` | *Three in a row wins.* | -
+main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
 (classic) board game suits: - [RobertTLange/gymnax](https://github.com/
 RobertTLange/gymnax): JAX implementation of popular RL environments ([classic
 control](https://gymnasium.farama.org/environments/classic_control), [bsuite]
 (https://github.com/deepmind/bsuite), MinAtar, etc) and meta RL tasks -
```

### Comparing `pgx-0.7.4/README.md` & `pgx-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,19 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not (state.terminated | state.terminated).all():
+while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
-
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
@@ -93,31 +91,32 @@
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
 |<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
-|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `beta` | *Animal-themed child-friendly shogi.* |
+|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
 |<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
-|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `beta` | *Checkmate opponent's king to win.* |
-|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `beta` | *Connect discs, win with four.* |
-|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `beta` | *Strategically place stones, claim territory.* |
-|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `beta` | *Connect opposite sides, block opponent.* |
+|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
+|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
+|<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
+|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
+|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
 |<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
 |<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
-|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `beta` | *Flip and conquer opponent's pieces.* |
-|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `beta` | *Japanese chess with captured pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
 |<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
-|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `beta` | *Three in a row wins.* |
+|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -21,64 +21,64 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.terminated).all():
+# vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
-â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in May 2023. Opinions and
-comments are more than welcome!  ## Supported games | Backgammon | Chess |
-Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
+## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
+| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
+/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
-friendly shogi.* | |Backgammon
+main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
+shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif]| `beta` | *Checkmate opponent's king to win.* |
-|Connect_Four
+assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
+Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/connect_four_light.gif]| `beta` | *Connect discs, win with
-four.* | |Go
+main/docs/assets/connect_four_light.gif]| `v0` | *Connect discs, win with
+four.* | |Gardner_Chess
+`"gardner_chess"`|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/gardner_chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
+main/docs/assets/gardner_chess_light.gif]| `v0` | *5x5 chess variant, excluding
+castling.* | |Go
 `"go_9x9"` `"go_19x19"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
 docs/assets/go-19x19_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/go-19x19_light.gif]| `beta` | *Strategically place stones,
-claim territory.* | |Hex
+main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
+territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-hex_light.gif]| `beta` | *Connect opposite sides, block opponent.* | |Kuhn
-Poker
+hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
 bluffing game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
@@ -96,27 +96,27 @@
 docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
 dodge bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/othello_light.gif]| `beta` | *Flip and conquer opponent's pieces.* |
+assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_light.gif] | `beta` | *Japanese chess with captured pieces.* |
+assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
 pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/tic_tac_toe_light.gif]| `beta` | *Three in a row wins.* | -
+main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
 (classic) board game suits: - [RobertTLange/gymnax](https://github.com/
 RobertTLange/gymnax): JAX implementation of popular RL environments ([classic
 control](https://gymnasium.farama.org/environments/classic_control), [bsuite]
 (https://github.com/deepmind/bsuite), MinAtar, etc) and meta RL tasks -
```

### Comparing `pgx-0.7.4/pgx/_mahjong/_hand.py` & `pgx-0.8.0/pgx/_mahjong/_hand.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,46 +37,34 @@
 
         last_draw = deck[-(16 * 3 + 4 + 1)].astype(int)
         hand = hand.at[0].set(Hand.add(hand[0], last_draw))  # type: ignore
 
         return hand
 
     @staticmethod
-    def cache(code: int) -> int:
+    def cache(code: int):
         return (Hand.CACHE[code >> 5] >> (code & 0b11111)) & 1
 
     @staticmethod
-    def can_ron(hand: jnp.ndarray, tile: int) -> bool:
+    def can_ron(hand: jnp.ndarray, tile: int):
         return Hand.can_tsumo(Hand.add(hand, tile))
 
     @staticmethod
-    def can_riichi(hand: jnp.ndarray) -> bool:
-        return jax.lax.fori_loop(
-            0,
-            34,
-            lambda i, sum: jax.lax.cond(
-                hand[i] == 0,
-                lambda: sum,
-                lambda: sum | Hand.is_tenpai(Hand.sub(hand, i)),
-            ),
-            False,
-        )
+    def can_riichi(hand: jnp.ndarray):
+        """手牌は14枚"""
+        return jax.vmap(
+            lambda i: (hand[i] != 0) & Hand.is_tenpai(Hand.sub(hand, i))
+        )(jnp.arange(34)).any()
 
     @staticmethod
-    def is_tenpai(hand: jnp.ndarray) -> bool:
-        return jax.lax.fori_loop(
-            0,
-            34,
-            lambda tile, sum: jax.lax.cond(
-                hand[tile] == 4,
-                lambda: False,
-                lambda: sum | Hand.can_ron(hand, tile),
-            ),
-            False,
-        )
+    def is_tenpai(hand: jnp.ndarray):
+        """手牌は13枚"""
+        return jax.vmap(
+            lambda tile: (hand[tile] != 4) & Hand.can_ron(hand, tile)
+        )(jnp.arange(34)).any()
 
     @staticmethod
     def can_tsumo(hand: jnp.ndarray):
         thirteen_orphan = (
             (hand[0] > 0)
             & (hand[8] > 0)
             & (hand[9] > 0)
@@ -93,24 +81,35 @@
                     + jnp.sum(hand[26:])
                 )
                 == 14
             )
         )
         seven_pairs = jnp.sum(hand == 2) == 7
 
-        heads, valid = jnp.int32(0), jnp.int32(1)
-        for suit in range(3):
-            valid &= Hand.cache(
+        def _is_valid(suit):
+            return Hand.cache(
                 jax.lax.fori_loop(
                     9 * suit,
                     9 * (suit + 1),
                     lambda i, code: code * 5 + hand[i].astype(int),
                     0,
                 )
             )
+
+        valid = jax.vmap(_is_valid)(jnp.arange(3)).all()
+
+        # これはうまく行かない
+        # heads = (
+        #     (jnp.sum(hand[0:9]) % 3 == 2)
+        #     + (jnp.sum(hand[9:18]) % 3 == 2)
+        #     + (jnp.sum(hand[18:27]) % 3 == 2)
+        # )
+
+        heads = jnp.int32(0)
+        for suit in range(3):
             heads += jnp.sum(hand[9 * suit : 9 * (suit + 1)]) % 3 == 2
 
         heads, valid = jax.lax.fori_loop(
             27,
             34,
             lambda i, tpl: (
                 tpl[0] + (hand[i] == 2),
@@ -141,29 +140,26 @@
     def can_chi(hand: jnp.ndarray, tile: int, action: int) -> bool:
         return jax.lax.cond(
             (tile >= 27) | (action < Action.CHI_L) | (Action.CHI_R < action),
             lambda: False,
             lambda: jax.lax.switch(
                 action - Action.CHI_L,
                 [
-                    lambda: jax.lax.cond(
-                        tile % 9 < 7,
-                        lambda: (hand[tile + 1] > 0) & (hand[tile + 2] > 0),
-                        lambda: False,
-                    ),
-                    lambda: jax.lax.cond(
-                        (tile % 9 < 8) & (tile % 9 > 0),
-                        lambda: (hand[tile - 1] > 0) & (hand[tile + 1] > 0),
-                        lambda: False,
-                    ),
-                    lambda: jax.lax.cond(
-                        tile % 9 > 1,
-                        lambda: (hand[tile - 2] > 0) & (hand[tile - 1] > 0),
-                        lambda: False,
+                    lambda: (tile % 9 < 7)
+                    & (hand[tile + 1] > 0)
+                    & (hand[tile + 2] > 0),
+                    lambda: (
+                        (tile % 9 < 8)
+                        & (tile % 9 > 0)
+                        & (hand[tile - 1] > 0)
+                        & (hand[tile + 1] > 0)
                     ),
+                    lambda: (tile % 9 > 1)
+                    & (hand[tile - 2] > 0)
+                    & (hand[tile - 1] > 0),
                 ],
             ),
         )
 
     @staticmethod
     def add(hand: jnp.ndarray, tile: int, x: int = 1) -> jnp.ndarray:
         return hand.at[tile].set(hand[tile] + x)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pgx-0.7.4/pgx/_mahjong/_meld.py` & `pgx-0.8.0/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_mahjong/_shanten.py` & `pgx-0.8.0/pgx/_mahjong/_shanten.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,21 @@
     # See the link below for the algorithm details.
     # https://github.com/sotetsuk/pgx/pull/123
 
     CACHE = load_shanten_cache()
 
     @staticmethod
     def discard(hand: jnp.ndarray) -> jnp.ndarray:
-        return jax.lax.map(
+        return jax.vmap(
             lambda i: jax.lax.cond(
                 hand[i] == 0,
                 lambda: 0,
                 lambda: Shanten.number(hand.at[i].set(hand[i] - 1)),
-            ),
-            jnp.arange(34),
-        )
+            )
+        )(jnp.arange(34))
 
     @staticmethod
     def number(hand: jnp.ndarray):
         return jnp.min(
             jnp.array(
                 [
                     Shanten.normal(hand),
@@ -65,15 +64,15 @@
             + (hand[18] > 0).astype(int)
             + jnp.sum(hand[26:34] > 0)
         )
         return 14 - n_kind - (n_pair > 0)
 
     @staticmethod
     def normal(hand: jnp.ndarray):
-        code = jax.lax.map(
+        code = jax.vmap(
             lambda suit: jax.lax.cond(
                 suit == 3,
                 lambda: jax.lax.fori_loop(
                     27,
                     34,
                     lambda i, code: code * 5 + hand[i].astype(int),
                     0,
@@ -81,23 +80,22 @@
                 + 1953125,
                 lambda: jax.lax.fori_loop(
                     9 * suit,
                     9 * (suit + 1),
                     lambda i, code: code * 5 + hand[i].astype(int),
                     0,
                 ),
-            ),
-            jnp.arange(4),
-        )
+            )
+        )(jnp.arange(4))
 
         n_set = jnp.sum(hand).astype(int) // 3
 
         return jnp.min(
-            jax.lax.map(
-                lambda suit: Shanten._normal(code, n_set, suit), jnp.arange(4)
+            jax.vmap(lambda suit: Shanten._normal(code, n_set, suit))(
+                jnp.arange(4)
             )
         )
 
     @staticmethod
     def _normal(code: jnp.ndarray, n_set, head_suit) -> int:
         cost = Shanten.CACHE[code[head_suit]][4]
         idx = jnp.full(4, 0).at[head_suit].set(5)
```

### Comparing `pgx-0.7.4/pgx/_mahjong/_yaku.py` & `pgx-0.8.0/pgx/_mahjong/_yaku.py`

 * *Files 8% similar despite different names*

```diff
@@ -318,44 +318,90 @@
             + (hand[32] == 3) * 4 * (2 - (is_ron & (32 == last)))
             + (hand[33] == 3) * 4 * (2 - (is_ron & (33 == last)))
             # NOTE: 東場東家
             + ((27 <= last) & (hand[last] == 2)),
             dtype=jnp.int32,
         )
 
-        for suit in range(3):
+        def _update_yaku(suit, tpl):
             code = jax.lax.fori_loop(
                 9 * suit,
                 9 * (suit + 1),
                 lambda i, code: code * 5 + hand[i].astype(int),
                 0,
             )
+            return Yaku.update(
+                tpl[0],
+                tpl[1],
+                tpl[2],
+                tpl[3],
+                tpl[4],
+                tpl[5],
+                tpl[6],
+                tpl[7],
+                code,
+                suit,
+                last,
+                is_ron,
+            )
+
+        (
+            is_pinfu,
+            is_outside,
+            n_double_chow,
+            all_chow,
+            all_pung,
+            n_concealed_pung,
+            nine_gates,
+            fu,
+        ) = jax.lax.fori_loop(
+            0,
+            3,
+            _update_yaku,
             (
                 is_pinfu,
                 is_outside,
                 n_double_chow,
                 all_chow,
                 all_pung,
                 n_concealed_pung,
                 nine_gates,
                 fu,
-            ) = Yaku.update(
-                is_pinfu,
-                is_outside,
-                n_double_chow,
-                all_chow,
-                all_pung,
-                n_concealed_pung,
-                nine_gates,
-                fu,
-                code,
-                suit,
-                last,
-                is_ron,
-            )
+            ),
+        )
+        # for suit in range(3):
+        #    code = jax.lax.fori_loop(
+        #        9 * suit,
+        #        9 * (suit + 1),
+        #        lambda i, code: code * 5 + hand[i].astype(int),
+        #        0,
+        #    )
+        #    (
+        #        is_pinfu,
+        #        is_outside,
+        #        n_double_chow,
+        #        all_chow,
+        #        all_pung,
+        #        n_concealed_pung,
+        #        nine_gates,
+        #        fu,
+        #    ) = Yaku.update(
+        #        is_pinfu,
+        #        is_outside,
+        #        n_double_chow,
+        #        all_chow,
+        #        all_pung,
+        #        n_concealed_pung,
+        #        nine_gates,
+        #        fu,
+        #        code,
+        #        suit,
+        #        last,
+        #        is_ron,
+        #    )
 
         n_concealed_pung += jnp.sum(hand[27:] >= 3) - (
             is_ron & (last >= 27) & (hand[last] >= 3)
         )
 
         fu *= is_pinfu == 0
         fu += 20 + 10 * (is_menzen & is_ron)
```

### Comparing `pgx-0.7.4/pgx/_src/api_test.py` & `pgx-0.8.0/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/assets/between.npy` & `pgx-0.8.0/pgx/_src/assets/between.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/assets/can_move.npy` & `pgx-0.8.0/pgx/_src/assets/can_move.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/chess_utils.py` & `pgx-0.8.0/pgx/_src/gardner_chess_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,188 +1,150 @@
 # type: ignore
+import jax
 import jax.numpy as jnp
-import jax.random
 
-TO_MAP = -jnp.ones((64, 73), dtype=jnp.int8)
-PLANE_MAP = -jnp.ones((64, 64), dtype=jnp.int8)  # ignores underpromotion
-# underpromotiona
-for from_ in range(64):
-    if (from_ % 8) not in (1, 6):
+TO_MAP = -jnp.ones((25, 49), dtype=jnp.int8)
+PLANE_MAP = -jnp.ones((25, 25), dtype=jnp.int8)  # ignores underpromotions
+# underpromotions
+for from_ in range(25):
+    if from_ % 5 != 3:  # 4th row in current player view
         continue
     for plane in range(9):
         dir_ = plane % 3
-        to = -1
-        if from_ % 8 == 6:
-            # white
-            # 8  7 15 23 31 39 47 55 63
-            # 7  6 14 22 30 38 46 54 62
-            # black
-            # 2  6 14 22 30 38 46 54 62
-            # 1  7 15 23 31 39 47 55 63
-            to = from_ + jnp.int8([+1, +9, -7])[dir_]
-        if not (0 <= to < 64):
+        # board index (white view)
+        # 5  4  9 14 19 24
+        # 4  3  8 13 18 23
+        # board index (flipped black view)
+        # 5  0  5 10 15 20
+        # 4  1  6 11 16 21
+        to = from_ + jnp.int8([+1, +6, -4])[dir_]
+        if not (0 <= to < 25):
             continue
         TO_MAP = TO_MAP.at[from_, plane].set(to)
 # normal move
-seq = list(range(1, 8))
-zeros = [0 for _ in range(7)]
-# 下
-dr = [-x for x in seq[::-1]]
-dc = [0 for _ in range(7)]
-# 上
-dr += [x for x in seq]
-dc += [0 for _ in range(7)]
-# 左
-dr += [0 for _ in range(7)]
-dc += [-x for x in seq[::-1]]
-# 右
-dr += [0 for _ in range(7)]
-dc += [x for x in seq]
-# 左下
-dr += [-x for x in seq[::-1]]
-dc += [-x for x in seq[::-1]]
-# 右上
-dr += [x for x in seq]
-dc += [x for x in seq]
-# 左上
-dr += [x for x in seq[::-1]]
-dc += [-x for x in seq[::-1]]
-# 右下
-dr += [-x for x in seq]
-dc += [x for x in seq]
-# knight moves
-dr += [-1, +1, -2, +2, -1, +1, -2, +2]
-dc += [-2, -2, -1, -1, +2, +2, +1, +1]
-for from_ in range(64):
-    for plane in range(9, 73):
-        r, c = from_ % 8, from_ // 8
+# fmt: off
+dr = [-4, -3, -2, -1,  1,  2,  3,  4,  0,  0,  0,  0,  0,  0,  0,  0, -4, -3, -2, -1,  1,  2,  3,  4,  4,  3,  2,  1, -1, -2, -3, -4, -1, +1, -2, +2, -1, +1, -2, +2]  # noqa
+dc = [ 0,  0,  0,  0,  0,  0,  0,  0, -4, -3, -2, -1, +1, +2, +3, +4, -4, -3, -2, -1, +1, +2, +3, +4, -4, -3, -2, -1, +1, +2, +3, +4, -2, -2, -1, -1, +2, +2, +1, +1]  # noqa
+# fmt: on
+for from_ in range(25):
+    for plane in range(9, 49):
+        r, c = from_ % 5, from_ // 5
         r = r + dr[plane - 9]
         c = c + dc[plane - 9]
-        if r < 0 or r >= 8 or c < 0 or c >= 8:
+        if r < 0 or r >= 5 or c < 0 or c >= 5:
             continue
-        to = jnp.int8(c * 8 + r)
+        to = jnp.int8(c * 5 + r)
         TO_MAP = TO_MAP.at[from_, plane].set(to)
         PLANE_MAP = PLANE_MAP.at[from_, to].set(jnp.int8(plane))
 
 
-CAN_MOVE = -jnp.ones((7, 64, 27), jnp.int8)
+CAN_MOVE = -jnp.ones((7, 25, 16), jnp.int8)
 # usage: CAN_MOVE[piece, from_x, from_y]
 # CAN_MOVE[0, :, :]はすべて-1
 # 将棋と違い、中央から点対称でないので、注意が必要。
 # 視点は常に白側のイメージが良い。
-# PAWN以外の動きは上下左右対称。PAWNは上下と斜めへ動ける駒と定義して、手番に応じてフィルタする。
+# PAWN以外の動きは上下左右対称。
 
 
 # PAWN
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
-        if jnp.abs(r1 - r0) == 1 and jnp.abs(c1 - c0) <= 1:
-            legal_dst.append(to)
-        # init move
-        if (r0 == 1 or r0 == 6) and (
-            jnp.abs(c1 - c0) == 0 and jnp.abs(r1 - r0) == 2
-        ):
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
+        if r1 - r0 == 1 and jnp.abs(c1 - c0) <= 1:
             legal_dst.append(to)
-    assert len(legal_dst) <= 8
+    assert len(legal_dst) <= 6, f"{from_=}, {to=}, {legal_dst=}"
     CAN_MOVE = CAN_MOVE.at[1, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 # KNIGHT
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
         if jnp.abs(r1 - r0) == 1 and jnp.abs(c1 - c0) == 2:
             legal_dst.append(to)
         if jnp.abs(r1 - r0) == 2 and jnp.abs(c1 - c0) == 1:
             legal_dst.append(to)
-    assert len(legal_dst) <= 27
+    assert len(legal_dst) <= 8
     CAN_MOVE = CAN_MOVE.at[2, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 # BISHOP
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
         if from_ == to:
             continue
         if jnp.abs(r1 - r0) == jnp.abs(c1 - c0):
             legal_dst.append(to)
-    assert len(legal_dst) <= 27
+    assert len(legal_dst) <= 8
     CAN_MOVE = CAN_MOVE.at[3, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 # ROOK
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
         if from_ == to:
             continue
         if jnp.abs(r1 - r0) == 0 or jnp.abs(c1 - c0) == 0:
             legal_dst.append(to)
-    assert len(legal_dst) <= 27
+    assert len(legal_dst) <= 8
     CAN_MOVE = CAN_MOVE.at[4, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 # QUEEN
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
         if from_ == to:
             continue
         if jnp.abs(r1 - r0) == 0 or jnp.abs(c1 - c0) == 0:
             legal_dst.append(to)
         if jnp.abs(r1 - r0) == jnp.abs(c1 - c0):
             legal_dst.append(to)
-    assert len(legal_dst) <= 27
+    assert len(legal_dst) <= 16
     CAN_MOVE = CAN_MOVE.at[5, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 # KING
-for from_ in range(64):
-    r0, c0 = from_ % 8, from_ // 8
+for from_ in range(25):
+    r0, c0 = from_ % 5, from_ // 5
     legal_dst = []
-    for to in range(64):
-        r1, c1 = to % 8, to // 8
+    for to in range(25):
+        r1, c1 = to % 5, to // 5
         if from_ == to:
             continue
         if (jnp.abs(r1 - r0) <= 1) and (jnp.abs(c1 - c0) <= 1):
             legal_dst.append(to)
-    # castling
-    # if from_ == 32:
-    #     legal_dst += [16, 48]
-    # if from_ == 39:
-    #     legal_dst += [23, 55]
     assert len(legal_dst) <= 8
     CAN_MOVE = CAN_MOVE.at[6, from_, : len(legal_dst)].set(jnp.int8(legal_dst))
 
 assert (CAN_MOVE[0, :, :] == -1).all()
 
-CAN_MOVE_ANY = -jnp.ones((64, 35), jnp.int8)
-for from_ in range(64):
+CAN_MOVE_ANY = -jnp.ones((25, 24), jnp.int8)
+for from_ in range(25):
     legal_dst = []
-    for i in range(27):
+    for i in range(16):
         to = CAN_MOVE[5, from_, i]  # QUEEN
         if to >= 0:
             legal_dst.append(to)
-    for i in range(27):
+    for i in range(16):
         to = CAN_MOVE[2, from_, i]  # KNIGHT
         if to >= 0:
             legal_dst.append(to)
+    assert len(legal_dst) <= 24
     CAN_MOVE_ANY = CAN_MOVE_ANY.at[from_, : len(legal_dst)].set(
         jnp.int8(legal_dst)
     )
 
-
-# Between
-BETWEEN = -jnp.ones((64, 64, 6), dtype=jnp.int8)
-for from_ in range(64):
-    for to in range(64):
-        r0, c0 = from_ % 8, from_ // 8
-        r1, c1 = to % 8, to // 8
+BETWEEN = -jnp.ones((25, 25, 3), dtype=jnp.int8)
+for from_ in range(25):
+    for to in range(25):
+        r0, c0 = from_ % 5, from_ // 5
+        r1, c1 = to % 5, to // 5
         if not (
             (jnp.abs(r1 - r0) == 0 or jnp.abs(c1 - c0) == 0)
             or (jnp.abs(r1 - r0) == jnp.abs(c1 - c0))
         ):
             continue
         dr = max(min(r1 - r0, 1), -1)
         dc = max(min(c1 - c0, 1), -1)
@@ -190,31 +152,31 @@
         c = c0
         bet = []
         while True:
             r += dr
             c += dc
             if r == r1 and c == c1:
                 break
-            bet.append(c * 8 + r)
-        assert len(bet) <= 6
+            bet.append(c * 5 + r)
+        assert len(bet) <= 3
         BETWEEN = BETWEEN.at[from_, to, : len(bet)].set(jnp.int8(bet))
 
-INIT_LEGAL_ACTION_MASK = jnp.zeros(64 * 73, dtype=jnp.bool_)
+
+INIT_LEGAL_ACTION_MASK = jnp.zeros(25 * 49, dtype=jnp.bool_)
 # fmt: off
-ixs = [89, 90, 652, 656, 673, 674, 1257, 1258, 1841, 1842, 2425, 2426, 3009, 3010, 3572, 3576, 3593, 3594, 4177, 4178]
+ixs = [62, 289, 293, 307, 552, 797, 1042]
 # fmt: on
 for ix in ixs:
     INIT_LEGAL_ACTION_MASK = INIT_LEGAL_ACTION_MASK.at[ix].set(True)
-assert INIT_LEGAL_ACTION_MASK.shape == (64 * 73,)
-assert INIT_LEGAL_ACTION_MASK.sum() == 20
+assert INIT_LEGAL_ACTION_MASK.shape == (25 * 49,)
+assert INIT_LEGAL_ACTION_MASK.sum() == 7
 
-INIT_POSSIBLE_PIECE_POSITIONS = jnp.int8(
-    [
-        [0, 1, 8, 9, 16, 17, 24, 25, 32, 33, 40, 41, 48, 49, 56, 57],
-        [0, 1, 8, 9, 16, 17, 24, 25, 32, 33, 40, 41, 48, 49, 56, 57],
-    ]
-)  # (2, 16)
-
-key = jax.random.PRNGKey(9999)
-HASH_TABLE = jax.random.randint(
-    key, shape=(64, 13, 2), minval=0, maxval=2**31 - 1, dtype=jnp.uint32
+
+key = jax.random.PRNGKey(238942)
+key, subkey = jax.random.split(key)
+ZOBRIST_BOARD = jax.random.randint(
+    subkey, shape=(25, 13, 2), minval=0, maxval=2**31 - 1, dtype=jnp.uint32
+)
+key, subkey = jax.random.split(key)
+ZOBRIST_SIDE = jax.random.randint(
+    subkey, shape=(2,), minval=0, maxval=2**31 - 1, dtype=jnp.uint32
 )
```

### Comparing `pgx-0.7.4/pgx/_src/dwg/animalshogi.py` & `pgx-0.8.0/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/backgammon.py` & `pgx-0.8.0/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.8.0/pgx/_src/dwg/bridge_bidding.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 def _make_bridge_dwg(dwg, state: BridgeBiddingState, config):
     NUM_CARD_TYPE = 13
     # fmt: off
     TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"]
     SUITS = ["\u2660", "\u2665", "\u2666", "\u2663"]  # ♠♡♢♣
     DENOMINATIONS = ["\u2663", "\u2666", "\u2665", "\u2660", "N"]  # ♣♢♡♠
     ACT = ["P", "X", "XX"]
+    BID_OFFSET_NUM = 3
     # fmt:on
     color_set = config["COLOR_SET"]
 
     # board
     board_g = dwg.g()
 
     # hand
@@ -206,21 +207,30 @@
             stroke_width="5px",
         )
     )
     for i, act in enumerate(state._bidding_history):
         if act == -1:
             break
         act_str = (
-            str(act // 5 + 1) + DENOMINATIONS[(act % 5)]
-            if 0 <= act < 35
-            else ACT[act - 35]
+            str((act - BID_OFFSET_NUM) // 5 + 1)
+            + DENOMINATIONS[(act - BID_OFFSET_NUM) % 5]
+            if BID_OFFSET_NUM <= act < 35 + BID_OFFSET_NUM
+            else ACT[act]
         )
         color = (
             "orangered"
-            if act % 5 == 1 or act % 5 == 2
+            if (
+                (act > BID_OFFSET_NUM)
+                and (
+                    (act - BID_OFFSET_NUM) % 5 == 1
+                    or (act - BID_OFFSET_NUM) % 5 == 2
+                )
+            )
+            or act == 1
+            or act == 2
             else color_set.text_color
         )
         board_g.add(
             dwg.text(
                 text=act_str,
                 insert=(_x + 15 + 50 * (i % 4), _y + 50 + 20 * (i // 4)),
                 fill=color,
```

### Comparing `pgx-0.7.4/pgx/_src/dwg/chess.py` & `pgx-0.8.0/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/connect_four.py` & `pgx-0.8.0/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/go.py` & `pgx-0.8.0/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/hex.py` & `pgx-0.8.0/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.8.0/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.8.0/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.8.0/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.8.0/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/othello.py` & `pgx-0.8.0/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/play2048.py` & `pgx-0.8.0/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/shogi.py` & `pgx-0.8.0/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.8.0/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/dwg/tictactoe.py` & `pgx-0.8.0/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/shogi_utils.py` & `pgx-0.8.0/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/struct.py` & `pgx-0.8.0/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/_src/visualizer.py` & `pgx-0.8.0/pgx/_src/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,44 @@
                     "none",
                     "gray",
                     "white",
                     "white",
                     "black",
                     "",
                 )
+        elif _state.env_id == "gardner_chess":
+            from pgx._src.dwg.gardner_chess import _make_gardner_chess_dwg
+
+            self.config["GRID_SIZE"] = 50
+            self.config["BOARD_WIDTH"] = 5
+            self.config["BOARD_HEIGHT"] = 5
+            self._make_dwg_group = _make_gardner_chess_dwg  # type:ignore
+            if (
+                self.config["COLOR_THEME"] is None
+                and self.config["COLOR_THEME"] == "dark"
+            ) or self.config["COLOR_THEME"] == "dark":
+                self.config["COLOR_SET"] = ColorSet(
+                    "none",
+                    "none",
+                    "#404040",
+                    "gray",
+                    "#1e1e1e",
+                    "silver",
+                    "",
+                )
+            else:
+                self.config["COLOR_SET"] = ColorSet(
+                    "none",
+                    "none",
+                    "gray",
+                    "white",
+                    "white",
+                    "black",
+                    "",
+                )
         elif _state.env_id == "connect_four":
             from pgx._src.dwg.connect_four import _make_connect_four_dwg
 
             self.config["GRID_SIZE"] = 35
             self.config["BOARD_WIDTH"] = 7
             self.config["BOARD_HEIGHT"] = 7
             self._make_dwg_group = _make_connect_four_dwg  # type:ignore
```

### Comparing `pgx-0.7.4/pgx/animal_shogi.py` & `pgx-0.8.0/pgx/animal_shogi.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,21 @@
 KING = jnp.int8(3)
 GOLD = jnp.int8(4)
 #  5: OPP_PAWN
 #  6: OPP_ROOK
 #  7: OPP_BISHOP
 #  8: OPP_KING
 #  9: OPP_GOLD
-INIT_BOARD = jnp.int8([6, -1, -1, 2, 8, 5, 0, 3, 7, -1, -1, 1])  # (12,)
+# fmt: off
+INIT_BOARD = jnp.int8(
+    [6, -1, -1, 2,
+     8, 5, 0, 3,
+     7, -1, -1, 1]
+)  # (12,)
+# fmt: on
 
 ZOBRIST_KEY = jax.random.PRNGKey(23279)
 ZOBRIST_SIDE = jax.random.randint(
     ZOBRIST_KEY, shape=(2,), minval=0, maxval=2**31 - 1, dtype=jnp.uint32
 )
 ZOBRIST_KEY, ZOBRIST_SUBKEY = jax.random.split(ZOBRIST_KEY)
 ZOBRIST_BOARD = jax.random.randint(
@@ -54,14 +60,17 @@
     shape=(2, 3, 3, 2),
     minval=0,
     maxval=2**31 - 1,
     dtype=jnp.uint32,
 )
 
 
+MAX_TERMINATION_STEPS = 256
+
+
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(132, dtype=jnp.bool_)  # (132,)
@@ -70,18 +79,23 @@
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     _board: jnp.ndarray = INIT_BOARD  # (12,)
     _hand: jnp.ndarray = jnp.zeros((2, 3), dtype=jnp.int8)
     _zobrist_hash: jnp.ndarray = jnp.uint32([233882788, 593924309])
     _hash_history: jnp.ndarray = (
-        jnp.zeros((101, 2), dtype=jnp.uint32)
+        jnp.zeros((MAX_TERMINATION_STEPS + 1, 2), dtype=jnp.uint32)
         .at[0]
         .set(jnp.uint32([233882788, 593924309]))
     )
+    _board_history: jnp.ndarray = (
+        (-jnp.ones((8, 12), dtype=jnp.int8)).at[0, :].set(INIT_BOARD)
+    )
+    _hand_history: jnp.ndarray = jnp.zeros((8, 6), dtype=jnp.int8)
+    _rep_history: jnp.ndarray = jnp.zeros((8,), dtype=jnp.int8)
 
     @property
     def env_id(self) -> v1.EnvId:
         return "animal_shogi"
 
 
 @dataclass
@@ -105,29 +119,27 @@
             lambda: Action(is_drop=FALSE, from_=sq, to=_to(sq, x)),  # type: ignore
         )
 
 
 class AnimalShogi(v1.Env):
     def __init__(self):
         super().__init__()
-        self.max_termination_steps: int = 100
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         state = state.replace(legal_action_mask=_legal_action_mask(state))  # type: ignore
         return state
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         state = _step(state, action)
         state = jax.lax.cond(
-            (0 <= self.max_termination_steps)
-            & (self.max_termination_steps <= state._step_count),
+            MAX_TERMINATION_STEPS <= state._step_count,
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
@@ -136,75 +148,106 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "animal_shogi"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _step(state: State, action: jnp.ndarray):
     a = Action._from_label(action)
     # apply move/drop action
     state = jax.lax.cond(a.is_drop, _step_drop, _step_move, *(state, a))
     is_try = (state._board[jnp.int8([0, 4, 8])] == KING).any()
 
+    # update board/hand history
+    board_history = jnp.roll(state._board_history, 8)
+    board_history = board_history.at[0].set(state._board)
+    state = state.replace(_board_history=board_history)  # type:ignore
+    hand_history = jnp.roll(state._hand_history, 8)
+    hand_history = hand_history.at[0].set(state._hand.flatten())
+    state = state.replace(_hand_history=hand_history)  # type:ignore
+
     state = _flip(state)
     state = state.replace(  # type: ignore
         _hash_history=state._hash_history.at[state._step_count].set(
             state._zobrist_hash
         ),
     )
 
+    rep = (state._hash_history == state._zobrist_hash).any(
+        axis=1
+    ).sum().astype(jnp.int8) - 1
+    is_rep_draw = rep >= 2
     legal_action_mask = _legal_action_mask(state)  # TODO: fix me
-    rep = (state._hash_history == state._zobrist_hash).any(axis=1).sum()
-    is_rep_draw = rep >= 3
     terminated = (~legal_action_mask.any()) | is_try | is_rep_draw
     # fmt: off
     reward = jax.lax.select(
         terminated & ~is_rep_draw,
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
         jnp.zeros(2, dtype=jnp.float32),
     )
+    # rep history
+    rep_history = jnp.roll(state._rep_history, 1)
+    rep_history = rep_history.at[0].set(rep)
     # fmt: on
     return state.replace(  # type: ignore
         legal_action_mask=legal_action_mask,
         terminated=terminated,
         rewards=reward,
+        _rep_history=rep_history,
     )
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
-    state, flip_state = jax.lax.cond(
-        state.current_player == player_id,
-        lambda: (state, _flip(state)),
-        lambda: (_flip(state), state),
+    # player_id's color
+    color = jax.lax.select(
+        state.current_player == player_id, state._turn, 1 - state._turn
     )
 
-    def is_piece(p, state):
-        return state._board == p
-
-    def num_hand(p, n, state):
-        return state._hand.flatten()[p] >= n
-
-    # fmt: off
-    piece_feat = jax.vmap(partial(is_piece, state=state))(jnp.arange(10))  # (10, 12)
-    hand_feat = jax.vmap(jax.vmap(
-        partial(num_hand, state=state), (None, 0)), (0, None)
-    )(jnp.arange(6), jnp.arange(1, 3)).flatten().reshape(12, 1)  # (12, 1)
-    hand_feat = jnp.tile(hand_feat, reps=(1, 12))  # (12, 12)
-    # fmt: on
+    state = jax.lax.cond(
+        state.current_player == player_id,
+        lambda: state,
+        lambda: _flip(state),
+    )
 
-    obs = jnp.vstack((piece_feat, hand_feat))
-    obs = obs.reshape(-1, 3, 4).transpose((2, 1, 0))
+    def make(i):
+        def is_piece(p, state):
+            return state._board_history[i] == p
+
+        def num_hand(p, n, state):
+            return state._hand_history[i, p] >= n
+
+        # fmt: off
+        piece_feat = jax.vmap(partial(is_piece, state=state))(jnp.arange(10))  # (10, 12)
+        hand_feat = jax.vmap(jax.vmap(
+            partial(num_hand, state=state), (None, 0)), (0, None)
+        )(jnp.arange(6), jnp.arange(1, 3)).flatten().reshape(12, 1)  # (12, 1)
+        hand_feat = jnp.tile(hand_feat, reps=(1, 12))  # (12, 12)
+        # fmt: on
+
+        ones = jnp.ones((1, 12), dtype=jnp.float32)
+        rep0 = ones * (state._rep_history[i] == 0)
+        rep1 = ones * (state._rep_history[i] == 1)
+        return jnp.vstack((piece_feat, hand_feat, rep0, rep1))  # (24, 12)
+
+    obs = (
+        jax.vmap(make)(jnp.arange(8)).reshape(-1, 12).astype(jnp.float32)
+    )  # (192 = 8 * 24, 12)
+    ones = jnp.ones((1, 12), dtype=jnp.float32)
+    obs = jnp.vstack(
+        [obs, ones * color, ones * state._step_count / MAX_TERMINATION_STEPS]
+    )  # (193, 12)
+    obs = obs.reshape(-1, 3, 4).transpose((2, 1, 0))  # channel last
     return jnp.flip(obs, axis=1)
 
 
 def _step_move(state: State, action: Action) -> State:
     piece = state._board[action.from_]
     # remove piece from the original position
     board = state._board.at[action.from_].set(EMPTY)
@@ -306,20 +349,26 @@
 
 
 def _flip(state):
     empty_mask = state._board == EMPTY
     board = (state._board + 5) % 10
     board = jnp.where(empty_mask, EMPTY, board)
     board = board[::-1]
+    empty_mask_hist = state._board_history == EMPTY
+    board_history = (state._board_history + 5) % 10
+    board_history = jnp.where(empty_mask_hist, EMPTY, board_history)
+    board_history = board_history[:, ::-1]
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
         _turn=(state._turn + 1) % 2,
         _board=board,
         _hand=state._hand[::-1],
         _zobrist_hash=state._zobrist_hash ^ ZOBRIST_SIDE,
+        _board_history=board_history,
+        _hand_history=jnp.roll(state._hand_history, 3, axis=1),
     )
 
 
 def _can_move(piece, from_, to):
     def can_move(piece, from_, to):
         """Can <piece> move from <from_> to <to>?"""
         x0, y0 = from_ // 4, from_ % 4
```

### Comparing `pgx-0.7.4/pgx/backgammon.py` & `pgx-0.8.0/pgx/backgammon.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,26 +32,22 @@
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     # micro action = 6 * src + die
     legal_action_mask: jnp.ndarray = jnp.zeros(6 * 26 + 6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Backgammon specific ---
-    # 各point(24) bar(2) off(2)にあるcheckerの数. 黒+, 白-
+    # points(24) bar(2) off(2). black+, white-
     _board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
-    # サイコロを振るたびにrngをsplitして更新する.
-    _rng: jax.random.KeyArray = jnp.zeros(2, dtype=jnp.uint16)
-    # サイコロの出目 0~5: 1~6
-    _dice: jnp.ndarray = jnp.zeros(2, dtype=jnp.int16)
-    # プレイできるサイコロの目
-    _playable_dice: jnp.ndarray = jnp.zeros(4, dtype=jnp.int16)
-    # プレイしたサイコロの目の数
-    _played_dice_num: jnp.ndarray = jnp.int16(0)
-    # 黒0, 白1
-    _turn: jnp.ndarray = jnp.int8(1)
+    _dice: jnp.ndarray = jnp.zeros(2, dtype=jnp.int16)  # 0~5: 1~6
+    _playable_dice: jnp.ndarray = jnp.zeros(
+        4, dtype=jnp.int16
+    )  # playable dice -1 for empty
+    _played_dice_num: jnp.ndarray = jnp.int16(0)  # the number of dice played
+    _turn: jnp.ndarray = jnp.int8(1)  # black: 0 white:1
 
     @property
     def env_id(self) -> v1.EnvId:
         return "backgammon"
 
 
 class Backgammon(v1.Env):
@@ -85,71 +81,71 @@
     def _illegal_action_penalty(self) -> float:
         return -3.0
 
 
 def _init(rng: jax.random.KeyArray) -> State:
     rng1, rng2, rng3 = jax.random.split(rng, num=3)
     current_player: jnp.ndarray = jax.random.bernoulli(rng1).astype(jnp.int8)
-    board: jnp.ndarray = _make_init_board()  # 初期配置は対象なので, turnに関係
+    board: jnp.ndarray = _make_init_board()
     terminated: jnp.ndarray = FALSE
     dice: jnp.ndarray = _roll_init_dice(rng2)
     playable_dice: jnp.ndarray = _set_playable_dice(dice)
     played_dice_num: jnp.ndarray = jnp.int16(0)
     turn: jnp.ndarray = _init_turn(dice)
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, playable_dice)
     state = State(  # type: ignore
         current_player=current_player,
-        _rng=rng3,
+        _rng_key=rng3,
         _board=board,
         terminated=terminated,
         _dice=dice,
         _playable_dice=playable_dice,
         _played_dice_num=played_dice_num,
         _turn=turn,
         legal_action_mask=legal_action_mask,
     )
     return state
 
 
 def _step(state: State, action: jnp.ndarray) -> State:
     """
-    terminated していない場合のstep 関数.
+    Step when not terminated
     """
     state = _update_by_action(state, action)
     return jax.lax.cond(
         _is_all_off(state._board),
         lambda: _winning_step(state),
         lambda: _no_winning_step(state, action),
     )
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     """
-    手番のplayerに対する観測を返す.
+    Return observation for player_id
     """
     board: jnp.ndarray = state._board
-    zero_one_dice_vec: jnp.ndarray = _to_zero_one_dice_vec(
+    playable_dice_count_vec: jnp.ndarray = _to_playable_dice_count(
         state._playable_dice
     )
     return jax.lax.cond(
         player_id == state.current_player,
-        lambda: jnp.concatenate((board, zero_one_dice_vec), axis=None),  # type: ignore
+        lambda: jnp.concatenate((board, playable_dice_count_vec), axis=None),  # type: ignore
         lambda: jnp.concatenate(
             (board, jnp.zeros(6, dtype=jnp.int8)), axis=None  # type: ignore
         ),
     )
 
 
-def _to_zero_one_dice_vec(playable_dice: jnp.ndarray) -> jnp.ndarray:
+def _to_playable_dice_count(playable_dice: jnp.ndarray) -> jnp.ndarray:
     """
-    playできるサイコロを6次元の0-1ベクトルで返す.
+    Return 6 dim vec which represents the number of playable die
     """
     dice_indices: jnp.ndarray = jnp.array(
         [0, 1, 2, 3], dtype=jnp.int8
-    )  # サイコロの数は最大4
+    )  # maximum number of playable dice is 4
 
     def _insert_dice_num(
         idx: jnp.ndarray, playable_dice: jnp.ndarray
     ) -> jnp.ndarray:
         vec: jnp.ndarray = jnp.zeros(6, dtype=jnp.int8)
         return (playable_dice[idx] != -1) * vec.at[playable_dice[idx]].set(
             1
@@ -160,123 +156,123 @@
     ).sum(axis=0, dtype=jnp.int8)
 
 
 def _winning_step(
     state: State,
 ) -> State:
     """
-    勝利者がいる場合のstep.
+    Step with winner
     """
     win_score = _calc_win_score(state._board)
     winner = state.current_player
     loser = 1 - winner
     reward = jnp.ones_like(state.rewards)
     reward = reward.at[winner].set(win_score)
     reward = reward.at[loser].set(-win_score)
     state = state.replace(terminated=TRUE)  # type: ignore
     return state.replace(rewards=reward)  # type: ignore
 
 
 def _no_winning_step(state: State, action: jnp.ndarray) -> State:
     """
-    勝利者がいない場合のstep, ターン終了の条件を満たせばターンを変更する.
+    Step with no winner. Change turn if turn end condition is satisfied.
     """
     return jax.lax.cond(
         (_is_turn_end(state) | (action // 6 == 0)),
         lambda: _change_turn(state),
         lambda: state,
     )
 
 
 def _update_by_action(state: State, action: jnp.ndarray) -> State:
     """
-    行動を受け取って状態をupdate
+    Update state by action
     """
     is_no_op = action // 6 == 0
-    rng = state._rng
+    rng_key = state._rng_key
     current_player: jnp.ndarray = state.current_player
     terminated: jnp.ndarray = state.terminated
     board: jnp.ndarray = _move(state._board, action)
     played_dice_num: jnp.ndarray = jnp.int16(state._played_dice_num + 1)
     playable_dice: jnp.ndarray = _update_playable_dice(
         state._playable_dice, state._played_dice_num, state._dice, action
     )
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, playable_dice)
     return jax.lax.cond(
         is_no_op,
         lambda: state,
         lambda: state.replace(  # type: ignore
             current_player=current_player,
-            _rng=rng,
+            _rng_key=rng_key,
             terminated=terminated,
             _board=board,
             _turn=state._turn,
             _dice=state._dice,
             _playable_dice=playable_dice,
             _played_dice_num=played_dice_num,
             legal_action_mask=legal_action_mask,
         ),
     )  # no-opの時はupdateしない
 
 
 def _flip_board(board):
     """
-    ターンが変わる際にボードを反転させ, -1をかける. そうすることで常に黒視点で考えることができる.
+    Flip a board when turn changes. Multiply -1 to the board so that we can always consider the board from black's perspective.
     """
     _board = board
     board = board.at[:24].set(jnp.flip(_board[:24]))
     board = board.at[24:26].set(jnp.flip(_board[24:26]))
     board = board.at[26:28].set(jnp.flip(_board[26:28]))
     return -1 * board
 
 
 def _make_init_board() -> jnp.ndarray:
     """
-    黒基準で初期化
+    Initialize the board based on black's perspective.
     """
     board: jnp.ndarray = jnp.array([2, 0, 0, 0, 0, -5, 0, -3, 0, 0, 0, 5, -5, 0, 0, 0, 3, 0, 5, 0, 0, 0, 0, -2, 0, 0, 0, 0], dtype=jnp.int8)  # type: ignore
     return board
 
 
 def _is_turn_end(state: State) -> bool:
     """
-    play可能なサイコロ数が0の場合ないしlegal_actionがない場合交代
+    Turn will end if there is no playable dice or no legal action.
     """
     return state._playable_dice.sum() == -4  # type: ignore
 
 
 def _change_turn(state: State) -> State:
     """
-    ターンを変更して新しい状態を返す.
+    Change turn and return new state.
     """
-    rng1, rng2 = jax.random.split(state._rng)
-    board: jnp.ndarray = _flip_board(state._board)  # boardを反転させて黒視点に変える
-    turn: jnp.ndarray = (state._turn + 1) % 2  # turnを変える
+    rng1, rng2 = jax.random.split(state._rng_key)
+    board: jnp.ndarray = _flip_board(state._board)
+    turn: jnp.ndarray = (state._turn + 1) % 2
     current_player: jnp.ndarray = (state.current_player + 1) % 2
     terminated: jnp.ndarray = state.terminated
-    dice: jnp.ndarray = _roll_dice(rng1)  # diceを振る
-    playable_dice: jnp.ndarray = _set_playable_dice(dice)  # play可能なサイコロを初期化
+    dice: jnp.ndarray = _roll_dice(rng1)
+    playable_dice: jnp.ndarray = _set_playable_dice(dice)
     played_dice_num: jnp.ndarray = jnp.int16(0)
     legal_action_mask: jnp.ndarray = _legal_action_mask(board, dice)
     return state.replace(  # type: ignore
         current_player=current_player,
-        _rng=rng2,
+        _rng_key=rng2,
         _board=board,
         terminated=terminated,
         _turn=turn,
         _dice=dice,
         _playable_dice=playable_dice,
         _played_dice_num=played_dice_num,
         legal_action_mask=legal_action_mask,
     )
 
 
 def _roll_init_dice(rng: jax.random.KeyArray) -> jnp.ndarray:
     """
-    # 違う目が出るまで振り続ける.
+    Roll till the dice are different.
     """
 
     init_dice_pattern: jnp.ndarray = jnp.array([[0, 1], [0, 2], [0, 3], [0, 4], [0, 5], [1, 0], [1, 2], [1, 3], [1, 4], [1, 5], [2, 0], [2, 1], [2, 3], [2, 4], [2, 5], [3, 0], [3, 1], [3, 2], [3, 4], [3, 5], [4, 0], [4, 1], [4, 2], [4, 3], [4, 5], [5, 0], [5, 1], [5, 2], [5, 3], [5, 4]], dtype=jnp.int16)  # type: ignore
     return jax.random.choice(rng, init_dice_pattern)
 
 
 def _roll_dice(rng: jax.random.KeyArray) -> jnp.ndarray:
@@ -284,24 +280,24 @@
         rng, shape=(1, 2), minval=0, maxval=6, dtype=jnp.int16
     )
     return roll[0]
 
 
 def _init_turn(dice: jnp.ndarray) -> jnp.ndarray:
     """
-    ゲーム開始時のターン決め.
-    サイコロの目が大きい方が手番.
+    Decide turn at the beginning of the game.
+    Begin with those who have bigger dice
     """
     diff = dice[1] - dice[0]
     return jnp.int8(diff > 0)
 
 
 def _set_playable_dice(dice: jnp.ndarray) -> jnp.ndarray:
     """
-    -1でemptyを表す.
+    -1 for empty
     """
     return (dice[0] == dice[1]) * jnp.array([dice[0]] * 4, dtype=jnp.int16) + (
         dice[0] != dice[1]
     ) * jnp.array([dice[0], dice[1], -1, -1], dtype=jnp.int16)
 
 
 def _update_playable_dice(
@@ -310,15 +306,15 @@
     dice: jnp.ndarray,
     action: jnp.ndarray,
 ) -> jnp.ndarray:
     _n = played_dice_num
     die_array = jnp.array([action % 6] * 4, dtype=jnp.int16)
     dice_indices: jnp.ndarray = jnp.array(
         [0, 1, 2, 3], dtype=jnp.int16
-    )  # サイコロの数は最大4
+    )  # maximum number of playable dice is 4
 
     def _update_for_diff_dice(
         die: jnp.ndarray, idx: jnp.ndarray, playable_dice: jnp.ndarray
     ):
         return (die == playable_dice[idx]) * -1 + (
             die != playable_dice[idx]
         ) * playable_dice[idx]
@@ -330,81 +326,81 @@
     ).astype(
         jnp.int16
     )
 
 
 def _home_board() -> jnp.ndarray:
     """
-    黒: [18~23], 白: [0~5]: 常に黒視点
+    black: [18~23], white: [0~5]: Always black's perspective
     """
     return jnp.arange(18, 24, dtype=jnp.int8)  # type: ignore
 
 
 def _off_idx() -> int:
     """
-    黒: 26, 白: 27: 常に黒視点
+    black: 26, white: 27: Always black's perspective
     """
     return 26  # type: ignore
 
 
 def _bar_idx() -> int:
     """
-    黒: 24, 白 25: 常に黒視点
+    black: 24, white 25: Always black's perspective
     """
     return 24  # type: ignore
 
 
 def _rear_distance(board: jnp.ndarray) -> jnp.ndarray:
     """
-    board上にあるcheckerについて, goal地点とcheckerの距離の最大値: 常に黒視点
+    The distance from the farthest checker to the goal: Always black's perspective
     """
     b = board[:24]
     exists = jnp.where((b > 0), size=24, fill_value=jnp.nan)[0]  # type: ignore
     return 24 - jnp.min(jnp.nan_to_num(exists, nan=jnp.int16(100)))
 
 
 def _is_all_on_home_board(board: jnp.ndarray) -> bool:
     """
-    全てのcheckerがhome boardにあれば, bear offできる.
+    One can bear off if all checkers are on home board.
     """
     home_board: jnp.ndarray = _home_board()
     on_home_board: int = jnp.clip(board[home_board], a_min=0, a_max=15).sum()
     off: int = board[_off_idx()]  # type: ignore
     return (15 - off) == on_home_board
 
 
 def _is_open(board: jnp.ndarray, point: int) -> bool:
     """
-    手番のplayerにとって, pointが空いてるかを判定する.
-    pointにある相手のcheckerの数が1以下なら自分のcheckerをそのpointにおける.
+    Check if the point is open for the current player: Always black's perspective
+    One can move to the point if there is no more than one opponent's checker.
     """
     checkers = board[point]
     return checkers >= -1  # type: ignore
 
 
 def _exists(board: jnp.ndarray, point: int) -> bool:
     """
-    指定pointに手番のchckerが存在するか.
+    Check if the point has the current player's checker: Always black's perspective
     """
     checkers = board[point]
     return checkers >= 1  # type: ignore
 
 
 def _calc_src(src: jnp.ndarray) -> int:
     """
-    boardのindexに合わせる.
+    Translate src to board index.
     """
     return (src == 1) * jnp.int16(_bar_idx()) + (src != 1) * jnp.int16(
         src - 2
     )  # type: ignore
 
 
 def _calc_tgt(src: int, die) -> int:
     """
-    boardのindexに合わせる. actionは src*6 + dieの形になっている. targetは黒ならsrcからdie分+白ならdie分-(目的地が逆だから.)
+    Translate tgt to board index.
     """
     return (src >= 24) * (jnp.int16(die) - 1) + (src < 24) * jnp.int16(
         _from_board(src, die)
     )  # type: ignore
 
 
 def _from_board(src: int, die: int) -> int:
@@ -412,114 +408,115 @@
     return _is_to_board * jnp.int16(src + die) + ((~_is_to_board)) * jnp.int16(
         _off_idx()
     )  # type: ignore
 
 
 def _decompose_action(action: jnp.ndarray):
     """
-    action(int)をsource, die, tagetに分解する.
+    Decompose action to src, die, tgt.
+    action = src*6 + die
     """
     src = _calc_src(action // 6)  # 0~25
     die = action % 6 + 1  # 0~5 -> 1~6
     tgt = _calc_tgt(src, die)
     return src, die, tgt
 
 
 def _is_action_legal(board: jnp.ndarray, action: jnp.ndarray) -> bool:
     """
-    micro actionの合法判定
+    Check if the action is legal.
     action = src * 6 + die
     src = [no op., from bar, 0, .., 23]
     """
     src, die, tgt = _decompose_action(action)
     _is_to_point = (0 <= tgt) & (tgt <= 23) & (src >= 0)
     return _is_to_point & _is_to_point_legal(board, src, tgt) | (
         ~_is_to_point
     ) & _is_to_off_legal(
         board, src, tgt, die
     )  # type: ignore
 
 
 def _distance_to_goal(src: int) -> int:
     """
-    goal までの距離: 常に黒視点
+    The distance from the src to the goal: Always black's perspective
     """
     return 24 - src  # type: ignore
 
 
 def _is_to_off_legal(board: jnp.ndarray, src: int, tgt: int, die: int):
     """
-    board外への移動についての合法判定
-    条件は
-    1. srcにcheckerがある
-    2. 自身のcheckeが全てhomeboardにある.
-    3. サイコロの目とgoalへの距離が同じ or srcが最後尾であり, サイコロの目がそれよりも大きい.
+    Check if the action is legal when the target is off.
+    The conditions are:
+    1. src has checkers.
+    2. All checkers are on home board.
+    3. The distance from the src to the goal is the same as the die or the src is the farthest checker and the die is bigger than the distance.
     """
     r = _rear_distance(board)
     d = _distance_to_goal(src)
     return (
         (src >= 0)
         & _exists(board, src)
         & _is_all_on_home_board(board)
         & ((d == die) | ((r <= die) & (r == d)))
     )  # type: ignore
 
 
 def _is_to_point_legal(board: jnp.ndarray, src: int, tgt: int) -> bool:
     """
-    tgtがpointの場合の合法手判定
+    Check if the action is legal when the target is point.
     """
     e = _exists(board, src)
     o = _is_open(board, tgt)
     return ((src >= 24) & e & o) | (
         (src < 24) & e & o & (board[_bar_idx()] == 0)
     )  # type: ignore
 
 
 def _move(board: jnp.ndarray, action: jnp.ndarray) -> jnp.ndarray:
     """
-    micro actionに基づく状態更新: 常に黒視点
+    Move checkers based on the action.
     """
     src, _, tgt = _decompose_action(action)
     board = board.at[_bar_idx() + 1].add(
         -1 * (board[tgt] == -1)
     )  # targetに相手のcheckerが一枚だけある時, それを相手のbarに移動
     board = board.at[src].add(-1)
     board = board.at[tgt].add(1 + (board[tgt] == -1))  # hitした際は符号が変わるので余分に+1
     return board
 
 
 def _is_all_off(board: jnp.ndarray) -> bool:
     """
     手番のプレイヤーのチェッカーが全てoffにあれば勝利となる. 常に黒視点
+    If all checkers are off, the player wins. Always black's perspective.
     """
     return board[_off_idx()] == 15  # type: ignore
 
 
 def _calc_win_score(board: jnp.ndarray) -> int:
     """
-    通常勝ち: 1点
-    gammon勝ち: 2点
-    backgammon勝ち: 3点
+    Normal win: 1 point
+    Gammon win: 2 points
+    Backgammon win: 3 points
     """
     g = _is_gammon(board)
     return 1 + g + (g & _remains_at_inner(board))
 
 
 def _is_gammon(board: jnp.ndarray) -> bool:
     """
-    相手のoffに一つもcheckerがなければgammon勝ち
+    If there is no opponent's checker on off, the player wins gammon.
     """
     return board[_off_idx() + 1] == 0  # type: ignore
 
 
 def _remains_at_inner(board: jnp.ndarray) -> bool:
     """
-    相手のoffに一つもcheckerがない && 相手のcheckerが一つでも自分のインナーに残っている
-    => backgammon勝ち
+    (1)If there is no opponent's checker on off and (2) there is at least one opponent's checker on inner, the player wins backgammon.
     """
     return jnp.take(board, _home_board()).sum() != 0  # type: ignore
 
 
 def _legal_action_mask(board: jnp.ndarray, dice: jnp.ndarray) -> jnp.ndarray:
     no_op_mask = jnp.zeros(26 * 6 + 6, dtype=jnp.bool_).at[0:6].set(TRUE)
     legal_action_mask = jax.vmap(
@@ -527,31 +524,31 @@
     )(die=dice).any(
         axis=0
     )  # (26*6 + 6)
     legal_action_exists = ~(legal_action_mask.sum() == 0)
     return (
         legal_action_exists * legal_action_mask
         + ~legal_action_exists * no_op_mask
-    )  # legal_actionがなければ, np_op maskを返す
+    )  # if there is no legal action, no-op is legal
 
 
 def _legal_action_mask_for_single_die(board: jnp.ndarray, die) -> jnp.ndarray:
     """
-    一つのサイコロの目に対するlegal micro action
+    Legal action mask for a single die.
     """
     return (die == -1) * jnp.zeros(26 * 6 + 6, dtype=jnp.bool_) + (
         die != -1
     ) * _legal_action_mask_for_valid_single_dice(board, die)
 
 
 def _legal_action_mask_for_valid_single_dice(
     board: jnp.ndarray, die
 ) -> jnp.ndarray:
     """
-    -1以外のサイコロの目に対して合法判定
+    Legal action mask for a single die when the die is valid.
     """
     src_indices = jnp.arange(
         26, dtype=jnp.int16
     )  # 26パターンのsrcに対してlegal_actionを求める.
 
     def _is_legal(idx: jnp.ndarray):
         action = idx * 6 + die
@@ -565,13 +562,12 @@
         axis=0
     )  # (26*6 + 6)
     return legal_action_mask
 
 
 def _get_abs_board(state: State) -> jnp.ndarray:
     """
-    visualization用
-    黒ならそのまま, 白なら反転して返す.
+    For visualization.
     """
     board: jnp.ndarray = state._board
     turn: jnp.ndarray = state._turn
     return jax.lax.cond(turn == 0, lambda: board, lambda: _flip_board(board))
```

### Comparing `pgx-0.7.4/pgx/bridge_bidding.py` & `pgx-0.8.0/pgx/bridge_bidding.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 # カードと数字の対応
 # 0~12 spade, 13~25 heart, 26~38 diamond, 39~51 club
 # それぞれのsuitにおいて以下の順で数字が並ぶ
 TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "T", "J", "Q", "K"]
+PASS_ACTION_NUM = 0
+DOUBLE_ACTION_NUM = 1
+REDOUBLE_ACTION_NUM = 2
+BID_OFFSET_NUM = 3
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(-1)
     observation: jnp.ndarray = jnp.zeros(478, dtype=jnp.bool_)
     rewards: jnp.ndarray = jnp.float32([0, 0, 0, 0])
@@ -51,14 +55,15 @@
     # index = 0 ~ 12がN, 13 ~ 25がE, 26 ~ 38がS, 39 ~ 51がWの持つ手札
     # 各要素にはカードを表す0 ~ 51の整数が格納される
     _hand: jnp.ndarray = jnp.zeros(52, dtype=jnp.int32)
     # bidding_history 各プレイヤーのbidを時系列順に記憶
     # 最大の行動系列長 = 319
     # 各要素には、行動を表す整数が格納される
     # bidを表す0 ~ 34, passを表す35, doubleを表す36, redoubleを表す37, 行動が行われていない-1
+    # TODO pass = 0, double = 1, redouble = 2, bid = 3 ~ 37に変更
     # 各ビッドがどのプレイヤーにより行われたかは、要素のindexから分かる（ix % 4）
     _bidding_history: jnp.ndarray = jnp.full(319, -1, dtype=jnp.int32)
     # dealer どのプレイヤーがdealerかを表す
     # 0 = N, 1 = E, 2 = S, 3 = W
     # dealerは最初にbidを行うプレイヤー
     _dealer: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
     # vul_NS NSチームがvulかどうかを表す
@@ -146,16 +151,16 @@
     vul_EW = jax.random.choice(rng4, jnp.bool_([False, True]))
     dealer = jax.random.randint(rng5, (1,), 0, 4, dtype=jnp.int8)[0]
     # shuffled players and arrange in order of NESW
     shuffled_players = _shuffle_players(rng6)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
-    legal_actions = legal_actions.at[36].set(False)
-    legal_actions = legal_actions.at[37].set(False)
+    legal_actions = legal_actions.at[DOUBLE_ACTION_NUM].set(False)
+    legal_actions = legal_actions.at[REDOUBLE_ACTION_NUM].set(False)
     state = State(  # type: ignore
         _shuffled_players=shuffled_players,
         current_player=current_player,
         _hand=hand,
         _dealer=dealer,
         _vul_NS=vul_NS,
         _vul_EW=vul_EW,
@@ -173,16 +178,16 @@
     vul_EW = jax.random.choice(rng3, jnp.bool_([False, True]))
     dealer = jax.random.randint(rng4, (1,), 0, 4, dtype=jnp.int8)[0]
     # shuffled players and arrange in order of NESW
     shuffled_players = _shuffle_players(rng5)
     current_player = shuffled_players[dealer]
     legal_actions = jnp.ones(38, dtype=jnp.bool_)
     # 最初はdable, redoubleできない
-    legal_actions = legal_actions.at[36].set(False)
-    legal_actions = legal_actions.at[37].set(False)
+    legal_actions = legal_actions.at[DOUBLE_ACTION_NUM].set(False)
+    legal_actions = legal_actions.at[REDOUBLE_ACTION_NUM].set(False)
     state = State(  # type: ignore
         _shuffled_players=shuffled_players,
         current_player=current_player,
         _hand=hand,
         _dealer=dealer,
         _vul_NS=vul_NS,
         _vul_EW=vul_EW,
@@ -254,17 +259,17 @@
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> State:
     # fmt: off
     state = state.replace(_bidding_history=state._bidding_history.at[state._turn].set(action))  # type: ignore
     # fmt: on
     return jax.lax.cond(
-        action >= 35,
+        action <= 2,
         lambda: jax.lax.switch(
-            action - 35,
+            action,
             [
                 lambda: jax.lax.cond(
                     _is_terminated(_state_pass(state)),
                     lambda: _terminated_step(
                         _state_pass(state), hash_keys, hash_values
                     ),
                     lambda: _continue_step(_state_pass(state)),
@@ -277,83 +282,110 @@
     )
 
 
 @jax.jit
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     """Returns the observation of a given player"""
     # make vul of observation
-    vul = jnp.array([state._vul_NS, state._vul_EW], dtype=jnp.bool_)
+    is_player_vul, is_non_player_vul = jax.lax.cond(
+        (_player_position(state.current_player, state) == 0)
+        | (_player_position(state.current_player, state) == 2),
+        lambda: (state._vul_NS, state._vul_EW),
+        lambda: (state._vul_EW, state._vul_NS),
+    )
+    vul = jnp.array(
+        [~is_player_vul, is_player_vul, ~is_non_player_vul, is_non_player_vul],
+        dtype=jnp.bool_,
+    )
 
     # make hand of observation
     hand = jnp.zeros(52, dtype=jnp.bool_)
     position = _player_position(player_id, state).astype(jnp.int16)
     hand = jax.lax.fori_loop(
         position * 13,
         (position + 1) * 13,
-        lambda i, hand: hand.at[state._hand[i]].set(True),
+        lambda i, hand: hand.at[
+            _convert_card_pgx_to_openspiel(state._hand[i])
+        ].set(True),
         hand,
     )
 
     # make history of observation
+    last_bid = 0
     obs_history = jnp.zeros(424, dtype=jnp.bool_)
-    last_bid = jnp.int16(-1)
-    flag = FALSE
-    obs_history, last_bid, flag, state = jax.lax.fori_loop(
+    state, player_id, last_bid, obs_history = jax.lax.fori_loop(
         0,
         state._turn.astype(jnp.int32),
         _make_obs_history,
-        (obs_history, last_bid, flag, state),
+        (state, player_id, last_bid, obs_history),
     )
     return jnp.concatenate((vul, obs_history, hand))
 
 
 @jax.jit
-def _make_obs_history(i, vals):
-    obs_history, last_bid, flag, state = vals
-    curr_pos = ((state._dealer + i) % 4).astype(jnp.int16)
-    return jax.lax.cond(
-        (flag != jnp.bool_(True)) & (state._bidding_history[i] == 35),
-        lambda: (obs_history.at[curr_pos].set(True), last_bid, flag, state),
-        lambda: jax.lax.cond(
-            (0 <= state._bidding_history[i])
-            & (state._bidding_history[i] <= 34),
-            lambda: (
-                obs_history.at[
-                    4
-                    + curr_pos * 35
-                    + state._bidding_history[i].astype(jnp.int16)
-                ].set(True),
-                state._bidding_history[i].astype(jnp.int16),
-                jnp.bool_(True),
-                state,
-            ),
-            lambda: jax.lax.switch(
-                state._bidding_history[i] - 35,
-                [
-                    lambda: (obs_history, last_bid, flag, state),
-                    lambda: (
-                        obs_history.at[144 + curr_pos * 35 + last_bid].set(
-                            True
-                        ),
-                        last_bid,
-                        flag,
-                        state,
-                    ),
+def _make_obs_history(turn, vuls):
+    state, player_id, last_bid, obs_history = vuls
+    action = state._bidding_history[turn]
+    relative_bidder = (
+        (turn + state._dealer.astype(jnp.int32)) % 4
+        + (4 - _player_position(player_id, state).astype(jnp.int32))
+    ) % 4
+    last_bid, obs_history = jax.lax.cond(
+        action <= 2,
+        lambda: jax.lax.switch(
+            action,
+            [
+                lambda: jax.lax.cond(
+                    last_bid == 0,
                     lambda: (
-                        obs_history.at[284 + curr_pos * 35 + last_bid].set(
-                            True
-                        ),
                         last_bid,
-                        flag,
-                        state,
+                        obs_history.at[relative_bidder].set(True),
                     ),
-                ],
-            ),
+                    lambda: (last_bid, obs_history),
+                ),
+                lambda: (
+                    last_bid,
+                    obs_history.at[
+                        4
+                        + (last_bid - BID_OFFSET_NUM) * 4 * 3
+                        + 4
+                        + relative_bidder
+                    ].set(True),
+                ),
+                lambda: (
+                    last_bid,
+                    obs_history.at[
+                        4
+                        + (last_bid - BID_OFFSET_NUM) * 4 * 3
+                        + 4 * 2
+                        + relative_bidder
+                    ].set(True),
+                ),
+            ],
         ),
+        lambda: (
+            action,
+            obs_history.at[
+                4 + (action - BID_OFFSET_NUM) * 4 * 3 + relative_bidder
+            ].set(True),
+        ),
+    )
+    return state, player_id, last_bid, obs_history
+
+
+@jax.jit
+def _convert_card_pgx_to_openspiel(card: int) -> jnp.ndarray:
+    """Convert numerical representation of cards from pgx to openspiel"""
+    OPEN_SPIEL_SUIT_NUM = jnp.array([3, 2, 1, 0], dtype=jnp.int32)
+    OPEN_SPIEL_RANK_NUM = jnp.array(
+        [12, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], dtype=jnp.int32
     )
+    suit = OPEN_SPIEL_SUIT_NUM[card // 13]
+    rank = OPEN_SPIEL_RANK_NUM[card % 13]
+    return suit + rank * 4
 
 
 @jax.jit
 def duplicate(
     init_state: State,
 ) -> State:
     """Make duplicated state where NSplayer and EWplayer are swapped"""
@@ -392,15 +424,15 @@
     state = state.replace(  # type: ignore
         current_player=state._shuffled_players[(state._dealer + state._turn + 1) % 4],
         _turn=state._turn + 1
     )
     # 次のターンにX, XXが合法手か判断
     x_mask, xx_mask = _update_legal_action_X_XX(state)
     return state.replace(  # type: ignore
-        legal_action_mask=state.legal_action_mask.at[36].set(x_mask).at[37].set(xx_mask),
+        legal_action_mask=state.legal_action_mask.at[PASS_ACTION_NUM].set(True).at[DOUBLE_ACTION_NUM].set(x_mask).at[REDOUBLE_ACTION_NUM].set(xx_mask),
         rewards=jnp.zeros(4, dtype=jnp.float32)
     )
     # fmt: on
 
 
 @jax.jit
 def _is_terminated(state: State) -> bool:
@@ -683,31 +715,32 @@
     return state.replace(_call_xx=jnp.bool_(True), _pass_num=jnp.int32(0))  # type: ignore
 
 
 @jax.jit
 def _state_bid(state: State, action: int) -> State:
     """Change state if bid is taken"""
     # 最後のbidとそのプレイヤーを保存
+    bid = action - BID_OFFSET_NUM
     # fmt: off
-    state = state.replace(_last_bid=jnp.int32(action), _last_bidder=state.current_player)  # type: ignore
+    state = state.replace(_last_bid=bid, _last_bidder=state.current_player)  # type: ignore
     # fmt: on
     # チーム内で各denominationを最初にbidしたプレイヤー
-    denomination = _bid_to_denomination(action)
+    denomination = _bid_to_denomination(bid)
     team = _position_to_team(_player_position(state._last_bidder, state))
     # fmt: off
     # team = 1ならEWチーム
     state = jax.lax.cond(team & (state._first_denomination_EW[denomination] == -1),
                          lambda: state.replace(_first_denomination_EW=state._first_denomination_EW.at[denomination].set(state._last_bidder.astype(jnp.int8))),  # type: ignore
                          lambda: state)  # type: ignore
     # team = 0ならNSチーム
     state = jax.lax.cond((team == 0) & (state._first_denomination_NS[denomination] == -1),
                          lambda: state.replace(_first_denomination_NS=state._first_denomination_NS.at[denomination].set(state._last_bidder.astype(jnp.int8))),  # type: ignore
                          lambda: state)  # type: ignore
     # fmt: on
-    # 小さいbidを非合法手にする
+    # pass, double, redouble, 小さいbidを一旦全て非合法手にする
     mask = jnp.arange(38) < action + 1
     return state.replace(  # type: ignore
         legal_action_mask=jnp.where(
             mask, jnp.bool_(0), state.legal_action_mask
         ),
         _call_x=jnp.bool_(False),
         _call_xx=jnp.bool_(False),
```

### Comparing `pgx-0.7.4/pgx/chess.py` & `pgx-0.8.0/pgx/chess.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,22 +16,29 @@
 import jax.numpy as jnp
 
 import pgx.v1 as v1
 from pgx._src.chess_utils import (  # type: ignore
     BETWEEN,
     CAN_MOVE,
     CAN_MOVE_ANY,
-    HASH_TABLE,
     INIT_LEGAL_ACTION_MASK,
     INIT_POSSIBLE_PIECE_POSITIONS,
     PLANE_MAP,
     TO_MAP,
+    ZOBRIST_BOARD,
+    ZOBRIST_CASTLING_KING,
+    ZOBRIST_CASTLING_QUEEN,
+    ZOBRIST_EN_PASSANT,
+    ZOBRIST_SIDE,
 )
 from pgx._src.struct import dataclass
 
+INIT_ZOBRIST_HASH = jnp.uint32([1172276016, 1112364556])
+MAX_TERMINATION_STEPS = 512  # from AZ paper
+
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 EMPTY = jnp.int8(0)
 PAWN = jnp.int8(1)
 KNIGHT = jnp.int8(2)
 BISHOP = jnp.int8(3)
@@ -120,19 +127,22 @@
     # (curr, opp) Flips every turn
     _can_castle_queen_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
     _can_castle_king_side: jnp.ndarray = jnp.ones(2, dtype=jnp.bool_)
     _en_passant: jnp.ndarray = jnp.int8(-1)  # En passant target. Flips.
     # # of moves since the last piece capture or pawn move
     _halfmove_count: jnp.ndarray = jnp.int32(0)
     _fullmove_count: jnp.ndarray = jnp.int32(1)  # increase every black move
-    _zobrist_hash: jnp.ndarray = jnp.uint32([1429435994, 901419182])
+    _zobrist_hash: jnp.ndarray = INIT_ZOBRIST_HASH
     _hash_history: jnp.ndarray = (
-        jnp.zeros((1001, 2), dtype=jnp.uint32)
+        jnp.zeros((MAX_TERMINATION_STEPS + 1, 2), dtype=jnp.uint32)
         .at[0]
-        .set(jnp.uint32([1429435994, 901419182]))
+        .set(INIT_ZOBRIST_HASH)
+    )
+    _board_history: jnp.ndarray = (
+        jnp.zeros((8, 64), dtype=jnp.int8).at[0, :].set(INIT_BOARD)
     )
     # index to possible piece positions for speeding up. Flips every turn.
     _possible_piece_positions: jnp.ndarray = INIT_POSSIBLE_PIECE_POSITIONS
 
     @property
     def env_id(self) -> v1.EnvId:
         return "chess"
@@ -182,71 +192,88 @@
         # plane = jax.lax.select(self.underpromotion >= 0, ..., plane)
         return jnp.int32(self.from_) * 73 + jnp.int32(plane)
 
 
 class Chess(v1.Env):
     def __init__(self):
         super().__init__()
-        # AlphaZero paper does not mention the number of max termination steps
-        # but we believe 1000 is large enough for Chess.
-        self.max_termination_steps = 1000
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         return state
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         state = _step(state, action)
         state = jax.lax.cond(
-            (0 <= self.max_termination_steps)
-            & (self.max_termination_steps <= state._step_count),
+            (MAX_TERMINATION_STEPS <= state._step_count),
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
-        return _observe(state)
+        return _observe(state, player_id)
 
     @property
     def id(self) -> v1.EnvId:
         return "chess"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _step(state: State, action: jnp.ndarray):
     a = Action._from_label(action)
     state = _update_zobrist_hash(state, a)
+
+    hash_ = state._zobrist_hash
+    hash_ ^= _hash_castling_en_passant(state)
+
     state = _apply_move(state, a)
     state = _flip(state)
+
+    hash_ ^= _hash_castling_en_passant(state)
+    state = state.replace(_zobrist_hash=hash_)  # type: ignore
+
+    state = _update_history(state)
     state = state.replace(  # type: ignore
         legal_action_mask=_legal_action_mask(state)
     )
     state = _check_termination(state)
     return state
 
 
+def _update_history(state: State):
+    # board history
+    board_history = jnp.roll(state._board_history, 64)
+    board_history = board_history.at[0].set(state._board)
+    state = state.replace(_board_history=board_history)  # type:ignore
+    # hash hist
+    hash_hist = jnp.roll(state._hash_history, 2)
+    hash_hist = hash_hist.at[0].set(state._zobrist_hash)
+    state = state.replace(_hash_history=hash_hist)  # type: ignore
+    return state
+
+
 def _check_termination(state: State):
     has_legal_action = state.legal_action_mask.any()
-    rep = (state._hash_history == state._zobrist_hash).any(axis=1).sum() - 1
     terminated = ~has_legal_action
     terminated |= state._halfmove_count >= 100
     terminated |= has_insufficient_pieces(state)
+    rep = (state._hash_history == state._zobrist_hash).all(axis=1).sum() - 1
     terminated |= rep >= 2
 
     is_checkmate = (~has_legal_action) & _is_checking(_flip(state))
     # fmt: off
     reward = jax.lax.select(
         is_checkmate,
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
@@ -418,14 +445,17 @@
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
         _board=-jnp.flip(state._board.reshape(8, 8), axis=1).flatten(),
         _turn=(state._turn + 1) % 2,
         _en_passant=_flip_pos(state._en_passant),
         _can_castle_queen_side=state._can_castle_queen_side[::-1],
         _can_castle_king_side=state._can_castle_king_side[::-1],
+        _board_history=-jnp.flip(
+            state._board_history.reshape(-1, 8, 8), axis=-1
+        ).reshape(-1, 64),
         _possible_piece_positions=state._possible_piece_positions[::-1],
     )
 
 
 def _legal_action_mask(state):
     def is_legal(a: Action):
         ok = _is_pseudo_legal(state, a)
@@ -593,107 +623,137 @@
     )
     opp_pos = jnp.nonzero(_flip(state)._board > 0, size=16, fill_value=-1)[
         0
     ].astype(jnp.int8)
     return jnp.vstack((my_pos, opp_pos))
 
 
-def _observe(state: State):
-    """Our observation design is very similar to OpenSpiel
-    except two differences:
-
-    - The board and plane index are oriented to the current agent (like AlphaZero)
-    - No plane for empty square (like AlphaZero)
-
-    There are 19 planes in total:
-
-    - [0, ... 5] 6 my pieces
-    - [6, ... 11] 6 opp pieces
-    - [12] 1 repetition count
-    - [13] 1 color
-    - [14, ..., 17] 4 castling
-    - [18] 1 no progress count
-    """
-
-    @jax.vmap
-    def is_piece(piece):
-        return _rotate((state._board == piece).reshape((8, 8))).astype(
-            jnp.float32
-        )
-
-    ONE_PLANE = jnp.ones((1, 8, 8), dtype=jnp.float32)
-
-    my_pieces = is_piece(jnp.arange(1, 7))
-    opp_pieces = is_piece(-jnp.arange(1, 7))
-    # See also https://github.com/LeelaChessZero/lc0/blob/f39ad6ceb62c186136fc80ad08c466217c485aa1/src/neural/encoder.cc#L290
-    rep = (state._hash_history == state._zobrist_hash).all(axis=1).sum() - 1
-    repetitions = ONE_PLANE * (rep >= 1)
-    color = ONE_PLANE * state._turn
-    my_queen_side_castling_right = ONE_PLANE * state._can_castle_queen_side[0]
-    my_king_side_castling_right = ONE_PLANE * state._can_castle_king_side[0]
-    opp_queen_side_castling_right = ONE_PLANE * state._can_castle_queen_side[1]
-    opp_king_side_castling_right = ONE_PLANE * state._can_castle_king_side[1]
-    no_progress_count = (
-        ONE_PLANE * state._halfmove_count.astype(jnp.float32) / 100.0
-    )
+def _observe(state: State, player_id: jnp.ndarray):
+    color = jax.lax.select(
+        state.current_player == player_id, state._turn, 1 - state._turn
+    )
+    ones = jnp.ones((1, 8, 8), dtype=jnp.float32)
+
+    state = jax.lax.cond(
+        state.current_player == player_id, lambda: state, lambda: _flip(state)
+    )
+
+    def make(i):
+        board = _rotate(state._board_history[i].reshape((8, 8)))
+
+        def piece_feat(p):
+            return (board == p).astype(jnp.float32)
+
+        my_pieces = jax.vmap(piece_feat)(jnp.arange(1, 7))
+        opp_pieces = jax.vmap(piece_feat)(-jnp.arange(1, 7))
+
+        h = state._hash_history[i, :]
+        rep = (state._hash_history == h).all(axis=1).sum() - 1
+        rep = jax.lax.select((h == 0).all(), 0, rep)
+        rep0 = ones * (rep == 0)
+        rep1 = ones * (rep >= 1)
+        return jnp.vstack([my_pieces, opp_pieces, rep0, rep1])
+
+    board_feat = jax.vmap(make)(jnp.arange(8)).reshape(-1, 8, 8)
+    color = color * ones
+    total_move_cnt = (state._step_count / MAX_TERMINATION_STEPS) * ones
+    my_queen_side_castling_right = ones * state._can_castle_queen_side[0]
+    my_king_side_castling_right = ones * state._can_castle_king_side[0]
+    opp_queen_side_castling_right = ones * state._can_castle_queen_side[1]
+    opp_king_side_castling_right = ones * state._can_castle_king_side[1]
+    no_prog_cnt = (state._halfmove_count.astype(jnp.float32) / 100.0) * ones
 
     return jnp.vstack(
         [
-            my_pieces,
-            opp_pieces,
-            repetitions,
+            board_feat,
             color,
+            total_move_cnt,
             my_queen_side_castling_right,
             my_king_side_castling_right,
             opp_queen_side_castling_right,
             opp_king_side_castling_right,
-            no_progress_count,
+            no_prog_cnt,
         ]
-    ).transpose(
-        (1, 2, 0)
-    )  # channel last
+    ).transpose((1, 2, 0))
 
 
 def _zobrist_hash(state):
     """
     >>> state = State()
     >>> _zobrist_hash(state)
-    Array([1429435994,  901419182], dtype=uint32)
+    Array([1172276016, 1112364556], dtype=uint32)
     """
+    hash_ = jnp.zeros(2, dtype=jnp.uint32)
+    hash_ = jax.lax.select(state._turn == 0, hash_, hash_ ^ ZOBRIST_SIDE)
     board = jax.lax.select(state._turn == 0, state._board, _flip(state)._board)
-    hash_ = jnp.uint32([0, 0])
 
     def xor(i, h):
         # 0, ..., 12 (white pawn, ..., black king)
         piece = board[i] + 6
-        return h ^ HASH_TABLE[i][piece]
+        return h ^ ZOBRIST_BOARD[i, piece]
 
     hash_ = jax.lax.fori_loop(0, 64, xor, hash_)
+    hash_ ^= _hash_castling_en_passant(state)
+    return hash_
+
+
+def _hash_castling_en_passant(state):
+    # we don't take care side (turn) as it's already taken into account in hash
+    zero = jnp.uint32([0, 0])
+    hash_ = zero
+    hash_ ^= jax.lax.select(
+        state._can_castle_queen_side[0], ZOBRIST_CASTLING_QUEEN[0], zero
+    )
+    hash_ ^= jax.lax.select(
+        state._can_castle_queen_side[1], ZOBRIST_CASTLING_QUEEN[1], zero
+    )
+    hash_ ^= jax.lax.select(
+        state._can_castle_king_side[0], ZOBRIST_CASTLING_KING[0], zero
+    )
+    hash_ ^= jax.lax.select(
+        state._can_castle_king_side[1], ZOBRIST_CASTLING_KING[1], zero
+    )
+    hash_ ^= ZOBRIST_EN_PASSANT[state._en_passant]
     return hash_
 
 
 def _update_zobrist_hash(state: State, action: Action):
-    """
-    >>> state = State()
-    >>> state = _update_zobrist_hash(state, Action._from_label(jnp.int32(89)))
-    >>> state._zobrist_hash
-    Array([ 511492215, 1223082425], dtype=uint32)
-    """
+    # do NOT take into account
+    #  - en passant, and
+    #  - castling
     hash_ = state._zobrist_hash
-    # fmt: off
-    board = jax.lax.select(state._turn == 0, state._board, _flip(state)._board)
-    from_ = jax.lax.select(state._turn == 0, action.from_, _flip_pos(action.from_))
+    source_piece = state._board[action.from_]
+    source_piece = jax.lax.select(
+        state._turn == 0, source_piece + 6, (source_piece * -1) + 6
+    )
+    destination_piece = state._board[action.to]
+    destination_piece = jax.lax.select(
+        state._turn == 0, destination_piece + 6, (destination_piece * -1) + 6
+    )
+    from_ = jax.lax.select(
+        state._turn == 0, action.from_, _flip_pos(action.from_)
+    )
     to = jax.lax.select(state._turn == 0, action.to, _flip_pos(action.to))
-    # fmt: on
-    piece = board[from_]
-    hash_ ^= HASH_TABLE[from_][piece]
-    hash_ ^= HASH_TABLE[to][piece]
+    hash_ ^= ZOBRIST_BOARD[from_, source_piece]  # 移動元駒を消す
+    hash_ ^= ZOBRIST_BOARD[from_, 6]  # 移動元をemptyに
+    hash_ ^= ZOBRIST_BOARD[to, destination_piece]  # 移動先の駒（empty含む）を消す
+    # underpromotion
+    source_piece = jax.lax.select(
+        action.underpromotion >= 0,
+        jax.lax.select(
+            state._turn == 0,
+            source_piece + 3 - action.underpromotion,
+            source_piece - (3 - action.underpromotion),
+        ),
+        source_piece,
+    )
+    hash_ ^= ZOBRIST_BOARD[to, source_piece]  # 移動先を動かした駒に
+    hash_ ^= ZOBRIST_SIDE
     return state.replace(  # type: ignore
         _zobrist_hash=hash_,
-        _hash_history=state._hash_history.at[state._step_count].set(hash_),
     )
 
 
 def _from_fen(fen: str):
     """Restore state from FEN
 
     >>> state = _from_fen(
@@ -773,15 +833,20 @@
     )
     state = state.replace(  # type: ignore
         _possible_piece_positions=jax.jit(_possible_piece_positions)(state)
     )
     state = state.replace(  # type: ignore
         legal_action_mask=jax.jit(_legal_action_mask)(state),
     )
+    state = state.replace(_zobrist_hash=_zobrist_hash(state))  # type: ignore
+    state = _update_history(state)
     state = jax.jit(_check_termination)(state)
+    state = state.replace(  # type: ignore
+        observation=jax.jit(_observe)(state, state.current_player)
+    )
     return state
 
 
 def _to_fen(state: State):
     """Convert state into FEN expression.
 
     - ポーン:P ナイト:N ビショップ:B ルーク:R クイーン:Q キング:K
```

### Comparing `pgx-0.7.4/pgx/connect_four.py` & `pgx-0.8.0/pgx/connect_four.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "connect_four"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _make_win_cache():
```

### Comparing `pgx-0.7.4/pgx/experimental/bridge_bidding.py` & `pgx-0.8.0/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/experimental/gym.py` & `pgx-0.8.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/experimental/pettingzoo.py` & `pgx-0.8.0/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/experimental/visualize.py` & `pgx-0.8.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/go.py` & `pgx-0.8.0/pgx/go.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return f"go_{int(self.size)}x{int(self.size)}"  # type: ignore
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _observe(state: State, player_id, size, history_length):
@@ -138,28 +138,31 @@
         however, it also describes as
 
           > the colour feature C is necessary because the komi is not observable.
 
         So, we use player_id's color to let the agent komi information.
         As long as it's called when state.current_player == player_id, this doesn't matter.
     """
+    my_turn = jax.lax.select(
+        player_id == state.current_player, state._turn, 1 - state._turn
+    )
     current_player_color = _my_color(state)  # -1 or 1
     my_color, opp_color = jax.lax.cond(
         player_id == state.current_player,
         lambda: (current_player_color, -1 * current_player_color),
         lambda: (-1 * current_player_color, current_player_color),
     )
 
     @jax.vmap
     def _make(i):
         color = jnp.int8([1, -1])[i % 2] * my_color
         return state._board_history[i // 2] == color
 
     log = _make(jnp.arange(history_length * 2))
-    color = jnp.full_like(log[0], my_color == 1)  # black=1, white=0
+    color = jnp.full_like(log[0], my_turn)  # black=0, white=1
 
     return jnp.vstack([log, color]).transpose().reshape((size, size, -1))
 
 
 def _init(key: jax.random.KeyArray, size: int, komi: float = 7.5) -> State:
     black_player = jnp.int8(jax.random.bernoulli(key))
     current_player = black_player
```

### Comparing `pgx-0.7.4/pgx/hex.py` & `pgx-0.8.0/pgx/hex.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((11, 11, 2), dtype=jnp.bool_)
     rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
-    legal_action_mask: jnp.ndarray = jnp.ones(11 * 11 + 1, dtype=jnp.bool_)
+    legal_action_mask: jnp.ndarray = (
+        jnp.ones(11 * 11 + 1, dtype=jnp.bool_).at[-1].set(FALSE)
+    )
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Hex specific ---
     _size: jnp.ndarray = jnp.int8(11)
     # 0(black), 1(white)
     _turn: jnp.ndarray = jnp.int8(0)
     # 11x11 board
@@ -77,15 +79,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "hex"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _init(rng: jax.random.KeyArray, size: int) -> State:
@@ -153,19 +155,24 @@
         player_id == state.current_player,
         state._board.reshape((size, size)),
         -state._board.reshape((size, size)),
     )
 
     my_board = board * 1 > 0
     opp_board = board * -1 > 0
-    my_color = jax.lax.select(
+    ones = jnp.ones_like(my_board)
+    color = jax.lax.select(
         player_id == state.current_player, state._turn, 1 - state._turn
-    ) * jnp.ones_like(my_board)
+    )
+    color = color * ones
+    can_swap = state.legal_action_mask[-1] * ones
 
-    return jnp.stack([my_board, opp_board, my_color], 2, dtype=jnp.bool_)
+    return jnp.stack(
+        [my_board, opp_board, color, can_swap], 2, dtype=jnp.bool_
+    )
 
 
 def _neighbour(xy, size):
     """
         (x,y-1)   (x+1,y-1)
     (x-1,y)    (x,y)    (x+1,y)
        (x-1,y+1)   (x,y+1)
```

### Comparing `pgx-0.7.4/pgx/kuhn_poker.py` & `pgx-0.8.0/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/leduc_holdem.py` & `pgx-0.8.0/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/minatar/asterix.py` & `pgx-0.8.0/pgx/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/minatar/breakout.py` & `pgx-0.8.0/pgx/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/minatar/freeway.py` & `pgx-0.8.0/pgx/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/minatar/seaquest.py` & `pgx-0.8.0/pgx/minatar/seaquest.py`

 * *Files 5% similar despite different names*

```diff
@@ -300,16 +300,15 @@
         rewards=r[jnp.newaxis],
         terminated=terminal,
     )
     return state
 
 
 def find_ix(arr):
-    ix = lax.while_loop(lambda i: arr[i][0] != -1, lambda i: i + 1, 0)
-    return ix
+    return (arr[:, 0] == -1).argmax()
 
 
 def _resolve_action(action, shot_timer, f_bullets, sub_x, sub_y, sub_or):
     f_bullets, shot_timer = lax.cond(
         (action == 5) & (shot_timer == 0),
         lambda: (
             f_bullets.at[find_ix(f_bullets)].set(
@@ -335,19 +334,22 @@
     sub_y = lax.cond(
         action == 4, lambda: lax.min(jnp.int32(8), sub_y + 1), lambda: sub_y
     )
     return f_bullets, shot_timer, sub_x, sub_y, sub_or
 
 
 def _update_by_f_bullets_hit(j, _f_bullets, e):
-    k = lax.while_loop(
-        lambda i: ~_is_hit(_f_bullets[j], e[i, 0], e[i, 1]) & (i < 25),
-        lambda i: i + 1,
-        0,
-    )
+    is_hit = (_f_bullets[j, 0] == e[:, 0]) & (_f_bullets[j, 1] == e[:, 1])
+    k = jnp.argmax(is_hit)
+    k = jax.lax.select(jnp.sum(is_hit) == 0, 25, k)
+    # k = lax.while_loop(
+    #     lambda i: ~hit[i] & (i < 25),
+    #     lambda i: i + 1,
+    #     0,
+    # )
     _f_bullets, e, removed = lax.cond(
         k < 25,
         lambda: (_remove_i(_f_bullets, j), _remove_i(e, k), TRUE),
         lambda: (_f_bullets, e, FALSE),
     )
     return _f_bullets, e, removed
 
@@ -526,19 +528,17 @@
         0, 25, _update_each, (f_bullets, e_subs, e_bullets, terminal, r)
     )
 
     return f_bullets, e_subs, e_bullets, terminal, r
 
 
 def _remove_i(arr, i):
-    N = arr.shape[0]
-    arr = lax.fori_loop(
-        i, N - 1, lambda j, _arr: _arr.at[j].set(arr[j + 1]), arr
-    )
-    return arr
+    mask = jnp.tile(jnp.arange(arr.shape[0]) < i, (arr.shape[1], 1)).T
+    rolled = jnp.roll(arr, -1, axis=0)
+    return jnp.where(mask, arr, rolled).at[-1, :].set(-1)
 
 
 def _remove_out_of_bound(arr, ix):
     arr = lax.fori_loop(
         0,
         ix,
         lambda i, a: lax.cond(
@@ -558,49 +558,57 @@
         ),
         arr,
     )
     return arr
 
 
 def _step_obj(arr, ix):
-    arr = lax.fori_loop(
-        0,
-        ix,
-        lambda i, a: a.at[i, 0].add(lax.cond(a[i, 2], lambda: 1, lambda: -1)),
+    arr_p = arr.at[:, 0].add(1)
+    arr_m = arr.at[:, 0].add(-1)
+    arr_2 = jnp.where(
+        jnp.tile(arr[:, 2], reps=(arr.shape[1], 1)).T, arr_p, arr_m
+    )
+    arr = jnp.where(
+        jnp.tile(jnp.arange(arr.shape[0]) < ix, reps=(arr.shape[1], 1)).T,
+        arr_2,
         arr,
     )
+    # arr = lax.fori_loop(
+    #     0,
+    #     ix,
+    #     lambda i, a: a.at[i, 0].add(lax.cond(a[i, 2], lambda: 1, lambda: -1)),
+    #     arr,
+    # )
     return arr
 
 
 def _hit(arr, ix, x, y):
-    return lax.fori_loop(
-        0,
-        ix,
-        lambda i, t: lax.cond(
-            (arr[i][0] == x) & (arr[i][1] == y), lambda: TRUE, lambda: t
-        ),
-        FALSE,
-    )
+    return (
+        (arr[:, 0] == x) & (arr[:, 1] == y) & (jnp.arange(arr.shape[0]) < ix)
+    ).any()
 
 
 def _update_enemy_bullets(e_bullets, sub_x, sub_y, terminal):
     ix = find_ix(e_bullets)
     terminal |= _hit(e_bullets, ix, sub_x, sub_y)
     e_bullets = _step_obj(e_bullets, ix)
     e_bullets = _remove_out_of_bound(e_bullets, ix)
     terminal |= _hit(e_bullets, ix, sub_x, sub_y)
     return e_bullets, terminal
 
 
 def _update_by_hit(j, _f_bullets, e):
-    k = lax.while_loop(
-        lambda i: ~_is_hit(e[j], _f_bullets[i, 0], _f_bullets[i, 1]) & (i < 5),
-        lambda i: i + 1,
-        0,
-    )
+    is_hit = (e[j, 0] == _f_bullets[:, 0]) & (e[j, 1] == _f_bullets[:, 1])
+    k = jnp.argmax(is_hit)
+    k = jax.lax.select(jnp.sum(is_hit) == 0, 5, k)
+    # k = lax.while_loop(
+    #     lambda i: ~_is_hit(e[j], _f_bullets[i, 0], _f_bullets[i, 1]) & (i < 5),
+    #     lambda i: i + 1,
+    #     0,
+    # )
     _f_bullets, e, removed = lax.cond(
         k < 5,
         lambda: (_remove_i(_f_bullets, k), _remove_i(e, j), TRUE),
         lambda: (_f_bullets, e, FALSE),
     )
     return _f_bullets, e, removed
 
@@ -728,119 +736,48 @@
     divers = divers.at[ix].set(
         jnp.array([x, diver_y, diver_lr, DIVER_MOVE_INTERVAL], dtype=jnp.int32)
     )
     return divers
 
 
 def _observe(state: State) -> jnp.ndarray:
-    obs = jnp.zeros((10, 10, 10), dtype=jnp.bool_)
+    obs = jnp.zeros((11, 11, 10), dtype=jnp.bool_)
     obs = obs.at[state._sub_y, state._sub_x, 0].set(TRUE)
     back_x = lax.cond(
         state._sub_or, lambda: state._sub_x - 1, lambda: state._sub_x + 1
     )
     obs = obs.at[state._sub_y, back_x, 1].set(TRUE)
     oxygen_guage = state._oxygen * 10 // MAX_OXYGEN
     # hotfix to align to original minatar
     oxygen_guage = lax.cond(
         state._oxygen < 0, lambda: jnp.int32(9), lambda: oxygen_guage
     )
-    obs = lax.fori_loop(
-        jnp.int32(0),
-        oxygen_guage,
-        lambda i, _obs: _obs.at[9, i, 7].set(TRUE),
-        obs,
-    )
-    obs = lax.fori_loop(
-        9 - state._diver_count,
-        jnp.int32(9),
-        lambda i, _obs: _obs.at[9, i, 8].set(TRUE),
-        obs,
-    )
-    obs = lax.fori_loop(
-        0,
-        5,
-        lambda i, _obs: lax.cond(
-            state._f_bullets[i][0] >= 0,
-            lambda: _obs.at[
-                state._f_bullets[i][1], state._f_bullets[i][0], 2
-            ].set(TRUE),
-            lambda: _obs,
-        ),
-        obs,
-    )
-    obs = lax.fori_loop(
-        0,
-        25,
-        lambda i, _obs: lax.cond(
-            state._e_bullets[i][0] >= 0,
-            lambda: _obs.at[
-                state._e_bullets[i][1], state._e_bullets[i][0], 4
-            ].set(TRUE),
-            lambda: _obs,
-        ),
-        obs,
+    obs = obs.at[9, :, 7].set(
+        jnp.where(jnp.arange(11) < oxygen_guage, TRUE, obs[9, :, 7])
     )
+    mask = (9 - state._diver_count <= jnp.arange(11)) & (jnp.arange(11) < 9)
+    obs = obs.at[9, :, 8].set(jnp.where(mask, TRUE, obs[9, :, 8]))
+    obs = obs.at[state._f_bullets[:, 1], state._f_bullets[:, 0], 2].set(TRUE)
+    obs = obs.at[state._e_bullets[:, 1], state._e_bullets[:, 0], 4].set(TRUE)
 
-    def set_e_fish(_obs, fish):
-        _obs = _obs.at[fish[1], fish[0], 5].set(TRUE)
-        back_x = fish[0] + jnp.array([1, -1])[fish[2]]
-        _obs = lax.cond(
-            (0 <= back_x) & (back_x <= 9),
-            lambda: _obs.at[fish[1], back_x, 3].set(TRUE),
-            lambda: _obs,
-        )
-        return _obs
-
-    obs = lax.fori_loop(
-        0,
-        25,
-        lambda i, _obs: lax.cond(
-            state._e_fish[i][0] >= 0,
-            lambda: set_e_fish(_obs, state._e_fish[i]),
-            lambda: _obs,
-        ),
-        obs,
+    obs = obs.at[state._e_fish[:, 1], state._e_fish[:, 0], 5].set(TRUE)
+    back_x = (
+        state._e_fish[:, 0]
+        + jnp.array([1, -1], dtype=jnp.int32)[state._e_fish[:, 2]]
     )
+    obs = obs.at[state._e_fish[:, 1], back_x, 3].set(TRUE)
 
-    def set_e_subs(_obs, sub):
-        _obs = _obs.at[sub[1], sub[0], 6].set(TRUE)
-        back_x = sub[0] + jnp.array([1, -1], dtype=jnp.int32)[sub[2]]
-        _obs = lax.cond(
-            (0 <= back_x) & (back_x <= 9),
-            lambda: _obs.at[sub[1], back_x, 3].set(TRUE),
-            lambda: _obs,
-        )
-        return _obs
-
-    obs = lax.fori_loop(
-        0,
-        25,
-        lambda i, _obs: lax.cond(
-            state._e_subs[i][0] >= 0,
-            lambda: set_e_subs(_obs, state._e_subs[i]),
-            lambda: _obs,
-        ),
-        obs,
+    obs = obs.at[state._e_subs[:, 1], state._e_subs[:, 0], 6].set(TRUE)
+    back_x = (
+        state._e_subs[:, 0]
+        + jnp.array([1, -1], dtype=jnp.int32)[state._e_subs[:, 2]]
     )
+    obs = obs.at[state._e_subs[:, 1], back_x, 3].set(TRUE)
 
-    def set_divers(_obs, diver):
-        _obs = _obs.at[diver[1], diver[0], 9].set(TRUE)
-        back_x = diver[0] + jnp.array([1, -1], dtype=jnp.int32)[diver[2]]
-        _obs = lax.cond(
-            (back_x >= 0) & (back_x <= 9),
-            lambda: _obs.at[diver[1], back_x, 3].set(TRUE),
-            lambda: _obs,
-        )
-        return _obs
-
-    obs = lax.fori_loop(
-        0,
-        5,
-        lambda i, _obs: lax.cond(
-            state._divers[i][0] >= 0,
-            lambda: set_divers(_obs, state._divers[i]),
-            lambda: _obs,
-        ),
-        obs,
+    obs = obs.at[state._divers[:, 1], state._divers[:, 0], 9].set(TRUE)
+    back_x = (
+        state._divers[:, 0]
+        + jnp.array([1, -1], dtype=jnp.int32)[state._divers[:, 2]]
     )
+    obs = obs.at[state._divers[:, 1], back_x, 3].set(TRUE)
 
-    return obs
+    return obs[:10, :10, :]
```

### Comparing `pgx-0.7.4/pgx/minatar/space_invaders.py` & `pgx-0.8.0/pgx/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/minatar/utils.py` & `pgx-0.8.0/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/othello.py` & `pgx-0.8.0/pgx/othello.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "othello"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 # fmt:off
```

### Comparing `pgx-0.7.4/pgx/play2048.py` & `pgx-0.8.0/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/shogi.py` & `pgx-0.8.0/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     LEGAL_FROM_IDX,
     NEIGHBOUR_IX,
     _from_sfen,
     _to_sfen,
 )
 from pgx._src.struct import dataclass
 
+MAX_TERMINATION_STEPS = 512  # From AZ paper
+
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 EMPTY = jnp.int8(-1)  # 空白
 PAWN = jnp.int8(0)  # 歩
 LANCE = jnp.int8(1)  # 香
 KNIGHT = jnp.int8(2)  # 桂
@@ -111,31 +113,29 @@
 
     def _to_sfen(self):
         state = self if self._turn % 2 == 0 else _flip(self)
         return _to_sfen(state)
 
 
 class Shogi(v1.Env):
-    def __init__(self, *, max_termination_steps: int = 1000):
+    def __init__(self):
         super().__init__()
-        self.max_termination_steps = max_termination_steps
 
     def _init(self, key: jax.random.KeyArray) -> State:
         state = _init_board()
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         return state.replace(current_player=current_player)  # type: ignore
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         # Note: Assume that illegal action is already filtered by Env.step
         state = _step(state, action)
         state = jax.lax.cond(
-            (0 <= self.max_termination_steps)
-            & (self.max_termination_steps <= state._step_count),
+            (MAX_TERMINATION_STEPS <= state._step_count),
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
@@ -144,15 +144,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "shogi"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 @dataclass
@@ -643,8 +643,8 @@
         my_effect_sum_feat.reshape(3, 9, 9),
         opp_piece_feat.reshape(14, 9, 9),
         opp_effect_feat.reshape(14, 9, 9),
         opp_effect_sum_feat.reshape(3, 9, 9),
     ]
     feat2 = my_hand_feat + opp_hand_feat + [checked]
     feat = jnp.vstack(feat1 + feat2)
-    return feat
+    return jnp.rot90(feat.transpose((1, 2, 0)), k=3)
```

### Comparing `pgx-0.7.4/pgx/sparrow_mahjong.py` & `pgx-0.8.0/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/pgx/tic_tac_toe.py` & `pgx-0.8.0/pgx/tic_tac_toe.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _init(rng: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.7.4/pgx/v1.py` & `pgx-0.8.0/pgx/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 EnvId = Literal[
     "2048",
     "animal_shogi",
     "backgammon",
     "bridge_bidding",
     "chess",
     "connect_four",
+    "gardner_chess",
     "go_9x9",
     "go_19x19",
     "hex",
     "kuhn_poker",
     "leduc_holdem",
     # "mahjong",
     "minatar-asterix",
@@ -357,14 +358,18 @@
         from pgx.chess import Chess
 
         return Chess()
     elif env_id == "connect_four":
         from pgx.connect_four import ConnectFour
 
         return ConnectFour()
+    elif env_id == "gardner_chess":
+        from pgx.gardner_chess import GardnerChess
+
+        return GardnerChess()
     elif env_id == "go_9x9":
         from pgx.go import Go
 
         return Go(size=9, komi=7.5)
     elif env_id == "go_19x19":
         from pgx.go import Go
```

### Comparing `pgx-0.7.4/pgx.egg-info/PKG-INFO` & `pgx-0.8.0/pgx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.7.4
+Version: 0.8.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,21 +58,19 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not (state.terminated | state.terminated).all():
+while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
-> ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in May 2023. Opinions and comments are more than welcome!
-
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
@@ -106,31 +104,32 @@
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
 |<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
-|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `beta` | *Animal-themed child-friendly shogi.* |
+|<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
 |<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
-|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `beta` | *Checkmate opponent's king to win.* |
-|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `beta` | *Connect discs, win with four.* |
-|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `beta` | *Strategically place stones, claim territory.* |
-|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `beta` | *Connect opposite sides, block opponent.* |
+|<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
+|<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
+|<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
+|<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
+|<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
 |<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
 |<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
 |<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
-|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `beta` | *Flip and conquer opponent's pieces.* |
-|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `beta` | *Japanese chess with captured pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
+|<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
 |<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
-|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `beta` | *Three in a row wins.* |
+|<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.7.4 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.8.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -27,64 +27,64 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.terminated).all():
+# vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
-â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
-change without notice. We aim to release v1.0.0 in May 2023. Opinions and
-comments are more than welcome!  ## Supported games | Backgammon | Chess |
-Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
+## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
+| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
+/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
-friendly shogi.* | |Backgammon
+main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
+shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif]| `beta` | *Checkmate opponent's king to win.* |
-|Connect_Four
+assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
+Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/connect_four_light.gif]| `beta` | *Connect discs, win with
-four.* | |Go
+main/docs/assets/connect_four_light.gif]| `v0` | *Connect discs, win with
+four.* | |Gardner_Chess
+`"gardner_chess"`|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/gardner_chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
+main/docs/assets/gardner_chess_light.gif]| `v0` | *5x5 chess variant, excluding
+castling.* | |Go
 `"go_9x9"` `"go_19x19"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
 docs/assets/go-19x19_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/go-19x19_light.gif]| `beta` | *Strategically place stones,
-claim territory.* | |Hex
+main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
+territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-hex_light.gif]| `beta` | *Connect opposite sides, block opponent.* | |Kuhn
-Poker
+hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
 bluffing game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
@@ -102,27 +102,27 @@
 docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
 dodge bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/othello_light.gif]| `beta` | *Flip and conquer opponent's pieces.* |
+assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_light.gif] | `beta` | *Japanese chess with captured pieces.* |
+assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
 pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/tic_tac_toe_light.gif]| `beta` | *Three in a row wins.* | -
+main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
 (classic) board game suits: - [RobertTLange/gymnax](https://github.com/
 RobertTLange/gymnax): JAX implementation of popular RL environments ([classic
 control](https://gymnasium.farama.org/environments/classic_control), [bsuite]
 (https://github.com/deepmind/bsuite), MinAtar, etc) and meta RL tasks -
```

### Comparing `pgx-0.7.4/pgx.egg-info/SOURCES.txt` & `pgx-0.8.0/pgx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 pgx/__init__.py
 pgx/animal_shogi.py
 pgx/backgammon.py
 pgx/bridge_bidding.py
 pgx/chess.py
 pgx/connect_four.py
+pgx/gardner_chess.py
 pgx/go.py
 pgx/hex.py
 pgx/kuhn_poker.py
 pgx/leduc_holdem.py
 pgx/othello.py
 pgx/play2048.py
 pgx/shogi.py
@@ -29,25 +30,27 @@
 pgx/_mahjong/_meld.py
 pgx/_mahjong/_shanten.py
 pgx/_mahjong/_yaku.py
 pgx/_mahjong/cache/__init__.py
 pgx/_src/__init__.py
 pgx/_src/api_test.py
 pgx/_src/chess_utils.py
+pgx/_src/gardner_chess_utils.py
 pgx/_src/shogi_utils.py
 pgx/_src/struct.py
 pgx/_src/visualizer.py
 pgx/_src/assets/between.npy
 pgx/_src/assets/can_move.npy
 pgx/_src/dwg/__init__.py
 pgx/_src/dwg/animalshogi.py
 pgx/_src/dwg/backgammon.py
 pgx/_src/dwg/bridge_bidding.py
 pgx/_src/dwg/chess.py
 pgx/_src/dwg/connect_four.py
+pgx/_src/dwg/gardner_chess.py
 pgx/_src/dwg/go.py
 pgx/_src/dwg/hex.py
 pgx/_src/dwg/kuhn_poker.py
 pgx/_src/dwg/leduc_holdem.py
 pgx/_src/dwg/othello.py
 pgx/_src/dwg/play2048.py
 pgx/_src/dwg/shogi.py
@@ -110,14 +113,15 @@
 tests/test_asterix.py
 tests/test_backgammon.py
 tests/test_breakout.py
 tests/test_bridge_bidding.py
 tests/test_chess.py
 tests/test_connect_four.py
 tests/test_freeway.py
+tests/test_gardner_chess.py
 tests/test_go.py
 tests/test_hex.py
 tests/test_kuhn_poker.py
 tests/test_leduc_holdem.py
 tests/test_mahjong.py
 tests/test_othello.py
 tests/test_play2048.py
```

### Comparing `pgx-0.7.4/setup.py` & `pgx-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.7.4",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
```

### Comparing `pgx-0.7.4/tests/minatar_utils.py` & `pgx-0.8.0/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_animal_shogi.py` & `pgx-0.8.0/tests/test_animal_shogi.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     assert state._hand[0, 0] == 1
     assert state._hand[1, 0] == 0
     assert state._hand.sum() == 1
 
 
 def test_observe():
     state = init(jax.random.PRNGKey(0))
-    assert state.observation.shape == (4, 3, 22)
+    assert state.observation.shape == (4, 3, 194)
 
     # my pawn
     expected = jnp.bool_(
         [[False, False, False],
          [False, False, False],
          [False, True,  False],
          [False, False, False]]
@@ -62,76 +62,86 @@
     # my bishop
     expected = jnp.bool_(
         [[False, False, False],
          [False, False, False],
          [False, False, False],
          [True , False, False]]
     )
+    print(state._board_history[0])
     assert (state.observation[:, :, 1] == expected).all()
 
     # opp king
     expected = jnp.bool_(
         [[False, True,  False],
          [False, False, False],
          [False, False, False],
          [False, False, False]]
     )
     assert (state.observation[:, :, 8] == expected).all()
 
-    state = State(
-        _board=jnp.int8([
-             8, -1, -1, -1,
-            -1, -1, -1,  3,
-            -1, -1, -1,  0]),
-        _hand=jnp.int8([[2, 0, 0], [0, 1, 0]])
-    )
-    state = state.replace(observation=_observe(state, state.current_player))
+    state = init(jax.random.PRNGKey(0))
+    state.save_svg("tests/assets/animal_shogi/test_obs_000.svg")
+    state = step(state, 6 + 12 * 3)
+    state.save_svg("tests/assets/animal_shogi/test_obs_001.svg")
+    # my pawn
     expected = jnp.bool_(
         [[False, False, False],
          [False, False, False],
-         [False, False, False],
-         [True, False, False]]
+         [False, False,  False],
+         [False, False, False]]
     )
     assert (state.observation[:, :, 0] == expected).all()
-    # hand
-    expected = jnp.bool_([True , True,
-                          False, False,
-                          False, False,
-                          False, False,
-                          True , False,
-                          False, False])
-    assert (state.observation[0, 0, 10:] == expected).all()
-
+    # opp pawn
+    expected = jnp.bool_(
+        [[False, False, False],
+         [False, False, False],
+         [False, True,  False],
+         [False, False, False]]
+    )
+    assert (state.observation[:, :, 5] == expected).all()
+    assert (state.observation[:, :, 10 + 6] == 1).all()  # opp captured pawn
+    state = step(state, 7 + 12 * 3)
+    state.save_svg("tests/assets/animal_shogi/test_obs_002.svg")
+    # opp king
+    # opp pawn in hand
+    # my pawn in hand @ 1-step before
+    # opp pawn in hand @ 1-step before
 
 def test_repetition():
     state = init(jax.random.PRNGKey(0))
     # first
     visualize(state, "tests/assets/animal_shogi/test_repetition_000.svg")
     assert not state.terminated
     assert state._turn == 0
+    assert (state.observation[:, :, 22] == 1).all()  # rep = 0
 
     state = step(state, 3 * 12 + 3)  # Up Rook
     visualize(state, "tests/assets/animal_shogi/test_repetition_002.svg")
     assert not state.terminated
     assert state._turn == 1
+    assert (state.observation[:, :, 22] == 1).all()  # rep = 0
 
     state = step(state, 3 * 12 + 3)  # Up Rook
     visualize(state, "tests/assets/animal_shogi/test_repetition_003.svg")
     assert not state.terminated
     assert state._turn == 0
+    assert (state.observation[:, :, 22] == 1).all()  # rep = 0
 
     state = step(state, 4 * 12 + 2)  # Down Rook
     visualize(state, "tests/assets/animal_shogi/test_repetition_004.svg")
     assert not state.terminated
     assert state._turn == 1
+    assert (state.observation[:, :, 22] == 1).all()  # rep = 0
 
     state = step(state, 4 * 12 + 2)  # Down Rook
     # second
     visualize(state, "tests/assets/animal_shogi/test_repetition_005.svg")
     assert not state.terminated
+    assert (state.observation[:, :, 22] == 0).all()  # rep = 0
+    assert (state.observation[:, :, 23] == 1).all()  # rep = 1
     assert state._turn == 0
 
     # same repetition
     state1 = step(state, 3 * 12 + 3)  # Up Rook
     assert not state1.terminated
     state1 = step(state1, 3 * 12 + 3)  # Up Rook
     assert not state1.terminated
```

### Comparing `pgx-0.7.4/tests/test_asterix.py` & `pgx-0.8.0/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_backgammon.py` & `pgx-0.8.0/tests/test_backgammon.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     dice: jnp.ndarray,
     playable_dice: jnp.ndarray,
     played_dice_num: jnp.ndarray,
     legal_action_mask=jnp.zeros(6 * 26 + 6, dtype=jnp.bool_),
 ):
     return State(
         current_player=current_player,
-        _rng=rng,
+        _rng_key=rng,
         _board=board,
         _turn=turn,
         _dice=dice,
         _playable_dice=playable_dice,
         _played_dice_num=played_dice_num,
         legal_action_mask=legal_action_mask,
     )
@@ -310,14 +310,28 @@
         played_dice_num=jnp.int16(0),
     )
     expected_obs = jnp.concatenate(
         (board, jnp.array([1, 1, 0, 0, 0, 0])), axis=None
     )
     assert (observe(state, jnp.int8(1)) == expected_obs).all()
 
+    state = make_test_state(
+        current_player=jnp.int8(1),
+        rng=rng,
+        board=board,
+        turn=jnp.int8(1),
+        dice=jnp.array([0, 1], dtype=jnp.int16),
+        playable_dice=jnp.array([1, 1, 1, 1], dtype=jnp.int16),
+        played_dice_num=jnp.int16(0),
+    )
+    expected_obs = jnp.concatenate(
+        (board, jnp.array([0, 4, 0, 0, 0, 0])), axis=None
+    )
+    assert (observe(state, jnp.int8(1)) == expected_obs).all()
+
     # current_playerが黒で, playできるdiceが(2)のみの場合
     state = make_test_state(
         current_player=jnp.int8(1),
         rng=rng,
         board=board,
         turn=jnp.int8(-1),
         dice=jnp.array([0, 1], dtype=jnp.int16),
```

### Comparing `pgx-0.7.4/tests/test_breakout.py` & `pgx-0.8.0/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_bridge_bidding.py` & `pgx-0.8.0/tests/test_bridge_bidding.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,17 +22,22 @@
     _state_to_pbn,
     _to_binary,
     _value_to_dds_tricks,
     duplicate,
     init,
 )
 
-
-DDS_HASH_TABLE_PATH = os.path.join(os.path.dirname(__file__), "assets/dds_hash_table.npy")
-env = BridgeBidding(dds_hash_table_path=DDS_HASH_TABLE_PATH )
+PASS_ACTION_NUM = 0
+DOUBLE_ACTION_NUM = 1
+REDOUBLE_ACTION_NUM = 2
+BID_OFFSET_NUM = 3
+DDS_HASH_TABLE_PATH = os.path.join(
+    os.path.dirname(__file__), "assets/dds_hash_table.npy"
+)
+env = BridgeBidding(dds_hash_table_path=DDS_HASH_TABLE_PATH)
 
 init_by_key = jax.jit(env.init)
 step = jax.jit(env.step)
 observe = jax.jit(env.observe)
 
 
 def test_shuffle_players():
@@ -49,16 +54,18 @@
     state = init(key)
     assert state._last_bid == -1
     assert state._last_bidder == -1
     assert not state._call_x
     assert not state._call_xx
     assert not state._pass_num
     assert _player_position(state.current_player, state) == state._dealer
-    assert state.legal_action_mask[:-2].all()
-    assert not state.legal_action_mask[-2:].all()
+    assert state.legal_action_mask[PASS_ACTION_NUM]
+    assert not state.legal_action_mask[DOUBLE_ACTION_NUM]
+    assert not state.legal_action_mask[REDOUBLE_ACTION_NUM]
+    assert state.legal_action_mask[BID_OFFSET_NUM:].all()
 
 
 def test_duplicate():
     key = jax.random.PRNGKey(0)
     for i in range(1000):
         key, subkey = jax.random.split(key)
         init_state = init(subkey)
@@ -84,15 +91,15 @@
             == duplicated_state._shuffled_players[2]
         )
 
 
 def test_illegal_action_penalty():
     key = jax.random.PRNGKey(0)
     state = init(key)
-    state = step(state, 36)
+    state = step(state, DOUBLE_ACTION_NUM)
     print(state.rewards)
     assert jnp.all(state.rewards == jnp.array([22800, -7600, 22800, 22800]))
 
 
 def test_step():
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
@@ -100,355 +107,420 @@
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P  P
+    # fmt: off
+    actions = iter([0, 0, 0,
+                    3, 11, 1, 0,
+                    0, 2, 0, 25,
+                    26, 0, 28, 1,
+                    2, 0, 33, 0,
+                    0, 0])
+    # fmt: on
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(0),
         _vul_EW=jnp.bool_(0),
     )
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
+    legal_action_mask = legal_action_mask.at[DOUBLE_ACTION_NUM].set(False)
+    legal_action_mask = legal_action_mask.at[REDOUBLE_ACTION_NUM].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
     first_denomination_EW = jnp.full(5, -1, dtype=jnp.int8)
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
     assert state._turn == 1
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[0].set(35)
+    bidding_history = bidding_history.at[0].set(0)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == np.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
     assert state._turn == 2
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[1].set(35)
+    bidding_history = bidding_history.at[1].set(0)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
     assert state._turn == 3
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[2].set(35)
+    bidding_history = bidding_history.at[2].set(0)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 3
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 0)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, -1, -1])
 
     assert state._turn == 4
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
-    bidding_history = bidding_history.at[3].set(0)
+    bidding_history = bidding_history.at[3].set(3)
     assert jnp.all(state._bidding_history == bidding_history)
-    legal_action_mask = legal_action_mask.at[0].set(False)
-    legal_action_mask = legal_action_mask.at[36].set(True)
+    legal_action_mask = legal_action_mask.at[3].set(False)
+    legal_action_mask = legal_action_mask.at[DOUBLE_ACTION_NUM].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 0
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 8)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 5
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[4].set(8)
+    bidding_history = bidding_history.at[4].set(11)
     assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
+
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 36)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 6
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[5].set(36)
+    bidding_history = bidding_history.at[5].set(DOUBLE_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(True)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 7
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[6].set(35)
+    bidding_history = bidding_history.at[6].set(PASS_ACTION_NUM)
     assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
+    )
+
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 8
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
-    bidding_history = bidding_history.at[7].set(35)
+    bidding_history = bidding_history.at[7].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(True)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(True)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 37)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 9
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[8].set(37)
+    bidding_history = bidding_history.at[8].set(REDOUBLE_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, -1, 3, -1])
 
     assert state._turn == 10
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[9].set(35)
+    bidding_history = bidding_history.at[9].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 9, False, state.legal_action_mask
+        jnp.arange(38) <= 11, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 22)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 11
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[10].set(22)
+    bidding_history = bidding_history.at[10].set(25)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 23, False, state.legal_action_mask
+        jnp.arange(38) <= 25, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 22
     assert _player_position(state._last_bidder, state) == 3
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 23)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -456,33 +528,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 12
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
-    bidding_history = bidding_history.at[11].set(23)
+    bidding_history = bidding_history.at[11].set(26)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 24, False, state.legal_action_mask
+        jnp.arange(38) <= 26, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 23
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -490,33 +569,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 13
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[12].set(35)
+    bidding_history = bidding_history.at[12].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 24, False, state.legal_action_mask
+        jnp.arange(38) <= 26, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 23
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 25)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -524,33 +610,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 14
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[13].set(25)
+    bidding_history = bidding_history.at[13].set(28)
     assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 26, False, state.legal_action_mask
+        jnp.arange(38) <= 28, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 36)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -558,33 +651,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 15
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[14].set(36)
+    bidding_history = bidding_history.at[14].set(DOUBLE_ACTION_NUM)
     assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 26, False, state.legal_action_mask
+        jnp.arange(38) <= 28, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(True)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(True)
     assert np.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert not state._call_xx
     assert np.all(state._first_denomination_NS == first_denomination_NS)
     assert np.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert np.all(state.rewards == np.zeros(4))
 
-    state = step(state, 37)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -593,33 +693,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 16
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
-    bidding_history = bidding_history.at[15].set(37)
+    bidding_history = bidding_history.at[15].set(REDOUBLE_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 26, False, state.legal_action_mask
+        jnp.arange(38) <= 28, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -628,33 +735,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 17
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[16].set(35)
+    bidding_history = bidding_history.at[16].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 26, False, state.legal_action_mask
+        jnp.arange(38) <= 28, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert np.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 30)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -663,33 +777,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 18
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[17].set(30)
+    bidding_history = bidding_history.at[17].set(33)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 31, False, state.legal_action_mask
+        jnp.arange(38) <= 33, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -698,33 +819,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 19
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[18].set(35)
+    bidding_history = bidding_history.at[18].set(PASS_ACTION_NUM)
     assert np.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 31, False, state.legal_action_mask
+        jnp.arange(38) <= 33, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(False)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -734,33 +862,40 @@
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 20
     assert state.current_player == 3
     assert _player_position(state.current_player, state) == 1
     assert not state.terminated
-    bidding_history = bidding_history.at[19].set(35)
+    bidding_history = bidding_history.at[19].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
-        jnp.arange(38) < 31, False, state.legal_action_mask
+        jnp.arange(38) <= 33, False, state.legal_action_mask
+    )
+    legal_action_mask = (
+        legal_action_mask.at[PASS_ACTION_NUM]
+        .set(True)
+        .at[DOUBLE_ACTION_NUM]
+        .set(True)
+        .at[REDOUBLE_ACTION_NUM]
+        .set(False)
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -770,23 +905,17 @@
     # Passが3回続いたので終了
     assert state.terminated == True
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state._turn == 20
     assert state.terminated
-    bidding_history = bidding_history.at[20].set(35)
+    bidding_history = bidding_history.at[20].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
-    legal_action_mask = jnp.where(
-        jnp.arange(38) < 31, False, state.legal_action_mask
-    )
-    legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
-    # legal_action_mask = legal_action_mask.at[36].set(True)
-    # legal_action_mask = legal_action_mask.at[37].set(False)s
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
@@ -800,23 +929,50 @@
     assert denomination == 0
     assert level == 7
     assert vul == 0
 
 
 def max_action_length_agent(state: State) -> int:
     if (state._last_bid == -1 and state._pass_num != 3) or (
-            state._last_bid != -1 and state._pass_num != 2
+        state._last_bid != -1 and state._pass_num != 2
     ):
-        return 35
-    elif state.legal_action_mask[36]:
-        return 36
-    elif state.legal_action_mask[37]:
-        return 37
+        return PASS_ACTION_NUM
+    elif state.legal_action_mask[DOUBLE_ACTION_NUM]:
+        return DOUBLE_ACTION_NUM
+    elif state.legal_action_mask[REDOUBLE_ACTION_NUM]:
+        return REDOUBLE_ACTION_NUM
     else:
-        return int(state._last_bid) + 1
+        return int(state._last_bid) + 1 + BID_OFFSET_NUM
+
+
+def test_max_action():
+    key = jax.random.PRNGKey(0)
+    HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
+    state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
+
+    for i in range(319):
+        if i < 318:
+            state = step(state, max_action_length_agent(state))
+            assert not state.terminated
+        else:
+            state = step(state, max_action_length_agent(state))
+            assert state.terminated
+
+
+def max_action_length_agent(state: State) -> int:
+    if (state._last_bid == -1 and state._pass_num != 3) or (
+        state._last_bid != -1 and state._pass_num != 2
+    ):
+        return PASS_ACTION_NUM
+    elif state.legal_action_mask[DOUBLE_ACTION_NUM]:
+        return DOUBLE_ACTION_NUM
+    elif state.legal_action_mask[REDOUBLE_ACTION_NUM]:
+        return REDOUBLE_ACTION_NUM
+    else:
+        return int(state._last_bid) + 1 + 3
 
 
 def test_max_action():
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
 
@@ -832,113 +988,118 @@
 def test_pass_out():
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   P
+    actions = iter([0, 0, 0, 0])
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[1], key)
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(0),
         _vul_EW=jnp.bool_(0),
     )
 
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
-    legal_action_mask = legal_action_mask.at[36].set(False)
-    legal_action_mask = legal_action_mask.at[37].set(False)
+    legal_action_mask = legal_action_mask.at[DOUBLE_ACTION_NUM].set(False)
+    legal_action_mask = legal_action_mask.at[REDOUBLE_ACTION_NUM].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
     first_denomination_EW = jnp.full(5, -1, dtype=jnp.int8)
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
     assert state._turn == 1
     assert state.current_player == 1
     assert _player_position(state.current_player, state) == 2
     assert not state.terminated
-    bidding_history = bidding_history.at[0].set(35)
+    bidding_history = bidding_history.at[0].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
     assert state._turn == 2
     assert state.current_player == 2
     assert _player_position(state.current_player, state) == 3
     assert not state.terminated
-    bidding_history = bidding_history.at[1].set(35)
+    bidding_history = bidding_history.at[1].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
     assert state._turn == 3
     assert state.current_player == 0
     assert _player_position(state.current_player, state) == 0
     assert not state.terminated
-    bidding_history = bidding_history.at[2].set(35)
+    bidding_history = bidding_history.at[2].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 3
     assert jnp.all(state.rewards == jnp.zeros(4))
 
-    state = step(state, 35)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   P
 
     assert state.terminated == True
     assert state._turn == 3
-    bidding_history = bidding_history.at[3].set(35)
+    bidding_history = bidding_history.at[3].set(PASS_ACTION_NUM)
     assert jnp.all(state._bidding_history == bidding_history)
     assert jnp.all(state.legal_action_mask == jnp.ones(38, dtype=jnp.bool_))
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
@@ -946,108 +1107,119 @@
     assert state._pass_num == 4
     assert jnp.all(state.rewards == jnp.zeros(4))
 
 
 def test_observe():
     # test init_obs
     # hand
+
+    # player_id: 0 = N, 1 = S, 2 = W, 3 = E
     # hand: N:J92.J76.K72.9432 AKQ6.84.J863.T65 87543.KQ9532..K7 T.AT.AQT954.AQJ8
     player0_hand = (
         jnp.zeros(52, dtype=jnp.bool_)
-        .at[jnp.array([1, 8, 10, 18, 19, 23, 27, 32, 38, 40, 41, 42, 47])]
+        .at[jnp.array([0, 1, 3, 4, 8, 18, 21, 22, 28, 31, 38, 39, 45])]
         .set(True)
     )
     player1_hand = (
         jnp.zeros(52, dtype=jnp.bool_)
-        .at[jnp.array([2, 3, 4, 6, 7, 14, 15, 17, 21, 24, 25, 45, 51])]
+        .at[jnp.array([2, 6, 7, 11, 14, 15, 20, 23, 27, 30, 42, 44, 46])]
         .set(True)
     )
     player2_hand = (
         jnp.zeros(52, dtype=jnp.bool_)
-        .at[jnp.array([9, 13, 22, 26, 29, 30, 34, 35, 37, 39, 46, 49, 50])]
+        .at[jnp.array([9, 13, 24, 29, 33, 34, 35, 36, 40, 41, 48, 49, 50])]
         .set(True)
     )
     player3_hand = (
         jnp.zeros(52, dtype=jnp.bool_)
-        .at[jnp.array([0, 5, 11, 12, 16, 20, 28, 31, 33, 36, 43, 44, 48])]
+        .at[jnp.array([5, 10, 12, 16, 17, 19, 25, 26, 32, 37, 43, 47, 51])]
         .set(True)
     )
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
     state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(0),
         _vul_EW=jnp.bool_(0),
     )
 
-    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+    init_obs = jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player0_hand))
+    init_obs = init_obs.at[0].set(True).at[2].set(True)
     obs = observe(state, 0)
-    print(_state_to_pbn(state))
     assert jnp.all(obs == init_obs)
 
-    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player1_hand))
+    init_obs = jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player1_hand))
+    init_obs = init_obs.at[0].set(True).at[2].set(True)
     obs = observe(state, 1)
     assert jnp.all(obs == init_obs)
 
-    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player2_hand))
+    init_obs = jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player2_hand))
+    init_obs = init_obs.at[0].set(True).at[2].set(True)
     obs = observe(state, 2)
     assert jnp.all(obs == init_obs)
 
-    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player3_hand))
+    init_obs = jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player3_hand))
+    init_obs = init_obs.at[0].set(True).at[2].set(True)
     obs = observe(state, 3)
     assert jnp.all(obs == init_obs)
 
     # vul
+    # dealer team: EW
+    # non dealer team: NS
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(1),
         _vul_EW=jnp.bool_(0),
     )
     init_obs = (
-        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+        jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player0_hand))
         .at[0]
         .set(True)
+        .at[3]
+        .set(True)
     )
     obs = observe(state, 0)
     assert jnp.all(obs == init_obs)
 
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(0),
         _vul_EW=jnp.bool_(1),
     )
     init_obs = (
-        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+        jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player0_hand))
         .at[1]
         .set(True)
+        .at[2]
+        .set(True)
     )
     obs = observe(state, 0)
 
     assert jnp.all(obs == init_obs)
 
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(1),
         _vul_EW=jnp.bool_(1),
     )
     init_obs = (
-        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
-        .at[0]
-        .set(True)
+        jnp.concatenate((jnp.zeros(428, dtype=jnp.bool_), player0_hand))
         .at[1]
         .set(True)
+        .at[3]
+        .set(True)
     )
     obs = observe(state, 0)
     assert jnp.all(obs == init_obs)
 
     # bid_history
     #
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
@@ -1057,309 +1229,610 @@
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P  P
     #
-
-    vul_history = jnp.zeros(426, dtype=jnp.bool_)
+    # fmt: off
+    actions = iter([0, 0, 0,
+                    3, 11, 1, 0,
+                    0, 2, 0, 25,
+                    26, 0, 28, 1,
+                    2, 0, 33, 0,
+                    0, 0])
+    # fmt: on
+    vul = jnp.zeros(4, dtype=jnp.bool_).at[0].set(True).at[2].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
 
     state = state.replace(
         _dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         _shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         _vul_NS=jnp.bool_(0),
         _vul_EW=jnp.bool_(0),
     )
-
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  ?
 
-    vul_history = vul_history.at[3].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[3].set(True)
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    correct_obs = jnp.concatenate((vul, history, player1_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  ?
 
-    vul_history = vul_history.at[4].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[2].set(True).at[3].set(True)
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    correct_obs = jnp.concatenate((vul, history, player2_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   ?
 
-    vul_history = vul_history.at[5].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[1].set(True).at[2].set(True).at[3].set(True)
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    correct_obs = jnp.concatenate((vul, history, player0_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 0)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C  ?
 
-    vul_history = vul_history.at[6].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[2].set(True)
+    history = history.at[4 + 3].set(True)
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    correct_obs = jnp.concatenate((vul, history, player3_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 8)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  ?
-
-    vul_history = vul_history.at[49].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[3].set(True)
+    history = history.at[4 + 2].set(True).at[4 + (11 - 3) * 12 + 3].set(True)
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    correct_obs = jnp.concatenate((vul, history, player1_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 36)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  ?
 
-    vul_history = vul_history.at[2 + 144 + 35 * 2 + 8].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    correct_obs = jnp.concatenate((vul, history, player2_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   ?
-
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[1].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 2]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    correct_obs = jnp.concatenate((vul, history, player0_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P  ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[2].set(True)
+    history = (
+        history.at[4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 1]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    correct_obs = jnp.concatenate((vul, history, player3_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 37)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  ?
 
-    vul_history = vul_history.at[2 + 284 + 35 + 8].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    correct_obs = jnp.concatenate((vul, history, player1_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P  ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 2]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    correct_obs = jnp.concatenate((vul, history, player2_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 22)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #   ?
 
-    vul_history = vul_history.at[2 + 4 + 35 * 3 + 22].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[1].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 1]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    correct_obs = jnp.concatenate((vul, history, player0_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 23)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  ?
 
-    vul_history = vul_history.at[2 + 4 + 35 * 0 + 23].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[2].set(True)
+    history = (
+        history.at[4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 0]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    correct_obs = jnp.concatenate((vul, history, player3_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P  ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 3]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 2]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    correct_obs = jnp.concatenate((vul, history, player1_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 25)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  ?
 
-    vul_history = vul_history.at[2 + 4 + 35 * 2 + 25].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 2]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    correct_obs = jnp.concatenate((vul, history, player2_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 36)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #   ?
 
-    vul_history = vul_history.at[2 + 144 + 35 * 3 + 25].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[1].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 1]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    correct_obs = jnp.concatenate((vul, history, player0_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 37)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  ?
 
-    vul_history = vul_history.at[2 + 284 + 35 * 0 + 25].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[2].set(True)
+    history = (
+        history.at[4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 0]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 2]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 8 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    correct_obs = jnp.concatenate((vul, history, player3_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P  ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 3]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 1]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 8 + 2]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    correct_obs = jnp.concatenate((vul, history, player1_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 30)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  ?
 
-    vul_history = vul_history.at[2 + 4 + 35 * 2 + 30].set(True)
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 2]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 0]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 8 + 1]
+        .set(True)
+        .at[4 + (33 - 3) * 12 + 3]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    correct_obs = jnp.concatenate((vul, history, player2_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[1].set(True).at[2].set(True).at[3].set(True)
+    history = (
+        history.at[4 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 2]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 1]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 3]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 8 + 0]
+        .set(True)
+        .at[4 + (33 - 3) * 12 + 2]
+        .set(True)
+    )
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    correct_obs = jnp.concatenate((vul, history, player0_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P  ?
 
+    history = jnp.zeros(424, dtype=jnp.bool_)
+    history = history.at[0].set(True).at[1].set(True).at[2].set(True)
+    history = (
+        history.at[4 + 3]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 0]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 4 + 1]
+        .set(True)
+        .at[4 + (11 - 3) * 12 + 8 + 0]
+        .set(True)
+        .at[4 + (25 - 3) * 12 + 2]
+        .set(True)
+        .at[4 + (26 - 3) * 12 + 3]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 1]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 4 + 2]
+        .set(True)
+        .at[4 + (28 - 3) * 12 + 8 + 3]
+        .set(True)
+        .at[4 + (33 - 3) * 12 + 1]
+        .set(True)
+    )
+
     obs = observe(state, state.current_player)
-    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    correct_obs = jnp.concatenate((vul, history, player3_hand))
     assert jnp.all(obs == correct_obs)
 
-    state = step(state, 35)
+    actions = iter(actions)
+    action = next(actions)
+    state = step(state, action)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
```

### Comparing `pgx-0.7.4/tests/test_chess.py` & `pgx-0.8.0/tests/test_chess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import jax
 import jax.numpy as jnp
 import pgx
-from pgx.chess import State, Action, KING, _rotate, Chess, QUEEN, EMPTY, ROOK, PAWN, _legal_action_mask, CAN_MOVE
+from pgx.chess import State, Action, KING, _rotate, Chess, QUEEN, EMPTY, ROOK, PAWN, _legal_action_mask, CAN_MOVE, _zobrist_hash
+from pgx.experimental.utils import act_randomly
 
 env = Chess()
 init = jax.jit(env.init)
 step = jax.jit(env.step)
+act_randomly = jax.jit(act_randomly)
 
 pgx.set_visualization_config(color_theme="dark")
 
 
 def p(s: str, b=False):
     """
     >>> p("e3")
@@ -18,14 +20,27 @@
     37
     """
     x = "abcdefgh".index(s[0])
     offset = int(s[1]) - 1 if not b else 8 - int(s[1])
     return x * 8 + offset
 
 
+def test_zobrist_hash():
+    key = jax.random.PRNGKey(0)
+    key, subkey = jax.random.split(key)
+    state = init(subkey)
+    assert (state._zobrist_hash == jax.jit(_zobrist_hash)(state)).all()
+    # for i in range(5):
+    while not state.terminated:
+        key, subkey = jax.random.split(key)
+        action = act_randomly(subkey, state)
+        state = step(state, action)
+        # state.save_svg("debug.svg")
+        assert (state._zobrist_hash == jax.jit(_zobrist_hash)(state)).all()
+
 def test_action():
     # See #704
     # queen moves
     state = State._from_fen("k7/8/8/8/8/8/1Q6/7K w - - 0 1")
     state.save_svg("tests/assets/chess/action_001.svg")
     action = Action._from_label(jnp.int32(672))
     assert action.from_ == p("b2")
@@ -566,14 +581,84 @@
     state = State._from_fen("kbR5/pn6/P1B5/8/8/8/8/7K b - - 0 1")
     state.save_svg("tests/assets/chess/terminal_024.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
     assert (state.rewards == 0.0).all()
 
+    # perpetual check
+    state = State._from_fen("7k/8/4r1pp/8/8/4q3/8/5Q1K w - - 0 1")
+    state.save_svg("tests/assets/chess/terminal_025.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(2942))
+    state.save_svg("tests/assets/chess/terminal_026.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    print(state._to_fen())
+    state = step(state, jnp.int32(4104))
+    state.save_svg("tests/assets/chess/terminal_027.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(3446))
+    state.save_svg("tests/assets/chess/terminal_028.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(4176))
+    state.save_svg("tests/assets/chess/terminal_029.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(3374))
+    state.save_svg("tests/assets/chess/terminal_030.svg")
+    assert (state.observation[:, :, 12] == 0).all()
+    assert (state.observation[:, :, 13] == 1).all()
+    print(state._to_fen())
+    state = step(state, jnp.int32(4104))
+    state = step(state, jnp.int32(3446))
+    state = step(state, jnp.int32(4176))
+    state = step(state, jnp.int32(3374))
+    assert state.terminated
+    assert (state.rewards == 0.0).all()
+
+    # repetition
+    state = State._from_fen("r6k/8/8/8/8/8/8/R6K w - - 0 1")
+    state.save_svg("tests/assets/chess/terminal_031.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/terminal_032.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/terminal_033.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(614))
+    state.save_svg("tests/assets/chess/terminal_034.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(614))
+    state.save_svg("tests/assets/chess/terminal_035.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(1196))
+    state.save_svg("tests/assets/chess/terminal_036.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(1196))
+    state.save_svg("tests/assets/chess/terminal_037.svg")
+    assert (state.observation[:, :, 12] == 0).all()
+    assert (state.observation[:, :, 13] == 1).all()
+    state = step(state, jnp.int32(30))
+    state = step(state, jnp.int32(30))
+    state = step(state, jnp.int32(613))
+    state = step(state, jnp.int32(613))
+    assert state.terminated
+    assert (state.rewards == 0.0).all()
+
 
 def test_buggy_samples():
     # Found buggy samples by random playing debug
 
     # Bishop by bishop
     state = State._from_fen("r1q1k1nr/2p2p1B/p3pb2/1p4pP/P1pBP3/5P1N/R2P2KP/1Nn2Q1R w kq - 4 23")
     state.save_svg("tests/assets/chess/buggy_samples_001.svg")
@@ -629,14 +714,15 @@
     state.save_svg("tests/assets/chess/buggy_samples_011.svg")
     expected_legal_actions = [16, 17, 263, 652, 654, 656, 701, 714, 715, 1517, 1984, 1985, 1986, 1987, 1988, 1989, 1990, 2000, 2001, 3154, 3182, 3197, 3853]
     assert state.legal_action_mask.sum() == len(expected_legal_actions), f"\nactual:{jnp.nonzero(state.legal_action_mask)[0]}\nexpected\n{expected_legal_actions}"
 
 
 def test_observe():
     state = init(jax.random.PRNGKey(0))
+    assert state.observation.shape == (8, 8, 119)
 
     # my pawn
     expected = jnp.float32(
         [
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
@@ -689,19 +775,20 @@
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0]
         ]
     )
     assert (state.observation[:, :, 11] == expected).all()
 
     # repetitions
-    assert (state.observation[:, :, 12] == 0).all()
-
-    # color
+    assert (state.observation[:, :, 12] == 1).all()
     assert (state.observation[:, :, 13] == 0).all()
 
+    # color
+    assert state._turn == 0
+    assert (state.observation[:, :, 112] == 0).all()
 
 
     state = step(state, jnp.int32(89))
 
     # my pawn
     expected = jnp.float32(
         [
@@ -729,17 +816,147 @@
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0]
         ]
     )
     assert (state.observation[:, :, 6] == expected).all()
 
     # repetitions
-    assert (state.observation[:, :, 12] == 0).all()
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
 
     # color
-    assert (state.observation[:, :, 13] == 1).all()
+    assert state._turn == 1
+    assert (state.observation[:, :, 112] == 1).all()
+
+    # repetition
+    # not repetition patterns
+    # not the same turn
+    state = State._from_fen("r6k/8/8/8/8/8/8/R6K w - - 0 1")
+    state.save_svg("tests/assets/chess/observe_001.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_002.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(31))
+    state.save_svg("tests/assets/chess/observe_003.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(614))
+    state.save_svg("tests/assets/chess/observe_004.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(1196))
+    state.save_svg("tests/assets/chess/observe_005.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+    state = step(state, jnp.int32(1196))
+    state.save_svg("tests/assets/chess/observe_006.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+
+    # not the same castling rights
+    state = State._from_fen("r5k1/8/8/8/8/8/8/R3K2R w KQ - 0 1")
+    state.save_svg("tests/assets/chess/observe_007.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_008.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_009.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_010.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_011.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+
+    # not the same en-passant position
+    state = State._from_fen("r5k1/8/8/8/8/8/P7/R3K3 w KQ - 0 1")
+    state.save_svg("tests/assets/chess/observe_012.svg")
+    state = step(state, jnp.int32(90))
+    state.save_svg("tests/assets/chess/observe_013.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_014.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_015.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_016.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_017.svg")
+    assert (state.observation[:, :, 12] == 1).all()
+    assert (state.observation[:, :, 13] == 0).all()
+
+    # castling rights
+    state = State._from_fen("r3k2r/8/8/8/8/8/8/R3K2R w KQkq - 0 1")
+    state.save_svg("tests/assets/chess/observe_018.svg")
+    assert (state.observation[:, :, 114] == 1).all()
+    assert (state.observation[:, :, 115] == 1).all()
+    assert (state.observation[:, :, 116] == 1).all()
+    assert (state.observation[:, :, 117] == 1).all()
+    state = step(state, jnp.int32(16))
+    state.save_svg("tests/assets/chess/observe_019.svg")
+    assert (state.observation[:, :, 116] == 0).all()
+    state = step(state, jnp.int32(16))
+    state.save_svg("tests/assets/chess/observe_020.svg")
+    assert (state.observation[:, :, 114] == 0).all()
+    state = step(state, jnp.int32(4104))
+    state.save_svg("tests/assets/chess/observe_021.svg")
+    assert (state.observation[:, :, 117] == 0).all()
+    state = step(state, jnp.int32(4104))
+    state.save_svg("tests/assets/chess/observe_022.svg")
+    assert (state.observation[:, :, 115] == 0).all()
+
+    # castling rights
+    state = State._from_fen("r3k2r/8/8/8/8/8/8/R3K2R w KQkq - 0 1")
+    state.save_svg("tests/assets/chess/observe_023.svg")
+    assert (state.observation[:, :, 114] == 1).all()
+    assert (state.observation[:, :, 115] == 1).all()
+    assert (state.observation[:, :, 116] == 1).all()
+    assert (state.observation[:, :, 117] == 1).all()
+    state = step(state, jnp.int32(2352))
+    state.save_svg("tests/assets/chess/observe_024.svg")
+    assert (state.observation[:, :, 116] == 0).all()
+    assert (state.observation[:, :, 117] == 0).all()
+    state = step(state, jnp.int32(2352))
+    state.save_svg("tests/assets/chess/observe_025.svg")
+    assert (state.observation[:, :, 114] == 0).all()
+    assert (state.observation[:, :, 115] == 0).all()
+
+    # castling rights
+    state = State._from_fen("r3k1nr/8/8/8/8/8/8/R3K2R w KQkq - 0 1")
+    state.save_svg("tests/assets/chess/observe_026.svg")
+    assert (state.observation[:, :, 114] == 1).all()
+    assert (state.observation[:, :, 115] == 1).all()
+    assert (state.observation[:, :, 116] == 1).all()
+    assert (state.observation[:, :, 117] == 1).all()
+    state = step(state, jnp.int32(4110))
+    state.save_svg("tests/assets/chess/observe_027.svg")
+    assert (state.observation[:, :, 115] == 0).all()
+    assert (state.observation[:, :, 117] == 0).all()
+    state = step(state, jnp.int32(22))
+    state.save_svg("tests/assets/chess/observe_028.svg")
+    assert (state.observation[:, :, 114] == 0).all()
+    assert (state.observation[:, :, 116] == 0).all()
+
+    # non progress move count
+    state = State._from_fen("r3k2r/p7/8/8/8/8/8/R3K2R w KQkq - 0 1")
+    state.save_svg("tests/assets/chess/observe_029.svg")
+    state = step(state, jnp.int32(16))
+    state.save_svg("tests/assets/chess/observe_030.svg")
+    assert (state.observation[:, :, 118] == 0.01).all()
+    state = step(state, jnp.int32(4104))
+    state.save_svg("tests/assets/chess/observe_031.svg")
+    assert (state.observation[:, :, 118] == 0.02).all()
+    # capture move
+    state = step(state, jnp.int32(4109))
+    state.save_svg("tests/assets/chess/observe_032.svg")
+    assert (state.observation[:, :, 118] == 0).all()
+    # pawn move
+    state = step(state, jnp.int32(90))
+    state.save_svg("tests/assets/chess/observe_032.svg")
+    assert (state.observation[:, :, 118] == 0).all()
 
 
 def test_api():
     import pgx
     env = pgx.make("chess")
     pgx.v1_api_test(env, 5)
```

### Comparing `pgx-0.7.4/tests/test_connect_four.py` & `pgx-0.8.0/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_freeway.py` & `pgx-0.8.0/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_go.py` & `pgx-0.8.0/tests/test_go.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,18 @@
     assert state.legal_action_mask[231]
 
 def test_observe():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert state.current_player == 1
     # player 0 is white, player 1 is black
+    obs = observe(state, 1)   # black turn, black view
+    assert (obs[:, :, -1] == 0).all()
+    obs = observe(state, 0)   # black turn, white view
+    assert (obs[:, :, -1] == 1).all()
 
     state = step(state=state, action=0)
     state = step(state=state, action=1)
     state = step(state=state, action=2)
     state = step(state=state, action=3)
     state = step(state=state, action=4)
     state = step(state=state, action=5)
@@ -302,21 +306,21 @@
     # fmt: on
     assert state.current_player == 1
     assert state._turn % 2 == 0  # black turn
     obs = observe(state, 0)   # white
     assert obs.shape == (5, 5, 17)
     assert (obs[:, :, 0] == (curr_board == -1)).all()
     assert (obs[:, :, 1] == (curr_board == 1)).all()
-    assert (obs[:, :, -1] == 0).all()
+    assert (obs[:, :, -1] == 1).all()
 
     obs = observe(state, 1)  # black
     assert obs.shape == (5, 5, 17)
     assert (obs[:, :, 0] == (curr_board == 1)).all()
     assert (obs[:, :, 1] == (curr_board == -1)).all()
-    assert (obs[:, :, -1] == 1).all()
+    assert (obs[:, :, -1] == 0).all()
 
 
 def test_legal_action():
     key = jax.random.PRNGKey(0)
 
     # =====
     # @ + @ + @
```

### Comparing `pgx-0.7.4/tests/test_hex.py` & `pgx-0.8.0/tests/test_hex.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     # fmt:on
     assert jnp.all(state._board == expected)
 
 
 def test_swap():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
+    assert ~state.legal_action_mask[-1]
     state = step(state, 1)
     state.save_svg("tests/assets/hex/swap_01.svg")
     assert (state._board != 0).sum() == 1
     assert state._board[1] == -2
     assert state.legal_action_mask[-1]
     state = step(state, 121)  # swap!
     state.save_svg("tests/assets/hex/swap_02.svg")
@@ -131,27 +132,35 @@
     @ O . . .
      . . . . .
       . . . . .
     """
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert state.current_player == 0
-    assert (jnp.zeros((11, 11, 3)) == observe(state, 0)).all()
+    assert state.observation[:, :, 0].sum() == 0
+    assert state.observation[:, :, 1].sum() == 0
+    assert state.observation[:, :, 2].sum() == 0
+    assert state.observation[:, :, 3].sum() == 0
+    assert state.observation.sum() == 0
+    assert (jnp.zeros((11, 11, 4)) == observe(state, 0)).all()
+    assert (state.observation[:, :, -1] == 0).all()
     state = step(state, 0)
     assert (observe(state, 0)[:, :, 2] == 0).all()
     assert (observe(state, 1)[:, :, 2] == 1).all()
+    assert (state.observation[:, :, -1] == 1).all()
     state = step(state, 1)
     assert (
-        jnp.zeros((11, 11, 3), dtype=jnp.bool_).at[0, 0, 0].set(True).at[0, 1, 1].set(True)
+        jnp.zeros((11, 11, 4), dtype=jnp.bool_).at[0, 0, 0].set(True).at[0, 1, 1].set(True)
         == observe(state, 0)
     ).all()
     assert (
-            jnp.zeros((11, 11, 3), dtype=jnp.bool_).at[0, 1, 0].set(True).at[0, 0, 1].set(True).at[:, :, 2].set(True)
+            jnp.zeros((11, 11, 4), dtype=jnp.bool_).at[0, 1, 0].set(True).at[0, 0, 1].set(True).at[:, :, 2].set(True)
         == observe(state, 1)
     ).all()
+    assert (state.observation[:, :, -1] == 0).all()
 
 
 def test_random_play():
     key = jax.random.PRNGKey(0)
     done = jnp.bool_(False)
     key, sub_key = jax.random.split(key)
     state = init(sub_key)
```

### Comparing `pgx-0.7.4/tests/test_kuhn_poker.py` & `pgx-0.8.0/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_leduc_holdem.py` & `pgx-0.8.0/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_othello.py` & `pgx-0.8.0/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_play2048.py` & `pgx-0.8.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_seaquest.py` & `pgx-0.8.0/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_shogi.py` & `pgx-0.8.0/tests/test_shogi.py`

 * *Files 6% similar despite different names*

```diff
@@ -267,129 +267,133 @@
 
 
 def test_observe():
     key = jax.random.PRNGKey(0)
     s: State = init(key)
     obs = observe(s, s.current_player)
 
-    assert obs.shape == (119, 9, 9)
+    assert obs.shape == (9, 9, 119)
 
-    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.]])
-    assert (obs[PAWN] == expected).all()  # 0
-
-    expected = jnp.bool_([[0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,1.,0.,0.,0.]])
-    assert (obs[DRAGON + 1] == expected).all()  # 14
-
-    expected = jnp.bool_([[0.,0.,0.,0.,0.,1.,1.,1.,0.],
-                          [0.,0.,0.,0.,0.,1.,1.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,1.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,0.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,0.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,0.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,1.,1.,1.],
-                          [0.,0.,0.,0.,0.,1.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,1.,1.,1.,1.]])
-    assert (obs[28] == expected).all()  # 利きの数1以上
-
-    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,1.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,1.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,1.,1.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.]])
-    assert (obs[29] == expected).all()  # 利きの数2以上
-
-    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,1.,0.],
-                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,0.,0.,0.,1.,0.,0.]])
-    assert (obs[30] == expected).all()  # 利きの数3以上
-
-    expected = jnp.bool_([[0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.],
-                          [0.,0.,1.,0.,0.,0.,0.,0.,0.]])
-    assert (obs[31] == expected).all()
-
-    expected = jnp.bool_([[0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.],
-                          [0.,0.,0.,1.,0.,0.,0.,0.,0.]])
-    assert (obs[45] == expected).all()
-
-    expected = jnp.bool_([[1.,1.,1.,1.,0.,0.,0.,0.,0.],
-                          [0.,1.,0.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,1.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,0.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,0.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,0.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,1.,1.,0.,0.,0.,0.,0.],
-                          [1.,1.,1.,1.,0.,0.,0.,0.,0.],
-                          [0.,1.,1.,1.,0.,0.,0.,0.,0.]])
-    assert (obs[59] == expected).all()
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+    assert (obs[:, :, PAWN] == expected).all()  # 0
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+    assert (obs[:, :, DRAGON + 1] == expected).all()  # 14
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [1.,0.,1.,0.,0.,0.,1.,1.,1.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [1.,0.,1.,1.,1.,1.,1.,1.,0.]])
+    assert (obs[:, :, 28] == expected).all()  # 利きの数1以上
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,0.,1.,0.,0.,0.,0.,0.,1.],
+                          [0.,1.,1.,1.,1.,1.,1.,0.,1.],
+                          [0.,0.,1.,0.,1.,0.,0.,0.,0.]])
+    assert (obs[:, :, 29] == expected).all()  # 利きの数2以上
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,1.,1.,1.,1.,1.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+
+    assert (obs[:, :, 30] == expected).all()  # 利きの数3以上
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+
+    assert (obs[:, :, 31] == expected).all()
+
+    expected = jnp.bool_([[0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+
+    assert (obs[:, :, 45] == expected).all()
+
+    expected = jnp.bool_([[0.,1.,1.,1.,1.,1.,1.,0.,1.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [1.,1.,1.,0.,0.,0.,1.,0.,1.],
+                          [1.,1.,1.,1.,1.,1.,1.,1.,1.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.],
+                          [0.,0.,0.,0.,0.,0.,0.,0.,0.]])
+
+    assert (obs[:, :, 59] == expected).all()
 
     # 駒打ち
     sfen = "1ns4nl/1r4k2/2p1gp3/1p1pp3p/l8/2P2PP2/1PNPP3P/2G2S3/2S1KG2L b BGS3Prbnl2p 1"
     s = State._from_sfen(sfen)
     visualize(s, "tests/assets/shogi/observe_001.svg")
     obs = observe(s, s.current_player)
 
     filled = [0, 1, 2, 16, 20, 24, 28, 29, 36, 40, 52, 54]
     for i in range(56):
         if i in filled:
-            assert obs[62 + i].all()
+            assert obs[:, :, 62 + i].all()
         else:
-            assert (~obs[62 + i]).all()
+            assert (~obs[:, :, 62 + i]).all()
 
     # 王手
     sfen = "lnsgkg1nl/1r5s1/pppppp1pp/6p2/8B/2P6/PP1PPPPPP/7R1/LNSGKGSNL b b 1"  # 先手番
     s = State._from_sfen(sfen)
     visualize(s, "tests/assets/shogi/observe_002.svg")
     obs = observe(s, s.current_player)
-    assert (~obs[-1]).all()
+    assert (~obs[:, :, -1]).all()
 
     sfen = "lnsgkg1nl/1r5s1/pppppp1pp/6p2/8B/2P6/PP1PPPPPP/7R1/LNSGKGSNL w b 1"  # 後手番
     s = State._from_sfen(sfen)
     visualize(s, "tests/assets/shogi/observe_003.svg")
     obs = observe(s, s.current_player)
-    assert obs[-1].all()
+    assert obs[:, :, -1].all()
 
     # TODO: player_id != current_player
 
 def test_sfen():
     sfen = "lnsgkg1nl/1r5s1/pppppp1pp/6p2/8B/2P6/PP1PPPPPP/7R1/LNSGKGSNL b b 1"
     s = State._from_sfen(sfen)
     visualize(s, "tests/assets/shogi/sfen_001.svg")
@@ -399,10 +403,9 @@
     s = State._from_sfen(sfen)
     visualize(s, "tests/assets/shogi/sfen_002.svg")
     assert s._to_sfen() == sfen
 
 
 def test_api():
     import pgx
-    # env = pgx.make("shogi")
-    env = Shogi(max_termination_steps=50)
-    pgx.v1_api_test(env, 5)
+    env = pgx.make("shogi")
+    pgx.v1_api_test(env, 1)
```

### Comparing `pgx-0.7.4/tests/test_space_invaders.py` & `pgx-0.8.0/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_sparrow_mahjong.py` & `pgx-0.8.0/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.7.4/tests/test_tic_tac_toe.py` & `pgx-0.8.0/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

