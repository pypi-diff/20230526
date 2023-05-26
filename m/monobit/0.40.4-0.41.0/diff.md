# Comparing `tmp/monobit-0.40.4.tar.gz` & `tmp/monobit-0.41.0.tar.gz`

## Comparing `monobit-0.40.4.tar` & `monobit-0.41.0.tar`

### file list

```diff
@@ -1,512 +1,516 @@
--rw-r--r--   0        0        0    26847 2020-02-02 00:00:00.000000 monobit-0.40.4/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.40.4/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.40.4/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.40.4/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/basetypes.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/binary.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/cachedprops.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/canvas.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/constants.py
--rw-r--r--   0        0        0    58298 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/encoding.py
--rw-r--r--   0        0        0    47288 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/font.py
--rw-r--r--   0        0        0    30606 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/glyph.py
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/labels.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/magic.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/pack.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/properties.py
--rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/raster.py
--rw-r--r--   0        0        0    13426 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/renderer.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/scripting.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/storage.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/streams.py
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/struct.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/taggers.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/vector.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/__init__.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/freedos/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/c0-pictures.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/iso2047.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/mac.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/bbc.py
--rw-r--r--   0        0        0    41778 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/borland.py
--rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/dec.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26408 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/geos.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/hurt.py
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/pkfont.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/psf.py
--rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/raw.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/signum.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/svg.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/vfont.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/__init__.py
--rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/sfnt.py
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/sfnt_writer.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/fonttools/E_B_S_C_.py
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/fonttools/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/fonttools/_b_d_a_t.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/fonttools/_b_h_e_d.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/sfnt/fonttools/_b_l_o_c.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/text/__init__.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/text/draw.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/text/hex.py
--rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/text/yaff.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/xlfd/__init__.py
--rw-r--r--   0        0        0    41958 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/xlfd/bdf.py
--rw-r--r--   0        0        0    18451 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/formats/xlfd/hbf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.40.4/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.40.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.40.4/LICENSE
--rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 monobit-0.40.4/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.40.4/pyproject.toml
--rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 monobit-0.40.4/PKG-INFO
+-rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 monobit-0.41.0/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.41.0/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.41.0/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.41.0/explore.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/basetypes.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/binary.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/cachedprops.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/chart.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/constants.py
+-rw-r--r--   0        0        0    58243 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/encoding.py
+-rw-r--r--   0        0        0    47906 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/font.py
+-rw-r--r--   0        0        0    31912 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/glyph.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/glyphmap.py
+-rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/labels.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/magic.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/pack.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/properties.py
+-rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/raster.py
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/renderer.py
+-rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripting.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/storage.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/streams.py
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/struct.py
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/taggers.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/vector.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/__init__.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/KOREAN.TXT
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/freedos/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/c0-pictures.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/iso2047.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/ms-linedraw.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/manual/windows-3.1.txt
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/charmaps/xfonts/viscii1.1-1.enc
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/compressors.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/container.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/directory.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/mac.py
+-rw-r--r--   0        0        0    15795 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/source.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/tar.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/containers/zip.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/__init__.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/amiga.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/bbc.py
+-rw-r--r--   0        0        0    40817 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/bmfont.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/borland.py
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/cpi.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/daisydot.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dashen.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dec.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/dosstart.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/figlet.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/fontx.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/fzx.py
+-rw-r--r--   0        0        0    26408 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/gdos.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/geos.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/hurt.py
+-rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/image.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mousegraphics.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mzfon.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/nearlyraw.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/palm.py
+-rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pcl.py
+-rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pcpaint.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pdf.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/pkfont.py
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/prebuilt.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/printshop.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/psf.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/raw.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/signum.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/svg.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/vfont.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xerox.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/dfont.py
+-rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/fond.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/iigs.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/lisa.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/mac/nfnt.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/__init__.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/gpifont.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/lx.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/os2/ne.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/__init__.py
+-rw-r--r--   0        0        0    16758 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/draw.py
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/hex.py
+-rw-r--r--   0        0        0    14275 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/text/yaff.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/LICENSE.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/__init__.py
+-rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/fnt.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/mz.py
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/ne.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/windows/pe.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    18398 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18469 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0    33745 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/pcf.py
+-rw-r--r--   0        0        0    25969 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/formats/xlfd/xlfd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.41.0/monobit/scripts/convert.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.41.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.41.0/LICENSE
+-rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 monobit-0.41.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.41.0/pyproject.toml
+-rw-r--r--   0        0        0    20306 2020-02-02 00:00:00.000000 monobit-0.41.0/PKG-INFO
```

### Comparing `monobit-0.40.4/YAFF.md` & `monobit-0.41.0/YAFF.md`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,16 @@
 - `right-kerning`: Adjustment to right bearing for specific glyph pairs. E.g. the pair `AV` may have negative
   kerning, so that they are displayed tighter than they otherwise would. Such an adjustment is
   specified in the `right-kerning` property of the `A` glyph, as a pair of the label for the `V` glyph and
   a numeric adjustment value.
 - `left-kerning`: Adjustment to left bearing for specific glyph pairs. The same adjustment as above could be
   specified in the `left-kerning` property of the `V` glyph, as a pair of the label for the `A` glyph and
   a numeric adjustment value. If both `left-kerning` and `right-kerning` are specified, they add up.
+- `scalable-width`: Advance width in fractional pixels, can be used for scaled rendering.
+- `scalable-height`: Advance height in fractional pixels, can be used for scaled rendering.
 
 
 ##### Rendering hints
 
 _Rendering hints_ affect the way decorations and transformations are applied. They are:
 - `direction`: Advance direction of writing. The following directions are supported:
   - `left-to-right`: left to right, top to bottom
```

### Comparing `monobit-0.40.4/explore.py` & `monobit-0.41.0/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/__init__.py` & `monobit-0.41.0/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/basetypes.py` & `monobit-0.41.0/monobit/basetypes.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/binary.py` & `monobit-0.41.0/monobit/binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,7 +30,18 @@
 def int_to_bytes(in_int, byteorder='big'):
     """Convert integer to bytes."""
     return in_int.to_bytes(max(1, ceildiv(in_int.bit_length(), 8)), byteorder)
 
 def bytes_to_int(in_bytes, byteorder='big'):
     """Convert integer to bytes."""
     return int.from_bytes(bytes(in_bytes), byteorder)
+
+
+def reverse_by_group(bitseq, fill='0', group_size=8):
+    """
+    Reverse bits in every byte in string representation of binary
+    Bit sequence is extended to end on byte boundary.
+    """
+    bitseq = bitseq.ljust(ceildiv(len(bitseq), group_size) * group_size, fill)
+    args = [iter(bitseq)] * group_size
+    bitseq = ''.join(''.join(_chunk[::-1]) for _chunk in zip(*args))
+    return bitseq
```

### Comparing `monobit-0.40.4/monobit/cachedprops.py` & `monobit-0.41.0/monobit/cachedprops.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/chart.py` & `monobit-0.41.0/monobit/chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 from itertools import product
 
 from .binary import ceildiv
 from .properties import Props
 from .basetypes import Coord
+from .glyphmap import GlyphMap
 
 
 def chart(
         font,
         columns=32, margin=(0, 0), padding=(0, 0),
         order='row-major', direction=(1, -1),
         codepoint_range=None,
@@ -48,15 +49,15 @@
     margin = Coord(*margin)
     # work out image geometry
     step_x = font.raster_size.x + padding.x
     step_y = font.raster_size.y + padding.y
     rows = ceildiv(len(font.glyphs), columns)
     # output glyph map
     traverse = grid_traverser(columns, rows, order, direction)
-    glyph_map = tuple(
+    glyph_map = GlyphMap(
         Props(
             glyph=_glyph, sheet=0,
             x=margin.x + col*step_x, y=margin.y + row*step_y,
         )
         for _glyph, (row, col) in zip(font.glyphs, traverse)
     )
     # determine image geometry
```

### Comparing `monobit-0.40.4/monobit/encoding.py` & `monobit-0.41.0/monobit/encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 from pathlib import Path
 import unicodedata
 from html.parser import HTMLParser
 from importlib.resources import files
 
 from .binary import int_to_bytes, align
-from .labels import Codepoint, to_label
+from .labels import Codepoint, to_label, to_labels
 
 
 _ENCODING_FILES = (
 
     ('txt', {}, (
         # iso standards
         # https://www.unicode.org/Public/MAPPINGS/ISO8859
@@ -840,20 +840,16 @@
         """Representation."""
         return f"{type(self).__name__}(name='{self.name}')"
 
 
 class EncodingName(str):
 
     def __new__(cls, value=''):
-        """Convert char or char sequence to char label."""
-        if not isinstance(value, str):
-            raise ValueError(
-                f'Can only convert `str` to encoding name, not `{type(value)}`.'
-            )
-        value = CharmapRegistry.normalise(value)
+        """Convert value to encoding name."""
+        value = CharmapRegistry.normalise(str(value))
         return super().__new__(cls, value)
 
 
 class Charmap(Encoder):
     """Convert between unicode and ordinals using stored mapping."""
 
     # charmap file format parameters
@@ -1052,32 +1048,35 @@
         """Representation."""
         return type(self).__name__ + '()'
 
 
 class Index(Encoder):
     """Convert from index to ordinals."""
 
-    def __init__(self, first_codepoint=0):
+    def __init__(self, code_range=(0,)):
         """Index converter."""
         super().__init__('index')
-        self._count = first_codepoint
+        # generator
+        self._code_range = to_labels(code_range)
 
     @staticmethod
     def char(*labels):
         """Convert codepoint to character, return empty string if missing."""
         raise TypeError('Can only use Index encoder to set codepoints, not character labels.')
 
     def codepoint(self, *labels):
         """Convert character to codepoint."""
-        self._count += 1
-        return Codepoint(self._count-1)
+        try:
+            return next(self._code_range)
+        except StopIteration:
+            return b''
 
     def __repr__(self):
         """Representation."""
-        return type(self).__name__ + f'(first_codepoint={self._count})'
+        return type(self).__name__ + '()'
 
 
 ###################################################################################################
 # charmap file readers
 
 @Charmap.register_loader('txt')
 @Charmap.register_loader('enc')
@@ -1310,20 +1309,21 @@
 
 
 # for use in function annotations
 def encoder(initialiser):
     """Retrieve or create a charmap from object or string."""
     if isinstance(initialiser, Encoder):
         return initialiser
-    if not initialiser:
+    if initialiser is None or not str(initialiser):
         return None
-    elif not isinstance(initialiser, str):
-        raise ValueError(
-            f'Encoding value must be string or Encoder object, not `{type(initialiser)}`'
-        )
+    initialiser = str(initialiser)
+    # numeric ranges - interpreted as indexer
+    if initialiser[:1].isdigit():
+        initialiser = to_labels(initialiser)
+        return Index(code_range=initialiser)
     try:
         return charmaps[initialiser]
     except KeyError:
         pass
     try:
         return Charmap.load(initialiser)
     except NotFoundError:
```

### Comparing `monobit-0.40.4/monobit/font.py` & `monobit-0.41.0/monobit/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 import logging
 from functools import wraps, partial, cache
 from pathlib import PurePath
 from unicodedata import normalize
 
 from .scripting import scriptable, get_scriptables, Any
 from .glyph import Glyph
-from .raster import turn_method
+from .raster import turn_method, NOT_SET
 from .basetypes import Coord, Bounds
 from .basetypes import to_int
-from .encoding import charmaps, encoder, EncodingName
+from .encoding import charmaps, encoder, EncodingName, Encoder
 from .taggers import tagger
 from .labels import Tag, Char, Codepoint, Label, to_label
 from .binary import ceildiv
 from .properties import extend_string
 from .cachedprops import HasProps, writable_property, checked_property
 from .taggers import tagmaps
 
 
-# sentinel object
-NOT_SET = object()
+def encoder_or_tagger(obj):
+    enc = encoder(obj)
+    if enc is None:
+        return tagger(obj)
+    return enc
 
 
 ###############################################################################
 # font class
 
 # pylint: disable=redundant-keyword-arg, no-member
 class FontProperties:
@@ -387,29 +390,26 @@
         advances = set(
             _glyph.advance_width
             for _glyph in self.glyphs if _glyph.advance_width
         )
         if len(set(advances)) > 2:
             return 'proportional'
         monospaced = len(set(advances)) == 1
-        negative = tuple(
-            _g for _g in self.glyphs
-            if _g.left_bearing < 0 or _g.right_bearing < 0
-            or _g.top_bearing < 0 or _g.bottom_bearing < 0
-        )
-        if not negative:
-            return 'character-cell' if monospaced else 'multi-cell'
-        # we have negative bearings; need to check if there's ink in them
-        # this should be rare (monospaced/bispaced with negative bearings)
+        # horizontal rendering
+        # check if all glyphs are rendered within the line height
+        # if there are vertical overlaps, it is not a charcell font
+        if self.ink_bounds.top - self.ink_bounds.bottom > self.line_height:
+            return 'monospace' if monospaced else 'proportional'
         if all(
-                (-_g.left_bearing < _g.padding.left)
-                and (-_g.right_bearing < _g.padding.right)
-                and (-_g.top_bearing < _g.padding.top)
-                and (-_g.bottom_bearing < _g.padding.bottom)
-                for _g in negative
+                (-_g.left_bearing <= _g.padding.left)
+                and (-_g.right_bearing <= _g.padding.right)
+                # if no negative metrics, these will be zero and hence satisfied.
+                and (-_g.top_bearing <= _g.padding.top)
+                and (-_g.bottom_bearing <= _g.padding.bottom)
+                for _g in self.glyphs
             ):
             return 'character-cell' if monospaced else 'multi-cell'
         return 'monospace' if monospaced else 'proportional'
 
     @checked_property
     def raster(self):
         """
@@ -431,19 +431,28 @@
     @checked_property
     def cell_size(self):
         """Width, height of the character cell."""
         if not self.glyphs or self.spacing == 'proportional':
             return Coord(0, 0)
         # smaller of the (at most two) advance widths is the cell size
         # in a multi-cell font, some glyphs may take up two cells.
-        cells = tuple(
-            (_g.advance_width, _g.advance_height)
-            for _g in self.glyphs
-        )
-        return Coord(*min(_c for _c in cells if all(_c)))
+        if self.has_vertical_metrics():
+            cells = tuple(
+                (_g.advance_width, _g.advance_height)
+                for _g in self.glyphs
+            )
+        else:
+            cells = tuple(
+                (_g.advance_width, self.line_height)
+                for _g in self.glyphs
+            )
+        sizes = tuple(_c for _c in cells if all(_c))
+        if not sizes:
+            return Coord(0, 0)
+        return Coord(*min(sizes))
 
     @checked_property
     def ink_bounds(self):
         """
         Minimum bounding box encompassing all glyphs at fixed origin,
         bottom-left origin cordinates.
         """
@@ -773,16 +782,14 @@
             comment=comment,
             **none_args,
         )
 
     ##########################################################################
     # property access
 
-    # __getattr__ = HasProps._getattr
-
     def get_comment(self, key=''):
         """Get global or property comment."""
         return self._comment.get(key, '')
 
     def _get_comment_dict(self):
         """Get all global and property comments as a dict."""
         return {**self._comment}
@@ -796,24 +803,23 @@
             def get_value(inner_self, key, inner_args, inner_kwargs):
                 if key in inner_kwargs:
                     return inner_kwargs[key]
                 return getattr(self, key)
 
         return FontFormatter().format(template, **kwargs)
 
-    def get_features(self):
-        """Get set of special features for this font."""
-        feats = set.union(*(_g.features for _g in self.glyphs))
+    @cache
+    def has_vertical_metrics(self):
+        """Check if this font has vertical metrics."""
         if any(
                 self.get_defined(_p)
                 for _p in ('line_width', 'left_extent', 'right_extent')
             ):
-            feats.add('vertical')
-        return feats
-
+            return True
+        return any(_g.has_vertical_metrics for _g in self.glyphs)
 
     ##########################################################################
     # glyph access
 
     @property
     def glyphs(self):
         return self._glyphs
@@ -945,16 +951,16 @@
 
     ##########################################################################
     # font operations
 
     @scriptable
     def label(
             self, *,
-            codepoint_from:encoder='', char_from:encoder='',
-            tag_from:tagger='', comment_from:tagger='',
+            codepoint_from:encoder=NOT_SET, char_from:encoder_or_tagger=NOT_SET,
+            tag_from:tagger=NOT_SET, comment_from:tagger=NOT_SET,
             overwrite:bool=False,
             match_whitespace:bool=True, match_graphical:bool=True
         ):
         """
         Add character and codepoint labels.
 
         codepoint_from: encoder registered name or filename to use to set codepoints from character labels
@@ -962,46 +968,46 @@
         tag_from: tagger registered name or filename to use to set tag labels
         comment_from: tagger registered name or filename to use to set comments
         overwrite: overwrite existing codepoints and/or characters
         match_whitespace: do not give blank glyphs a non-whitespace char label (default: True)
         match_graphical: do not give non-blank glyphs a non-graphical label (default: True)
         """
         nargs = sum(
-            bool(_arg)
+            _arg is not NOT_SET
             for _arg in (codepoint_from, char_from, tag_from, comment_from)
         )
         if nargs > 1:
             raise ValueError(
                 'Can only set one of character, codepoint, tag or comment with one label() call. '
                 'Use separate calls to set more.'
             )
         # default action: label chars with font encoding
         if nargs == 0 and self.encoding:
             char_from = encoder(self.encoding)
-            if not char_from:
+            if char_from is NOT_SET:
                 logging.warning(f'Encoding `{self.encoding}` not recognised.')
                 return self
         encoding = self.encoding
         if overwrite or not self.encoding:
-            if char_from:
+            if char_from is not NOT_SET and isinstance(char_from, Encoder):
                 encoding = char_from.name
-            elif codepoint_from:
+            elif codepoint_from is not NOT_SET and codepoint_from is not None:
                 encoding = codepoint_from.name
         kwargs = dict(
             overwrite=overwrite,
             match_whitespace=match_whitespace,
             match_graphical=match_graphical,
         )
-        if codepoint_from:
+        if codepoint_from is not NOT_SET:
             kwargs.update(dict(codepoint_from=codepoint_from))
-        elif char_from:
+        elif char_from is not NOT_SET:
             kwargs.update(dict(char_from=char_from))
-        elif tag_from:
+        elif tag_from is not NOT_SET:
             kwargs.update(dict(tag_from=tag_from))
-        elif comment_from:
+        elif comment_from is not NOT_SET:
             kwargs.update(dict(comment_from=comment_from))
         else:
             return self
         return self.modify(encoding=encoding, glyphs=tuple(
             _glyph.label(**kwargs)
             for _glyph in self.glyphs
         ))
@@ -1235,15 +1241,15 @@
         """
         Reduce glyphs to their bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         create_vertical_metrics = (
-            create_vertical_metrics or 'vertical' in self.get_features()
+            create_vertical_metrics or self.has_vertical_metrics()
         )
         font = self._apply_to_all_glyphs(
             Glyph.reduce,
             adjust_metrics=adjust_metrics,
             create_vertical_metrics=create_vertical_metrics,
         )
         if not adjust_metrics:
@@ -1292,14 +1298,16 @@
         """
         Stretch by repeating rows and/or columns.
 
         factor_x: number of times to repeat horizontally
         factor_y: number of times to repeat vertically
         adjust_metrics: also stretch metrics (default: True)
         """
+        if (factor_x, factor_y) == (1, 1):
+            return self
         font = self._apply_to_all_glyphs(
             Glyph.stretch,
             factor_x=factor_x, factor_y=factor_y,
             adjust_metrics=adjust_metrics,
         )
         if not adjust_metrics:
             return font
@@ -1317,14 +1325,16 @@
         """
         Shrink by removing rows and/or columns.
 
         factor_x: factor to shrink horizontally
         factor_y: factor to shrink vertically
         adjust_metrics: also stretch metrics (default: True)
         """
+        if (factor_x, factor_y) == (1, 1):
+            return self
         font = self._apply_to_all_glyphs(
             Glyph.shrink,
             factor_x=factor_x, factor_y=factor_y,
             adjust_metrics=adjust_metrics,
         )
         if not adjust_metrics:
             return font
```

### Comparing `monobit-0.40.4/monobit/glyph.py` & `monobit-0.41.0/monobit/glyph.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from functools import cache
 
 from .encoding import is_graphical, is_blank
 from .labels import Codepoint, Char, Tag, to_label
 from .raster import Raster, NOT_SET, turn_method
 from .properties import Props, extend_string
-from .cachedprops import HasProps, checked_property
+from .cachedprops import HasProps, checked_property, writable_property
 from .basetypes import Coord, Bounds, to_number
 from .scripting import scriptable
 from .vector import StrokePath
 
 
 ##############################################################################
 # kerning table
@@ -85,14 +85,18 @@
     bottom_bearing: int = 0
     # leftward offset from origin to matrix left edge
     shift_left: int = 0
 
     # path segments for stroke fonts
     path: StrokePath = StrokePath()
 
+    # overridable
+    scalable_width: float
+    scalable_height: float
+
     # non overridable known properties
     advance_width: int
     advance_height: int
     width: int
     height: int
     ink_bounds: Bounds
     bounding_box: Coord
@@ -114,14 +118,24 @@
         return self.left_bearing + self.width + self.right_bearing
 
     @checked_property
     def advance_height(self):
         """Internal advance width of glyph, including internal bearings."""
         return self.top_bearing + self.height + self.bottom_bearing
 
+    @writable_property
+    def scalable_width(self):
+        """Overridable, fractional advance width."""
+        return self.advance_width
+
+    @writable_property
+    def scalable_height(self):
+        """Overridable, fractional advance height."""
+        return self.advance_height
+
     @checked_property
     def width(self):
         """Raster width of glyph."""
         return self._pixels.width
 
     @checked_property
     def height(self):
@@ -214,14 +228,18 @@
         if (self.width, self.height) != (other.width, other.height):
             return False
         for p in (*self._props.keys(), *other._props.keys()):
             if not getattr(self, p) == getattr(other, p):
                 return False
         return self.as_matrix() == other.as_matrix()
 
+    def __hash__(self):
+        """Needs to exist if __eq__ defined."""
+        return super().__hash__()
+
     def __repr__(self):
         """Text representation."""
         elements = (
             f"labels={repr(self._labels)}" if self._labels else '',
             "comment=({})".format(
                 "\n  '" + "\n',\n  '".join(self.comment.splitlines()) + "'"
             ) if self._comment else '',
@@ -274,55 +292,66 @@
             labels=labels,
             comment=comment or '',
             **properties,
             _trustme=True,
         )
 
     def label(
-            self, codepoint_from=None, char_from=None,
-            tag_from=None, comment_from=None,
+            self, codepoint_from=NOT_SET, char_from=NOT_SET,
+            tag_from=NOT_SET, comment_from=NOT_SET,
             overwrite=False, match_whitespace=True, match_graphical=True,
         ):
         """
            Set labels or comment using provided encoder or tagger object.
 
            char_from: Encoder object used to set char labels
            codepoint_from: Encoder object used to set codepoint labels
            tag_from: Tagger object used to set tag labels
            comment_from: Tagger object used to set comment
            overwrite: overwrite codepoint or char if already given
            match_whitespace: do not give blank glyphs a non-whitespace char label (default: True)
            match_graphical: do not give non-blank glyphs a non-graphical label (default: True)
         """
         if sum(
-                _arg is not None
+                _arg is not NOT_SET
                 for _arg in (codepoint_from, char_from, tag_from, comment_from)
             ) > 1:
             raise ValueError(
                 'Can only set one of character, codepoint, tag or comment with one label() call. '
                 'Use separate calls to set more.'
            )
         labels = self.get_labels()
         # use codepage to find codepoint if not set
-        if codepoint_from and (overwrite or not self.codepoint):
-            return self.modify(codepoint=codepoint_from.codepoint(*labels))
+        if codepoint_from is not NOT_SET:
+            if not codepoint_from:
+                if overwrite:
+                    return self.modify(codepoint=None)
+            elif overwrite or not self.codepoint:
+                return self.modify(codepoint=codepoint_from.codepoint(*labels))
         # use codepage to find char if not set
-        if char_from and (overwrite or not self.char):
-            char = char_from.char(*labels)
-            if match_whitespace and self.is_blank() and char and not is_blank(char):
-                return self
-            if match_graphical and not self.is_blank() and char and not is_graphical(char):
-                return self
-            return self.modify(char=char)
-        if tag_from:
+        if char_from is not NOT_SET:
+            if not char_from:
+                if overwrite:
+                    return self.modify(char=None)
+            elif overwrite or not self.char:
+                char = char_from.char(*labels)
+                if match_whitespace and self.is_blank() and char and not is_blank(char):
+                    return self
+                if match_graphical and not self.is_blank() and char and not is_graphical(char):
+                    return self
+                return self.modify(char=char)
+        if tag_from is not NOT_SET:
+            if not tag_from:
+                if overwrite:
+                    return self.modify(tag=None)
             return self.modify(tag=tag_from.tag(*labels))
-        if comment_from:
-            return self.modify(
-                comment=extend_string(self.comment, comment_from.comment(*labels))
-            )
+        if comment_from is not NOT_SET:
+            if not comment_from:
+                return self.modify(comment=None)
+            return self.modify(comment=comment_from.comment(*labels))
         return self
 
     def append(
             self, *,
             comment=None, **properties
         ):
         """Return a copy of the glyph with changes."""
@@ -375,37 +404,21 @@
 
     # __getattr__ = HasProps._getattr
 
     @property
     def comment(self):
         return self._comment
 
-    @property
-    def features(self):
-        """Get set of special features for this glyph."""
-        feats = set()
-        if any(
-                self.get_defined(_p)
-                for _p in ('top_bearing', 'bottom_bearing', 'shift_left')
-            ):
-            feats.add('vertical')
-        if any(
-                self.get_defined(_p)
-                for _p in ('left_kerning', 'right_kerning')
-            ):
-            feats.add('kerning')
-        if any(
-                self._get_property(_p) < 0
-                for _p in (
-                    'left_bearing', 'right_bearing',
-                    'top_bearing', 'bottom_bearing'
-                )
-            ):
-            feats.add('overlap')
-        return feats
+    @cache
+    def has_vertical_metrics(self):
+        """Check if this glyph has vertical metrics."""
+        return any(
+            self.get_defined(_p)
+            for _p in ('top_bearing', 'bottom_bearing', 'shift_left')
+        )
 
     ##########################################################################
     # label access
 
     @property
     def tags(self):
         return tuple(_l for _l in self._labels if isinstance(_l, Tag))
@@ -453,32 +466,36 @@
             bitseq, stride=stride, width=width, align=align, _0=_0, _1=_1
         )
         return cls(pixels, **kwargs)
 
     @classmethod
     def from_bytes(
             cls, byteseq, width, height=NOT_SET,
-            *, align='left', stride=NOT_SET,
+            *, align='left', order='row-major', stride=NOT_SET,
+            byte_swap=0, bit_order='big',
             **kwargs
         ):
         """Create glyph from bytes/bytearray/int sequence."""
         pixels = Raster.from_bytes(
-            byteseq, width, height, align=align, stride=stride
+            byteseq, width, height,
+            align=align, stride=stride, order=order,
+            byte_swap=byte_swap, bit_order=bit_order,
         )
         return cls(pixels, **kwargs)
 
     @classmethod
     def from_hex(cls, hexstr, width, height=NOT_SET, *, align='left', **kwargs):
         """Create glyph from hex string."""
         pixels = Raster.from_hex(hexstr, width, height, align=align)
         return cls(pixels, **kwargs)
 
     @classmethod
-    def from_path(cls, strokepath, *, advance_width=None, **kwargs):
+    def from_path(cls, path, *, advance_width=None, **kwargs):
         """Draw the StrokePath and create a Glyph."""
+        strokepath = StrokePath(path)
         raster = Raster(strokepath.draw())
         if advance_width is None:
             advance_width = strokepath.bounds.right
         return cls(
             raster, path=strokepath,
             right_bearing=advance_width-strokepath.bounds.right,
             left_bearing=strokepath.bounds.left,
@@ -509,21 +526,37 @@
         """Convert glyph to a string of quadrant block characters."""
         return self._pixels.as_blocks()
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return self._pixels.as_vector(ink=ink, paper=paper)
 
+    def as_bits(self, ink=1, paper=0):
+        """Return flat bits as bytes string."""
+        return self._pixels.as_bits(ink=ink, paper=paper)
+
     def as_byterows(self, *, align='left'):
         """Convert glyph to rows of bytes."""
         return self._pixels.as_byterows(align=align)
 
-    def as_bytes(self, *, align='left'):
-        """Convert glyph to flat bytes."""
-        return self._pixels.as_bytes(align=align)
+    def as_bytes(
+            self, *, align='left', stride=NOT_SET, byte_swap=0,
+            bit_order='big',
+        ):
+        """
+        Convert raster to flat bytes.
+
+        stride: number of pixels per row (default: what's needed for alignment)
+        align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        byte_swap: swap byte order in units of n bytes, 0 (default) for no swap
+        bit_order: per-byte bit endianness; 'little' for lsb left, 'big' (default) for msb left
+        """
+        return self._pixels.as_bytes(
+            align=align, stride=stride, byte_swap=byte_swap, bit_order=bit_order,
+        )
 
     def as_hex(self, *, align='left'):
         """Convert glyph to hex string."""
         return self._pixels.as_hex(align=align)
 
 
     ##########################################################################
@@ -608,15 +641,15 @@
         top: number of rows to remove from top
         adjust_metrics: make the operation render-invariant (default: True)
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         if not any((left, bottom, right, top)):
             return self
         create_vertical_metrics = (
-            create_vertical_metrics or 'vertical' in self.features
+            create_vertical_metrics or self.has_vertical_metrics()
         )
         # reduce raster
         pixels = self._pixels.crop(left, bottom, right, top)
         if not adjust_metrics:
             return self.modify(pixels)
         else:
             # shift-left adjustment rounds differently for odd-width than even width
```

### Comparing `monobit-0.40.4/monobit/labels.py` & `monobit-0.41.0/monobit/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,38 +253,39 @@
         return self._value
 
 
 ##############################################################################
 # label sets
 
 def to_labels(set_str):
-    """Convert from iterable or string representation to tuple of labels."""
-    return to_tuple(set_str, to_label, label_range)
+    """Convert from iterable or string representation to label generator."""
+    return to_range(set_str, to_label, label_range)
 
-def to_tuple(set_str, converter=to_int, inclusive_range=lambda _l, _u: range(_l, _u+1)):
-    """Convert from iterable or string representation to tuple."""
+def to_range(set_str, converter=to_int, inclusive_range=lambda _l, _u: range(_l, _u+1)):
+    """Convert from iterable or string representation to generator."""
     if not isinstance(set_str, str):
-        return tuple(converter(_item) for _item in set_str)
+        return (converter(_item) for _item in set_str)
     elements = set_str.split(',')
     elements = (_e.partition('-') for _e in elements)
     elements = (
         inclusive_range(converter(_e[0]), converter(_e[2]))
         if all(_e) else (converter(_e[0]),)
         for _e in elements
     )
     elements = (_i for _e in elements for _i in _e)
-    return tuple(converter(_i) for _i in elements)
+    return (converter(_i) for _i in elements)
 
 def label_range(lower, upper):
     """Range of labels, inclusive of bounds."""
     if not type(lower) == type(upper):
         raise TypeError('Bounds must be of same type')
     lower, upper = to_label(lower), to_label(upper)
     if isinstance(lower, (bytes, int)):
-        return (Codepoint(_i) for _i in range(ord(lower), ord(upper)+1))
+        intrange = range(int(Codepoint(lower)), int(Codepoint(upper))+1)
+        return (Codepoint(_i) for _i in intrange)
     if isinstance(lower, str):
         return (Char(chr(_i)) for _i in range(ord(lower), ord(upper)+1))
     raise TypeError(f'Bounds must be Char or Codepoint, not {type(lower)}')
 
 
 CONVERTERS[tuple[Label]] = to_labels
 CONVERTERS[tuple[Char]] = to_labels
```

### Comparing `monobit-0.40.4/monobit/magic.py` & `monobit-0.41.0/monobit/magic.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/pack.py` & `monobit-0.41.0/monobit/pack.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/properties.py` & `monobit-0.41.0/monobit/properties.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/raster.py` & `monobit-0.41.0/monobit/raster.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import zip_longest
 
-from .binary import ceildiv
+from .binary import ceildiv, reverse_by_group
 from .basetypes import Bounds, Coord
 
 # sentinel object
 NOT_SET = object()
 
 
 # turn function for Raster, Glyph and Font
@@ -101,14 +101,17 @@
                 self._width = width
             else:
                 self._width = 0
         else:
             self._width = len(self._pixels[0])
 
 
+    def __bool__(self):
+        return bool(self.height and self.width)
+
     # NOTE - these following are shadowed in GlyphProperties
 
     @property
     def width(self):
         """Raster width of glyph."""
         return self._width
 
@@ -247,48 +250,60 @@
             offset = stride - width
         else:
             offset = 0
         excess = len(bitseq) % stride
         if excess:
             if _1 in bitseq[-excess:]:
                 raise ValueError(
-                    'Bit string overruns by nonzero %d-bit sequence [%s].',
-                    excess, bitseq[-excess:]
+                    'Bit string overruns by nonzero %d-bit sequence [%s].'
+                    % (excess, bitseq[-excess:])
                 )
             bitseq = bitseq[:-excess]
         if height is NOT_SET:
             # used as slice bound, None means all
             height = None
         rows = tuple(
             bitseq[_offs:_offs+width]
             for _offs in range(offset, len(bitseq), stride)
         )[:height]
         return cls(rows, _0=_0, _1=_1)
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return tuple(
-            _c
-            for _row in self.as_matrix(ink=ink, paper=paper)
-            for _c in _row
+            ink if _c == self._1 else paper
+            for _c in ''.join(self._pixels)
+        )
+
+    def as_bits(self, ink=1, paper=0):
+        """Return flat bits as bytes string."""
+        return (
+            ''.join(self._pixels).encode('latin-1')
+            .replace(self._1.encode('latin-1'), bytes((ink,)))
+            .replace(self._0.encode('latin-1'), bytes((paper,)))
         )
 
+
     @classmethod
     def from_bytes(
-                cls, byteseq, width=NOT_SET, height=NOT_SET,
-                *, align='left', stride=NOT_SET,
-                **kwargs
+            cls, byteseq, width=NOT_SET, height=NOT_SET,
+            *, align='left', order='row-major', stride=NOT_SET,
+            byte_swap=0, bit_order='big',
+            **kwargs
         ):
         """
         Create raster from bytes/bytearray/int sequence.
 
         width: raster width in pixels
         height: raster height in pixels
         stride: number of pixels per row (default: what's needed for alignment)
         align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        order: 'row-major' (default) or 'column-major' order of the byte array (no effect if align == 'bit')
+        byte_swap: swap byte order in units of n bytes, 0 (default) for no swap
+        bit_order: per-byte bit endianness; 'little' for lsb left, 'big' (default) for msb left
         """
         if all(_arg is NOT_SET for _arg in (width, height, stride)):
             raise ValueError(
                 'At least one of width, height or stride must be speecified'
             )
         if width == 0 or height == 0:
             if height is NOT_SET:
@@ -303,62 +318,120 @@
             else:
                 stride = 8 * ceildiv(width, 8)
         else:
             if width is NOT_SET:
                 stride = (8 * len(byteseq)) // height
             else:
                 stride = width
+        if byte_swap:
+            orig_length = len(byteseq)
+            byteseq = byteseq.ljust(ceildiv(len(byteseq), byte_swap)*byte_swap, b'\0')
+            # grouper
+            args = [iter(byteseq)] * byte_swap
+            byteseq = b''.join(bytes(_chunk[::-1]) for _chunk in zip(*args))
+            byteseq = byteseq[:orig_length]
+        # byte matrix order. no effect for bit alignment
+        if order == 'column-major' and align != 'bit':
+            byteseq = b''.join(
+                byteseq[_offs::height]
+                for _offs in range(height)
+            )
         if not byteseq:
             bitseq = ''
         else:
             bitseq = bin(
                 int.from_bytes(byteseq, 'big'))[2:].zfill(8*len(byteseq)
             )
+        # per-byte bit swap.
+        if bit_order == 'little':
+            bitseq = reverse_by_group(bitseq)
         return cls.from_vector(
             bitseq, width=width, height=height, stride=stride, align=align,
             _0='0', _1='1',
         )
 
-    def as_byterows(self, *, align='left'):
+    def as_byterows(self, *, align='left', bit_order='big'):
         """
         Convert raster to bytes, by row
 
         align: 'left' or 'right'
+        bit_order: per-byte bit endianness; 'little' for lsb left, 'big' (default) for msb left
         """
         if not self.height or not self.width:
             return ()
         rows = (
             ''.join(_row)
             for _row in self.as_matrix(paper='0', ink='1')
         )
         bytewidth = ceildiv(self.width, 8)
         if align.startswith('l'):
             rows = (_row.ljust(8*bytewidth, '0') for _row in rows)
+        else:
+            rows = (_row.rjust(8*bytewidth, '0') for _row in rows)
+        if bit_order == 'little':
+            rows = (reverse_by_group(_row) for _row in rows)
         byterows = (int(_row, 2).to_bytes(bytewidth, 'big') for _row in rows)
         return byterows
 
-    def as_bytes(self, *, align='left'):
+    def as_bytes(
+            self, *,
+            align='left', stride=NOT_SET, byte_swap=0, bit_order='big',
+        ):
         """
         Convert raster to flat bytes.
 
+        stride: number of pixels per row (default: what's needed for alignment)
         align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        byte_swap: swap byte order in units of n bytes, 0 (default) for no swap
+        bit_order: per-byte bit endianness; 'little' for lsb left, 'big' (default) for msb left
         """
         if not self.height or not self.width:
             return b''
-        if align.startswith('b'):
+        if stride is not NOT_SET:
+            if align == 'right':
+                raster = self.expand(left=stride-self.width)
+            else:
+                # left or bit-aligned
+                raster = self.expand(right=stride-self.width)
+        else:
+            raster = self
+        if align == 'bit':
             bits = ''.join(
                 ''.join(_row)
-                for _row in self.as_matrix(paper='0', ink='1')
+                for _row in raster.as_matrix(paper='0', ink='1')
             )
+            # per-byte bit swap.
+            if bit_order == 'little':
+                bits = reverse_by_group(bits)
             bytesize = ceildiv(len(bits), 8)
-            byterow = int(bits, 2).to_bytes(bytesize, 'big')
-            return byterow
+            byterows = (int(bits, 2).to_bytes(bytesize, 'big'),)
         else:
-            byterows = self.as_byterows(align=align)
-            return b''.join(byterows)
+            byterows = raster.as_byterows(align=align, bit_order=bit_order)
+        byteseq = b''.join(byterows)
+        if byte_swap:
+            # grouper
+            byteseq = byteseq.ljust(ceildiv(len(byteseq), byte_swap)*byte_swap, b'\0')
+            args = [iter(byteseq)] * byte_swap
+            byteseq = b''.join(bytes(_chunk[::-1]) for _chunk in zip(*args))
+        return byteseq
+
+    def get_byte_size(self, *, align='left', stride=NOT_SET):
+        """
+        Calculate size of bytes representation
+
+        stride: number of pixels per row (default: what's needed for alignment)
+        align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        """
+        if not self.height or not self.width:
+            return 0
+        if stride is NOT_SET:
+            stride = self.width
+        if align == 'bit':
+            return ceildiv(stride * self.height, 8)
+        return ceildiv(stride, 8) * self.height
 
     @classmethod
     def from_hex(cls, hexstr, width, height=NOT_SET, *, align='left'):
         """Create raster from hex string."""
         byteseq = bytes.fromhex(hexstr)
         return cls.from_bytes(byteseq, width, height, align=align)
```

### Comparing `monobit-0.40.4/monobit/renderer.py` & `monobit-0.41.0/monobit/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         """Use NFC as poor-man's grapheme cluster. This works... sometimes."""
         for c in normalize('NFC', text):
             yield c
 
 from .binary import ceildiv
 from .labels import Char, Codepoint
 from .raster import Raster, blockstr
-from .canvas import Canvas
 from .properties import Props
 from .glyph import Glyph
+from .glyphmap import GlyphMap
 
 
 DIRECTIONS = {
     'n': 'normal',
     'l': 'left-to-right',
     'r': 'right-to-left',
     't': 'top-to-bottom',
@@ -100,17 +100,15 @@
     else:
         _render = _render_horizontal
         min_margin = _adjust_margins_horizontal(glyphs), 0
     margin_x, margin_y = margin or min_margin
     glyph_map = _render(
         font, glyphs, margin_x, margin_y, align, adjust_bearings
     )
-    canvas = Canvas.from_glyph_map(glyph_map)
-    return canvas
-
+    return glyph_map
 
 def _adjust_margins_horizontal(glyphs):
     """Ensure margins are wide enough for any negative bearings."""
     glyphs = tuple(_row for _row in glyphs if _row)
     if not glyphs:
         return 0
     min_left = min(_row[0].left_bearing for _row in glyphs)
@@ -131,17 +129,17 @@
         font, glyphs, margin_x, margin_y, align, adjust_bearings
     ):
     """Render text horizontally."""
     # descent-line of the bottom-most row is at bottom margin
     # if a glyph extends below the descent line or left of the origin,
     # it may draw into the margin
     baseline = -margin_y - font.ascent
-    glyph_map = []
+    glyph_map = GlyphMap()
     # append empty glyph at start and end for margins
-    glyph_map.append(Props(glyph=Glyph(), sheet=0, x=0, y=0))
+    glyph_map.append_glyph(Glyph(), 0, 0, sheet=0)
     for glyph_row in glyphs:
         # x, y are relative to the left margin & baseline
         x = 0
         grid_x, grid_y = [], []
         for count, glyph in enumerate(glyph_row):
             # adjust origin for kerning
             if count:
@@ -155,34 +153,33 @@
             # advance origin to next glyph
             x += glyph.advance_width
         if align == 'right':
             start = -margin_x - x
         else:
             start = margin_x
         # append empty glyph at start and end for margins
-        glyph_map.append(Props(
-            glyph=Glyph(), sheet=0,
-            x=start+x+margin_x, y=baseline-font.descent-margin_y
-        ))
+        glyph_map.append_glyph(
+            Glyph(), start+x+margin_x, baseline-font.descent-margin_y, sheet=0,
+        )
         for glyph, x, y in zip(glyph_row, grid_x, grid_y):
-            glyph_map.append(Props(glyph=glyph, sheet=0, x=start+x, y=y))
+            glyph_map.append_glyph(glyph, start+x, y, sheet=0)
         # move to next line
         baseline -= font.line_height
     return glyph_map
 
 
 def _render_vertical(
         font, glyphs, margin_x, margin_y, align, adjust_bearings
     ):
     """Render text vertically."""
     # central axis (with leftward bias)
     baseline = font.line_width // 2
     # default is ttb right-to-left
-    glyph_map = []
-    glyph_map.append(Props(glyph=Glyph(), sheet=0, x=0, y=0))
+    glyph_map = GlyphMap()
+    glyph_map.append_glyph(Glyph(), 0, 0, sheet=0)
     for glyph_row in glyphs:
         y = 0
         grid_x, grid_y = [], []
         for count, glyph in enumerate(glyph_row):
             # advance origin to next glyph
             if count:
                 y -= adjust_bearings
@@ -190,21 +187,22 @@
             grid_y.append(y + glyph.bottom_bearing)
             grid_x.append(baseline - (glyph.width//2) - glyph.shift_left)
         if align == 'bottom':
             start = margin_y - y
         else:
             start = -margin_y
         # append empty glyph at start and end for margins
-        glyph_map.append(Props(
-            glyph=Glyph(), sheet=0,
+        glyph_map.append_glyph(
+            Glyph(),
             x=baseline + (font.line_width+1)//2 + margin_x*2,
-            y=start+y-margin_y
-        ))
+            y=start+y-margin_y,
+            sheet=0,
+        )
         for glyph, x, y in zip(glyph_row, grid_x, grid_y):
-            glyph_map.append(Props(glyph=glyph, sheet=0, x=margin_x+x, y=start+y))
+            glyph_map.append_glyph(glyph, margin_x+x, start+y, sheet=0)
         # move to next line
         baseline += font.line_width
     return glyph_map
 
 
 def _get_direction(font, text, direction, align):
     """Get direction and alignment."""
```

### Comparing `monobit-0.40.4/monobit/scripting.py` & `monobit-0.41.0/monobit/scripting.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 def wrap_main(debug=False):
     """Main script context."""
     # set log level
     if debug:
         loglevel = logging.DEBUG
     else:
         loglevel = logging.WARNING
-    logging.basicConfig(level=loglevel, format='%(levelname)s: %(message)s')
+    logging.basicConfig(level=loglevel, format='%(levelname)s: %(message)s', force=True)
     # run main script
     try:
         yield
     except BrokenPipeError:
         # happens e.g. when piping to `head`
         # https://stackoverflow.com/questions/16314321/suppressing-printout-of-exception-ignored-message-in-python-3
         sys.stdout = os.fdopen(1)
```

### Comparing `monobit-0.40.4/monobit/storage.py` & `monobit-0.41.0/monobit/storage.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/streams.py` & `monobit-0.41.0/monobit/streams.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/struct.py` & `monobit-0.41.0/monobit/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,21 @@
     # the following allow this class to mostly stand in for an int
     # we should not aften need this as struct/array elements
     # come out as Pyton basetype int/bytes
 
     def __index__(self):
         return int(self)
 
+    def __and__(self, rhs):
+        return int(self) & rhs
+
+    def __or__(self, rhs):
+        return int(self) & rhs
+
+
 
 class ScalarType(_WrappedCType):
     """Wrapper for scalar types. Mostly used to define arrays and structs."""
 
     def __init__(self, endian, ctype):
         if endian[:1].lower() in ('b', '>'):
             self._ctype = ctype.__ctype_be__
```

### Comparing `monobit-0.40.4/monobit/taggers.py` & `monobit-0.41.0/monobit/taggers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import unicodedata
 import pkgutil
 from pathlib import Path
 
 from .encoding import unicode_name, is_printable, NotFoundError
 from .labels import to_label, Tag
+from .properties import reverse_dict
 
 
 class Tagger:
     """Add tags or comments to a font's glyphs."""
 
     name = 'unknown-tagger'
 
@@ -104,14 +105,15 @@
 
 class MappingTagger(Tagger):
     """Tag on the basis of a mapping table."""
 
     def __init__(self, mapping, name=''):
         """Set up mapping."""
         self._chr2tag = mapping
+        self._tag2chr = reverse_dict(mapping)
         self.name = name
 
     @classmethod
     def load(cls, filename, *, name='', **kwargs):
         """Create new charmap from file."""
         try:
             data = pkgutil.get_data(__name__, filename)
@@ -132,14 +134,24 @@
         except KeyError:
             return self.get_default_tag(char)
 
     def get_default_tag(self, char):
         """Construct a default tag for unmapped glyphs."""
         return ''
 
+    def char(self, *labels):
+        """Get char value from tagmap."""
+        for label in labels:
+            if isinstance(label, Tag):
+                try:
+                    return self._tag2chr[label.value]
+                except KeyError:
+                    pass
+        return ''
+
 
 class AdobeTagger(MappingTagger):
 
     name = 'adobe'
 
     def get_default_tag(self, char):
         """Construct a default tag for unmapped glyphs."""
@@ -190,31 +202,30 @@
 ###################################################################################################
 
 # for use in function annotations
 def tagger(initialiser):
     """Retrieve or create a tagmap from object or string."""
     if isinstance(initialiser, Tagger):
         return initialiser
-    elif not isinstance(initialiser, str):
-        raise ValueError(
-            f'Tagger value must be string or Tagger object, not `{type(initialiser)}`'
-        )
+    if initialiser is None or not str(initialiser):
+        return None
+    initialiser = str(initialiser)
     try:
         return tagmaps[initialiser]
     except KeyError:
         pass
     return MappingTagger.load(initialiser)
 
 
 tagmaps = {
     'char': CharTagger(),
     'codepoint': CodepointTagger(),
     'name': UnicodeTagger(),
     'desc': UnicodeTagger(include_char=True),
-    'adobe': AdobeTagger.load('charmaps/agl/aglfn.txt', separator=';', unicode_column=0, tag_column=1),
-    'truetype': AdobeTagger.load('charmaps/agl/aglfn.txt', separator=';', unicode_column=0, tag_column=1),
-    'sgml': SGMLTagger.load('charmaps/misc/SGML.TXT', separator='\t', unicode_column=2),
+    'adobe': AdobeTagger.load('charmaps/agl/aglfn.txt', name='adobe', separator=';', unicode_column=0, tag_column=1),
+    'truetype': AdobeTagger.load('charmaps/agl/aglfn.txt', name='truetype', separator=';', unicode_column=0, tag_column=1),
+    'sgml': SGMLTagger.load('charmaps/misc/SGML.TXT', name='sgml', separator='\t', unicode_column=2),
 }
 
 # truetype mapping is adobe mapping *but* with .null for NUL
 # https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6post.html
 tagmaps['truetype']._chr2tag['\0'] = '.null'
```

### Comparing `monobit-0.40.4/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.41.0/monobit/charmaps/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.41.0/monobit/charmaps/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/adobe/symbol.txt` & `monobit-0.41.0/monobit/charmaps/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.41.0/monobit/charmaps/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/agl/LICENSE.md` & `monobit-0.41.0/monobit/charmaps/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/agl/README.md` & `monobit-0.41.0/monobit/charmaps/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/agl/aglfn.txt` & `monobit-0.41.0/monobit/charmaps/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.41.0/monobit/charmaps/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.41.0/monobit/charmaps/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.41.0/monobit/charmaps/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.41.0/monobit/charmaps/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.41.0/monobit/charmaps/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.41.0/monobit/charmaps/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.41.0/monobit/charmaps/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.41.0/monobit/charmaps/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.41.0/monobit/charmaps/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.41.0/monobit/charmaps/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.41.0/monobit/charmaps/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.41.0/monobit/charmaps/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.41.0/monobit/charmaps/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.41.0/monobit/charmaps/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.41.0/monobit/charmaps/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.41.0/monobit/charmaps/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.41.0/monobit/charmaps/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.41.0/monobit/charmaps/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.41.0/monobit/charmaps/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.41.0/monobit/charmaps/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/THAI.TXT` & `monobit-0.41.0/monobit/charmaps/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.41.0/monobit/charmaps/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.41.0/monobit/charmaps/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/README.md` & `monobit-0.41.0/monobit/charmaps/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.41.0/monobit/charmaps/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-de` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-es` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-it` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-us` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.41.0/monobit/charmaps/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.41.0/monobit/charmaps/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/dkuug/x0201-7` & `monobit-0.41.0/monobit/charmaps/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.41.0/monobit/charmaps/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/emacs/README.md` & `monobit-0.41.0/monobit/charmaps/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.41.0/monobit/charmaps/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.41.0/monobit/charmaps/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/evertype/README.md` & `monobit-0.41.0/monobit/charmaps/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1116.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1117.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1118.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1119.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1125.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/113.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/1131.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30000.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30001.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30002.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30003.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30004.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30005.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30006.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30007.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30008.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30009.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30010.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30011.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30012.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30013.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30014.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30015.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30016.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30017.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30018.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30019.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30020.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30021.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30022.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30023.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30024.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30025.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30026.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30027.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30028.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30029.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30030.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30031.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30032.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30033.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30034.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30039.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/30040.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/3012.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/3021.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/3845.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/3846.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/3848.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/437.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/57781.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/58152.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/58210.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/58335.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/59234.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/59829.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/60258.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/60853.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/61282.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/62306.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/667.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/668.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/737.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/770.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/771.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/772.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/773.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/774.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/775.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/777.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/778.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/790.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/808.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/848.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/849.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/850.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/851.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/852.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/853.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/855.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/856.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/857.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/858.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/859.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/860.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/861.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/862.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/863.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/864.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/865.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/866.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/867.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/869.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/872.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/895.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/899.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/991.ucp` & `monobit-0.41.0/monobit/charmaps/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/freedos/README.md` & `monobit-0.41.0/monobit/charmaps/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iana/Amiga-1251` & `monobit-0.41.0/monobit/charmaps/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iana/PTCP154` & `monobit-0.41.0/monobit/charmaps/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.41.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.41.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.41.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.41.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.41.0/monobit/charmaps/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/README.md` & `monobit-0.41.0/monobit/charmaps/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.41.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.41.0/monobit/charmaps/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.41.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.41.0/monobit/charmaps/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.41.0/monobit/charmaps/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.41.0/monobit/charmaps/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.41.0/monobit/charmaps/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.41.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.41.0/monobit/charmaps/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/hp48.txt` & `monobit-0.41.0/monobit/charmaps/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.41.0/monobit/charmaps/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/iso2047.txt` & `monobit-0.41.0/monobit/charmaps/manual/iso2047.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.41.0/monobit/charmaps/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/ms-linedraw.txt` & `monobit-0.41.0/monobit/charmaps/manual/ms-linedraw.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/russup3.ucp` & `monobit-0.41.0/monobit/charmaps/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.41.0/monobit/charmaps/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.41.0/monobit/charmaps/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.41.0/monobit/charmaps/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.41.0/monobit/charmaps/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.41.0/monobit/charmaps/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.41.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.41.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.41.0/monobit/charmaps/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.41.0/monobit/charmaps/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/CP424.TXT` & `monobit-0.41.0/monobit/charmaps/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/CP856.TXT` & `monobit-0.41.0/monobit/charmaps/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.41.0/monobit/charmaps/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.41.0/monobit/charmaps/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.41.0/monobit/charmaps/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.41.0/monobit/charmaps/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.41.0/monobit/charmaps/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.41.0/monobit/charmaps/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.41.0/monobit/charmaps/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.41.0/monobit/charmaps/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/SGML.TXT` & `monobit-0.41.0/monobit/charmaps/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.41.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.41.0/monobit/charmaps/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.41.0/monobit/charmaps/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/README.md` & `monobit-0.41.0/monobit/charmaps/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.41.0/monobit/charmaps/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.41.0/monobit/charmaps/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/moztw/eten.txt` & `monobit-0.41.0/monobit/charmaps/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.41.0/monobit/charmaps/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.41.0/monobit/charmaps/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.41.0/monobit/charmaps/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/vietstd/unicode.html` & `monobit-0.41.0/monobit/charmaps/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.41.0/monobit/charmaps/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/gem.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/lics.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.41.0/monobit/charmaps/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.41.0/monobit/charmaps/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.41.0/monobit/charmaps/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.41.0/monobit/charmaps/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/charmaps/xfonts/viscii1.1-1.enc` & `monobit-0.41.0/monobit/charmaps/xfonts/viscii1.1-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/compressors.py` & `monobit-0.41.0/monobit/containers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/container.py` & `monobit-0.41.0/monobit/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/directory.py` & `monobit-0.41.0/monobit/containers/directory.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/mac.py` & `monobit-0.41.0/monobit/containers/mac.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/source.py` & `monobit-0.41.0/monobit/containers/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     return int(cvalue, 0)
 
 
 _C_PARAMS = dict(
     delimiters='{}',
     comment='//',
     separator=';',
+    block_comment=('/*','*/'),
 )
 
 _JS_PARAMS = dict(
     delimiters='[]',
     comment='//',
     separator=',',
 )
@@ -65,15 +66,17 @@
 _PY_PARAMS = dict(
     comment='#',
     separator='',
 )
 
 _PAS_PARAMS = dict(
     delimiters='()',
-    comment='{',
+    # pascal has block comments only
+    comment='',
+    block_comment=('{','}'),
     int_conv=_int_from_pascal,
     separator=';',
 )
 
 
 ###############################################################################
 
@@ -98,20 +101,20 @@
 @loaders.register(
     name='json',
     patterns=('*.js', '*.json',),
     wrapper=True,
 )
 def load_json(infile, *, identifier:str='', format='', **kwargs):
     """
-    Extract font file encoded in JSON or JavaScript source code.
+    Extract font file encoded in JSON dictionary.
 
-    identifier: text at start of line where encoded file starts (default: first list [])
+    identifier: text at start of line where encoded file starts (default: first list [] in dict)
     """
     return _load_coded_binary(
-        infile, identifier=identifier, format=format, assign='',
+        infile, identifier=identifier, format=format, assign=':',
         **_JS_PARAMS, **kwargs
     )
 
 
 @loaders.register(
     name='python',
     patterns=('*.py',),
@@ -184,72 +187,96 @@
         **kwargs
     )
 
 
 def _load_coded_binary(
         infile, *, identifier, delimiters, comment,
         assign='=', int_conv=_int_from_c,
+        block_comment=(),
         # dummy for load; keep out of kwargs
         separator='',
         format='', **kwargs,
     ):
     """Load font from binary encoded in source code."""
     fonts = []
     while True:
         try:
-            coded_data = _get_payload(
-                infile.text, identifier, delimiters, comment, assign
+            found_identifier, coded_data = _get_payload(
+                infile.text, identifier, delimiters, comment, assign,
+                block_comment=block_comment,
             )
         except FileFormatError as e:
             # raised at end of file
             break
-        data = bytes(int_conv(_s) for _s in coded_data.split(',') if _s.strip())
         try:
-            with Stream.from_data(data, mode='r') as bytesio:
+            data = bytes(int_conv(_s) for _s in coded_data.split(',') if _s.strip())
+        except ValueError:
+            logging.warning(
+                f'Could not convert coded data for identifier {found_identifier}'
+            )
+        try:
+            with Stream.from_data(data, mode='r', name=found_identifier) as bytesio:
                 fonts.extend(load_stream(bytesio, format=format, **kwargs))
         except FileFormatError as e:
             logging.debug(e)
             continue
     return fonts
 
 
-def _get_payload(instream, identifier, delimiters, comment, assign):
+def _get_payload(
+        instream, identifier, delimiters, comment, assign, block_comment=()
+    ):
     """Find the identifier and get the part between delimiters."""
+    def _strip_line(line):
+        if comment:
+            line, _, _ = line.partition(comment)
+        if block_comment:
+            while block_comment[0] in line:
+                before, _, after = line.partition(block_comment[0])
+                _, _, after = after.partition(block_comment[1])
+                line = before + after
+        line = line.strip(' \r\n')
+        return line
+
     start, end = delimiters
+    found_identifier = ''
     for line in instream:
-        if comment in line:
-            line, _ = line.split(comment, 1)
-        line = line.strip(' \r\n')
+        line = _strip_line(line)
         if identifier in line and assign in line:
             if identifier:
-                _, line = line.split(identifier)
-            if start in line:
-                _, line = line.split(start)
-                break
+                _, _, line = line.partition(identifier)
+                found_identifier = identifier
+            else:
+                found_identifier, _, _ = line.partition(assign)
+                *_, found_identifier = found_identifier.strip().split()
+        if found_identifier and start in line:
+            _, line = line.split(start)
+            break
     else:
         raise FileFormatError(
             f'No payload with identifier `{identifier}` found in file'
         )
+    # special case: whole array in one line
     if end in line:
         line, _ = line.split(end, 1)
         return line
+    # multi-line array
     payload = [line]
     for line in instream:
-        if comment in line:
-            line, _ = line.split(comment, 1)
-        line = line.strip(' \r\n')
+        line = _strip_line(line)
         if start in line:
             _, line = line.split(start, 1)
         if end in line:
             line, _ = line.split(end, 1)
             payload.append(line)
             break
         if line:
             payload.append(line)
-    return ''.join(payload)
+    return found_identifier, ''.join(payload)
+
 
 
 @loaders.register(
     name='basic',
     patterns=('*.bas',),
     wrapper=True,
 )
@@ -338,15 +365,15 @@
     outstream.text.write('}\n')
 
 
 @savers.register(linked=load_source, wrapper=True)
 def save_source(
         fonts, outstream, *,
         identifier:str, assign:str='=', delimiters:str='{}', comment:str='//',
-        separator=';',
+        separator:str=';',
         bytes_per_line:int=16, distribute:bool=True,
         format='raw',
         **kwargs
     ):
     """
     Save to font file encoded in source code.
 
@@ -364,14 +391,16 @@
         format=format, distribute=distribute, separator=separator,
         **kwargs
     )
 
 def _save_coded_binary(
         fonts, outstream,
         identifier_template, assign_template, delimiters, comment, separator,
+        # block_comment is unused in writer but specified in arguments for reader
+        block_comment=None,
         bytes_per_line=16, format='raw', distribute=True, **kwargs
     ):
     """
     Generate font file encoded as source code.
 
     identifier_template: Template for the identifier. May include font properties.
     assign_template: assignment operator. May include `identifier` and `bytesize` variable.
```

### Comparing `monobit-0.40.4/monobit/containers/tar.py` & `monobit-0.41.0/monobit/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/containers/zip.py` & `monobit-0.41.0/monobit/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/amiga.py` & `monobit-0.41.0/monobit/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/bbc.py` & `monobit-0.41.0/monobit/formats/bbc.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/bmfont.py` & `monobit-0.41.0/monobit/formats/bmfont.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ..struct import little_endian as le
 from ..properties import Props, reverse_dict
 from ..storage import loaders, savers
 from ..font import Font, Coord
 from ..glyph import Glyph
 from ..labels import Codepoint, Char
 from ..chart import grid_map
+from ..glyphmap import GlyphMap
 
 from .windows import CHARSET_MAP, CHARSET_REVERSE_MAP
 
 
 # text/xml/binary format: https://www.angelcode.com/products/bmfont/doc/file_format.html
 # json format: https://github.com/Jam3/load-bmfont/blob/master/json-spec.md
 
@@ -693,15 +694,15 @@
         )
     else:
         # crop glyphs
         glyphs = tuple(_g.reduce() for _g in font.glyphs)
         if size is None:
             n_layers = 4 if packed else 1
             size = _estimate_size(glyphs, n_layers, padding, spacing)
-        glyph_map = _map_glyphs_to_image(
+        glyph_map = spritesheet(
             glyphs, size=size, spacing=spacing, padding=padding,
         )
     # draw images
     sheets = _draw_images(glyph_map, packed, paper, ink, border)
     # save images and record names
     pages = _save_pages(outfile, font, sheets, image_format)
     # create the descriptor data structure
@@ -1003,15 +1004,18 @@
 
 
 ###############################################################################
 # draw spritesheets
 
 def _draw_images(glyph_map, packed, paper, ink, border):
     """Draw images based on glyph map."""
-    images = glyph_map_to_images(glyph_map, paper=paper, ink=ink, border=border)
+    images = glyph_map.to_images(
+        paper=paper, ink=ink, border=border,
+        invert_y=True, transparent=False
+    )
     width, height = images[0].width, images[0].height
     # pack 4 sheets per image in RGBA layers
     if packed:
         # grouper: quartets, fill with empties
         empty = Image.new('L', (width, height), border)
         args = [iter(images)] * 4
         quartets = zip_longest(*args, fillvalue=empty)
@@ -1019,38 +1023,18 @@
             # bmfont channel order is B, G, R, A
             Image.merge('RGBA', (_q[2], _q[1], _q[0], _q[3]))
             for _q in quartets
         )
     return images
 
 
-def glyph_map_to_images(glyph_map, *, paper, ink, border):
-    """Draw images based on glyph map."""
-    paper, ink, border = 0, 255, 32
-    last = max(_entry.sheet for _entry in glyph_map)
-    min_x = min(_entry.x for _entry in glyph_map)
-    min_y = min(_entry.y for _entry in glyph_map)
-    max_x = max(_entry.x + _entry.glyph.width for _entry in glyph_map)
-    max_y = max(_entry.y + _entry.glyph.height for _entry in glyph_map)
-    # we don't need +1 as we already included the width/height of the glyphs
-    # e.g. if I have a 2-pixel wide glyph at x=0, I need a 2-pixel image
-    width, height = max_x - min_x, max_y - min_y
-    images = [Image.new('L', (width, height), border) for _ in range(last+1)]
-    for entry in glyph_map:
-        charimg = Image.new('L', (entry.glyph.width, entry.glyph.height))
-        data = entry.glyph.as_vector(ink, paper)
-        charimg.putdata(data)
-        images[entry.sheet].paste(charimg, (entry.x, entry.y))
-    return images
-
-
 ###############################################################################
 # packed spritesheets
 
-def _map_glyphs_to_image(glyphs, *, size, spacing, padding):
+def spritesheet(glyphs, *, size, spacing, padding):
     """Determine where to draw glyphs in sprite sheets."""
     # sort by area, large to small. keep mapping table
     sorted_glyphs = tuple(sorted(
         enumerate(glyphs),
         key=lambda _p: _p[1].width*_p[1].height,
         reverse=True,
     ))
@@ -1063,15 +1047,15 @@
     spx, spy = spacing
     # ensure sheet is larger than largest glyph
     if any(
             _g.width + spx > use_width or _g.height + spy > use_height
             for _g in glyphs
         ):
         raise ValueError('Image size is too small for largest glyph.')
-    glyph_map = []
+    glyph_map = GlyphMap()
     sheets = []
     while True:
         # output glyphs
         sheets.append(SpriteNode(0, 0, use_width, use_height, depth=0))
         for number, glyph in enumerate(glyphs):
             if glyph.height and glyph.width:
                 for i, sheet in enumerate(sheets):
@@ -1080,22 +1064,22 @@
                         break
                     except (FullError, DoesNotFitError):
                         pass
                 else:
                     # we don't fit, get next sheet
                     glyphs = glyphs[number:]
                     break
-            glyph_map.append(Props(
-                glyph=glyph, sheet=i, x=x+padding.left, y=y+padding.top,
-            ))
+            glyph_map.append_glyph(
+                glyph, x+padding.left, y+padding.top, sheet=i
+            )
         else:
             # all done, get out
             break
     # put chars in original glyph order
-    glyph_map = [glyph_map[order_mapping[_i]] for _i in range(len(glyph_map))]
+    glyph_map.reorder(order_mapping)
     return glyph_map
 
 
 def _estimate_size(glyphs, n_layers, padding, spacing):
     """Estimate required size of sprite sheet."""
     max_width = max(_g.width for _g in glyphs)
     max_height = max(_g.height for _g in glyphs)
```

### Comparing `monobit-0.40.4/monobit/formats/borland.py` & `monobit-0.41.0/monobit/formats/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/cpi.py` & `monobit-0.41.0/monobit/formats/cpi.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/daisydot.py` & `monobit-0.41.0/monobit/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/dashen.py` & `monobit-0.41.0/monobit/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/dec.py` & `monobit-0.41.0/monobit/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/dosstart.py` & `monobit-0.41.0/monobit/formats/dosstart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/figlet.py` & `monobit-0.41.0/monobit/formats/figlet.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/fontx.py` & `monobit-0.41.0/monobit/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/fzx.py` & `monobit-0.41.0/monobit/formats/fzx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/gdos.py` & `monobit-0.41.0/monobit/formats/gdos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/geos.py` & `monobit-0.41.0/monobit/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/hurt.py` & `monobit-0.41.0/monobit/formats/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/image.py` & `monobit-0.41.0/monobit/formats/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from ..basetypes import Coord, RGB
 from ..binary import ceildiv
 from ..storage import loaders, savers
 from ..magic import FileFormatError
 from ..font import Font
 from ..glyph import Glyph
 from ..chart import chart, grid_traverser
-from ..canvas import Canvas
 
 
 DEFAULT_IMAGE_FORMAT = 'png'
 
 
 # available background policies
 # -----------------------------
@@ -256,35 +255,14 @@
         codepoint_range: first and last codepoint to include (includes bounds and undefined codepoints; default: all codepoints)
         """
         if len(fonts) > 1:
             raise FileFormatError('Can only save one font to image file.')
         font = fonts[0]
         font = font.stretch(*scale)
         glyph_map = chart(font, columns, margin, padding, order, direction, codepoint_range)
-        img, = glyph_map_to_images(glyph_map, border=border, paper=paper, ink=ink)
+        img, = glyph_map.to_images(
+            border=border, paper=paper, ink=ink, transparent=False
+        )
         try:
             img.save(outfile, format=image_format or Path(outfile).suffix[1:])
         except (KeyError, ValueError, TypeError):
             img.save(outfile, format=DEFAULT_IMAGE_FORMAT)
-
-
-#FIXME merge with bmfont
-def glyph_map_to_images(glyph_map, *, paper, ink, border):
-    """Draw images based on glyph map."""
-    paper, ink, border = 0, 255, 32
-    last = max(_entry.sheet for _entry in glyph_map)
-    min_x = min(_entry.x for _entry in glyph_map)
-    min_y = min(_entry.y for _entry in glyph_map)
-    max_x = max(_entry.x + _entry.glyph.width for _entry in glyph_map)
-    max_y = max(_entry.y + _entry.glyph.height for _entry in glyph_map)
-    # we don't need +1 as we already included the width/height of the glyphs
-    # e.g. if I have a 2-pixel wide glyph at x=0, I need a 2-pixel image
-    width, height = max_x - min_x, max_y - min_y
-    images = [Image.new('L', (width, height), border) for _ in range(last+1)]
-    for entry in glyph_map:
-        charimg = Image.new('L', (entry.glyph.width, entry.glyph.height))
-        data = entry.glyph.as_vector(ink, paper)
-        charimg.putdata(data)
-        # Image has ttb y coords, we have btt
-        # our character origin is bottom left
-        images[entry.sheet].paste(charimg, (entry.x, height-entry.glyph.height-entry.y))
-    return images
```

### Comparing `monobit-0.40.4/monobit/formats/mousegraphics.py` & `monobit-0.41.0/monobit/formats/mousegraphics.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mzfon.py` & `monobit-0.41.0/monobit/formats/mzfon.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/nearlyraw.py` & `monobit-0.41.0/monobit/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/palm.py` & `monobit-0.41.0/monobit/formats/palm.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/pcl.py` & `monobit-0.41.0/monobit/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/pcpaint.py` & `monobit-0.41.0/monobit/formats/pcpaint.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/pdf.py` & `monobit-0.41.0/monobit/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/pkfont.py` & `monobit-0.41.0/monobit/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/printshop.py` & `monobit-0.41.0/monobit/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/psf.py` & `monobit-0.41.0/monobit/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/raw.py` & `monobit-0.41.0/monobit/formats/raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,27 +44,29 @@
 @loaders.register(
     name='raw',
     patterns=('*.814', '.car', '*.64c', '*.udg', '*.ch8', _FXX),
 )
 def load_binary(
         instream, *,
         cell:Coord=NOT_SET, count:int=-1, offset:int=0, padding:int=0,
-        align:str='left', strike_count:int=1, strike_bytes:int=-1,
+        align:str='left', byte_order:str='row-major',
+        strike_count:int=1, strike_bytes:int=-1,
         first_codepoint:int=0
     ):
     """
     Load character-cell font from binary bitmap.
 
     cell: size X,Y of character cell (default: 8x8 or determine from filename)
     offset: number of bytes in file before bitmap starts (default: 0)
     padding: number of bytes between encoded glyph rows (default: 0)
     count: number of glyphs to extract (<= 0 means all; default: all)
     strike_count: number of glyphs in glyph row (<=0 for all; default: 1)
     strike_bytes: strike width in bytes (<=0 means as many as needed to fit the glyphs; default: as needed)
     align: alignment of strike row ('left' for most-, 'right' for least-significant; 'bit' for bit-aligned; default: 'left')
+    byte_order: 'row-major' (default) or 'column-major' byte order (affect cell sizes wider than 8 pixels)
     first_codepoint: first code point in bitmap (default: 0)
     """
     # determine cell size from filename, if not given
     if cell is NOT_SET:
         if Glob('*.814').fits(instream):
             width, height = 8, 14
         elif Glob('*.car').fits(instream):
@@ -83,15 +85,16 @@
             width, height = 8, 8
     else:
         width, height = cell
     # get through the offset
     instream.read(offset)
     return load_bitmap(
         instream, width, height, count, padding, align,
-        strike_count, strike_bytes, first_codepoint
+        strike_count, strike_bytes, first_codepoint,
+        byte_order=byte_order
     )
 
 @savers.register(linked=load_binary)
 def save_binary(
         fonts, outstream, *,
         strike_count:int=1, align:str='left', padding:int=0,
     ):
@@ -110,22 +113,24 @@
 
 
 ###############################################################################
 # bitmap reader
 
 def load_bitmap(
         instream, width, height, count=-1, padding=0, align='left',
-        strike_count=1, strike_bytes=-1, first_codepoint=0,
+        strike_count=1, strike_bytes=-1, first_codepoint=0, *,
+        byte_order='row-major',
     ):
     """Load fixed-width font from bitmap."""
     data, count, cells_per_row, bytes_per_row, nrows = _extract_data_and_geometry(
         instream, width, height, count, padding, strike_count, strike_bytes,
     )
     cells = _extract_cells(
-        data, width, height, align, cells_per_row, bytes_per_row, nrows
+        data, width, height, align, cells_per_row, bytes_per_row, nrows,
+        byte_order=byte_order,
     )
     # reduce to given count, if exceeded
     cells = cells[:count]
     # assign codepoints
     glyphs = tuple(
         Glyph(_cell, codepoint=_index)
         for _index, _cell in enumerate(cells, first_codepoint)
@@ -170,24 +175,25 @@
     data = data.ljust(nrows * row_bytes, b'\0')
     if nrows == 0 or row_bytes == 0:
         return b'', 0, 0, 0, 0
     return data, count, strike_count, row_bytes, nrows
 
 
 def _extract_cells(
-        data, width, height, align, cells_per_row, bytes_per_row, nrows
+        data, width, height, align, cells_per_row, bytes_per_row, nrows, *,
+        byte_order='row-major',
     ):
     """Extract glyphs from bitmap strike with given geometry."""
     # extract one strike row at a time
     # note that the strikes may not be immediately contiguous if there's padding
     glyphrows = (
         Raster.from_bytes(
             data[_i*bytes_per_row : (_i+1)*bytes_per_row],
             width*cells_per_row, height,
-            align=align
+            align=align, byte_order=byte_order,
         )
         for _i in range(nrows)
     )
     # clip out glyphs
     cells = tuple(
         _glyphrow.crop(
             left=_i*width,
```

### Comparing `monobit-0.40.4/monobit/formats/signum.py` & `monobit-0.41.0/monobit/formats/signum.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/svg.py` & `monobit-0.41.0/monobit/formats/svg.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/vfont.py` & `monobit-0.41.0/monobit/formats/vfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/__init__.py` & `monobit-0.41.0/monobit/formats/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/dfont.py` & `monobit-0.41.0/monobit/formats/mac/dfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/fond.py` & `monobit-0.41.0/monobit/formats/mac/fond.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/iigs.py` & `monobit-0.41.0/monobit/formats/mac/iigs.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/lisa.py` & `monobit-0.41.0/monobit/formats/mac/lisa.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/mac/nfnt.py` & `monobit-0.41.0/monobit/formats/mac/nfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/os2/__init__.py` & `monobit-0.41.0/monobit/formats/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/os2/gpifont.py` & `monobit-0.41.0/monobit/formats/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/os2/lx.py` & `monobit-0.41.0/monobit/formats/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/os2/ne.py` & `monobit-0.41.0/monobit/formats/os2/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/sfnt/sfnt.py` & `monobit-0.41.0/monobit/formats/sfnt/sfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/sfnt/sfnt_writer.py` & `monobit-0.41.0/monobit/formats/sfnt/sfnt_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         for _name, _g in glyphs.items()
     }]
     fb.font[tag] = ebdt
 
 
 def convert_to_glyph(glyph, fb, align):
     """Create fontTools bitmap glyph."""
-    if 'vertical' in glyph.features:
+    if glyph.has_vertical_metrics():
         # big metrics
         if align == 'byte':
             format = 6
         else:
             # bit aligned
             format = 7
     else:
@@ -352,15 +352,15 @@
             descender=-font.descent,
             widthMax=font.max_width,
             minOriginSB=min((_g.left_bearing for _g in font.glyphs)),
             minAdvanceSB=min((_g.right_bearing for _g in font.glyphs)),
             maxBeforeBL=max((_g.height + _g.shift_up for _g in font.glyphs)),
             minAfterBL=min((_g.shift_up for _g in font.glyphs)),
         )
-        if 'vertical' in font.get_features():
+        if font.has_vertical_metrics():
             vert = _create_sbit_line_metrics(
                 ascender=font.right_extent,
                 descender=-font.left_extent,
                 widthMax=max((_g.advance_height for _g in font.glyphs), default=0),
                 minOriginSB=min((_g.top_bearing for _g in font.glyphs)),
                 minAdvanceSB=min((_g.bottom_bearing for _g in font.glyphs)),
                 maxBeforeBL=max((_g.shift_left + _g.width//2 for _g in font.glyphs)),
@@ -381,15 +381,14 @@
 
 
 def _prepare_for_sfnt(font, glyph_names):
     """Prepare monobit font for storing in sfnt."""
     # get char labels if we don't have them but we do have an encoding
     font = font.label(match_whitespace=False, match_graphical=False)
     default = font.get_default_glyph()
-    features = font.get_features()
     # we need a name for each glyph to be able to store it
     # if glyph_names == 'tags', must be tagged already
     # otherwise, only glyphs without chars must have names
     if glyph_names != 'tag':
         font = font.label(tag_from=glyph_names or 'truetype', overwrite=True)
         # tag remaining glyphs based on index
         glyphs = (
@@ -406,27 +405,27 @@
             )
             logging.debug(
                 'Dropped glyphs: %s',
                 tuple(_g.get_labels()[0] for _g in dropped if _g.get_labels())
             )
     # cut back to glyph bounding boxes
     font = font.reduce()
-    return font, default, features
+    return font, default
 
 
 
 def _create_sfnt(font, funits_per_em, align, flavour, glyph_names):
     """Convert to a fontTools TTFont object."""
     # converter from pixels to design units
     # note that x and y ppem are equal - if not, fontforge rejects the bitmap
     def _to_funits(pixel_amount):
         return ceildiv(pixel_amount * funits_per_em, font.pixel_size)
 
     check_fonttools()
-    font, default, features = _prepare_for_sfnt(font, glyph_names)
+    font, default = _prepare_for_sfnt(font, glyph_names)
     # get the storable glyphs
     glyphnames = ('.notdef', *(_t.value for _t in font.get_tags()))
     glyphs = {
         _name: font.get_glyph(tag=_name, missing=default)
         for _name in glyphnames
     }
     # build font object
@@ -438,15 +437,15 @@
     _setup_eblc_table(fb, font, flavour)
     if flavour == 'ms':
         _setup_ebsc_table(fb, {font.pixel_size: EBSC_SIZES})
     if flavour != 'apple':
         fb.setupHorizontalMetrics(_convert_to_hmtx_props(glyphs, _to_funits))
         fb.setupHorizontalHeader(**_convert_to_hhea_props(font, _to_funits))
         # check for vertical metrics, include `vhea` and `vmtx` if present
-        if 'vertical' in features:
+        if font.has_vertical_metrics():
             fb.setupVerticalMetrics(_convert_to_vmtx_props(glyphs, _to_funits))
             fb.setupVerticalHeader(**_convert_to_vhea_props(font, _to_funits))
     fb.setupNameTable(_convert_to_name_props(font))
     if flavour != 'apple':
         fb.setupOS2(**_convert_to_os_2_props(font, _to_funits))
     # for otb: version-3 table, defines no names
     fb.setupPost(
```

### Comparing `monobit-0.40.4/monobit/formats/sfnt/fonttools/E_B_S_C_.py` & `monobit-0.41.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/sfnt/fonttools/__init__.py` & `monobit-0.41.0/monobit/formats/sfnt/fonttools/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/text/draw.py` & `monobit-0.41.0/monobit/formats/text/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,53 +9,58 @@
 import string
 
 from ...storage import loaders, savers
 from ...font import Font
 from ...glyph import Glyph
 from ...labels import Tag, Char
 from ...magic import FileFormatError
+from ...encoding import charmaps
+from ...binary import align
 
 
 ##############################################################################
 # hexdraw
 
 @loaders.register(
     name='hexdraw',
     patterns=('*.draw',),
 )
-def load_hexdraw(instream, ink:str='#', paper:str='-'):
+def load_hexdraw(instream, ink:str='#', paper:str='-', unicode:bool=True):
     """
     Load font from a hexdraw file.
 
     ink: character used for inked/foreground pixels (default #)
     paper: character used for uninked/background pixels (default -)
+    unicode: interpret codepoint as Unicode (default: True)
     """
     DrawGlyph.ink = ink
     DrawGlyph.paper = paper
     return _load_draw(
-        instream.text, blocktypes=(DrawGlyph, DrawComment, Empty)
+        instream.text, blocktypes=(DrawGlyph, DrawComment, Empty),
+        unicode=unicode
     )
 
 
 @savers.register(linked=load_hexdraw)
-def save_hexdraw(fonts, outstream, ink:str='#', paper:str='-'):
+def save_hexdraw(fonts, outstream, ink:str='#', paper:str='-', unicode:bool=True):
     """
     Save font to a hexdraw file.
 
     ink: character to use for inked/foreground pixels (default #)
     paper: character to use for uninked/background pixels (default -)
+    unicode: use unicode char labels for codepoints (default: True)
     """
     if len(fonts) > 1:
         raise FileFormatError("Can only save one font to hexdraw file.")
-    _save_draw(fonts[0], outstream.text, ink=ink, paper=paper)
+    _save_draw(fonts[0], outstream.text, ink=ink, paper=paper, unicode=unicode)
 
 
 # read hexdraw file
 
-def _load_draw(text_stream, *, blocktypes):
+def _load_draw(text_stream, *, blocktypes, unicode):
     """Parse a hexdraw-style file."""
     glyphs = []
     font_comments = []
     current_comment = []
     for block in iter_blocks(text_stream, blocktypes):
         if isinstance(block, DrawComment):
             if not glyphs:
@@ -69,47 +74,61 @@
             glyphs.append(block.get_value().modify(
                 comment='\n\n'.join(current_comment),
             ))
             current_comment = []
         elif isinstance(block, Unparsed):
             logging.debug('Unparsed lines: %s', block.get_value())
     font_comments.extend(current_comment)
-    return Font(
+    if not unicode:
+        glyphs = tuple(
+            _g.label(codepoint_from=charmaps['unicode']).modify(char=None)
+            for _g in glyphs
+        )
+    font = Font(
         glyphs,
         comment='\n\n'.join(font_comments)
     )
 
+    return font
+
 
 # write hexdraw file
 
-def _save_draw(font, outstream, *, ink, paper):
+def _save_draw(font, outstream, *, ink, paper, unicode):
     """Write one font to a plaintext stream as hexdraw."""
     font = font.equalise_horizontal()
-    # ensure char labels are set
-    font = font.label(char_from=font.encoding, match_whitespace=False, match_graphical=False)
+    if unicode:
+        # ensure char labels are set
+        font = font.label(char_from=font.encoding, match_whitespace=False, match_graphical=False)
     # write global comment
     if font.get_comment():
         outstream.write(
             format_comment(font.get_comment(), comment_char='%') + '\n'
         )
     # write glyphs
     for i, glyph in enumerate(font.glyphs):
-        if not glyph.char:
+        if unicode:
+            char = glyph.char
+        else:
+            cpbytes = bytes(glyph.codepoint)
+            cpbytes = cpbytes.rjust(align(len(cpbytes), 2), b'\0')
+            char = cpbytes.decode('utf-32-be')
+        if not char:
             logging.warning(
                 "Can't encode glyph without Unicode character label in .draw file;"
                 " skipping index %d", i
             )
-        elif len(glyph.char) > 1:
+        elif len(char) > 1:
             logging.warning(
                 "Can't encode grapheme cluster %s in .draw file; skipping.",
-                ascii(glyph.char)
+                ascii(char)
             )
         else:
             glyphtxt = glyph.as_text(start='\t', ink=ink, paper=paper, end='\n')
-            outstream.write(f'\n{ord(glyph.char):04x}:')
+            outstream.write(f'\n{ord(char):04x}:')
             outstream.write(glyphtxt)
 
 
 def format_comment(comments, comment_char):
     """Format a multiline comment."""
     return '\n'.join(
         f'{comment_char} {_line}'
```

### Comparing `monobit-0.40.4/monobit/formats/text/hex.py` & `monobit-0.41.0/monobit/formats/text/hex.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 # loader
 
 def _load_hex(instream):
     """Load 8x16 multi-cell font from Unifont .HEX file."""
     return _load_draw(
-        instream.text, blocktypes=(HexGlyph, DrawComment, Empty)
+        instream.text, blocktypes=(HexGlyph, DrawComment, Empty), unicode=True
     )
 
 
 class HexGlyph(DrawGlyph):
 
     def ends(self, line):
         # single line per glyph
```

### Comparing `monobit-0.40.4/monobit/formats/text/yaff.py` & `monobit-0.41.0/monobit/formats/text/yaff.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,16 +165,22 @@
             font_comments.extend(current_comment)
             current_comment = []
         if isinstance(block, YaffComment):
             current_comment.append(block.get_value())
         elif not isinstance(block, (YaffProperty, YaffGlyph, YaffPropertyOrGlyph)):
             logging.debug('Unparsed lines: %s', block.get_value())
     font_comments.extend(current_comment)
+    # construct glyphs, including path-only glyphs
+    glyphs = (
+        Glyph(**vars(_g)) if _g.pixels or not hasattr(_g, 'path')
+        else Glyph.from_path(**vars(_g - 'pixels'))
+        for _g in glyphs
+    )
     return Font(
-        (Glyph(**vars(_g)) for _g in glyphs), **font_props,
+        glyphs, **font_props,
         comment={'': '\n\n'.join(font_comments), **font_prop_comms},
     )
 
 
 class YaffComment(DrawComment):
 
     def starts(self, line):
```

### Comparing `monobit-0.40.4/monobit/formats/windows/LICENSE.md` & `monobit-0.41.0/monobit/formats/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/windows/__init__.py` & `monobit-0.41.0/monobit/formats/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/windows/fnt.py` & `monobit-0.41.0/monobit/formats/windows/fnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/windows/mz.py` & `monobit-0.41.0/monobit/formats/windows/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/windows/ne.py` & `monobit-0.41.0/monobit/formats/windows/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/windows/pe.py` & `monobit-0.41.0/monobit/formats/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/monobit/formats/xlfd/hbf.py` & `monobit-0.41.0/monobit/formats/xlfd/hbf.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 from ...storage import loaders, savers
 from ...magic import FileFormatError
 from ...font import Font, Coord
 from ...glyph import Glyph
 from ...binary import ceildiv
 
-from .bdf import read_props, _parse_xlfd_properties, _create_xlfd_properties
-from .bdf import _create_xlfd_name
+from .bdf import read_props
+from .xlfd import _parse_xlfd_properties, _create_xlfd_properties
+from .xlfd import _create_xlfd_name
 # from ..text.yaff import _globalise_glyph_metrics
 from ..windows import _normalise_metrics
 
 
 @loaders.register(
     name='hbf',
     magic=(b'HBF_START_FONT ',),
```

### Comparing `monobit-0.40.4/monobit/scripts/banner.py` & `monobit-0.41.0/monobit/scripts/banner.py`

 * *Files 9% similar despite different names*

```diff
@@ -210,43 +210,43 @@
             transformations.append((Font.shear, (), {}))
         if args.underline:
             transformations.append((Font.underline, (), {}))
         if args.outline:
             transformations.append((Font.outline, (), {}))
         #######################################################################
         # render
-        canvas = render(
+        glyph_map = render(
             font, args.text,
             margin=args.margin,
             direction=args.direction, align=args.align, adjust_bearings=args.expand,
             missing='default',
             transformations=transformations,
         )
         # transformations
-        canvas = canvas.stretch(*args.scale)
-        canvas = canvas.turn(clockwise=args.rotate)
+        glyph_map.stretch(*args.scale)
+        glyph_map.turn(clockwise=args.rotate)
         #######################################################################
         # output
         if args.image or args.output and not args.output.endswith('.txt'):
             ink = RGB.create(args.ink or (0, 0, 0))
             paper = RGB.create(args.paper or (255, 255, 255))
             border = RGB.create(args.border) if args.border else paper
-            image = canvas.as_image(ink=ink, paper=paper, border=border)
+            image = glyph_map.as_image(ink=ink, paper=paper, border=border)
             if args.output:
                 image.save(args.output)
             else:
                 image.show()
         else:
             if args.blocks:
-                text = canvas.as_blocks()
+                text = glyph_map.as_blocks()
             else:
                 ink = args.ink or '@'
                 paper = args.paper or '.'
                 border = args.border or paper
-                text = canvas.as_text(ink=ink, paper=paper, border=border) + '\n'
+                text = glyph_map.as_text(ink=ink, paper=paper, border=border) + '\n'
             if not args.output:
                 sys.stdout.write(text)
             else:
                 with open(args.output, 'w') as outfile:
                     outfile.write(text)
```

### Comparing `monobit-0.40.4/monobit/scripts/convert.py` & `monobit-0.41.0/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/LICENSE` & `monobit-0.41.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.40.4/README.md` & `monobit-0.41.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,20 @@
 
 
 Supported bitmap formats
 ------------------------
 
 | Format                | Short Name | Typical Extension           | Read  | Write |
 |-----------------------|------------|-----------------------------|-------|-------|
+| Xerox Alto CONVERT    | `alto`     | `.al`                       | ✔     |       |
 | Amiga Font Contents   | `amiga-fc` | `.font`                     | ✔     |       |
 | Amiga font            | `amiga`    |                             | ✔     |       |
 | BBC soft font         | `bbc`      |                             | ✔     | ✔     |
 | X11/Adobe BDF         | `bdf`      | `.bdf`                      | ✔     | ✔     |
+| Xerox Alto BITBLT     | `bitblt`   | `.strike` `.ks`             | ✔     |       |
 | AngelCode BMFont [P]  | `bmfont` | `.fnt` `.xml` `.json` + images | ✔    | ✔     |
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           | ✔     | ✔     |
 | Codepage Information  | `cpi`      | `.cpi`                      | ✔     | ✔     |
 | Consoleet / vfontas   | `consoleet`| `.txt`                      | ✔     |       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` | ✔     |       |
 | Dashen                | `dashen`   | `.pft`                      | ✔     |       |
 | DEC DRCS soft font    | `dec`      |                             | ✔     | ✔     |
@@ -119,21 +121,24 @@
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
 | MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
 | mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
+| X11 Portable Compiled Format |  `pcf` | `.pcf`                   | ✔     | ✔     |
+| Xerox Alto PrePress   | `prepress` | `.ac`                       | ✔     |       |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
 | PCPaint, GRASP, ChiWriter | `pcpaint` | `.set` `.fnt`  `.sft` `.pft` `.eft` ... | ✔ |  |
 | PDF chart [R]         | `pdf`      | `.pdf`                      |       | ✔     |
 | TeX PKFONT            | `pkfont`   | `.pk`                       | ✔     |       |
+| Adobe Prebuilt Format | `prebuilt` | `.bepf` `.lepf`             | ✔     |       |
 | The Print Shop        | `printshop`| `.pnf`                      | ✔     |       |
 | PC Screen Font        | `psf`      | `.psf` `.psfu`              | ✔     | ✔ (version 2) |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | PSF2TXT               | `psf2txt`  | `.txt`                      | ✔     |       |
 | Signum! 2             | `signum`   | `.e24` `.p9` `.p24` `.l30`  | ✔     |       |
 | SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   | ✔ (OTB) |
 | SFNT collection       | `ttcf`     | `.otc` `.ttc` [F] [**]      | ✔     | ✔ (OTB) |
@@ -306,18 +311,20 @@
 
 `monobit` would not exist without those documenting,
 reverse-engineering, implementing and preserving font formats and files:
 - [The Internet Archive](https://archive.org)
 - [Archive Team](http://fileformats.archiveteam.org/wiki/Fonts)
 - [Jason Scott's textfiles.com](http://textfiles.com)
 - [John Elliott's homepage](http://www.seasip.info)
-- [Simon Tatham's fonts page](https://www.chiark.greenend.org.uk/~sgtatham/fonts/):
+- [Simon Tatham's fonts page](https://www.chiark.greenend.org.uk/~sgtatham/fonts/)
 - [Aivosto's character set documentation](https://www.aivosto.com/articles/charsets.html)
 - [Rebecca Bettencourt's character set documentation](https://www.kreativekorp.com/charset/)
 - [Xiphoseer's Signum Document Toolbox](https://sdo.dseiler.eu/)
+- [George Williams et al.'s FontForge documentation](https://fontforge.org/docs/index.html)
+- [FreeType Glyph Conventions](https://freetype.org/freetype2/docs/glyphs/index.html)
 - ... and many others
 
 
 Other software
 --------------
 
 Other bitmap font tools you could use in conjunction with (or instead of) `monobit` include:
```

### Comparing `monobit-0.40.4/pyproject.toml` & `monobit-0.41.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.40.4"
+version = "0.41.0"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.40.4/PKG-INFO` & `monobit-0.41.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monobit
-Version: 0.40.4
+Version: 0.41.0
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
         
@@ -127,18 +127,20 @@
 
 
 Supported bitmap formats
 ------------------------
 
 | Format                | Short Name | Typical Extension           | Read  | Write |
 |-----------------------|------------|-----------------------------|-------|-------|
+| Xerox Alto CONVERT    | `alto`     | `.al`                       | ✔     |       |
 | Amiga Font Contents   | `amiga-fc` | `.font`                     | ✔     |       |
 | Amiga font            | `amiga`    |                             | ✔     |       |
 | BBC soft font         | `bbc`      |                             | ✔     | ✔     |
 | X11/Adobe BDF         | `bdf`      | `.bdf`                      | ✔     | ✔     |
+| Xerox Alto BITBLT     | `bitblt`   | `.strike` `.ks`             | ✔     |       |
 | AngelCode BMFont [P]  | `bmfont` | `.fnt` `.xml` `.json` + images | ✔    | ✔     |
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           | ✔     | ✔     |
 | Codepage Information  | `cpi`      | `.cpi`                      | ✔     | ✔     |
 | Consoleet / vfontas   | `consoleet`| `.txt`                      | ✔     |       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` | ✔     |       |
 | Dashen                | `dashen`   | `.pft`                      | ✔     |       |
 | DEC DRCS soft font    | `dec`      |                             | ✔     | ✔     |
@@ -161,21 +163,24 @@
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
 | MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
 | mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
+| X11 Portable Compiled Format |  `pcf` | `.pcf`                   | ✔     | ✔     |
+| Xerox Alto PrePress   | `prepress` | `.ac`                       | ✔     |       |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
 | PCPaint, GRASP, ChiWriter | `pcpaint` | `.set` `.fnt`  `.sft` `.pft` `.eft` ... | ✔ |  |
 | PDF chart [R]         | `pdf`      | `.pdf`                      |       | ✔     |
 | TeX PKFONT            | `pkfont`   | `.pk`                       | ✔     |       |
+| Adobe Prebuilt Format | `prebuilt` | `.bepf` `.lepf`             | ✔     |       |
 | The Print Shop        | `printshop`| `.pnf`                      | ✔     |       |
 | PC Screen Font        | `psf`      | `.psf` `.psfu`              | ✔     | ✔ (version 2) |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | PSF2TXT               | `psf2txt`  | `.txt`                      | ✔     |       |
 | Signum! 2             | `signum`   | `.e24` `.p9` `.p24` `.l30`  | ✔     |       |
 | SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   | ✔ (OTB) |
 | SFNT collection       | `ttcf`     | `.otc` `.ttc` [F] [**]      | ✔     | ✔ (OTB) |
@@ -348,18 +353,20 @@
 
 `monobit` would not exist without those documenting,
 reverse-engineering, implementing and preserving font formats and files:
 - [The Internet Archive](https://archive.org)
 - [Archive Team](http://fileformats.archiveteam.org/wiki/Fonts)
 - [Jason Scott's textfiles.com](http://textfiles.com)
 - [John Elliott's homepage](http://www.seasip.info)
-- [Simon Tatham's fonts page](https://www.chiark.greenend.org.uk/~sgtatham/fonts/):
+- [Simon Tatham's fonts page](https://www.chiark.greenend.org.uk/~sgtatham/fonts/)
 - [Aivosto's character set documentation](https://www.aivosto.com/articles/charsets.html)
 - [Rebecca Bettencourt's character set documentation](https://www.kreativekorp.com/charset/)
 - [Xiphoseer's Signum Document Toolbox](https://sdo.dseiler.eu/)
+- [George Williams et al.'s FontForge documentation](https://fontforge.org/docs/index.html)
+- [FreeType Glyph Conventions](https://freetype.org/freetype2/docs/glyphs/index.html)
 - ... and many others
 
 
 Other software
 --------------
 
 Other bitmap font tools you could use in conjunction with (or instead of) `monobit` include:
```

