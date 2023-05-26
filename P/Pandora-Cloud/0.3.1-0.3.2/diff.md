# Comparing `tmp/Pandora-Cloud-0.3.1.tar.gz` & `tmp/Pandora-Cloud-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-pox9zxpo/Pandora-Cloud-0.3.1.tar", last modified: Thu May 25 12:16:30 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-mi50wdm9/Pandora-Cloud-0.3.2.tar", last modified: Fri May 26 03:49:31 2023, max compression
```

## Comparing `Pandora-Cloud-0.3.1.tar` & `Pandora-Cloud-0.3.2.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/buildManifest1.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/58-107b19eac1b472e5.js
--rw-r--r--   0 runner    (1001) docker     (123)  1258865 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/588-439179c71d396f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
--rw-r--r--   0 runner    (1001) docker     (123)   338994 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/734-f1cef41ade2ec244.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
--rw-r--r--   0 runner    (1001) docker     (123)  1003471 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-16b8642aca9f7fea.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-ec4e8336fb15f89f.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-bb8fda2bb300c73d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
--rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-0233e94d3495a1c6.js
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-347e5b868a9f07a5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   124225 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/css/0ba7ad504b2624b8.css
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/
--rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32180 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/images/share-sidebar-link.png
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:30.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-25 12:16:15.000000 Pandora-Cloud-0.3.1/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/buildManifest1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/58-107b19eac1b472e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1258865 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/588-439179c71d396f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
+-rw-r--r--   0 runner    (1001) docker     (123)   338994 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/734-f1cef41ade2ec244.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1003471 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-16b8642aca9f7fea.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-ec4e8336fb15f89f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-bb8fda2bb300c73d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-0233e94d3495a1c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/webpack-347e5b868a9f07a5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   124225 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/css/0ba7ad504b2624b8.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32180 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/images/share-sidebar-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:31.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-26 03:49:18.000000 Pandora-Cloud-0.3.2/src/pandora_cloud/server.py
```

### Comparing `Pandora-Cloud-0.3.1/LICENSE` & `Pandora-Cloud-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/PKG-INFO` & `Pandora-Cloud-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/PKG-INFO` & `Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-Cloud
-Version: 0.3.1
+Version: 0.3.2
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/pengzhile/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora-cloud
 Project-URL: Tracker, https://github.com/pengzhile/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `Pandora-Cloud-0.3.1/Pandora_Cloud.egg-info/SOURCES.txt` & `Pandora-Cloud-0.3.2/Pandora_Cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/pandora_cloud/flask/static/_next/static/chunks/58-107b19eac1b472e5.js
 src/pandora_cloud/flask/static/_next/static/chunks/588-439179c71d396f90.js
 src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
 src/pandora_cloud/flask/static/_next/static/chunks/734-f1cef41ade2ec244.js
 src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
 src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
 src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
+src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 src/pandora_cloud/flask/static/_next/static/chunks/webpack-347e5b868a9f07a5.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/app-16b8642aca9f7fea.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/index-bb8fda2bb300c73d.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
 src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
```

### Comparing `Pandora-Cloud-0.3.1/README.md` & `Pandora-Cloud-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/setup.py` & `Pandora-Cloud-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/buildManifest1.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/MYarkpkg17PeZHlffaxc-/buildManifest1.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/58-107b19eac1b472e5.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/58-107b19eac1b472e5.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/588-439179c71d396f90.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/588-439179c71d396f90.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/734-f1cef41ade2ec244.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/734-f1cef41ade2ec244.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-16b8642aca9f7fea.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-16b8642aca9f7fea.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-ec4e8336fb15f89f.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-ec4e8336fb15f89f.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-bb8fda2bb300c73d.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-bb8fda2bb300c73d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-0233e94d3495a1c6.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-0233e94d3495a1c6.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-347e5b868a9f07a5.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/chunks/webpack-347e5b868a9f07a5.js`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/_next/static/css/0ba7ad504b2624b8.css` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/_next/static/css/0ba7ad504b2624b8.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/apple-touch-icon.png` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/favicon-16x16.png` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/favicon-32x32.png` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/images/share-sidebar-link.png` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/images/share-sidebar-link.png`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/service-worker.js` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/service-worker.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,15 @@
 self.addEventListener('install', event => {
     event.waitUntil(
         caches.open('pandora-cloud-cache').then(function(cache) {
             return cache.addAll([
+                '/apple-touch-icon.png',
+                '/favicon-16x16.png',
+                '/favicon-32x32.png',
+                '/images/share-sidebar-link.png',
                 '/ulp/react-components/1.66.5/css/main.cdn.min.css',
                 '/fonts/colfax/ColfaxAIRegular.woff2',
                 '/fonts/colfax/ColfaxAIRegular.woff',
                 '/fonts/colfax/ColfaxAIRegularItalic.woff2',
                 '/fonts/colfax/ColfaxAIRegularItalic.woff',
                 '/fonts/colfax/ColfaxAIBold.woff2',
                 '/fonts/colfax/ColfaxAIBold.woff',
@@ -49,14 +53,15 @@
                 '/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js',
                 '/_next/static/chunks/pages/bypass-338530f42d5b2105.js',
                 '/_next/static/chunks/pages/payments/business-e449df976df219cb.js',
                 '/_next/static/chunks/pages/payments/success-66b11e86067b001d.js',
                 '/_next/static/chunks/pages/share/[[...shareParams]]-0233e94d3495a1c6.js',
                 '/_next/static/chunks/pages/status-6557d60655b68492.js',
                 '/_next/static/chunks/259-c6320349d8f3ff4a.js',
+                '/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js',
             ]);
         })
     );
 });
 
 self.addEventListener('fetch', function(event) {
     event.respondWith(
```

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/chat.html` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/detail.html` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/flask/templates/login.html` & `Pandora-Cloud-0.3.2/src/pandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `Pandora-Cloud-0.3.1/src/pandora_cloud/server.py` & `Pandora-Cloud-0.3.2/src/pandora_cloud/server.py`

 * *Files identical despite different names*

