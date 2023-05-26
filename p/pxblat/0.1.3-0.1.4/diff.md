# Comparing `tmp/pxblat-0.1.3.tar.gz` & `tmp/pxblat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxblat-0.1.3.tar", max compression
+gzip compressed data, was "pxblat-0.1.4.tar", max compression
```

## Comparing `pxblat-0.1.3.tar` & `pxblat-0.1.4.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0     1067 2023-05-25 08:59:43.011577 pxblat-0.1.3/LICENSE
--rw-r--r--   0        0        0     4129 2023-05-25 08:59:43.011577 pxblat-0.1.3/README.md
--rw-r--r--   0        0        0     5729 2023-05-25 08:59:43.447581 pxblat-0.1.3/build.py
--rw-r--r--   0        0        0     1903 2023-05-25 09:00:38.891914 pxblat-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/__init__.py
--rw-r--r--   0        0        0       40 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/__init__.py
--rw-r--r--   0        0        0      327 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/cli.py
--rw-r--r--   0        0        0     6221 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/client.py
--rw-r--r--   0        0        0     2325 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/fa2twobit.py
--rw-r--r--   0        0        0      214 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/log.py
--rw-r--r--   0        0        0     7914 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/cli/server.py
--rw-r--r--   0        0        0       54 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/__init__.py
--rw-r--r--   0        0        0    22786 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/__init__.pyi
--rw-r--r--   0        0        0       40 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/.clang-format
--rw-r--r--   0        0        0     1966 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/_extc.cpp
--rw-r--r--   0        0        0       11 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/_extc.modules
--rw-r--r--   0        0        0       81 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/_extc.sources
--rw-r--r--   0        0        0     2163 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
--rw-r--r--   0        0        0     9044 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/gfClient.cpp
--rw-r--r--   0        0        0    17169 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/gfServer.cpp
--rw-r--r--   0        0        0     2721 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/gfServer_1.cpp
--rw-r--r--   0        0        0     3431 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/binder/pygfServer.cpp
--rw-r--r--   0        0        0    33509 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/bs_thread_pool.hpp
--rw-r--r--   0        0        0    28417 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/dbg.h
--rw-r--r--   0        0        0     1986 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/faToTwoBit.cpp
--rw-r--r--   0        0        0     1243 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/faToTwoBit.hpp
--rw-r--r--   0        0        0    13734 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfClient.cpp
--rw-r--r--   0        0        0     4866 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfClient.hpp
--rw-r--r--   0        0        0     6429 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfClient2.cpp
--rw-r--r--   0        0        0      506 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfClient2.hpp
--rw-r--r--   0        0        0    60953 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfServer.cpp
--rw-r--r--   0        0        0    11648 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/gfServer.hpp
--rw-r--r--   0        0        0    11360 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/pygfServer.cpp
--rw-r--r--   0        0        0      979 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/bindings/pygfServer.hpp
--rw-r--r--   0        0        0    24597 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/blat.c
--rw-r--r--   0        0        0     3485 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/faToTwoBit.c
--rw-r--r--   0        0        0     9944 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/gfClient.c
--rw-r--r--   0        0        0    53782 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/gfServer.c
--rw-r--r--   0        0        0       40 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/.clang-format
--rw-r--r--   0        0        0     2088 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/bandExt.h
--rw-r--r--   0        0        0     1073 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/base64.h
--rw-r--r--   0        0        0    27036 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/cheapcgi.h
--rw-r--r--   0        0        0     2097 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/filePath.h
--rw-r--r--   0        0        0      871 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/gfxPoly.h
--rw-r--r--   0        0        0     1034 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/hex.h
--rw-r--r--   0        0        0    10111 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/htmlPage.h
--rw-r--r--   0        0        0     9985 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/htmshell.h
--rw-r--r--   0        0        0      332 2023-05-25 08:59:43.451581 pxblat-0.1.3/src/pxblat/extc/include/aux/https.h
--rw-r--r--   0        0        0     4404 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/internet.h
--rw-r--r--   0        0        0     1990 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/kxTok.h
--rw-r--r--   0        0        0    16767 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/memgfx.h
--rw-r--r--   0        0        0     2997 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/mime.h
--rw-r--r--   0        0        0     1166 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/portimpl.h
--rw-r--r--   0        0        0     4401 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/rbTree.h
--rw-r--r--   0        0        0      164 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/aux/srcVersion.h
--rw-r--r--   0        0        0      916 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/aliType.h
--rw-r--r--   0        0        0    10193 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/axt.h
--rw-r--r--   0        0        0     6449 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/bPlusTree.h
--rw-r--r--   0        0        0     4355 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/binRange.h
--rw-r--r--   0        0        0     3456 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/bits.h
--rw-r--r--   0        0        0     5877 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/chain.h
--rw-r--r--   0        0        0     1839 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/chainBlock.h
--rw-r--r--   0        0        0    56916 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/common.h
--rw-r--r--   0        0        0     4198 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/dlist.h
--rw-r--r--   0        0        0     2681 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/dnaseq.h
--rw-r--r--   0        0        0    10058 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/dnautil.h
--rw-r--r--   0        0        0     3658 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/dystring.h
--rw-r--r--   0        0        0     2795 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/errAbort.h
--rw-r--r--   0        0        0     2128 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/errCatch.h
--rw-r--r--   0        0        0     5228 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/fa.h
--rw-r--r--   0        0        0    10590 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/fuzzyFind.h
--rw-r--r--   0        0        0    19945 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/genoFind.h
--rw-r--r--   0        0        0     1115 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/gfClientLib.h
--rw-r--r--   0        0        0     2884 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/gfInternal.h
--rw-r--r--   0        0        0    12187 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/hash.h
--rw-r--r--   0        0        0    14055 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/linefile.h
--rw-r--r--   0        0        0     3618 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/localmem.h
--rw-r--r--   0        0        0    10130 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/maf.h
--rw-r--r--   0        0        0     1786 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/memalloc.h
--rw-r--r--   0        0        0    12155 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/net.h
--rw-r--r--   0        0        0    12162 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/netlib.h
--rw-r--r--   0        0        0     4114 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/nib.h
--rw-r--r--   0        0        0     8773 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/obscure.h
--rw-r--r--   0        0        0      605 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/ooc.h
--rw-r--r--   0        0        0     3981 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/options.h
--rw-r--r--   0        0        0     1910 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/patSpace.h
--rw-r--r--   0        0        0     7300 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/pipeline.h
--rw-r--r--   0        0        0     6256 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/portable.h
--rw-r--r--   0        0        0    14633 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/psl.h
--rw-r--r--   0        0        0     4818 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/rangeTree.h
--rw-r--r--   0        0        0     2459 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/repMask.h
--rw-r--r--   0        0        0     3070 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/sig.h
--rw-r--r--   0        0        0     6814 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/sqlList.h
--rw-r--r--   0        0        0     3444 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/sqlNum.h
--rw-r--r--   0        0        0     2492 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/supStitch.h
--rw-r--r--   0        0        0     2086 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/trans3.h
--rw-r--r--   0        0        0     8657 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/twoBit.h
--rw-r--r--   0        0        0     9058 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/udc.h
--rw-r--r--   0        0        0     1821 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/core/verbose.h
--rw-r--r--   0        0        0        0 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/net/gfNet.h
--rw-r--r--   0        0        0     2278 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/include/net/log.h
--rw-r--r--   0        0        0       40 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/.clang-format
--rw-r--r--   0        0        0    31426 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/aux/axt.c
--rw-r--r--   0        0        0    14386 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/aux/bandExt.c
--rw-r--r--   0        0        0     2996 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/aux/base64.c
--rw-r--r--   0        0        0    11289 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/aux/binRange.c
--rw-r--r--   0        0        0    25709 2023-05-25 08:59:43.455581 pxblat-0.1.3/src/pxblat/extc/src/aux/blastOut.c
--rw-r--r--   0        0        0    80472 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/cheapcgi.c
--rw-r--r--   0        0        0    32618 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/ffSeedExtend.c
--rw-r--r--   0        0        0     6436 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/filePath.c
--rw-r--r--   0        0        0     2363 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/hex.c
--rw-r--r--   0        0        0    53011 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/htmlPage.c
--rw-r--r--   0        0        0    46630 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/htmshell.c
--rw-r--r--   0        0        0    27672 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/https.c
--rw-r--r--   0        0        0     2489 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/intExp.c
--rw-r--r--   0        0        0    16703 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/internet.c
--rw-r--r--   0        0        0    24031 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/maf.c
--rw-r--r--   0        0        0     2306 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/mafFromAxt.c
--rw-r--r--   0        0        0    16690 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/mime.c
--rw-r--r--   0        0        0    62706 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/net.c
--rw-r--r--   0        0        0    62778 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/netlib.c
--rw-r--r--   0        0        0     1742 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/ooc.c
--rw-r--r--   0        0        0    11962 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/patSpace.c
--rw-r--r--   0        0        0     3896 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/portimpl.c
--rw-r--r--   0        0        0    13003 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/rangeTree.c
--rw-r--r--   0        0        0    18572 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/rbTree.c
--rw-r--r--   0        0        0     5678 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/repMask.c
--rw-r--r--   0        0        0      848 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/servBrcMcw.c
--rw-r--r--   0        0        0     1033 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/servCrunx.c
--rw-r--r--   0        0        0      864 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/servcis.c
--rw-r--r--   0        0        0      906 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/servmsII.c
--rw-r--r--   0        0        0      921 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/servpws.c
--rw-r--r--   0        0        0    27041 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/sqlList.c
--rw-r--r--   0        0        0     7239 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/sqlNum.c
--rw-r--r--   0        0        0     3898 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/aux/wildcmp.c
--rw-r--r--   0        0        0      930 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/aliType.c
--rw-r--r--   0        0        0    19732 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/bPlusTree.c
--rw-r--r--   0        0        0     9051 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/bits.c
--rw-r--r--   0        0        0    17259 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/chain.c
--rw-r--r--   0        0        0    17077 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/chainBlock.c
--rw-r--r--   0        0        0    90522 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/common.c
--rw-r--r--   0        0        0     9450 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/dlist.c
--rw-r--r--   0        0        0     4604 2023-05-25 08:59:43.459581 pxblat-0.1.3/src/pxblat/extc/src/core/dnaseq.c
--rw-r--r--   0        0        0    29952 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/dnautil.c
--rw-r--r--   0        0        0     7156 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/dystring.c
--rw-r--r--   0        0        0    12046 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/errAbort.c
--rw-r--r--   0        0        0     3932 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/errCatch.c
--rw-r--r--   0        0        0    15611 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/fa.c
--rw-r--r--   0        0        0     3714 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/ffAli.c
--rw-r--r--   0        0        0    10802 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/ffAliHelp.c
--rw-r--r--   0        0        0     4868 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/ffScore.c
--rw-r--r--   0        0        0    40189 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/fuzzyFind.c
--rw-r--r--   0        0        0    70461 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/genoFind.c
--rw-r--r--   0        0        0    52425 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/gfBlatLib.c
--rw-r--r--   0        0        0     6363 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/gfClientLib.c
--rw-r--r--   0        0        0     3845 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/gfInternal.c
--rw-r--r--   0        0        0    18190 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/gfOut.c
--rw-r--r--   0        0        0    22265 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/hash.c
--rw-r--r--   0        0        0     5273 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/kxTok.c
--rw-r--r--   0        0        0    40326 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/linefile.c
--rw-r--r--   0        0        0     7256 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/localmem.c
--rw-r--r--   0        0        0    15074 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/memalloc.c
--rw-r--r--   0        0        0    12778 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/nib.c
--rw-r--r--   0        0        0    24969 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/obscure.c
--rw-r--r--   0        0        0    13012 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/options.c
--rw-r--r--   0        0        0    20522 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/osunix.c
--rw-r--r--   0        0        0    23419 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/pipeline.c
--rw-r--r--   0        0        0    63467 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/psl.c
--rw-r--r--   0        0        0     1203 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/servcl.c
--rw-r--r--   0        0        0    26961 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/supStitch.c
--rw-r--r--   0        0        0     3216 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/trans3.c
--rw-r--r--   0        0        0    33527 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/twoBit.c
--rw-r--r--   0        0        0    71967 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/udc.c
--rw-r--r--   0        0        0     4255 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/core/verbose.c
--rw-r--r--   0        0        0     2571 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/net/gfNet.c
--rw-r--r--   0        0        0     8795 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/extc/src/net/log.c
--rw-r--r--   0        0        0     3052 2023-05-25 08:59:43.463581 pxblat-0.1.3/src/pxblat/parser.py
--rw-r--r--   0        0        0        0 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/py.typed
--rw-r--r--   0        0        0     1042 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/__init__.py
--rw-r--r--   0        0        0     9920 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/basic.py
--rw-r--r--   0        0        0     3514 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/client.py
--rw-r--r--   0        0        0     6789 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/server.py
--rw-r--r--   0        0        0      725 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/status.py
--rw-r--r--   0        0        0      115 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/server/utils.py
--rw-r--r--   0        0        0     3431 2023-05-25 08:59:43.467581 pxblat-0.1.3/src/pxblat/utils.py
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 pxblat-0.1.3/setup.py
--rw-r--r--   0        0        0     4991 1970-01-01 00:00:00.000000 pxblat-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-26 09:39:53.058861 pxblat-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5077 2023-05-26 09:39:53.058861 pxblat-0.1.4/README.md
+-rw-r--r--   0        0        0     8696 2023-05-26 09:39:53.494868 pxblat-0.1.4/build.py
+-rw-r--r--   0        0        0     1903 2023-05-26 09:40:23.423267 pxblat-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/cli.py
+-rw-r--r--   0        0        0     6221 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/client.py
+-rw-r--r--   0        0        0     2325 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/fa2twobit.py
+-rw-r--r--   0        0        0      214 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/log.py
+-rw-r--r--   0        0        0     7914 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/cli/server.py
+-rw-r--r--   0        0        0       54 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/__init__.py
+-rw-r--r--   0        0        0    22786 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/.clang-format
+-rw-r--r--   0        0        0     1966 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/_extc.cpp
+-rw-r--r--   0        0        0       11 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/_extc.modules
+-rw-r--r--   0        0        0       81 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/_extc.sources
+-rw-r--r--   0        0        0     2163 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
+-rw-r--r--   0        0        0    10994 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/gfClient.cpp
+-rw-r--r--   0        0        0    20542 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/gfServer.cpp
+-rw-r--r--   0        0        0     2721 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/gfServer_1.cpp
+-rw-r--r--   0        0        0     3431 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/binder/pygfServer.cpp
+-rw-r--r--   0        0        0    33509 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/bs_thread_pool.hpp
+-rw-r--r--   0        0        0    28417 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/dbg.h
+-rw-r--r--   0        0        0     1986 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/faToTwoBit.cpp
+-rw-r--r--   0        0        0     1243 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/faToTwoBit.hpp
+-rw-r--r--   0        0        0    13734 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfClient.cpp
+-rw-r--r--   0        0        0     4866 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfClient.hpp
+-rw-r--r--   0        0        0     6429 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfClient2.cpp
+-rw-r--r--   0        0        0      506 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfClient2.hpp
+-rw-r--r--   0        0        0    60953 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfServer.cpp
+-rw-r--r--   0        0        0    11648 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/gfServer.hpp
+-rw-r--r--   0        0        0    11360 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/pygfServer.cpp
+-rw-r--r--   0        0        0      979 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/bindings/pygfServer.hpp
+-rw-r--r--   0        0        0    24597 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/blat.c
+-rw-r--r--   0        0        0     3485 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/faToTwoBit.c
+-rw-r--r--   0        0        0     9944 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/gfClient.c
+-rw-r--r--   0        0        0    53782 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/gfServer.c
+-rw-r--r--   0        0        0       40 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/.clang-format
+-rw-r--r--   0        0        0     2088 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/bandExt.h
+-rw-r--r--   0        0        0     1073 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/base64.h
+-rw-r--r--   0        0        0    27036 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/cheapcgi.h
+-rw-r--r--   0        0        0     2097 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/filePath.h
+-rw-r--r--   0        0        0      871 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/gfxPoly.h
+-rw-r--r--   0        0        0     1034 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/hex.h
+-rw-r--r--   0        0        0    10111 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/htmlPage.h
+-rw-r--r--   0        0        0     9985 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/htmshell.h
+-rw-r--r--   0        0        0      332 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/https.h
+-rw-r--r--   0        0        0     4404 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/internet.h
+-rw-r--r--   0        0        0     1990 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/kxTok.h
+-rw-r--r--   0        0        0    16767 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/memgfx.h
+-rw-r--r--   0        0        0     2997 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/mime.h
+-rw-r--r--   0        0        0     1166 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/portimpl.h
+-rw-r--r--   0        0        0     4401 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/rbTree.h
+-rw-r--r--   0        0        0      164 2023-05-26 09:39:53.498868 pxblat-0.1.4/src/pxblat/extc/include/aux/srcVersion.h
+-rw-r--r--   0        0        0      916 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/aliType.h
+-rw-r--r--   0        0        0    10193 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/axt.h
+-rw-r--r--   0        0        0     6449 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/bPlusTree.h
+-rw-r--r--   0        0        0     4355 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/binRange.h
+-rw-r--r--   0        0        0     3456 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/bits.h
+-rw-r--r--   0        0        0     5877 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/chain.h
+-rw-r--r--   0        0        0     1839 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/chainBlock.h
+-rw-r--r--   0        0        0    56916 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/common.h
+-rw-r--r--   0        0        0     4198 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/dlist.h
+-rw-r--r--   0        0        0     2681 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/dnaseq.h
+-rw-r--r--   0        0        0    10058 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/dnautil.h
+-rw-r--r--   0        0        0     3658 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/dystring.h
+-rw-r--r--   0        0        0     2795 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/errAbort.h
+-rw-r--r--   0        0        0     2128 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/errCatch.h
+-rw-r--r--   0        0        0     5228 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/fa.h
+-rw-r--r--   0        0        0    10590 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/fuzzyFind.h
+-rw-r--r--   0        0        0    19945 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/genoFind.h
+-rw-r--r--   0        0        0     1115 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/gfClientLib.h
+-rw-r--r--   0        0        0     2884 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/gfInternal.h
+-rw-r--r--   0        0        0    12187 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/hash.h
+-rw-r--r--   0        0        0    14055 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/linefile.h
+-rw-r--r--   0        0        0     3618 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/localmem.h
+-rw-r--r--   0        0        0    10130 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/maf.h
+-rw-r--r--   0        0        0     1786 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/memalloc.h
+-rw-r--r--   0        0        0    12155 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/net.h
+-rw-r--r--   0        0        0    12162 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/netlib.h
+-rw-r--r--   0        0        0     4114 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/nib.h
+-rw-r--r--   0        0        0     8773 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/obscure.h
+-rw-r--r--   0        0        0      605 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/ooc.h
+-rw-r--r--   0        0        0     3981 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/options.h
+-rw-r--r--   0        0        0     1910 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/patSpace.h
+-rw-r--r--   0        0        0     7300 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/pipeline.h
+-rw-r--r--   0        0        0     6256 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/portable.h
+-rw-r--r--   0        0        0    14633 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/psl.h
+-rw-r--r--   0        0        0     4818 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/rangeTree.h
+-rw-r--r--   0        0        0     2459 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/repMask.h
+-rw-r--r--   0        0        0     3070 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/sig.h
+-rw-r--r--   0        0        0     6814 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/sqlList.h
+-rw-r--r--   0        0        0     3444 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/sqlNum.h
+-rw-r--r--   0        0        0     2492 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/supStitch.h
+-rw-r--r--   0        0        0     2086 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/trans3.h
+-rw-r--r--   0        0        0     8657 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/twoBit.h
+-rw-r--r--   0        0        0     9058 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/udc.h
+-rw-r--r--   0        0        0     1821 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/core/verbose.h
+-rw-r--r--   0        0        0        0 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/net/gfNet.h
+-rw-r--r--   0        0        0     2278 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/include/net/log.h
+-rw-r--r--   0        0        0       40 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/.clang-format
+-rw-r--r--   0        0        0    31426 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/axt.c
+-rw-r--r--   0        0        0    14386 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/bandExt.c
+-rw-r--r--   0        0        0     2996 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/base64.c
+-rw-r--r--   0        0        0    11289 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/binRange.c
+-rw-r--r--   0        0        0    25709 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/blastOut.c
+-rw-r--r--   0        0        0    80472 2023-05-26 09:39:53.502869 pxblat-0.1.4/src/pxblat/extc/src/aux/cheapcgi.c
+-rw-r--r--   0        0        0    32618 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/ffSeedExtend.c
+-rw-r--r--   0        0        0     6436 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/filePath.c
+-rw-r--r--   0        0        0     2363 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/hex.c
+-rw-r--r--   0        0        0    53011 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/htmlPage.c
+-rw-r--r--   0        0        0    46630 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/htmshell.c
+-rw-r--r--   0        0        0    27672 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/https.c
+-rw-r--r--   0        0        0     2489 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/intExp.c
+-rw-r--r--   0        0        0    16703 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/internet.c
+-rw-r--r--   0        0        0    24031 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/maf.c
+-rw-r--r--   0        0        0     2306 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/mafFromAxt.c
+-rw-r--r--   0        0        0    16690 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/mime.c
+-rw-r--r--   0        0        0    62706 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/net.c
+-rw-r--r--   0        0        0    62778 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/netlib.c
+-rw-r--r--   0        0        0     1742 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/ooc.c
+-rw-r--r--   0        0        0    11962 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/patSpace.c
+-rw-r--r--   0        0        0     3896 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/portimpl.c
+-rw-r--r--   0        0        0    13003 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/rangeTree.c
+-rw-r--r--   0        0        0    18572 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/rbTree.c
+-rw-r--r--   0        0        0     5678 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/repMask.c
+-rw-r--r--   0        0        0      848 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/servBrcMcw.c
+-rw-r--r--   0        0        0     1033 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/servCrunx.c
+-rw-r--r--   0        0        0      864 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/servcis.c
+-rw-r--r--   0        0        0      906 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/servmsII.c
+-rw-r--r--   0        0        0      921 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/servpws.c
+-rw-r--r--   0        0        0    27041 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/sqlList.c
+-rw-r--r--   0        0        0     7239 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/sqlNum.c
+-rw-r--r--   0        0        0     3898 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/aux/wildcmp.c
+-rw-r--r--   0        0        0      930 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/aliType.c
+-rw-r--r--   0        0        0    19732 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/bPlusTree.c
+-rw-r--r--   0        0        0     9051 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/bits.c
+-rw-r--r--   0        0        0    17259 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/chain.c
+-rw-r--r--   0        0        0    17077 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/chainBlock.c
+-rw-r--r--   0        0        0    90522 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/common.c
+-rw-r--r--   0        0        0     9450 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/dlist.c
+-rw-r--r--   0        0        0     4604 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/dnaseq.c
+-rw-r--r--   0        0        0    29952 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/dnautil.c
+-rw-r--r--   0        0        0     7156 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/dystring.c
+-rw-r--r--   0        0        0    12046 2023-05-26 09:39:53.506868 pxblat-0.1.4/src/pxblat/extc/src/core/errAbort.c
+-rw-r--r--   0        0        0     3932 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/errCatch.c
+-rw-r--r--   0        0        0    15611 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/fa.c
+-rw-r--r--   0        0        0     3714 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/ffAli.c
+-rw-r--r--   0        0        0    10802 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/ffAliHelp.c
+-rw-r--r--   0        0        0     4868 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/ffScore.c
+-rw-r--r--   0        0        0    40189 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/fuzzyFind.c
+-rw-r--r--   0        0        0    70461 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/genoFind.c
+-rw-r--r--   0        0        0    52425 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/gfBlatLib.c
+-rw-r--r--   0        0        0     6363 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/gfClientLib.c
+-rw-r--r--   0        0        0     3845 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/gfInternal.c
+-rw-r--r--   0        0        0    18190 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/gfOut.c
+-rw-r--r--   0        0        0    22265 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/hash.c
+-rw-r--r--   0        0        0     5273 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/kxTok.c
+-rw-r--r--   0        0        0    40326 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/linefile.c
+-rw-r--r--   0        0        0     7256 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/localmem.c
+-rw-r--r--   0        0        0    15074 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/memalloc.c
+-rw-r--r--   0        0        0    12778 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/nib.c
+-rw-r--r--   0        0        0    24969 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/obscure.c
+-rw-r--r--   0        0        0    13012 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/options.c
+-rw-r--r--   0        0        0    20522 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/osunix.c
+-rw-r--r--   0        0        0    23419 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/pipeline.c
+-rw-r--r--   0        0        0    63467 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/psl.c
+-rw-r--r--   0        0        0     1203 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/servcl.c
+-rw-r--r--   0        0        0    26961 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/supStitch.c
+-rw-r--r--   0        0        0     3216 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/trans3.c
+-rw-r--r--   0        0        0    33527 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/twoBit.c
+-rw-r--r--   0        0        0    71967 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/udc.c
+-rw-r--r--   0        0        0     4255 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/core/verbose.c
+-rw-r--r--   0        0        0     2571 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/net/gfNet.c
+-rw-r--r--   0        0        0     8795 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/extc/src/net/log.c
+-rw-r--r--   0        0        0     3052 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/parser.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/py.typed
+-rw-r--r--   0        0        0     1042 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/server/__init__.py
+-rw-r--r--   0        0        0     9920 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/server/basic.py
+-rw-r--r--   0        0        0     3514 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/server/client.py
+-rw-r--r--   0        0        0     6789 2023-05-26 09:39:53.510869 pxblat-0.1.4/src/pxblat/server/server.py
+-rw-r--r--   0        0        0      725 2023-05-26 09:39:53.514869 pxblat-0.1.4/src/pxblat/server/status.py
+-rw-r--r--   0        0        0      115 2023-05-26 09:39:53.514869 pxblat-0.1.4/src/pxblat/server/utils.py
+-rw-r--r--   0        0        0     3431 2023-05-26 09:39:53.514869 pxblat-0.1.4/src/pxblat/utils.py
+-rw-r--r--   0        0        0     6662 1970-01-01 00:00:00.000000 pxblat-0.1.4/setup.py
+-rw-r--r--   0        0        0     5939 1970-01-01 00:00:00.000000 pxblat-0.1.4/PKG-INFO
```

### Comparing `pxblat-0.1.3/LICENSE` & `pxblat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/README.md` & `pxblat-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# PxBLAT
+# PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT
 
-<div align="center">
-<h1 align="center">
-<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
-<br>
-pxblat
-</h1>
-<h3 align="center">PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT</h3>
-<p align="center">
-
-<img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white" alt="" />
-<img src="https://img.shields.io/badge/Markdown-000000.svg?style=for-the-badge&logo=Markdown&logoColor=white" alt="pack" />
-<img src="https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white" alt="h" />
-<img src="https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black" alt="python" />
-</p>
-
-</div>
+[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)
+[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)
+[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)
+[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)
+[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
+[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)
+[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)
+[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)
+[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge&token=71639758-1cb2-48ed-a3b6-a79c60e568a5)](https://app.codecov.io/gh/cauliyang/pxblat)
+[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)
+[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)
 
 ---
 
 ## 📚 Table of Contents
 
 - [📚 Table of Contents](#-table-of-contents)
 - [📍Overview](#-introdcution)
 - [🔮 Features](#-features)
-- [⚙️ Project Structure](#project-structure)
-- [🧩 Modules](#modules)
 - [🏎💨 Getting Started](#-getting-started)
-- [🗺 Roadmap](#-roadmap)
 - [🤝 Contributing](#-contributing)
 - [🪪 License](#-license)
 - [📫 Contact](#-contact)
 - [🙏 Acknowledgments](#-acknowledgments)
 
 ---
```

### Comparing `pxblat-0.1.3/pyproject.toml` & `pxblat-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxblat"
-version = "0.1.3"
+version = "0.1.4"
 description = "A native python binding for blat suit"
 authors = ["Yangyang Li <yangyang.li@northwestern.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -67,18 +67,18 @@
 "src/pxblat/cli/fa2twobit.py" = ["B008", "PLR0913"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-sugar = "^0.9.7"
 black = "^23.3.0"
-ruff = "^0.0.263"
+ruff = "^0.0.270"
 ipython = "^8.13.1"
 pybind11-stubgen = "^0.13.0"
-invoke = "^2.1.1"
+invoke = "^2.1.2"
 ipdb = "^0.13.13"
 pysam = "^0.21.0"
 pytest-ordering = "^0.6"
 pytest-xdist = "^3.3.1"
 scienceplots = "^2.0.1"
 tikzplotlib = "^0.10.1"
 nox = "^2023.4.22"
```

### Comparing `pxblat-0.1.3/src/pxblat/cli/client.py` & `pxblat-0.1.4/src/pxblat/cli/client.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/cli/fa2twobit.py` & `pxblat-0.1.4/src/pxblat/cli/fa2twobit.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/cli/server.py` & `pxblat-0.1.4/src/pxblat/cli/server.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/__init__.pyi` & `pxblat-0.1.4/src/pxblat/extc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/binder/_extc.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/binder/_extc.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/binder/faToTwoBit.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/binder/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/binder/gfClient.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/binder/gfClient.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -63,14 +63,44 @@
 		cl.def("withInName", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withInName, "C++: cppbinding::gfClientOption::withInName(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inName_"));
 		cl.def("withOutName", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withOutName, "C++: cppbinding::gfClientOption::withOutName(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outName_"));
 		cl.def("withInSeq", (struct cppbinding::gfClientOption & (cppbinding::gfClientOption::*)(const std::string &)) &cppbinding::gfClientOption::withInSeq, "C++: cppbinding::gfClientOption::withInSeq(const std::string &) --> struct cppbinding::gfClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inseq_"));
 		cl.def("to_string", (std::string (cppbinding::gfClientOption::*)() const) &cppbinding::gfClientOption::to_string, "C++: cppbinding::gfClientOption::to_string() const --> std::string");
 
 		cl.def("__str__", [](cppbinding::gfClientOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
 
+        cl.def(pybind11::pickle([](const cppbinding::gfClientOption& p){
+               return pybind11::make_tuple(p.hostName, p.portName,p.tType, p.qType, p.dots,
+                                           p.nohead, p.minScore, p.minIdentity,
+                                           p.outputFormat, p.maxIntron, p.genome,
+                                           p.genomeDataDir, p.isDynamic, p.SeqDir,
+                                           p.inName, p.outName, p.inSeq); },
+                                [](pybind11::tuple t){
+                                if (t.size() != 17)
+                                    throw std::runtime_error("Invalid state!");
+
+                                cppbinding::gfClientOption p{};
+                                p.hostName = t[0].cast<std::string>();
+                                p.portName = t[1].cast<std::string>();
+                                p.tType = t[2].cast<std::string>();
+                                p.qType = t[3].cast<std::string>();
+                                p.dots = t[4].cast<bool>();
+                                p.nohead = t[5].cast<bool>();
+                                p.minScore = t[6].cast<long>();
+                                p.minIdentity = t[7].cast<long>();
+                                p.outputFormat = t[8].cast<std::string>();
+                                p.maxIntron = t[9].cast<long>();
+                                p.genome = t[10].cast<std::string>();
+                                p.genomeDataDir = t[11].cast<std::string>();
+                                p.isDynamic = t[12].cast<bool>();
+                                p.SeqDir = t[13].cast<std::string>();
+                                p.inName = t[14].cast<std::string>();
+                                p.outName = t[15].cast<std::string>();
+                                p.inSeq = t[16].cast<std::string>();
+                                return p;}));
+
 
 	}
 	// cppbinding::pygfClient(struct cppbinding::gfClientOption &) file:gfClient.hpp line:118
   M("cppbinding").def("pygfClient", [](cppbinding::gfClientOption&o) {
     auto ret = cppbinding::pygfClient(o);
     return pybind11::bytes(ret);
   }, "C++: cppbinding::pygfClient(struct cppbinding::gfClientOption &) --> std::string", pybind11::arg("option"));
```

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/binder/gfServer_1.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/binder/gfServer_1.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/binder/pygfServer.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/binder/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/bs_thread_pool.hpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/bs_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/dbg.h` & `pxblat-0.1.4/src/pxblat/extc/bindings/dbg.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/faToTwoBit.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/faToTwoBit.hpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/faToTwoBit.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/gfClient.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/gfClient.hpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/gfClient.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/gfClient2.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/gfClient2.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/gfServer.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/gfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/gfServer.hpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/gfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/pygfServer.cpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/bindings/pygfServer.hpp` & `pxblat-0.1.4/src/pxblat/extc/bindings/pygfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/blat.c` & `pxblat-0.1.4/src/pxblat/extc/blat.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/faToTwoBit.c` & `pxblat-0.1.4/src/pxblat/extc/faToTwoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/gfClient.c` & `pxblat-0.1.4/src/pxblat/extc/gfClient.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/gfServer.c` & `pxblat-0.1.4/src/pxblat/extc/gfServer.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/bandExt.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/bandExt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/base64.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/base64.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/cheapcgi.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/cheapcgi.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/filePath.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/filePath.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/gfxPoly.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/gfxPoly.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/hex.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/hex.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/htmlPage.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/htmlPage.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/htmshell.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/htmshell.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/internet.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/internet.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/kxTok.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/kxTok.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/memgfx.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/memgfx.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/mime.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/mime.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/portimpl.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/portimpl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/aux/rbTree.h` & `pxblat-0.1.4/src/pxblat/extc/include/aux/rbTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/aliType.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/aliType.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/axt.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/axt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/bPlusTree.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/bPlusTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/binRange.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/binRange.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/bits.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/bits.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/chain.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/chain.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/chainBlock.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/chainBlock.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/common.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/common.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/dlist.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/dlist.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/dnaseq.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/dnaseq.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/dnautil.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/dnautil.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/dystring.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/dystring.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/errAbort.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/errAbort.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/errCatch.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/errCatch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/fa.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/fa.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/fuzzyFind.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/fuzzyFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/genoFind.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/genoFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/gfClientLib.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/gfClientLib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/gfInternal.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/gfInternal.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/hash.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/hash.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/linefile.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/linefile.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/localmem.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/localmem.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/maf.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/maf.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/memalloc.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/memalloc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/net.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/net.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/netlib.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/netlib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/nib.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/nib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/obscure.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/obscure.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/ooc.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/ooc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/options.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/options.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/patSpace.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/patSpace.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/pipeline.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/portable.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/portable.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/psl.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/psl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/rangeTree.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/rangeTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/repMask.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/repMask.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/sig.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/sig.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/sqlList.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/sqlList.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/sqlNum.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/sqlNum.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/supStitch.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/supStitch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/trans3.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/trans3.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/twoBit.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/twoBit.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/udc.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/udc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/core/verbose.h` & `pxblat-0.1.4/src/pxblat/extc/include/core/verbose.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/include/net/log.h` & `pxblat-0.1.4/src/pxblat/extc/include/net/log.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/axt.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/axt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/bandExt.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/bandExt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/base64.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/base64.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/binRange.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/binRange.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/blastOut.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/blastOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/cheapcgi.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/cheapcgi.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/ffSeedExtend.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/ffSeedExtend.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/filePath.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/filePath.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/hex.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/hex.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/htmlPage.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/htmlPage.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/htmshell.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/htmshell.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/https.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/https.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/intExp.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/intExp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/internet.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/internet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/maf.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/maf.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/mafFromAxt.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/mafFromAxt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/mime.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/mime.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/net.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/net.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/netlib.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/netlib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/ooc.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/ooc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/patSpace.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/patSpace.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/portimpl.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/portimpl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/rangeTree.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/rangeTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/rbTree.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/rbTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/repMask.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/repMask.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/servBrcMcw.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/servBrcMcw.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/servCrunx.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/servCrunx.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/servcis.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/servcis.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/servmsII.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/servmsII.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/servpws.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/servpws.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/sqlList.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/sqlList.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/sqlNum.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/sqlNum.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/aux/wildcmp.c` & `pxblat-0.1.4/src/pxblat/extc/src/aux/wildcmp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/aliType.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/aliType.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/bPlusTree.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/bPlusTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/bits.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/bits.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/chain.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/chain.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/chainBlock.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/chainBlock.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/common.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/common.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/dlist.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/dlist.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/dnaseq.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/dnaseq.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/dnautil.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/dnautil.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/dystring.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/dystring.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/errAbort.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/errAbort.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/errCatch.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/errCatch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/fa.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/fa.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/ffAli.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/ffAli.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/ffAliHelp.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/ffAliHelp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/ffScore.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/ffScore.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/fuzzyFind.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/fuzzyFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/genoFind.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/genoFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/gfBlatLib.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/gfBlatLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/gfClientLib.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/gfClientLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/gfInternal.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/gfInternal.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/gfOut.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/gfOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/hash.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/hash.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/kxTok.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/kxTok.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/linefile.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/linefile.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/localmem.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/localmem.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/memalloc.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/memalloc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/nib.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/nib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/obscure.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/obscure.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/options.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/options.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/osunix.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/osunix.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/pipeline.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/pipeline.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/psl.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/psl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/servcl.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/servcl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/supStitch.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/supStitch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/trans3.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/trans3.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/twoBit.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/twoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/udc.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/udc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/core/verbose.c` & `pxblat-0.1.4/src/pxblat/extc/src/core/verbose.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/net/gfNet.c` & `pxblat-0.1.4/src/pxblat/extc/src/net/gfNet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/extc/src/net/log.c` & `pxblat-0.1.4/src/pxblat/extc/src/net/log.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/parser.py` & `pxblat-0.1.4/src/pxblat/parser.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/server/__init__.py` & `pxblat-0.1.4/src/pxblat/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/server/basic.py` & `pxblat-0.1.4/src/pxblat/server/basic.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/server/client.py` & `pxblat-0.1.4/src/pxblat/server/client.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/server/server.py` & `pxblat-0.1.4/src/pxblat/server/server.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/server/status.py` & `pxblat-0.1.4/src/pxblat/server/status.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/src/pxblat/utils.py` & `pxblat-0.1.4/src/pxblat/utils.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.1.3/setup.py` & `pxblat-0.1.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,17 +32,17 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['pxblat = pxblat.cli.cli:app']}
 
 setup_kwargs = {
     'name': 'pxblat',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A native python binding for blat suit',
-    'long_description': '# PxBLAT\n\n<div align="center">\n<h1 align="center">\n<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />\n<br>\npxblat\n</h1>\n<h3 align="center">PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT</h3>\n<p align="center">\n\n<img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white" alt="" />\n<img src="https://img.shields.io/badge/Markdown-000000.svg?style=for-the-badge&logo=Markdown&logoColor=white" alt="pack" />\n<img src="https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white" alt="h" />\n<img src="https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black" alt="python" />\n</p>\n\n</div>\n\n---\n\n## 📚 Table of Contents\n\n- [📚 Table of Contents](#-table-of-contents)\n- [📍Overview](#-introdcution)\n- [🔮 Features](#-features)\n- [⚙️ Project Structure](#project-structure)\n- [🧩 Modules](#modules)\n- [🏎💨 Getting Started](#-getting-started)\n- [🗺 Roadmap](#-roadmap)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [📫 Contact](#-contact)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n---\n\n## 🔮 Feautres\n\n- no intermidiate files, all in memory\n- no system call\n- no need to bother with log files to get status of tool\n- no need to worry about file format\n- no other dependency\n- higher proformance and Ergonomics (compare with current blat endpoint)\n\n## TODO\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] multi-connection server\n- [ ] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [ ] add too to dokerhub\n- [ ] add tool to pip\n- [ ] change abort to throw exceptions\n\n---\n\n<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-src-open.svg" width="80" />\n\n## 🚀 Getting Started\n\n### ✅ Prerequisites\n\nBefore you begin, ensure that you have the following prerequisites installed:\n\n> `[📌  INSERT-PROJECT-PREREQUISITES]`\n\n### 💻 Installation\n\n1. Clone the pxblat repository:\n\n```sh\ngit clone https://github.com/cauliyang/pxblat.git\n```\n\n2. Change to the project directory:\n\n```sh\ncd pxblat\n```\n\n3. Install the dependencies:\n\n```sh\npoetry install\n```\n\n### 🤖 Using pxblat\n\n```sh\npxblat\n```\n\n### 🧪 Running Tests\n\n```sh\npytest\n```\n\n<hr />\n\n## 🛠 Future Development\n\n- [x] [📌 COMPLETED-TASK]\n- [ ] [📌 INSERT-TASK]\n- [ ] [📌 INSERT-TASK]\n\n---\n\n## 🤝 Contributing\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```sh\ngit checkout -b new-feature-branch\n```\n\n4. Make changes to the project\'s codebase.\n5. Commit your changes to your local branch with a clear commit message that explains the changes you\'ve made.\n\n```sh\ngit commit -m \'Implemented new feature.\'\n```\n\n6. Push your changes to your forked repository on GitHub using the following command\n\n```sh\ngit push origin new-feature-branch\n```\n\n7. Create a pull request to the original repository.\n   Open a new pull request to the original project repository. In the pull request, describe the changes you\'ve made and why they\'re necessary.\n   The project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n---\n\n## \U0001faaa License\n\nThis project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.\n\n---\n\n## 🙏 Acknowledgments\n\n[📌 INSERT-DESCRIPTION]\n\n---\n',
+    'long_description': '# PxBLAT: An Efficient and Ergonomics Python Binding Library for BLAT\n\n[![python](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)](https://www.python.org/)\n[![c++](https://img.shields.io/badge/C++-00599C.svg?style=for-the-badge&logo=C++&logoColor=white)](https://en.cppreference.com/w/)\n[![c](https://img.shields.io/badge/C-A8B9CC.svg?style=for-the-badge&logo=C&logoColor=black)](https://www.gnu.org/software/gnu-c-manual/)\n[![pypi](https://img.shields.io/pypi/v/pxblat.svg?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![pyversion](https://img.shields.io/pypi/pyversions/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![license](https://img.shields.io/pypi/l/pxblat?style=for-the-badge)](https://opensource.org/licenses/mit)\n[![precommit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=for-the-badge&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json&style=for-the-badge)](https://github.com/charliermarsh/ruff)\n[![download](https://img.shields.io/pypi/dm/pxblat?style=for-the-badge)](https://pypi.org/project/pxblat/)\n[![Codecov](https://img.shields.io/codecov/c/github/cauliyang/pxblat/main?style=for-the-badge&token=71639758-1cb2-48ed-a3b6-a79c60e568a5)](https://app.codecov.io/gh/cauliyang/pxblat)\n[![lastcommit](https://img.shields.io/github/last-commit/cauliyang/pxblat?style=for-the-badge)](https://github.com/cauliyang/pxblat/)\n[![tests](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml/badge.svg?style=for-the-badge)](https://github.com/cauliyang/pxblat/actions/workflows/tests.yml)\n\n---\n\n## 📚 Table of Contents\n\n- [📚 Table of Contents](#-table-of-contents)\n- [📍Overview](#-introdcution)\n- [🔮 Features](#-features)\n- [🏎💨 Getting Started](#-getting-started)\n- [🤝 Contributing](#-contributing)\n- [\U0001faaa License](#-license)\n- [📫 Contact](#-contact)\n- [🙏 Acknowledgments](#-acknowledgments)\n\n---\n\n## 🔮 Feautres\n\n- no intermidiate files, all in memory\n- no system call\n- no need to bother with log files to get status of tool\n- no need to worry about file format\n- no other dependency\n- higher proformance and Ergonomics (compare with current blat endpoint)\n\n## TODO\n\n- [x] parser gfclient result\n- [x] parse gfserver query result\n- [x] multi-connection server\n- [ ] benchmarking multi connection and original version\n- [x] test result with original version\n- [x] fix build.py to build ssl, hts, maybe libuv when install with pip\n- [ ] add tool to conda channel\n- [ ] add too to dokerhub\n- [ ] add tool to pip\n- [ ] change abort to throw exceptions\n\n---\n\n<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-src-open.svg" width="80" />\n\n## 🚀 Getting Started\n\n### ✅ Prerequisites\n\nBefore you begin, ensure that you have the following prerequisites installed:\n\n> `[📌  INSERT-PROJECT-PREREQUISITES]`\n\n### 💻 Installation\n\n1. Clone the pxblat repository:\n\n```sh\ngit clone https://github.com/cauliyang/pxblat.git\n```\n\n2. Change to the project directory:\n\n```sh\ncd pxblat\n```\n\n3. Install the dependencies:\n\n```sh\npoetry install\n```\n\n### 🤖 Using pxblat\n\n```sh\npxblat\n```\n\n### 🧪 Running Tests\n\n```sh\npytest\n```\n\n<hr />\n\n## 🛠 Future Development\n\n- [x] [📌 COMPLETED-TASK]\n- [ ] [📌 INSERT-TASK]\n- [ ] [📌 INSERT-TASK]\n\n---\n\n## 🤝 Contributing\n\nContributions are always welcome! Please follow these steps:\n\n1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.\n2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.\n3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).\n\n```sh\ngit checkout -b new-feature-branch\n```\n\n4. Make changes to the project\'s codebase.\n5. Commit your changes to your local branch with a clear commit message that explains the changes you\'ve made.\n\n```sh\ngit commit -m \'Implemented new feature.\'\n```\n\n6. Push your changes to your forked repository on GitHub using the following command\n\n```sh\ngit push origin new-feature-branch\n```\n\n7. Create a pull request to the original repository.\n   Open a new pull request to the original project repository. In the pull request, describe the changes you\'ve made and why they\'re necessary.\n   The project maintainers will review your changes and provide feedback or merge them into the main branch.\n\n---\n\n## \U0001faaa License\n\nThis project is licensed under the `[📌  INSERT-LICENSE-TYPE]` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.\n\n---\n\n## 🙏 Acknowledgments\n\n[📌 INSERT-DESCRIPTION]\n\n---\n',
     'author': 'Yangyang Li',
     'author_email': 'yangyang.li@northwestern.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

