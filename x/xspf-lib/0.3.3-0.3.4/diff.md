# Comparing `tmp/xspf_lib-0.3.3.tar.gz` & `tmp/xspf_lib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf_lib-0.3.3.tar", last modified: Fri May 26 09:46:40 2023, max compression
+gzip compressed data, was "xspf_lib-0.3.4.tar", last modified: Fri May 26 10:31:01 2023, max compression
```

## Comparing `xspf_lib-0.3.3.tar` & `xspf_lib-0.3.4.tar`

### file list

```diff
@@ -1,113 +1,114 @@
--rw-r--r--   0        0        0     1072 2023-05-26 09:46:21.995764 xspf_lib-0.3.3/LICENSE
--rw-r--r--   0        0        0     3408 2023-05-26 09:46:21.995764 xspf_lib-0.3.3/README.rst
--rw-r--r--   0        0        0     1345 2023-05-26 09:46:40.551542 xspf_lib-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     6946 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_module.py
--rw-r--r--   0        0        0     3523 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_testcases_fail_validation.py
--rw-r--r--   0        0        0     8113 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_testcases_pass_validation.py
--rw-r--r--   0        0        0      260 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/test_uri.py
--rw-r--r--   0        0        0      126 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/README.txt
--rw-r--r--   0        0        0      198 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-attribute-forbidden-annotation.xspf
--rw-r--r--   0        0        0      149 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-attribute-forbidden-playlist.xspf
--rw-r--r--   0        0        0      382 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-baddate.xspf
--rw-r--r--   0        0        0      237 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-badversion.xspf
--rw-r--r--   0        0        0      190 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-element-forbidden-attribution.xspf
--rw-r--r--   0        0        0      159 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-extension-application-missing.xspf
--rw-r--r--   0        0        0      153 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-link-rel-missing.xspf
--rw-r--r--   0        0        0      323 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-annotation.xspf
--rw-r--r--   0        0        0      314 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-creator.xspf
--rw-r--r--   0        0        0      331 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-meta.xspf
--rw-r--r--   0        0        0      308 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-markup-title.xspf
--rw-r--r--   0        0        0      153 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-meta-rel-missing.xspf
--rw-r--r--   0        0        0      232 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-missingtracklist.xspf
--rw-r--r--   0        0        0      182 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-missingversion.xspf
--rw-r--r--   0        0        0      199 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-missing.xspf
--rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-nested-broken.xspf
--rw-r--r--   0        0        0      381 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-namespace-wrong-string.xspf
--rw-r--r--   0        0        0      120 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-attribution.xspf
--rw-r--r--   0        0        0       93 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-playlist.xspf
--rw-r--r--   0        0        0      100 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-nonleaf-content-trackList.xspf
--rw-r--r--   0        0        0      127 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-root-name.xspf
--rw-r--r--   0        0        0      313 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-annotation.xspf
--rw-r--r--   0        0        0      279 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-attribution.xspf
--rw-r--r--   0        0        0      299 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-creator.xspf
--rw-r--r--   0        0        0      320 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-date.xspf
--rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-identifier.xspf
--rw-r--r--   0        0        0      311 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-image.xspf
--rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-info.xspf
--rw-r--r--   0        0        0      321 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-license.xspf
--rw-r--r--   0        0        0      350 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-location.xspf
--rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-title.xspf
--rw-r--r--   0        0        0      257 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/playlist-toomany-tracklist.xspf
--rw-r--r--   0        0        0      370 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-badint-duration.xspf
--rw-r--r--   0        0        0      370 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-badint-tracknum.xspf
--rw-r--r--   0        0        0      194 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-extension-application-missing.xspf
--rw-r--r--   0        0        0      188 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-link-rel-missing.xspf
--rw-r--r--   0        0        0      316 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-album.xspf
--rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-annotation.xspf
--rw-r--r--   0        0        0      324 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-creator.xspf
--rw-r--r--   0        0        0      338 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-meta.xspf
--rw-r--r--   0        0        0      316 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-markup-title.xspf
--rw-r--r--   0        0        0      188 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-meta-rel-missing.xspf
--rw-r--r--   0        0        0      123 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-nonleaf-content.xspf
--rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-album.xspf
--rw-r--r--   0        0        0      372 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-annotation.xspf
--rw-r--r--   0        0        0      354 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-creator.xspf
--rw-r--r--   0        0        0      352 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-duration.xspf
--rw-r--r--   0        0        0      364 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-image.xspf
--rw-r--r--   0        0        0      358 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-info.xspf
--rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-title.xspf
--rw-r--r--   0        0        0      352 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/fail/track-toomany-tracknum.xspf
--rw-r--r--   0        0        0      605 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf
--rw-r--r--   0        0        0      137 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-annotation.xspf
--rw-r--r--   0        0        0      134 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-creator.xspf
--rw-r--r--   0        0        0      157 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-meta.xspf
--rw-r--r--   0        0        0      132 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-empty-title.xspf
--rw-r--r--   0        0        0      379 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extension.xspf
--rw-r--r--   0        0        0     3342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extensive.xspf
--rw-r--r--   0        0        0      869 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-inverted-order.xspf
--rw-r--r--   0        0        0      250 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-nested-proper.xspf
--rw-r--r--   0        0        0      139 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-nondefault.xspf
--rw-r--r--   0        0        0      205 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-namespace-two-additions.xspf
--rw-r--r--   0        0        0      336 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-attribution-identifier.xspf
--rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-attribution-location.xspf
--rw-r--r--   0        0        0      317 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-extension.xspf
--rw-r--r--   0        0        0      298 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-identifier.xspf
--rw-r--r--   0        0        0      283 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-image.xspf
--rw-r--r--   0        0        0      280 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-info.xspf
--rw-r--r--   0        0        0      289 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-license.xspf
--rw-r--r--   0        0        0      305 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-link-content.xspf
--rw-r--r--   0        0        0      314 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-link-rel.xspf
--rw-r--r--   0        0        0      292 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-location.xspf
--rw-r--r--   0        0        0      303 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-noturi-meta.xspf
--rw-r--r--   0        0        0      572 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-relative-paths.xspf
--rw-r--r--   0        0        0      162 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-whitespace-dateTime.xspf
--rw-r--r--   0        0        0     1543 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-xml-base.xspf
--rw-r--r--   0        0        0      174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-album.xspf
--rw-r--r--   0        0        0      179 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-annotation.xspf
--rw-r--r--   0        0        0      176 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-creator.xspf
--rw-r--r--   0        0        0      199 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-meta.xspf
--rw-r--r--   0        0        0      174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-empty-title.xspf
--rw-r--r--   0        0        0      320 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extension.xspf
--rw-r--r--   0        0        0     4160 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extensive.xspf
--rw-r--r--   0        0        0      917 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-inverted-order.xspf
--rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-extension.xspf
--rw-r--r--   0        0        0      329 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-identifier.xspf
--rw-r--r--   0        0        0      309 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-image.xspf
--rw-r--r--   0        0        0      305 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-info.xspf
--rw-r--r--   0        0        0      353 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-link-rel.xspf
--rw-r--r--   0        0        0      330 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-link.xspf
--rw-r--r--   0        0        0      321 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-location.xspf
--rw-r--r--   0        0        0      342 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-noturi-meta-rel.xspf
--rw-r--r--   0        0        0      412 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-anyURI.xspf
--rw-r--r--   0        0        0      414 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-in-between.xspf
--rw-r--r--   0        0        0      326 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/tests/testcase/version_1/pass/track-whitespace-nonNegativeInteger.xspf
--rw-r--r--   0        0        0      353 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/__init__.py
--rw-r--r--   0        0        0      431 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/base.py
--rw-r--r--   0        0        0     4434 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/builders.py
--rw-r--r--   0        0        0      386 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/constants.py
--rw-r--r--   0        0        0    17089 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/elements.py
--rw-r--r--   0        0        0    13174 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/parsers.py
--rw-r--r--   0        0        0      377 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/types.py
--rw-r--r--   0        0        0      604 2023-05-26 09:46:21.999764 xspf_lib-0.3.3/xspf_lib/utils.py
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 xspf_lib-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3408 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/README.rst
+-rw-r--r--   0        0        0     1465 2023-05-26 10:31:01.617670 xspf_lib-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     6946 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/test_module.py
+-rw-r--r--   0        0        0     3523 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/test_testcases_fail_validation.py
+-rw-r--r--   0        0        0     8113 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/test_testcases_pass_validation.py
+-rw-r--r--   0        0        0      260 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/test_uri.py
+-rw-r--r--   0        0        0      126 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/README.txt
+-rw-r--r--   0        0        0      198 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-attribute-forbidden-annotation.xspf
+-rw-r--r--   0        0        0      149 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-attribute-forbidden-playlist.xspf
+-rw-r--r--   0        0        0      382 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-baddate.xspf
+-rw-r--r--   0        0        0      237 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-badversion.xspf
+-rw-r--r--   0        0        0      190 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-element-forbidden-attribution.xspf
+-rw-r--r--   0        0        0      159 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-extension-application-missing.xspf
+-rw-r--r--   0        0        0      153 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-link-rel-missing.xspf
+-rw-r--r--   0        0        0      323 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-markup-annotation.xspf
+-rw-r--r--   0        0        0      314 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-markup-creator.xspf
+-rw-r--r--   0        0        0      331 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-markup-meta.xspf
+-rw-r--r--   0        0        0      308 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-markup-title.xspf
+-rw-r--r--   0        0        0      153 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      232 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-missingtracklist.xspf
+-rw-r--r--   0        0        0      182 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-missingversion.xspf
+-rw-r--r--   0        0        0      199 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-namespace-missing.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-namespace-nested-broken.xspf
+-rw-r--r--   0        0        0      381 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-namespace-wrong-string.xspf
+-rw-r--r--   0        0        0      120 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-nonleaf-content-attribution.xspf
+-rw-r--r--   0        0        0       93 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-nonleaf-content-playlist.xspf
+-rw-r--r--   0        0        0      100 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-nonleaf-content-trackList.xspf
+-rw-r--r--   0        0        0      127 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-root-name.xspf
+-rw-r--r--   0        0        0      313 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-annotation.xspf
+-rw-r--r--   0        0        0      279 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-attribution.xspf
+-rw-r--r--   0        0        0      299 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-creator.xspf
+-rw-r--r--   0        0        0      320 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-date.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-identifier.xspf
+-rw-r--r--   0        0        0      311 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-image.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-info.xspf
+-rw-r--r--   0        0        0      321 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-license.xspf
+-rw-r--r--   0        0        0      350 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-location.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-title.xspf
+-rw-r--r--   0        0        0      257 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/playlist-toomany-tracklist.xspf
+-rw-r--r--   0        0        0      370 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-badint-duration.xspf
+-rw-r--r--   0        0        0      370 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-badint-tracknum.xspf
+-rw-r--r--   0        0        0      194 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-extension-application-missing.xspf
+-rw-r--r--   0        0        0      188 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-link-rel-missing.xspf
+-rw-r--r--   0        0        0      316 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-markup-album.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-markup-annotation.xspf
+-rw-r--r--   0        0        0      324 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-markup-creator.xspf
+-rw-r--r--   0        0        0      338 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-markup-meta.xspf
+-rw-r--r--   0        0        0      316 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-markup-title.xspf
+-rw-r--r--   0        0        0      188 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      123 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-nonleaf-content.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-album.xspf
+-rw-r--r--   0        0        0      372 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-annotation.xspf
+-rw-r--r--   0        0        0      354 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-creator.xspf
+-rw-r--r--   0        0        0      352 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-duration.xspf
+-rw-r--r--   0        0        0      364 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-image.xspf
+-rw-r--r--   0        0        0      358 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-info.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-title.xspf
+-rw-r--r--   0        0        0      352 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/fail/track-toomany-tracknum.xspf
+-rw-r--r--   0        0        0      605 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf
+-rw-r--r--   0        0        0      137 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-empty-annotation.xspf
+-rw-r--r--   0        0        0      134 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-empty-creator.xspf
+-rw-r--r--   0        0        0      157 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-empty-meta.xspf
+-rw-r--r--   0        0        0      132 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-empty-title.xspf
+-rw-r--r--   0        0        0      379 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-extension.xspf
+-rw-r--r--   0        0        0     3342 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-extensive.xspf
+-rw-r--r--   0        0        0      869 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-inverted-order.xspf
+-rw-r--r--   0        0        0      250 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-namespace-nested-proper.xspf
+-rw-r--r--   0        0        0      139 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-namespace-nondefault.xspf
+-rw-r--r--   0        0        0      205 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-namespace-two-additions.xspf
+-rw-r--r--   0        0        0      336 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-attribution-identifier.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-attribution-location.xspf
+-rw-r--r--   0        0        0      317 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-extension.xspf
+-rw-r--r--   0        0        0      298 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-identifier.xspf
+-rw-r--r--   0        0        0      283 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-image.xspf
+-rw-r--r--   0        0        0      280 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-info.xspf
+-rw-r--r--   0        0        0      289 2023-05-26 10:30:45.393446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-license.xspf
+-rw-r--r--   0        0        0      305 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-link-content.xspf
+-rw-r--r--   0        0        0      314 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      292 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-location.xspf
+-rw-r--r--   0        0        0      303 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-noturi-meta.xspf
+-rw-r--r--   0        0        0      572 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-relative-paths.xspf
+-rw-r--r--   0        0        0      162 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-whitespace-dateTime.xspf
+-rw-r--r--   0        0        0     1543 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-xml-base.xspf
+-rw-r--r--   0        0        0      174 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-empty-album.xspf
+-rw-r--r--   0        0        0      179 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-empty-annotation.xspf
+-rw-r--r--   0        0        0      176 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-empty-creator.xspf
+-rw-r--r--   0        0        0      199 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-empty-meta.xspf
+-rw-r--r--   0        0        0      174 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-empty-title.xspf
+-rw-r--r--   0        0        0      320 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-extension.xspf
+-rw-r--r--   0        0        0     4160 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-extensive.xspf
+-rw-r--r--   0        0        0      917 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-inverted-order.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-extension.xspf
+-rw-r--r--   0        0        0      329 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-identifier.xspf
+-rw-r--r--   0        0        0      309 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-image.xspf
+-rw-r--r--   0        0        0      305 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-info.xspf
+-rw-r--r--   0        0        0      353 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      330 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-link.xspf
+-rw-r--r--   0        0        0      321 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-location.xspf
+-rw-r--r--   0        0        0      342 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-noturi-meta-rel.xspf
+-rw-r--r--   0        0        0      412 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-whitespace-anyURI.xspf
+-rw-r--r--   0        0        0      414 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-whitespace-in-between.xspf
+-rw-r--r--   0        0        0      326 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/tests/testcase/version_1/pass/track-whitespace-nonNegativeInteger.xspf
+-rw-r--r--   0        0        0      416 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/_version.py
+-rw-r--r--   0        0        0      431 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/base.py
+-rw-r--r--   0        0        0     4434 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/builders.py
+-rw-r--r--   0        0        0      386 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/constants.py
+-rw-r--r--   0        0        0    17089 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/elements.py
+-rw-r--r--   0        0        0    13174 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/parsers.py
+-rw-r--r--   0        0        0      377 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/types.py
+-rw-r--r--   0        0        0      604 2023-05-26 10:30:45.397446 xspf_lib-0.3.4/xspf_lib/utils.py
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 xspf_lib-0.3.4/PKG-INFO
```

### Comparing `xspf_lib-0.3.3/LICENSE` & `xspf_lib-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/README.rst` & `xspf_lib-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/pyproject.toml` & `xspf_lib-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "xspf-lib"
-version = "0.3.3"
 description = "Library for work with xspf format"
 authors = [
     { name = "Dzmitry Izaitka", email = "dem214overlord@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.7"
 readme = "README.rst"
@@ -15,14 +14,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Video",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+dynamic = []
+version = "0.3.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Source = "https://github.com/dem214/xspf-lib"
 "Bug Tracker" = "https://github.com/dem214/xspf-lib/issues"
@@ -30,14 +31,19 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tool.pdm.version]
+source = "scm"
+write_to = "xspf_lib/_version.py"
+write_template = "__version__ = '{}'"
+
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=7.3.1",
 ]
 lint = [
     "flake8>=5.0.4",
     "flake8-pyprojecttoml>=0.0.2",
```

### Comparing `xspf_lib-0.3.3/tests/test_module.py` & `xspf_lib-0.3.4/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/test_testcases_fail_validation.py` & `xspf_lib-0.3.4/tests/test_testcases_fail_validation.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/test_testcases_pass_validation.py` & `xspf_lib-0.3.4/tests/test_testcases_pass_validation.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-extensive.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-extensive.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-inverted-order.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-inverted-order.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-relative-paths.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-relative-paths.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/playlist-xml-base.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/playlist-xml-base.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/track-extensive.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/track-extensive.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/tests/testcase/version_1/pass/track-inverted-order.xspf` & `xspf_lib-0.3.4/tests/testcase/version_1/pass/track-inverted-order.xspf`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/xspf_lib/builders.py` & `xspf_lib-0.3.4/xspf_lib/builders.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/xspf_lib/elements.py` & `xspf_lib-0.3.4/xspf_lib/elements.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/xspf_lib/parsers.py` & `xspf_lib-0.3.4/xspf_lib/parsers.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/xspf_lib/utils.py` & `xspf_lib-0.3.4/xspf_lib/utils.py`

 * *Files identical despite different names*

### Comparing `xspf_lib-0.3.3/PKG-INFO` & `xspf_lib-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspf-lib
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library for work with xspf format
 Keywords: xspf playlist
 Author-Email: Dzmitry Izaitka <dem214overlord@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.3 Summary: Library for work
+Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.4 Summary: Library for work
 with xspf format Keywords: xspf playlist Author-Email: Dzmitry Izaitka
 gmail.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic
 :: Multimedia :: Video Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Project-URL: Source, https://github.com/dem214/xspf-lib
 Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues Project-
```

