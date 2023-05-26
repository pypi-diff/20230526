# Comparing `tmp/xspf_lib-0.3.2.tar.gz` & `tmp/xspf_lib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf_lib-0.3.2.tar", last modified: Sat May 20 23:10:55 2023, max compression
+gzip compressed data, was "xspf_lib-0.3.3.tar", last modified: Fri May 26 09:46:40 2023, max compression
```

## Comparing `xspf_lib-0.3.2.tar` & `xspf_lib-0.3.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     1072 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/LICENSE
--rw-r--r--   0        0        0     3321 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/README.rst
--rw-r--r--   0        0        0     1262 2023-05-20 23:10:55.671792 xspf_lib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     6946 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/test_module.py
--rw-r--r--   0        0        0     3523 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/test_testcases_fail_validation.py
--rw-r--r--   0        0        0     8113 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/test_testcases_pass_validation.py
--rw-r--r--   0        0        0      260 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/test_uri.py
--rw-r--r--   0        0        0      126 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/README.txt
--rw-r--r--   0        0        0      198 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-attribute-forbidden-annotation.xspf
--rw-r--r--   0        0        0      149 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-attribute-forbidden-playlist.xspf
--rw-r--r--   0        0        0      382 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-baddate.xspf
--rw-r--r--   0        0        0      237 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-badversion.xspf
--rw-r--r--   0        0        0      190 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-element-forbidden-attribution.xspf
--rw-r--r--   0        0        0      159 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-extension-application-missing.xspf
--rw-r--r--   0        0        0      153 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-link-rel-missing.xspf
--rw-r--r--   0        0        0      323 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-markup-annotation.xspf
--rw-r--r--   0        0        0      314 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-markup-creator.xspf
--rw-r--r--   0        0        0      331 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-markup-meta.xspf
--rw-r--r--   0        0        0      308 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-markup-title.xspf
--rw-r--r--   0        0        0      153 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-meta-rel-missing.xspf
--rw-r--r--   0        0        0      232 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-missingtracklist.xspf
--rw-r--r--   0        0        0      182 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-missingversion.xspf
--rw-r--r--   0        0        0      199 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-namespace-missing.xspf
--rw-r--r--   0        0        0      289 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-namespace-nested-broken.xspf
--rw-r--r--   0        0        0      381 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-namespace-wrong-string.xspf
--rw-r--r--   0        0        0      120 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-nonleaf-content-attribution.xspf
--rw-r--r--   0        0        0       93 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-nonleaf-content-playlist.xspf
--rw-r--r--   0        0        0      100 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-nonleaf-content-trackList.xspf
--rw-r--r--   0        0        0      127 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-root-name.xspf
--rw-r--r--   0        0        0      313 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-annotation.xspf
--rw-r--r--   0        0        0      279 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-attribution.xspf
--rw-r--r--   0        0        0      299 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-creator.xspf
--rw-r--r--   0        0        0      320 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-date.xspf
--rw-r--r--   0        0        0      336 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-identifier.xspf
--rw-r--r--   0        0        0      311 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-image.xspf
--rw-r--r--   0        0        0      330 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-info.xspf
--rw-r--r--   0        0        0      321 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-license.xspf
--rw-r--r--   0        0        0      350 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-location.xspf
--rw-r--r--   0        0        0      289 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-title.xspf
--rw-r--r--   0        0        0      257 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/playlist-toomany-tracklist.xspf
--rw-r--r--   0        0        0      370 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-badint-duration.xspf
--rw-r--r--   0        0        0      370 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-badint-tracknum.xspf
--rw-r--r--   0        0        0      194 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-extension-application-missing.xspf
--rw-r--r--   0        0        0      188 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-link-rel-missing.xspf
--rw-r--r--   0        0        0      316 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-markup-album.xspf
--rw-r--r--   0        0        0      336 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-markup-annotation.xspf
--rw-r--r--   0        0        0      324 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-markup-creator.xspf
--rw-r--r--   0        0        0      338 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-markup-meta.xspf
--rw-r--r--   0        0        0      316 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-markup-title.xspf
--rw-r--r--   0        0        0      188 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-meta-rel-missing.xspf
--rw-r--r--   0        0        0      123 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-nonleaf-content.xspf
--rw-r--r--   0        0        0      342 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-album.xspf
--rw-r--r--   0        0        0      372 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-annotation.xspf
--rw-r--r--   0        0        0      354 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-creator.xspf
--rw-r--r--   0        0        0      352 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-duration.xspf
--rw-r--r--   0        0        0      364 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-image.xspf
--rw-r--r--   0        0        0      358 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-info.xspf
--rw-r--r--   0        0        0      342 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-title.xspf
--rw-r--r--   0        0        0      352 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/fail/track-toomany-tracknum.xspf
--rw-r--r--   0        0        0      605 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf
--rw-r--r--   0        0        0      137 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-empty-annotation.xspf
--rw-r--r--   0        0        0      134 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-empty-creator.xspf
--rw-r--r--   0        0        0      157 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-empty-meta.xspf
--rw-r--r--   0        0        0      132 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-empty-title.xspf
--rw-r--r--   0        0        0      379 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-extension.xspf
--rw-r--r--   0        0        0     3342 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-extensive.xspf
--rw-r--r--   0        0        0      869 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-inverted-order.xspf
--rw-r--r--   0        0        0      250 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-namespace-nested-proper.xspf
--rw-r--r--   0        0        0      139 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-namespace-nondefault.xspf
--rw-r--r--   0        0        0      205 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-namespace-two-additions.xspf
--rw-r--r--   0        0        0      336 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-attribution-identifier.xspf
--rw-r--r--   0        0        0      330 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-attribution-location.xspf
--rw-r--r--   0        0        0      317 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-extension.xspf
--rw-r--r--   0        0        0      298 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-identifier.xspf
--rw-r--r--   0        0        0      283 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-image.xspf
--rw-r--r--   0        0        0      280 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-info.xspf
--rw-r--r--   0        0        0      289 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-license.xspf
--rw-r--r--   0        0        0      305 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-link-content.xspf
--rw-r--r--   0        0        0      314 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-link-rel.xspf
--rw-r--r--   0        0        0      292 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-location.xspf
--rw-r--r--   0        0        0      303 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-noturi-meta.xspf
--rw-r--r--   0        0        0      572 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-relative-paths.xspf
--rw-r--r--   0        0        0      162 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-whitespace-dateTime.xspf
--rw-r--r--   0        0        0     1543 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-xml-base.xspf
--rw-r--r--   0        0        0      174 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-empty-album.xspf
--rw-r--r--   0        0        0      179 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-empty-annotation.xspf
--rw-r--r--   0        0        0      176 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-empty-creator.xspf
--rw-r--r--   0        0        0      199 2023-05-20 23:10:36.723666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-empty-meta.xspf
--rw-r--r--   0        0        0      174 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-empty-title.xspf
--rw-r--r--   0        0        0      320 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-extension.xspf
--rw-r--r--   0        0        0     4160 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-extensive.xspf
--rw-r--r--   0        0        0      917 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-inverted-order.xspf
--rw-r--r--   0        0        0      342 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-extension.xspf
--rw-r--r--   0        0        0      329 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-identifier.xspf
--rw-r--r--   0        0        0      309 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-image.xspf
--rw-r--r--   0        0        0      305 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-info.xspf
--rw-r--r--   0        0        0      353 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-link-rel.xspf
--rw-r--r--   0        0        0      330 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-link.xspf
--rw-r--r--   0        0        0      321 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-location.xspf
--rw-r--r--   0        0        0      342 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-noturi-meta-rel.xspf
--rw-r--r--   0        0        0      412 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-whitespace-anyURI.xspf
--rw-r--r--   0        0        0      414 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-whitespace-in-between.xspf
--rw-r--r--   0        0        0      326 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/tests/testcase/version_1/pass/track-whitespace-nonNegativeInteger.xspf
--rw-r--r--   0        0        0      353 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/__init__.py
--rw-r--r--   0        0        0      268 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/base.py
--rw-r--r--   0        0        0     4437 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/builders.py
--rw-r--r--   0        0        0      386 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/constants.py
--rw-r--r--   0        0        0    14039 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/elements.py
--rw-r--r--   0        0        0    13174 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/parsers.py
--rw-r--r--   0        0        0      358 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/types.py
--rw-r--r--   0        0        0      604 2023-05-20 23:10:36.727666 xspf_lib-0.3.2/xspf_lib/utils.py
--rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 xspf_lib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-26 09:46:21.995764 xspf_lib-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3408 2023-05-26 09:46:21.995764 xspf_lib-0.3.3/README.rst
+-rw-r--r--   0        0        0     1345 2023-05-26 09:46:40.551542 xspf_lib-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     6946 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_module.py
+-rw-r--r--   0        0        0     3523 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_testcases_fail_validation.py
+-rw-r--r--   0        0        0     8113 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_testcases_pass_validation.py
+-rw-r--r--   0        0        0      260 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_uri.py
+-rw-r--r--   0        0        0      126 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/README.txt
+-rw-r--r--   0        0        0      198 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-attribute-forbidden-annotation.xspf
+-rw-r--r--   0        0        0      149 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-attribute-forbidden-playlist.xspf
+-rw-r--r--   0        0        0      382 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-baddate.xspf
+-rw-r--r--   0        0        0      237 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-badversion.xspf
+-rw-r--r--   0        0        0      190 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-element-forbidden-attribution.xspf
+-rw-r--r--   0        0        0      159 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-extension-application-missing.xspf
+-rw-r--r--   0        0        0      153 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-link-rel-missing.xspf
+-rw-r--r--   0        0        0      323 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-annotation.xspf
+-rw-r--r--   0        0        0      314 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-creator.xspf
+-rw-r--r--   0        0        0      331 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-meta.xspf
+-rw-r--r--   0        0        0      308 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-title.xspf
+-rw-r--r--   0        0        0      153 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      232 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-missingtracklist.xspf
+-rw-r--r--   0        0        0      182 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-missingversion.xspf
+-rw-r--r--   0        0        0      199 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-missing.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-nested-broken.xspf
+-rw-r--r--   0        0        0      381 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-wrong-string.xspf
+-rw-r--r--   0        0        0      120 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-attribution.xspf
+-rw-r--r--   0        0        0       93 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-playlist.xspf
+-rw-r--r--   0        0        0      100 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-trackList.xspf
+-rw-r--r--   0        0        0      127 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-root-name.xspf
+-rw-r--r--   0        0        0      313 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-annotation.xspf
+-rw-r--r--   0        0        0      279 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-attribution.xspf
+-rw-r--r--   0        0        0      299 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-creator.xspf
+-rw-r--r--   0        0        0      320 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-date.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-identifier.xspf
+-rw-r--r--   0        0        0      311 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-image.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-info.xspf
+-rw-r--r--   0        0        0      321 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-license.xspf
+-rw-r--r--   0        0        0      350 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-location.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-title.xspf
+-rw-r--r--   0        0        0      257 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-tracklist.xspf
+-rw-r--r--   0        0        0      370 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-badint-duration.xspf
+-rw-r--r--   0        0        0      370 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-badint-tracknum.xspf
+-rw-r--r--   0        0        0      194 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-extension-application-missing.xspf
+-rw-r--r--   0        0        0      188 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-link-rel-missing.xspf
+-rw-r--r--   0        0        0      316 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-album.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-annotation.xspf
+-rw-r--r--   0        0        0      324 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-creator.xspf
+-rw-r--r--   0        0        0      338 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-meta.xspf
+-rw-r--r--   0        0        0      316 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-title.xspf
+-rw-r--r--   0        0        0      188 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      123 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-nonleaf-content.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-album.xspf
+-rw-r--r--   0        0        0      372 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-annotation.xspf
+-rw-r--r--   0        0        0      354 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-creator.xspf
+-rw-r--r--   0        0        0      352 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-duration.xspf
+-rw-r--r--   0        0        0      364 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-image.xspf
+-rw-r--r--   0        0        0      358 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-info.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-title.xspf
+-rw-r--r--   0        0        0      352 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-tracknum.xspf
+-rw-r--r--   0        0        0      605 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf
+-rw-r--r--   0        0        0      137 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-annotation.xspf
+-rw-r--r--   0        0        0      134 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-creator.xspf
+-rw-r--r--   0        0        0      157 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-meta.xspf
+-rw-r--r--   0        0        0      132 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-title.xspf
+-rw-r--r--   0        0        0      379 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extension.xspf
+-rw-r--r--   0        0        0     3342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extensive.xspf
+-rw-r--r--   0        0        0      869 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-inverted-order.xspf
+-rw-r--r--   0        0        0      250 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-nested-proper.xspf
+-rw-r--r--   0        0        0      139 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-nondefault.xspf
+-rw-r--r--   0        0        0      205 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-two-additions.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-attribution-identifier.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-attribution-location.xspf
+-rw-r--r--   0        0        0      317 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-extension.xspf
+-rw-r--r--   0        0        0      298 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-identifier.xspf
+-rw-r--r--   0        0        0      283 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-image.xspf
+-rw-r--r--   0        0        0      280 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-info.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-license.xspf
+-rw-r--r--   0        0        0      305 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-link-content.xspf
+-rw-r--r--   0        0        0      314 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      292 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-location.xspf
+-rw-r--r--   0        0        0      303 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-meta.xspf
+-rw-r--r--   0        0        0      572 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-relative-paths.xspf
+-rw-r--r--   0        0        0      162 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-whitespace-dateTime.xspf
+-rw-r--r--   0        0        0     1543 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-xml-base.xspf
+-rw-r--r--   0        0        0      174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-album.xspf
+-rw-r--r--   0        0        0      179 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-annotation.xspf
+-rw-r--r--   0        0        0      176 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-creator.xspf
+-rw-r--r--   0        0        0      199 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-meta.xspf
+-rw-r--r--   0        0        0      174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-title.xspf
+-rw-r--r--   0        0        0      320 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extension.xspf
+-rw-r--r--   0        0        0     4160 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extensive.xspf
+-rw-r--r--   0        0        0      917 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-inverted-order.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-extension.xspf
+-rw-r--r--   0        0        0      329 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-identifier.xspf
+-rw-r--r--   0        0        0      309 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-image.xspf
+-rw-r--r--   0        0        0      305 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-info.xspf
+-rw-r--r--   0        0        0      353 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-link.xspf
+-rw-r--r--   0        0        0      321 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-location.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-meta-rel.xspf
+-rw-r--r--   0        0        0      412 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-anyURI.xspf
+-rw-r--r--   0        0        0      414 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-in-between.xspf
+-rw-r--r--   0        0        0      326 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-nonNegativeInteger.xspf
+-rw-r--r--   0        0        0      353 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/__init__.py
+-rw-r--r--   0        0        0      431 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/base.py
+-rw-r--r--   0        0        0     4434 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/builders.py
+-rw-r--r--   0        0        0      386 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/constants.py
+-rw-r--r--   0        0        0    17089 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/elements.py
+-rw-r--r--   0        0        0    13174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/parsers.py
+-rw-r--r--   0        0        0      377 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/types.py
+-rw-r--r--   0        0        0      604 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/utils.py
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 xspf_lib-0.3.3/PKG-INFO
```

### Comparing `xspf_lib-0.3.2/LICENSE` & `xspf_lib-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/README.rst` & `xspf_lib-0.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 ========
 xspf-lib
 ========
 
 .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
+    :target: https://github.com/dem214/xspf-lib/actions
     :alt: Python package
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
+    :alt: isort
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
+   :alt: black
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
 
 Library to work with xspf.
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 ======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
-workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
-image:: https://img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
-https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
-commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
-commit/pre-commit :alt: pre-commit Library to work with xspf. Requirements ----
--------- * `Python 3.8 or higher
+workflows/Python%20package/badge.svg?branch=master :target: https://github.com/
+dem214/xspf-lib/actions :alt: Python package .. image:: https://img.shields.io/
+badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336 :target: https://
+pycqa.github.io/isort/ :alt: isort .. image:: https://img.shields.io/badge/
+code%20style-black-000000.svg :target: https://github.com/psf/black :alt: black
+.. image:: https://img.shields.io/badge/pre--commit-enabled-
+brightgreen?logo=pre-commit :target: https://github.com/pre-commit/pre-commit :
+alt: pre-commit Library to work with xspf. Requirements ------------ * `Python
+3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
 duration=177000, annotation="#2 in GB 1975", info="https://ru.wikipedia.org/
 wiki/Killer_Queen", image="file:///home/images/killer_queen_cover.png") >>>
```

### Comparing `xspf_lib-0.3.2/pyproject.toml` & `xspf_lib-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xspf-lib"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library for work with xspf format"
 authors = [
     { name = "Dzmitry Izaitka", email = "dem214overlord@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.rst"
@@ -22,14 +22,15 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Source = "https://github.com/dem214/xspf-lib"
 "Bug Tracker" = "https://github.com/dem214/xspf-lib/issues"
+Documentation = "https://xspf-lib.readthedocs.io/"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
@@ -38,14 +39,17 @@
     "pytest>=7.3.1",
 ]
 lint = [
     "flake8>=5.0.4",
     "flake8-pyprojecttoml>=0.0.2",
     "mypy>=1.3.0",
 ]
+docs = [
+    "sphinx>=4.3.2",
+]
 
 [tool.pdm.scripts]
 test = "pytest"
 flake8 = "flake8 xspf_lib"
 mypy = "mypy xspf_lib"
 
 [tool.pdm.scripts.lint]
```

### Comparing `xspf_lib-0.3.2/tests/test_module.py` & `xspf_lib-0.3.3/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/test_testcases_fail_validation.py` & `xspf_lib-0.3.3/tests/test_testcases_fail_validation.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/test_testcases_pass_validation.py` & `xspf_lib-0.3.3/tests/test_testcases_pass_validation.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-extensive.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extensive.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-inverted-order.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-inverted-order.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-relative-paths.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-relative-paths.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/playlist-xml-base.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-xml-base.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/track-extensive.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extensive.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/tests/testcase/version_1/pass/track-inverted-order.xspf` & `xspf_lib-0.3.3/tests/testcase/version_1/pass/track-inverted-order.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/xspf_lib/builders.py` & `xspf_lib-0.3.3/xspf_lib/builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .constants import XML_NAMESPACE
 from .utils import quote
 
 if TYPE_CHECKING:
     from .elements import Playlist, Track
 
 
-class _XML_Builder:
+class _XMLBuilder:
     def __init__(self):
         self.entity: Union["Track", "Playlist", None] = None
 
     def build_track(self, track: "Track"):
         self.entity = track
         self.xml_element = Et.Element("track")
 
@@ -137,12 +137,12 @@
         parameter_iter: Iterable[XMLAble] = getattr(self.entity, parameter_name)
         self.xml_element.extend(
             parameter.to_xml_element() for parameter in parameter_iter
         )
 
 
 def build_track(track: "Track") -> Et.Element:
-    return _XML_Builder().build_track(track)
+    return _XMLBuilder().build_track(track)
 
 
 def build_playlist(playlist: "Playlist") -> Et.Element:
-    return _XML_Builder().build_playlist(playlist)
+    return _XMLBuilder().build_playlist(playlist)
```

### Comparing `xspf_lib-0.3.2/xspf_lib/parsers.py` & `xspf_lib-0.3.3/xspf_lib/parsers.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/xspf_lib/utils.py` & `xspf_lib-0.3.3/xspf_lib/utils.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.2/PKG-INFO` & `xspf_lib-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: xspf-lib
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for work with xspf format
 Keywords: xspf playlist
 Author-Email: Dzmitry Izaitka <dem214overlord@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Source, https://github.com/dem214/xspf-lib
 Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues
+Project-URL: Documentation, https://xspf-lib.readthedocs.io/
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 ========
 xspf-lib
 ========
 
 .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
+    :target: https://github.com/dem214/xspf-lib/actions
     :alt: Python package
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
+    :alt: isort
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
+   :alt: black
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
 
 Library to work with xspf.
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.2 Summary: Library for work
+Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.3 Summary: Library for work
 with xspf format Keywords: xspf playlist Author-Email: Dzmitry Izaitka
 gmail.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic
 :: Multimedia :: Video Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Project-URL: Source, https://github.com/dem214/xspf-lib
-Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues Requires-
-Python: >=3.7 Description-Content-Type: text/x-rst ======== xspf-lib ========
-.. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/
-badge.svg?branch=master :alt: Python package .. image:: https://img.shields.io/
-badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336 :target: https://
-pycqa.github.io/isort/ .. image:: https://img.shields.io/badge/code%20style-
-black-000000.svg :target: https://github.com/psf/black .. image:: https://
-img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit :target:
+Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues Project-
+URL: Documentation, https://xspf-lib.readthedocs.io/ Requires-Python: >=3.7
+Description-Content-Type: text/x-rst ======== xspf-lib ======== .. image::
+https://github.com/dem214/xspf-lib/workflows/Python%20package/
+badge.svg?branch=master :target: https://github.com/dem214/xspf-lib/actions :
+alt: Python package .. image:: https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
+:alt: isort .. image:: https://img.shields.io/badge/code%20style-black-
+000000.svg :target: https://github.com/psf/black :alt: black .. image:: https:/
+/img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit :target:
 https://github.com/pre-commit/pre-commit :alt: pre-commit Library to work with
 xspf. Requirements ------------ * `Python 3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
```

